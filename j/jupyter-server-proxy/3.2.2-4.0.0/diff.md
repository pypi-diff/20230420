# Comparing `tmp/jupyter-server-proxy-3.2.2.tar.gz` & `tmp/jupyter_server_proxy-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-server-proxy-3.2.2.tar", last modified: Thu Sep  8 00:27:38 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyter-server-proxy-3.2.2.tar` & `jupyter_server_proxy-4.0.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy/
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    12311 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy/etc/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/etc/jupyter-server-proxy-jupyterserverextension.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/etc/jupyter-server-proxy-nbextension.json
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/etc/jupyter-server-proxy-notebookserverextension.json
--rw-r--r--   0 runner    (1001) docker     (121)    28034 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/568.f25cbf5a25d42e5d9003.js
--rw-r--r--   0 runner    (1001) docker     (121)     6210 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/remoteEntry.e84826446ca2e8c10352.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-08 00:27:36.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/static/tree.js
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4582 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-09-08 00:27:38.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-08 00:27:37.000000 jupyter-server-proxy-3.2.2/jupyter_server_proxy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-08 00:27:34.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     4861 2022-09-08 00:27:34.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 00:27:38.277204 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3549 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (121)   223149 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-08 00:27:38.281204 jupyter-server-proxy-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-09-08 00:26:46.000000 jupyter-server-proxy-3.2.2/setup.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/.flake8
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/RELEASE.md
+-rw-r--r--   0        0        0    25448 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/screenshot.png
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/setup.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/api.py
+-rw-r--r--   0        0        0    12946 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/config.py
+-rw-r--r--   0        0        0    32574 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/handlers.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/unixsock.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/utils.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/websocket.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/etc/jupyter_notebook_config.d/jupyter-server-proxy.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/etc/jupyter_server_config.d/jupyter-server-proxy.json
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/etc/nbconfig/tree.d/jupyter-server-proxy.json
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/package.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/568.d5fa5a0c0d3b0516bea8.js
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/remoteEntry.6bef4394de3b3e455a6a.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/jupyter_server_proxy/static/tree.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/.gitignore
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/.yarnrc
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/LICENSE
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/README.md
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/package.json
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/tsconfig.json
+-rw-r--r--   0        0        0   156734 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/yarn.lock
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/labextension/src/index.ts
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/test_config.py
+-rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/test_proxies.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/Classic.robot
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/Lab.robot
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/__init__.robot
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/test_acceptance.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/resources/index.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/acceptance/resources/jupyter_config.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/resources/gzipserver.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/resources/httpinfo.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/resources/jupyter_server_config.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/resources/proxyextension.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/tests/resources/websocket.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/LICENSE
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/README.md
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 jupyter_server_proxy-4.0.0/PKG-INFO
```

### Comparing `jupyter-server-proxy-3.2.2/LICENSE` & `jupyter_server_proxy-4.0.0/labextension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-server-proxy-3.2.2/PKG-INFO` & `jupyter_server_proxy-4.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,21 @@
-Metadata-Version: 2.1
-Name: jupyter-server-proxy
-Version: 3.2.2
-Summary: Jupyter server extension to supervise and proxy web services
-Home-page: https://github.com/jupyterhub/jupyter-server-proxy
-Author: Ryan Lovett & Yuvi Panda
-Author-email: rylo@berkeley.edu
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab :: 2
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: acceptance
-License-File: LICENSE
-
 # Jupyter Server Proxy
 
 [![ReadTheDocs badge](https://img.shields.io/readthedocs/jupyter-server-proxy?logo=read-the-docs)](https://jupyter-server-proxy.readthedocs.io/)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jupyterhub/jupyter-server-proxy/Test?logo=github)](https://github.com/jupyterhub/jupyter-server-proxy/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jupyterhub/jupyter-server-proxy/test.yaml?logo=github&branch=main)](https://github.com/jupyterhub/jupyter-server-proxy/actions)
 [![PyPI badge](https://img.shields.io/pypi/v/jupyter-server-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/jupyter-server-proxy)
 [![Conda badge](https://img.shields.io/conda/vn/conda-forge/jupyter-server-proxy?logo=conda-forge)](https://anaconda.org/conda-forge/jupyter-server-proxy)
-[![NPM badge](https://img.shields.io/npm/v/@jupyterlab/server-proxy.svg?logo=npm)](https://www.npmjs.com/package/@jupyterlab/server-proxy)
+[![NPM badge](https://img.shields.io/npm/v/@jupyterhub/jupyter-server-proxy.svg?logo=npm)](https://www.npmjs.com/package/@jupyterhub/jupyter-server-proxy)
 
 Jupyter Server Proxy lets you run arbitrary external processes (such as
 RStudio, Shiny Server, Syncthing, PostgreSQL, Code Server, etc)
 alongside your notebook server and provide authenticated web access to
 them using a path like `/rstudio` next to others like `/lab`. Alongside
 the python package that provides the main functionality, the JupyterLab
-extension (`@jupyterlab/server-proxy`) provides buttons in the
+extension (`@jupyterhub/jupyter-server-proxy`) provides buttons in the
 JupyterLab launcher window to get to RStudio for example.
 
 **Note:** This project used to be called **nbserverproxy**. As
 nbserverproxy is an older version of jupyter-server-proxy, uninstall
 nbserverproxy before installing jupyter-server-proxy to avoid conflicts.
 
 The primary use cases are:
@@ -53,73 +23,83 @@
 1.  Use with JupyterHub / Binder to allow launching users into web
     interfaces that have nothing to do with Jupyter - such as RStudio,
     Shiny, or OpenRefine.
 2.  Allow access from frontend javascript (in classic notebook or
     JupyterLab extensions) to access web APIs of other processes running
     locally in a safe manner. This is used by the [JupyterLab
     extension](https://github.com/dask/dask-labextension) for
-    [dask](https://dask.org/).
+    [dask](https://www.dask.org/).
 
 [The documentation](https://jupyter-server-proxy.readthedocs.io/)
 contains information on installation & usage.
 
+## Security warning
+
+Jupyter Server Proxy is often used to start a user defined process listening to
+some network port (e.g. `http://localhost:4567`) for a user starting a Jupyter Server
+that only that user has permission to access. The user can then access the
+started process proxied through the Jupyter Server.
+
+For safe use of Jupyter Server Proxy, you should ensure that the process started
+by Jupyter Server proxy can't be accessed directly by another user and bypass
+the Jupyter Server's authorization!
+
+A common strategy to enforce access proxied via Jupyter Server is to start
+Jupyter Server within a container and only allow network access to the Jupyter
+Server via the container.
+
+> For more insights, see [Ryan Lovett's comment about
+> it](https://github.com/jupyterhub/jupyter-server-proxy/pull/359#issuecomment-1350118197).
+
 ## Install
 
 ### Requirements
 
-* `jupyterlab>=2` or `notebook`
+Either `jupyterlab>=3` or `notebook` is required.
 
 ### Python package
 
-#### pip
+#### `pip`
 
-```
+```bash
 pip install jupyter-server-proxy
 ```
 
-#### conda
+#### `conda`
 
-```
+```bash
 conda install jupyter-server-proxy -c conda-forge
 ```
 
 ### JupyterLab extension
 
-Note that as the JupyterLab extension only is a graphical interface to
-launch registered applications in the python package, the extension
-requires the python package to be installed.
+A JupyterLab extension is bundled with the Python package to provide launch
+buttons in JupyterLab's Launcher panel for registered server processes.
 
-As of version 3.0.0 the Python package ships with a JupyterLab 3 compatible
-extension, making this step only needed for JupyterLab 2.
+![](docs/source/_static/images/labextension-launcher.png)
 
-```
-jupyter labextension install @jupyterlab/server-proxy
-```
+Clicking on them opens the proxied application in a new browser window.
 
 ## Disable
 
 ### Server extension
 
-``` 
-jupyter serverextension disable jupyter_server_proxy
+```bash
+jupyter serverextension disable --sys-prefix jupyter_server_proxy
+jupyter server extension disable --sys-prefix jupyter_server_proxy
 ```
 
 ### Notebook classic extension
 
-```
-jupyter nbextension disable --py jupyter_server_proxy
+```bash
+jupyter nbextension disable --sys-prefix --py jupyter_server_proxy
 ```
 
 ### JupyterLab extension
 
-Note that the extension name provided to the command (`jupyterlab-server-proxy`) does not correspond
-to the extension package name (`@jupyterlab/server-proxy`). The `jupyter labextension list` will
-incorrectly report the extension as still being enabled after executing the disable command.
-This will be fixed in the next major release of jupyter-server-proxy.
-
-```
-jupyter labextension disable jupyterlab-server-proxy
+```bash
+jupyter labextension disable @jupyterhub/jupyter-server-proxy
 ```
 
-## Local development
+#### Local development
 
-See [CONTRIBUTING.md](CONTRIBUTING.md).
+To setup a local development environment, see the [contributing guide](https://github.com/jupyterhub/jupyter-server-proxy/blob/main/CONTRIBUTING.md).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/__init__.py` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,82 @@
-from .handlers import setup_handlers
-from .config import ServerProxy as ServerProxyConfig, make_handlers, get_entrypoint_server_processes, make_server_process
 from jupyter_server.utils import url_path_join as ujoin
-from .api import ServersInfoHandler, IconHandler
+
+from .api import IconHandler, ServersInfoHandler
+from .config import ServerProxy as ServerProxyConfig
+from .config import get_entrypoint_server_processes, make_handlers, make_server_process
+from .handlers import setup_handlers
+
 
 # Jupyter Extension points
 def _jupyter_server_extension_points():
-    return [{
-        'module': 'jupyter_server_proxy',
-    }]
+    return [
+        {
+            "module": "jupyter_server_proxy",
+        }
+    ]
+
 
 def _jupyter_nbextension_paths():
-    return [{
-        "section": "tree",
-        "dest": "jupyter_server_proxy",
-        'src': 'static',
-        "require": "jupyter_server_proxy/tree"
-    }]
+    return [
+        {
+            "section": "tree",
+            "dest": "jupyter_server_proxy",
+            "src": "static",
+            "require": "jupyter_server_proxy/tree",
+        }
+    ]
+
+
+def _jupyter_labextension_paths():
+    return [
+        {
+            "src": "labextension",
+            "dest": "@jupyterhub/jupyter-server-proxy",
+        }
+    ]
 
 
 def _load_jupyter_server_extension(nbapp):
     # Set up handlers picked up via config
-    base_url = nbapp.web_app.settings['base_url']
+    base_url = nbapp.web_app.settings["base_url"]
     serverproxy_config = ServerProxyConfig(parent=nbapp)
 
     server_processes = [
         make_server_process(name, server_process_config, serverproxy_config)
         for name, server_process_config in serverproxy_config.servers.items()
     ]
     server_processes += get_entrypoint_server_processes(serverproxy_config)
     server_handlers = make_handlers(base_url, server_processes)
-    nbapp.web_app.add_handlers('.*', server_handlers)
+    nbapp.web_app.add_handlers(".*", server_handlers)
 
     # Set up default non-server handler
     setup_handlers(
         nbapp.web_app,
         serverproxy_config,
     )
 
     icons = {}
     for sp in server_processes:
         if sp.launcher_entry.enabled and sp.launcher_entry.icon_path:
             icons[sp.name] = sp.launcher_entry.icon_path
 
-    nbapp.web_app.add_handlers('.*', [
-        (ujoin(base_url, 'server-proxy/servers-info'), ServersInfoHandler, {'server_processes': server_processes}),
-        (ujoin(base_url, 'server-proxy/icon/(.*)'), IconHandler, {'icons': icons}),
-    ])
+    nbapp.web_app.add_handlers(
+        ".*",
+        [
+            (
+                ujoin(base_url, "server-proxy/servers-info"),
+                ServersInfoHandler,
+                {"server_processes": server_processes},
+            ),
+            (ujoin(base_url, "server-proxy/icon/(.*)"), IconHandler, {"icons": icons}),
+        ],
+    )
+
+    nbapp.log.debug(
+        "[jupyter-server-proxy] Started with known servers: %s",
+        ", ".join([p.name for p in server_processes]),
+    )
 
 
 # For backward compatibility
 load_jupyter_server_extension = _load_jupyter_server_extension
 _jupyter_server_extension_paths = _jupyter_server_extension_points
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/config.py` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,183 +1,214 @@
 """
 Traitlets based configuration for jupyter_server_proxy
 """
+import sys
+from collections import namedtuple
+from warnings import warn
+
+if sys.version_info < (3, 10):  # pragma: no cover
+    from importlib_metadata import entry_points
+else:  # pragma: no cover
+    from importlib.metadata import entry_points
+
 from jupyter_server.utils import url_path_join as ujoin
 from traitlets import Dict, List, Tuple, Union, default, observe
 from traitlets.config import Configurable
-from tornado import httpclient
-from warnings import warn
-from .handlers import SuperviseAndProxyHandler, AddSlashHandler, RewritableResponse
-import pkg_resources
-from collections import namedtuple
-from .utils import call_with_asked_args
+
+from .handlers import AddSlashHandler, NamedLocalProxyHandler, SuperviseAndProxyHandler
 
 try:
     # Traitlets >= 4.3.3
     from traitlets import Callable
 except ImportError:
     from .utils import Callable
 
-def _make_serverproxy_handler(name, command, environment, timeout, absolute_url, port, mappath, request_headers_override, rewrite_response):
+
+LauncherEntry = namedtuple(
+    "LauncherEntry", ["enabled", "icon_path", "title", "path_info"]
+)
+ServerProcess = namedtuple(
+    "ServerProcess",
+    [
+        "name",
+        "command",
+        "environment",
+        "timeout",
+        "absolute_url",
+        "port",
+        "unix_socket",
+        "mappath",
+        "launcher_entry",
+        "new_browser_tab",
+        "request_headers_override",
+        "rewrite_response",
+    ],
+)
+
+
+def _make_namedproxy_handler(sp: ServerProcess):
+    class _Proxy(NamedLocalProxyHandler):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.name = sp.name
+            self.proxy_base = sp.name
+            self.absolute_url = sp.absolute_url
+            self.port = sp.port
+            self.unix_socket = sp.unix_socket
+            self.mappath = sp.mappath
+            self.rewrite_response = sp.rewrite_response
+
+        def get_request_headers_override(self):
+            return self._realize_rendered_template(sp.request_headers_override)
+
+    return _Proxy
+
+
+def _make_supervisedproxy_handler(sp: ServerProcess):
     """
     Create a SuperviseAndProxyHandler subclass with given parameters
     """
+
     # FIXME: Set 'name' properly
     class _Proxy(SuperviseAndProxyHandler):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
-            self.name = name
-            self.proxy_base = name
-            self.absolute_url = absolute_url
-            self.requested_port = port
-            self.mappath = mappath
-            self.rewrite_response = rewrite_response
-
-        @property
-        def process_args(self):
-            return {
-                'port': self.port,
-                'base_url': self.base_url,
-            }
-
-        def _render_template(self, value):
-            args = self.process_args
-            if type(value) is str:
-                return value.format(**args)
-            elif type(value) is list:
-                return [self._render_template(v) for v in value]
-            elif type(value) is dict:
-                return {
-                    self._render_template(k): self._render_template(v)
-                    for k, v in value.items()
-                }
-            else:
-                raise ValueError('Value of unrecognized type {}'.format(type(value)))
-
-        def _realize_rendered_template(self, attribute):
-            '''Call any callables, then render any templated values.'''
-            if callable(attribute):
-                attribute = self._render_template(
-                    call_with_asked_args(attribute, self.process_args)
-                )
-            return self._render_template(attribute)
-
-        def get_cmd(self):
-            return self._realize_rendered_template(command)
+            self.name = sp.name
+            self.command = sp.command
+            self.proxy_base = sp.name
+            self.absolute_url = sp.absolute_url
+            self.requested_port = sp.port
+            self.requested_unix_socket = sp.unix_socket
+            self.mappath = sp.mappath
+            self.rewrite_response = sp.rewrite_response
 
         def get_env(self):
-            return self._realize_rendered_template(environment)
+            return self._realize_rendered_template(sp.environment)
 
         def get_request_headers_override(self):
-            return self._realize_rendered_template(request_headers_override)
+            return self._realize_rendered_template(sp.request_headers_override)
 
         def get_timeout(self):
-            return timeout
+            return sp.timeout
 
     return _Proxy
 
 
 def get_entrypoint_server_processes(serverproxy_config):
     sps = []
-    for entry_point in pkg_resources.iter_entry_points('jupyter_serverproxy_servers'):
+    for entry_point in entry_points(group="jupyter_serverproxy_servers"):
         name = entry_point.name
         server_process_config = entry_point.load()()
-        sps.append(
-            make_server_process(name, server_process_config, serverproxy_config)
-        )
+        sps.append(make_server_process(name, server_process_config, serverproxy_config))
     return sps
 
+
 def make_handlers(base_url, server_processes):
     """
     Get tornado handlers for registered server_processes
     """
     handlers = []
     for sp in server_processes:
-        handler = _make_serverproxy_handler(
-            sp.name,
-            sp.command,
-            sp.environment,
-            sp.timeout,
-            sp.absolute_url,
-            sp.port,
-            sp.mappath,
-            sp.request_headers_override,
-            sp.rewrite_response,
+        if sp.command:
+            handler = _make_supervisedproxy_handler(sp)
+            kwargs = dict(state={})
+        else:
+            if not (sp.port or isinstance(sp.unix_socket, str)):
+                warn(
+                    f"Server proxy {sp.name} does not have a command, port "
+                    f"number or unix_socket path. At least one of these is "
+                    f"required."
+                )
+                continue
+            handler = _make_namedproxy_handler(sp)
+            kwargs = {}
+        handlers.append(
+            (
+                ujoin(base_url, sp.name, r"(.*)"),
+                handler,
+                kwargs,
+            )
         )
-        handlers.append((
-            ujoin(base_url, sp.name, r'(.*)'), handler, dict(state={}),
-        ))
-        handlers.append((
-            ujoin(base_url, sp.name), AddSlashHandler
-        ))
+        handlers.append((ujoin(base_url, sp.name), AddSlashHandler))
     return handlers
 
-LauncherEntry = namedtuple('LauncherEntry', ['enabled', 'icon_path', 'title', 'path_info'])
-ServerProcess = namedtuple('ServerProcess', [
-    'name', 'command', 'environment', 'timeout', 'absolute_url', 'port',
-    'mappath', 'launcher_entry', 'new_browser_tab', 'request_headers_override', 'rewrite_response',
-])
 
 def make_server_process(name, server_process_config, serverproxy_config):
-    le = server_process_config.get('launcher_entry', {})
+    le = server_process_config.get("launcher_entry", {})
     return ServerProcess(
         name=name,
-        command=server_process_config['command'],
-        environment=server_process_config.get('environment', {}),
-        timeout=server_process_config.get('timeout', 5),
-        absolute_url=server_process_config.get('absolute_url', False),
-        port=server_process_config.get('port', 0),
-        mappath=server_process_config.get('mappath', {}),
+        command=server_process_config.get("command", list()),
+        environment=server_process_config.get("environment", {}),
+        timeout=server_process_config.get("timeout", 5),
+        absolute_url=server_process_config.get("absolute_url", False),
+        port=server_process_config.get("port", 0),
+        unix_socket=server_process_config.get("unix_socket", None),
+        mappath=server_process_config.get("mappath", {}),
         launcher_entry=LauncherEntry(
-            enabled=le.get('enabled', True),
-            icon_path=le.get('icon_path'),
-            title=le.get('title', name),
-            path_info=le.get('path_info', name + "/")
+            enabled=le.get("enabled", True),
+            icon_path=le.get("icon_path"),
+            title=le.get("title", name),
+            path_info=le.get("path_info", name + "/"),
+        ),
+        new_browser_tab=server_process_config.get("new_browser_tab", True),
+        request_headers_override=server_process_config.get(
+            "request_headers_override", {}
         ),
-        new_browser_tab=server_process_config.get('new_browser_tab', True),
-        request_headers_override=server_process_config.get('request_headers_override', {}),
         rewrite_response=server_process_config.get(
-            'rewrite_response',
+            "rewrite_response",
             tuple(),
         ),
     )
 
+
 class ServerProxy(Configurable):
     servers = Dict(
         {},
         help="""
         Dictionary of processes to supervise & proxy.
 
         Key should be the name of the process. This is also used by default as
         the URL prefix, and all requests matching this prefix are routed to this process.
 
         Value should be a dictionary with the following keys:
           command
-            A list of strings that should be the full command to be executed.
-            The optional template arguments {{port}} and {{base_url}} will be substituted with the
-            port the process should listen on and the base-url of the notebook.
+            An optional list of strings that should be the full command to be executed.
+            The optional template arguments {{port}}, {{unix_socket}} and {{base_url}}
+            will be substituted with the port or Unix socket path the process should
+            listen on and the base-url of the notebook.
 
             Could also be a callable. It should return a list.
 
+            If the command is not specified or is an empty list, the server
+            process is assumed to be started ahead of time and already available
+            to be proxied to.
+
           environment
             A dictionary of environment variable mappings. As with the command
-            traitlet, {{port}} and {{base_url}} will be substituted.
+            traitlet, {{port}}, {{unix_socket}} and {{base_url}} will be substituted.
 
             Could also be a callable. It should return a dictionary.
 
           timeout
             Timeout in seconds for the process to become ready, default 5s.
 
           absolute_url
             Proxy requests default to being rewritten to '/'. If this is True,
             the absolute URL will be sent to the backend instead.
 
           port
             Set the port that the service will listen on. The default is to automatically select an unused port.
 
+          unix_socket
+            If set, the service will listen on a Unix socket instead of a TCP port.
+            Set to True to use a socket in a new temporary folder, or a string
+            path to a socket. This overrides port.
+
+            Proxying websockets over a Unix socket requires Tornado >= 6.3.
+
           mappath
             Map request paths to proxied paths.
             Either a dictionary of request paths to proxied paths,
             or a callable that takes parameter ``path`` and returns the proxied path.
 
           launcher_entry
             A dictionary of various options for entries in classic notebook / jupyterlab launchers.
@@ -201,15 +232,15 @@
 
           new_browser_tab
             Set to True (default) to make the proxied server interface opened as a new browser tab. Set to False
             to have it open a new JupyterLab tab. This has no effect in classic notebook.
 
           request_headers_override
             A dictionary of additional HTTP headers for the proxy request. As with
-            the command traitlet, {{port}} and {{base_url}} will be substituted.
+            the command traitlet, {{port}}, {{unix_socket}} and {{base_url}} will be substituted.
 
           rewrite_response
             An optional function to rewrite the response for the given service.
             Input is a RewritableResponse object which is an argument that MUST be named
             ``response``. The function should modify one or more of the attributes
             ``.body``, ``.headers``, ``.code``, or ``.reason`` of the ``response``
             argument. For example:
@@ -239,28 +270,28 @@
 
             Note that if the order is reversed to ``[cats_only, dog_to_cat]``, then accessing
             ``/cat-club`` will produce a "403 Forbidden" response with body "cats not allowed"
             instead of "dogs not allowed".
 
             Defaults to the empty tuple ``tuple()``.
         """,
-        config=True
+        config=True,
     )
 
     non_service_rewrite_response = Union(
         default_value=tuple(),
         trait_types=[List(), Tuple(), Callable()],
         help="""
         A function (or list or tuple of functions) to rewrite the response for a
         non-service request, for example a request to ``/proxy/<host>:<port><path>``.
 
         See the description for ``rewrite_response`` for more information.
         Defaults to the empty tuple ``tuple()``.
         """,
-        config=True
+        config=True,
     )
 
     host_allowlist = Union(
         trait_types=[List(), Callable()],
         help="""
         List of allowed hosts.
         Can also be a function that decides whether a host can be proxied.
@@ -275,25 +306,26 @@
             def host_allowlist(handler, host):
                 handler.log.info("Request to proxy to host " + host)
                 return host.startswith("10.")
             c.ServerProxy.host_allowlist = host_allowlist
 
         Defaults to a list of ["localhost", "127.0.0.1"].
         """,
-        config=True
+        config=True,
     )
 
     @default("host_allowlist")
     def _host_allowlist_default(self):
         return ["localhost", "127.0.0.1"]
 
     host_whitelist = Union(
         trait_types=[List(), Callable()],
         help="Deprecated, use host_allowlist",
-        config=True)
+        config=True,
+    )
 
     @observe("host_whitelist")
     def _host_whitelist_deprecated(self, change):
         old_attr = change.name
         if self.host_allowlist != change.new:
             # only warn if different
             # protects backward-compatible config from warnings
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/handlers.py` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,77 @@
 """
 Authenticated HTTP proxy for Jupyter Notebooks
 
 Some original inspiration from https://github.com/senko/tornado-proxy
 """
 
-import inspect
-import socket
 import os
-from urllib.parse import urlunparse, urlparse, quote
-import aiohttp
+import socket
 from asyncio import Lock
 from copy import copy
+from tempfile import mkdtemp
+from urllib.parse import quote, urlparse, urlunparse
 
-from tornado import gen, web, httpclient, httputil, process, websocket, ioloop, version_info
-
-from jupyter_server.utils import ensure_async, url_path_join
+import aiohttp
 from jupyter_server.base.handlers import JupyterHandler, utcnow
-from traitlets.traitlets import HasTraits
+from jupyter_server.utils import ensure_async, url_path_join
+from simpervisor import SupervisedProcess
+from tornado import httpclient, httputil, web
+from tornado.simple_httpclient import SimpleAsyncHTTPClient
 from traitlets import Bytes, Dict, Instance, Integer, Unicode, Union, default, observe
+from traitlets.traitlets import HasTraits
 
+from .unixsock import UnixResolver
 from .utils import call_with_asked_args
 from .websocket import WebSocketHandlerMixin, pingable_ws_connect
-from simpervisor import SupervisedProcess
 
 
 class RewritableResponse(HasTraits):
     """
     A class to hold the response to be rewritten by rewrite_response
     """
+
     # The following should not be modified (or even accessed) by rewrite_response.
     # It is used to initialize the default values of the traits.
     orig_response = Instance(klass=httpclient.HTTPResponse)
 
     # The following are modifiable by rewrite_response
     headers = Union(trait_types=[Dict(), Instance(klass=httputil.HTTPHeaders)])
     body = Bytes()
     code = Integer()
     reason = Unicode(allow_none=True)
 
-    @default('headers')
+    @default("headers")
     def _default_headers(self):
         return copy(self.orig_response.headers)
 
-    @default('body')
+    @default("body")
     def _default_body(self):
         return self.orig_response.body
 
-    @default('code')
+    @default("code")
     def _default_code(self):
         return self.orig_response.code
 
-    @default('reason')
+    @default("reason")
     def _default_reason(self):
         return self.orig_response.reason
 
-    @observe('code')
+    @observe("code")
     def _observe_code(self, change):
         # HTTP status codes are mapped to short descriptions in the
         # httputil.responses dictionary, 200 maps to "OK", 403 maps to
         # "Forbidden" etc.
         #
         # If code is updated and it previously had a reason matching its short
         # description, we update reason to match the new code's short
         # description.
         #
-        if self.reason == httputil.responses.get(change['old'], 'Unknown'):
-            self.reason = httputil.responses.get(change['new'], 'Unknown')
+        if self.reason == httputil.responses.get(change["old"], "Unknown"):
+            self.reason = httputil.responses.get(change["new"], "Unknown")
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # Trigger the default value to be set from orig_response on instantiation.
         # Otherwise _observe_code will receive change['old'] == 0.
         self.code
 
@@ -80,37 +82,42 @@
         new = copy(self)
         func(new)
         return new
 
 
 class AddSlashHandler(JupyterHandler):
     """Add trailing slash to URLs that need them."""
+
     @web.authenticated
     def get(self, *args):
         src = urlparse(self.request.uri)
-        dest = src._replace(path=src.path + '/')
+        dest = src._replace(path=src.path + "/")
         self.redirect(urlunparse(dest))
 
+
 class ProxyHandler(WebSocketHandlerMixin, JupyterHandler):
     """
     A tornado request handler that proxies HTTP and websockets from
     a given host/port combination. This class is not meant to be
     used directly as a means of overriding CORS. This presents significant
     security risks, and could allow arbitrary remote code access. Instead, it is
     meant to be subclassed and used for proxying URLs from trusted sources.
 
     Subclasses should implement open, http_get, post, put, delete, head, patch,
     and options.
     """
+
+    unix_socket = None  # Used in subclasses
+
     def __init__(self, *args, **kwargs):
-        self.proxy_base = ''
-        self.absolute_url = kwargs.pop('absolute_url', False)
-        self.host_allowlist = kwargs.pop('host_allowlist', ['localhost', '127.0.0.1'])
+        self.proxy_base = ""
+        self.absolute_url = kwargs.pop("absolute_url", False)
+        self.host_allowlist = kwargs.pop("host_allowlist", ["localhost", "127.0.0.1"])
         self.rewrite_response = kwargs.pop(
-            'rewrite_response',
+            "rewrite_response",
             tuple(),
         )
         self.subprotocols = None
         super().__init__(*args, **kwargs)
 
     # Support/use jupyter_server config arguments allow_origin and allow_origin_pat
     # to enable cross origin requests propagated by e.g. inverting proxies.
@@ -118,99 +125,105 @@
     def check_origin(self, origin=None):
         return JupyterHandler.check_origin(self, origin)
 
     # Support all the methods that tornado does by default except for GET which
     # is passed to WebSocketHandlerMixin and then to WebSocketHandler.
 
     async def open(self, port, proxied_path):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement open')
+        raise NotImplementedError("Subclasses of ProxyHandler should implement open")
 
-    async def http_get(self, host, port, proxy_path=''):
-        '''Our non-websocket GET.'''
-        raise NotImplementedError('Subclasses of ProxyHandler should implement http_get')
+    async def http_get(self, host, port, proxy_path=""):
+        """Our non-websocket GET."""
+        raise NotImplementedError(
+            "Subclasses of ProxyHandler should implement http_get"
+        )
 
-    def post(self, host, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement this post')
+    def post(self, host, port, proxy_path=""):
+        raise NotImplementedError(
+            "Subclasses of ProxyHandler should implement this post"
+        )
 
-    def put(self, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement this put')
+    def put(self, port, proxy_path=""):
+        raise NotImplementedError(
+            "Subclasses of ProxyHandler should implement this put"
+        )
 
-    def delete(self, host, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement delete')
+    def delete(self, host, port, proxy_path=""):
+        raise NotImplementedError("Subclasses of ProxyHandler should implement delete")
 
-    def head(self, host, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement head')
+    def head(self, host, port, proxy_path=""):
+        raise NotImplementedError("Subclasses of ProxyHandler should implement head")
 
-    def patch(self, host, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement patch')
+    def patch(self, host, port, proxy_path=""):
+        raise NotImplementedError("Subclasses of ProxyHandler should implement patch")
 
-    def options(self, host, port, proxy_path=''):
-        raise NotImplementedError('Subclasses of ProxyHandler should implement options')
+    def options(self, host, port, proxy_path=""):
+        raise NotImplementedError("Subclasses of ProxyHandler should implement options")
 
     def on_message(self, message):
         """
         Called when we receive a message from our client.
 
         We proxy it to the backend.
         """
         self._record_activity()
-        if hasattr(self, 'ws'):
+        if hasattr(self, "ws"):
             self.ws.write_message(message, binary=isinstance(message, bytes))
 
     def on_ping(self, data):
         """
         Called when the client pings our websocket connection.
 
         We proxy it to the backend.
         """
-        self.log.debug('jupyter_server_proxy: on_ping: {}'.format(data))
+        self.log.debug(f"jupyter_server_proxy: on_ping: {data}")
         self._record_activity()
-        if hasattr(self, 'ws'):
+        if hasattr(self, "ws"):
             self.ws.protocol.write_ping(data)
 
     def on_pong(self, data):
         """
         Called when we receive a ping back.
         """
-        self.log.debug('jupyter_server_proxy: on_pong: {}'.format(data))
+        self.log.debug(f"jupyter_server_proxy: on_pong: {data}")
 
     def on_close(self):
         """
         Called when the client closes our websocket connection.
 
         We close our connection to the backend too.
         """
-        if hasattr(self, 'ws'):
+        if hasattr(self, "ws"):
             self.ws.close()
 
     def _record_activity(self):
         """Record proxied activity as API activity
 
         avoids proxied traffic being ignored by the notebook's
         internal idle-shutdown mechanism
         """
-        self.settings['api_last_activity'] = utcnow()
+        self.settings["api_last_activity"] = utcnow()
 
     def _get_context_path(self, host, port):
         """
         Some applications need to know where they are being proxied from.
         This is either:
         - {base_url}/proxy/{port}
         - {base_url}/proxy/{host}:{port}
         - {base_url}/proxy/absolute/{port}
         - {base_url}/proxy/absolute/{host}:{port}
         - {base_url}/{proxy_base}
         """
-        host_and_port = str(port) if host == 'localhost' else host + ":" + str(port)
+        host_and_port = str(port) if host == "localhost" else host + ":" + str(port)
         if self.proxy_base:
             return url_path_join(self.base_url, self.proxy_base)
         if self.absolute_url:
-            return url_path_join(self.base_url, 'proxy', 'absolute', host_and_port)
+            return url_path_join(self.base_url, "proxy", "absolute", host_and_port)
         else:
-            return url_path_join(self.base_url, 'proxy', host_and_port)
+            return url_path_join(self.base_url, "proxy", host_and_port)
 
     def get_client_uri(self, protocol, host, port, proxied_path):
         if self.absolute_url:
             context_path = self._get_context_path(host, port)
             client_path = url_path_join(context_path, proxied_path)
         else:
             client_path = proxied_path
@@ -224,102 +237,118 @@
         # and "un-reserved" characters as safe that won't need quoting. The
         # un-reserved need to be marked safe to ensure the quote function behave
         # the same in py36 as py37.
         #
         # ref: https://tools.ietf.org/html/rfc3986#section-2.2
         client_path = quote(client_path, safe=":/?#[]@!$&'()*+,;=-._~")
 
-        client_uri = '{protocol}://{host}:{port}{path}'.format(
+        client_uri = "{protocol}://{host}:{port}{path}".format(
             protocol=protocol,
             host=host,
             port=port,
             path=client_path,
         )
         if self.request.query:
-            client_uri += '?' + self.request.query
+            client_uri += "?" + self.request.query
 
         return client_uri
 
     def _build_proxy_request(self, host, port, proxied_path, body):
-
         headers = self.proxy_request_headers()
 
-        client_uri = self.get_client_uri('http', host, port, proxied_path)
+        client_uri = self.get_client_uri("http", host, port, proxied_path)
         # Some applications check X-Forwarded-Context and X-ProxyContextPath
         # headers to see if and where they are being proxied from.
         if not self.absolute_url:
             context_path = self._get_context_path(host, port)
-            headers['X-Forwarded-Context'] = context_path
-            headers['X-ProxyContextPath'] = context_path
+            headers["X-Forwarded-Context"] = context_path
+            headers["X-ProxyContextPath"] = context_path
             # to be compatible with flask/werkzeug wsgi applications
-            headers['X-Forwarded-Prefix'] = context_path
+            headers["X-Forwarded-Prefix"] = context_path
 
         req = httpclient.HTTPRequest(
-            client_uri, method=self.request.method, body=body,
+            client_uri,
+            method=self.request.method,
+            body=body,
             decompress_response=False,
-            headers=headers, **self.proxy_request_options())
+            headers=headers,
+            **self.proxy_request_options(),
+        )
         return req
 
     def _check_host_allowlist(self, host):
         if callable(self.host_allowlist):
             return self.host_allowlist(self, host)
         else:
             return host in self.host_allowlist
 
     @web.authenticated
     async def proxy(self, host, port, proxied_path):
-        '''
+        """
         This serverextension handles:
             {base_url}/proxy/{port([0-9]+)}/{proxied_path}
             {base_url}/proxy/absolute/{port([0-9]+)}/{proxied_path}
             {base_url}/{proxy_base}/{proxied_path}
-        '''
+        """
 
         if not self._check_host_allowlist(host):
             self.set_status(403)
-            self.write("Host '{host}' is not allowed. "
-                       "See https://jupyter-server-proxy.readthedocs.io/en/latest/arbitrary-ports-hosts.html for info.".format(host=host))
+            self.write(
+                "Host '{host}' is not allowed. "
+                "See https://jupyter-server-proxy.readthedocs.io/en/latest/arbitrary-ports-hosts.html for info.".format(
+                    host=host
+                )
+            )
             return
 
         # Remove hop-by-hop headers that don't necessarily apply to the request we are making
         # to the backend. See https://github.com/jupyterhub/jupyter-server-proxy/pull/328
         # for more information
         hop_by_hop_headers = [
-            'Proxy-Connection',
-            'Keep-Alive',
-            'Transfer-Encoding',
-            'TE',
-            'Connection',
-            'Trailer',
-            'Upgrade',
-            'Proxy-Authorization',
-            'Proxy-Authenticate'
+            "Proxy-Connection",
+            "Keep-Alive",
+            "Transfer-Encoding",
+            "TE",
+            "Connection",
+            "Trailer",
+            "Upgrade",
+            "Proxy-Authorization",
+            "Proxy-Authenticate",
         ]
         for header_to_remove in hop_by_hop_headers:
             if header_to_remove in self.request.headers:
                 del self.request.headers[header_to_remove]
 
         self._record_activity()
 
-        if self.request.headers.get("Upgrade", "").lower() == 'websocket':
+        if self.request.headers.get("Upgrade", "").lower() == "websocket":
             # We wanna websocket!
             # jupyterhub/jupyter-server-proxy@36b3214
-            self.log.info("we wanna websocket, but we don't define WebSocketProxyHandler")
+            self.log.info(
+                "we wanna websocket, but we don't define WebSocketProxyHandler"
+            )
             self.set_status(500)
 
         body = self.request.body
         if not body:
-            if self.request.method in  {'POST', 'PUT'}:
-                body = b''
+            if self.request.method in {"POST", "PUT"}:
+                body = b""
             else:
                 body = None
 
-        client = httpclient.AsyncHTTPClient()
+        if self.unix_socket is not None:
+            # Port points to a Unix domain socket
+            self.log.debug("Making client for Unix socket %r", self.unix_socket)
+            assert host == "localhost", "Unix sockets only possible on localhost"
+            client = SimpleAsyncHTTPClient(resolver=UnixResolver(self.unix_socket))
+        else:
+            client = httpclient.AsyncHTTPClient()
 
         req = self._build_proxy_request(host, port, proxied_path, body)
+
         self.log.debug(f"Proxying request to {req.url}")
 
         try:
             # Here, "response" is a tornado.httpclient.HTTPResponse object.
             response = await client.fetch(req, raise_error=False)
         except httpclient.HTTPError as err:
             # We need to capture the timeout error even with raise_error=False,
@@ -353,19 +382,19 @@
             if isinstance(rewrite_response, (list, tuple)):
                 rewrite_responses = rewrite_response
             else:
                 rewrite_responses = [rewrite_response]
 
             # To be passed on-demand as args to the rewrite_response functions.
             optional_args_to_rewrite_function = {
-                'request': self.request,
-                'orig_response': original_response,
-                'host': host,
-                'port': port,
-                'path': proxied_path
+                "request": self.request,
+                "orig_response": original_response,
+                "host": host,
+                "port": port,
+                "path": proxied_path,
             }
 
             # Initial value for rewriting
             rewritten_response = original_response
 
             for rewrite in rewrite_responses:
                 # The rewrite function is a function of the RewritableResponse object
@@ -373,55 +402,66 @@
                 # convert it to a function of only ``response`` by plugging in the
                 # known values for all the other parameters. (This is called partial
                 # evaluation.)
                 def rewrite_pe(rewritable_response: RewritableResponse):
                     return call_with_asked_args(
                         rewrite,
                         {
-                            'response': rewritable_response,
-                            **optional_args_to_rewrite_function
-                        }
+                            "response": rewritable_response,
+                            **optional_args_to_rewrite_function,
+                        },
                     )
+
                 # Now we can cleanly apply the partially evaulated function to a copy of
                 # the rewritten response.
                 rewritten_response = rewritten_response._apply_to_copy(rewrite_pe)
 
             ## status
             self.set_status(rewritten_response.code, rewritten_response.reason)
 
             # clear tornado default header
             self._headers = httputil.HTTPHeaders()
             for header, v in rewritten_response.headers.get_all():
-                if header not in ('Content-Length', 'Transfer-Encoding',
-                                  'Connection'):
+                if header not in ("Content-Length", "Transfer-Encoding", "Connection"):
                     # some header appear multiple times, eg 'Set-Cookie'
                     self.add_header(header, v)
 
             if rewritten_response.body:
                 self.write(rewritten_response.body)
 
-    async def proxy_open(self, host, port, proxied_path=''):
+    async def proxy_open(self, host, port, proxied_path=""):
         """
         Called when a client opens a websocket connection.
 
         We establish a websocket connection to the proxied backend &
         set up a callback to relay messages through.
         """
 
         if not self._check_host_allowlist(host):
             self.set_status(403)
-            self.log.info("Host '{host}' is not allowed. "
-                          "See https://jupyter-server-proxy.readthedocs.io/en/latest/arbitrary-ports-hosts.html for info.".format(host=host))
+            self.log.info(
+                "Host '{host}' is not allowed. "
+                "See https://jupyter-server-proxy.readthedocs.io/en/latest/arbitrary-ports-hosts.html for info.".format(
+                    host=host
+                )
+            )
             self.close()
             return
 
-        if not proxied_path.startswith('/'):
-            proxied_path = '/' + proxied_path
+        if not proxied_path.startswith("/"):
+            proxied_path = "/" + proxied_path
+
+        if self.unix_socket is not None:
+            assert host == "localhost", "Unix sockets only possible on localhost"
+            self.log.debug("Opening websocket on Unix socket %r", port)
+            resolver = UnixResolver(self.unix_socket)  # Requires tornado >= 6.3
+        else:
+            resolver = None
 
-        client_uri = self.get_client_uri('ws', host, port, proxied_path)
+        client_uri = self.get_client_uri("ws", host, port, proxied_path)
         headers = self.proxy_request_headers()
 
         def message_cb(message):
             """
             Callback when the backend sends messages to us
 
             We just pass it back to the frontend
@@ -440,77 +480,83 @@
 
             We just pass it back to the frontend.
             """
             self._record_activity()
             self.ping(data)
 
         async def start_websocket_connection():
-            self.log.info('Trying to establish websocket connection to {}'.format(client_uri))
+            self.log.info(f"Trying to establish websocket connection to {client_uri}")
             self._record_activity()
             request = httpclient.HTTPRequest(url=client_uri, headers=headers)
-            self.ws = await pingable_ws_connect(request=request,
-                on_message_callback=message_cb, on_ping_callback=ping_cb,
-                subprotocols=self.subprotocols)
+            self.ws = await pingable_ws_connect(
+                request=request,
+                on_message_callback=message_cb,
+                on_ping_callback=ping_cb,
+                subprotocols=self.subprotocols,
+                resolver=resolver,
+            )
             self._record_activity()
-            self.log.info('Websocket connection established to {}'.format(client_uri))
+            self.log.info(f"Websocket connection established to {client_uri}")
 
         # Wait for the WebSocket to be connected before resolving.
         # Otherwise, messages sent by the client before the
         # WebSocket successful connection would be dropped.
         await start_websocket_connection()
 
     def proxy_request_headers(self):
-        '''A dictionary of headers to be used when constructing
-        a tornado.httpclient.HTTPRequest instance for the proxy request.'''
+        """A dictionary of headers to be used when constructing
+        a tornado.httpclient.HTTPRequest instance for the proxy request."""
         headers = self.request.headers.copy()
         # Merge any manually configured request headers
         headers.update(self.get_request_headers_override())
         return headers
 
     def get_request_headers_override(self):
-        '''Add additional request headers. Typically overridden in subclasses.'''
+        """Add additional request headers. Typically overridden in subclasses."""
         return {}
 
     def proxy_request_options(self):
-        '''A dictionary of options to be used when constructing
-        a tornado.httpclient.HTTPRequest instance for the proxy request.'''
-        return dict(follow_redirects=False, connect_timeout=250.0, request_timeout=300.0)
+        """A dictionary of options to be used when constructing
+        a tornado.httpclient.HTTPRequest instance for the proxy request."""
+        return dict(
+            follow_redirects=False, connect_timeout=250.0, request_timeout=300.0
+        )
 
     def check_xsrf_cookie(self):
-        '''
+        """
         http://www.tornadoweb.org/en/stable/guide/security.html
 
         Defer to proxied apps.
-        '''
-        pass
+        """
 
     def select_subprotocol(self, subprotocols):
-        '''Select a single Sec-WebSocket-Protocol during handshake.'''
+        """Select a single Sec-WebSocket-Protocol during handshake."""
         self.subprotocols = subprotocols
         if isinstance(subprotocols, list) and subprotocols:
-            self.log.debug('Client sent subprotocols: {}'.format(subprotocols))
+            self.log.debug(f"Client sent subprotocols: {subprotocols}")
             return subprotocols[0]
         return super().select_subprotocol(subprotocols)
 
 
 class LocalProxyHandler(ProxyHandler):
     """
     A tornado request handler that proxies HTTP and websockets
     from a port on the local system. Same as the above ProxyHandler,
     but specific to 'localhost'.
 
     The arguments "port" and "proxied_path" in each method are extracted from
     the URL as capture groups in the regex specified in the add_handlers
     method.
     """
+
     async def http_get(self, port, proxied_path):
         return await self.proxy(port, proxied_path)
 
     async def open(self, port, proxied_path):
-        return await self.proxy_open('localhost', port, proxied_path)
+        return await self.proxy_open("localhost", port, proxied_path)
 
     def post(self, port, proxied_path):
         return self.proxy(port, proxied_path)
 
     def put(self, port, proxied_path):
         return self.proxy(port, proxied_path)
 
@@ -523,15 +569,16 @@
     def patch(self, port, proxied_path):
         return self.proxy(port, proxied_path)
 
     def options(self, port, proxied_path):
         return self.proxy(port, proxied_path)
 
     def proxy(self, port, proxied_path):
-        return super().proxy('localhost', port, proxied_path)
+        return super().proxy("localhost", port, proxied_path)
+
 
 class RemoteProxyHandler(ProxyHandler):
     """
     A tornado request handler that proxies HTTP and websockets
     from a port on a specified remote system.
 
     The arguments "host", "port" and "proxied_path" in each method are
@@ -562,151 +609,250 @@
 
     async def open(self, host, port, proxied_path):
         return await self.proxy_open(host, port, proxied_path)
 
     def proxy(self, host, port, proxied_path):
         return super().proxy(host, port, proxied_path)
 
+
+class NamedLocalProxyHandler(LocalProxyHandler):
+    """
+    A tornado request handler that proxies HTTP and websockets from a port on
+    the local system. The port is specified in config, and associated with a
+    name which forms part of the URL.
+
+    Config will create a subclass of this for each named proxy. A further
+    subclass below is used for named proxies where we also start the server.
+    """
+
+    port = 0
+    mappath = {}
+
+    @property
+    def process_args(self):
+        return {
+            "port": self.port,
+            "unix_socket": (self.unix_socket or ""),
+            "base_url": self.base_url,
+        }
+
+    def _render_template(self, value):
+        args = self.process_args
+        if type(value) is str:
+            return value.format(**args)
+        elif type(value) is list:
+            return [self._render_template(v) for v in value]
+        elif type(value) is dict:
+            return {
+                self._render_template(k): self._render_template(v)
+                for k, v in value.items()
+            }
+        else:
+            raise ValueError(f"Value of unrecognized type {type(value)}")
+
+    def _realize_rendered_template(self, attribute):
+        """Call any callables, then render any templated values."""
+        if callable(attribute):
+            attribute = self._render_template(
+                call_with_asked_args(attribute, self.process_args)
+            )
+        return self._render_template(attribute)
+
+    @web.authenticated
+    async def proxy(self, port, path):
+        if not path.startswith("/"):
+            path = "/" + path
+        if self.mappath:
+            if callable(self.mappath):
+                path = call_with_asked_args(self.mappath, {"path": path})
+            else:
+                path = self.mappath.get(path, path)
+
+        return await ensure_async(super().proxy(port, path))
+
+    async def http_get(self, path):
+        return await ensure_async(self.proxy(self.port, path))
+
+    async def open(self, path):
+        return await super().open(self.port, path)
+
+    def post(self, path):
+        return self.proxy(self.port, path)
+
+    def put(self, path):
+        return self.proxy(self.port, path)
+
+    def delete(self, path):
+        return self.proxy(self.port, path)
+
+    def head(self, path):
+        return self.proxy(self.port, path)
+
+    def patch(self, path):
+        return self.proxy(self.port, path)
+
+    def options(self, path):
+        return self.proxy(self.port, path)
+
+
 # FIXME: Move this to its own file. Too many packages now import this from nbrserverproxy.handlers
-class SuperviseAndProxyHandler(LocalProxyHandler):
-    '''Manage a given process and requests to it '''
+class SuperviseAndProxyHandler(NamedLocalProxyHandler):
+    """
+    A tornado request handler that proxies HTTP and websockets from a local
+    process which is launched on demand to handle requests. The command and
+    other process options are specified in config.
+
+    A subclass of this will be made for each configured server process.
+    """
 
     def __init__(self, *args, **kwargs):
         self.requested_port = 0
+        self.requested_unix_socket = False
         self.mappath = {}
+        self.command = list()
         super().__init__(*args, **kwargs)
 
     def initialize(self, state):
         self.state = state
-        if 'proc_lock' not in state:
-            state['proc_lock'] = Lock()
+        if "proc_lock" not in state:
+            state["proc_lock"] = Lock()
 
-    name = 'process'
+    name = "process"
 
     @property
     def port(self):
         """
         Allocate either the requested port or a random empty port for use by
         application
         """
-        if 'port' not in self.state:
-            sock = socket.socket()
-            sock.bind(('', self.requested_port))
-            self.state['port'] = sock.getsockname()[1]
-            sock.close()
-        return self.state['port']
+        if self.requested_unix_socket:  # unix_socket has priority over port
+            return 0
+
+        if "port" not in self.state:
+            if self.requested_port:
+                self.state["port"] = self.requested_port
+            else:
+                sock = socket.socket()
+                sock.bind(("", self.requested_port))
+                self.state["port"] = sock.getsockname()[1]
+                sock.close()
+
+        return self.state["port"]
+
+    @property
+    def unix_socket(self):
+        if "unix_socket" not in self.state:
+            if self.requested_unix_socket is True:
+                sock_dir = mkdtemp(prefix="jupyter-server-proxy-")
+                sock_path = os.path.join(sock_dir, "socket")
+            elif self.requested_unix_socket:
+                sock_path = self.requested_unix_socket
+            else:
+                sock_path = None
+            self.state["unix_socket"] = sock_path
+        return self.state["unix_socket"]
+
+    def get_cmd(self):
+        return self._realize_rendered_template(self.command)
 
     def get_cwd(self):
         """Get the current working directory for our process
 
         Override in subclass to launch the process in a directory
         other than the current.
         """
         return os.getcwd()
 
     def get_env(self):
-        '''Set up extra environment variables for process. Typically
-           overridden in subclasses.'''
+        """Set up extra environment variables for process. Typically
+        overridden in subclasses."""
         return {}
 
     def get_timeout(self):
         """
         Return timeout (in s) to wait before giving up on process readiness
         """
         return 5
 
     async def _http_ready_func(self, p):
-        url = 'http://localhost:{}'.format(self.port)
-        async with aiohttp.ClientSession() as session:
+        if self.unix_socket is not None:
+            url = "http://localhost"
+            connector = aiohttp.UnixConnector(self.unix_socket)
+        else:
+            url = f"http://localhost:{self.port}"
+            connector = None  # Default, TCP connector
+        async with aiohttp.ClientSession(connector=connector) as session:
             try:
                 async with session.get(url, allow_redirects=False) as resp:
                     # We only care if we get back *any* response, not just 200
                     # If there's an error response, that can be shown directly to the user
-                    self.log.debug('Got code {} back from {}'.format(resp.status, url))
+                    self.log.debug(f"Got code {resp.status} back from {url}")
                     return True
             except aiohttp.ClientConnectionError:
-                self.log.debug('Connection to {} refused'.format(url))
+                self.log.debug(f"Connection to {url} refused")
                 return False
 
     async def ensure_process(self):
         """
         Start the process
         """
         # We don't want multiple requests trying to start the process at the same time
         # FIXME: Make sure this times out properly?
         # Invariant here should be: when lock isn't being held, either 'proc' is in state &
         # running, or not.
-        async with self.state['proc_lock']:
-            if 'proc' not in self.state:
+        async with self.state["proc_lock"]:
+            if "proc" not in self.state:
                 # FIXME: Prevent races here
                 # FIXME: Handle graceful exits of spawned processes here
+
+                # When command option isn't truthy, it means its a process not
+                # to be managed/started by jupyter-server-proxy. This means we
+                # won't await its readiness or similar either.
                 cmd = self.get_cmd()
+                if not cmd:
+                    self.state["proc"] = "process not managed by jupyter-server-proxy"
+                    return
 
                 # Set up extra environment variables for process
                 server_env = os.environ.copy()
                 server_env.update(self.get_env())
 
                 timeout = self.get_timeout()
 
-                proc = SupervisedProcess(self.name, *cmd, env=server_env, ready_func=self._http_ready_func, ready_timeout=timeout, log=self.log)
-                self.state['proc'] = proc
+                proc = SupervisedProcess(
+                    self.name,
+                    *cmd,
+                    env=server_env,
+                    ready_func=self._http_ready_func,
+                    ready_timeout=timeout,
+                    log=self.log,
+                )
+                self.state["proc"] = proc
 
                 try:
                     await proc.start()
 
                     is_ready = await proc.ready()
 
                     if not is_ready:
                         await proc.kill()
-                        raise web.HTTPError(500, 'could not start {} in time'.format(self.name))
+                        raise web.HTTPError(500, f"could not start {self.name} in time")
                 except:
                     # Make sure we remove proc from state in any error condition
-                    del self.state['proc']
+                    del self.state["proc"]
                     raise
 
-
     @web.authenticated
     async def proxy(self, port, path):
-        if not path.startswith('/'):
-            path = '/' + path
-        if self.mappath:
-            if callable(self.mappath):
-                path = call_with_asked_args(self.mappath, {'path': path})
-            else:
-                path = self.mappath.get(path, path)
-
         await self.ensure_process()
-
-        return await ensure_async(super().proxy(self.port, path))
-
-
-    async def http_get(self, path):
-        return await ensure_async(self.proxy(self.port, path))
+        return await ensure_async(super().proxy(port, path))
 
     async def open(self, path):
         await self.ensure_process()
-        return await super().open(self.port, path)
-
-    def post(self, path):
-        return self.proxy(self.port, path)
-
-    def put(self, path):
-        return self.proxy(self.port, path)
-
-    def delete(self, path):
-        return self.proxy(self.port, path)
-
-    def head(self, path):
-        return self.proxy(self.port, path)
-
-    def patch(self, path):
-        return self.proxy(self.port, path)
-
-    def options(self, path):
-        return self.proxy(self.port, path)
+        return await super().open(path)
 
 
 def setup_handlers(web_app, serverproxy_config):
     host_allowlist = serverproxy_config.host_allowlist
     rewrite_response = serverproxy_config.non_service_rewrite_response
     web_app.add_handlers(
         ".*",
@@ -755,10 +901,7 @@
                 {
                     "absolute_url": True,
                     "rewrite_response": rewrite_response,
                 },
             ),
         ],
     )
-
-
-# vim: set et ts=4 sw=4:
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/package.json` & `jupyter_server_proxy-4.0.0/labextension/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7976102941176472%*

 * *Differences: {"'description'": "'A JupyterLab extension accompanying the PyPI package jupyter-server-proxy "*

 * *                  "adding launcher items for configured server processes.'",*

 * * "'devDependencies'": "{'rimraf': '^3.0.2', 'typescript': '~4.8.4', 'yarn-deduplicate': '^6.0.0', "*

 * *                      "'npm-run-all': '^4.1.5'}",*

 * * "'files'": "{insert: [(0, 'LICENSE')], delete: [1]}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'name'": "'@jupyterhub/jupyter-server-proxy'",*

 * * "'resolutions'": "OrderedDict([('loader-uti […]*

```diff
@@ -6,58 +6,58 @@
     "bugs": {
         "url": "https://github.com/jupyterhub/jupyter-server-proxy/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^2.0 || ^3.0",
         "@jupyterlab/launcher": "^2.0 || ^3.0"
     },
-    "description": "Jupyter server extension to supervise and proxy web services",
+    "description": "A JupyterLab extension accompanying the PyPI package jupyter-server-proxy adding launcher items for configured server processes.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.2.4",
-        "rimraf": "^2.6.1",
-        "typescript": "~3.7.0"
+        "npm-run-all": "^4.1.5",
+        "rimraf": "^3.0.2",
+        "typescript": "~4.8.4",
+        "yarn-deduplicate": "^6.0.0"
     },
     "files": [
-        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "LICENSE",
+        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterhub/jupyter-server-proxy",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.e84826446ca2e8c10352.js"
-        },
         "extension": true,
         "outputDir": "../jupyter_server_proxy/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "@jupyterlab/server-proxy",
+    "name": "@jupyterhub/jupyter-server-proxy",
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterhub/jupyter-server-proxy.git"
     },
+    "resolutions": {
+        "loader-utils": ">=2.0.3"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "build:lib": "tsc -b",
+        "build:prod": "jlpm clean && jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyter_server_proxy/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
+        "deduplicate": "yarn-deduplicate -s fewer --fail",
         "install:extension": "jupyter labextension develop --overwrite .",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "jlpm build:lib -w --preserveWatchOutput"
     },
     "types": "lib/index.d.ts",
-    "version": "3.2.2"
+    "version": "4.0.0"
 }
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/568.f25cbf5a25d42e5d9003.js` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/568.d5fa5a0c0d3b0516bea8.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,106 +1,81 @@
 "use strict";
-(self.webpackChunk_jupyterlab_server_proxy = self.webpackChunk_jupyterlab_server_proxy || []).push([
+(self.webpackChunk_jupyterhub_jupyter_server_proxy = self.webpackChunk_jupyterhub_jupyter_server_proxy || []).push([
     [568], {
-        568: function(e, t, r) {
-            var n = this && this.__awaiter || function(e, t, r, n) {
-                return new(r || (r = Promise))((function(o, a) {
-                    function l(e) {
-                        try {
-                            i(n.next(e))
-                        } catch (e) {
-                            a(e)
-                        }
-                    }
-
-                    function s(e) {
-                        try {
-                            i(n.throw(e))
-                        } catch (e) {
-                            a(e)
-                        }
-                    }
-
-                    function i(e) {
-                        var t;
-                        e.done ? o(e.value) : (t = e.value, t instanceof r ? t : new r((function(e) {
-                            e(t)
-                        }))).then(l, s)
-                    }
-                    i((n = n.apply(e, t || [])).next())
-                }))
-            };
-            Object.defineProperty(t, "__esModule", {
-                value: !0
+        568: (e, r, t) => {
+            t.r(r), t.d(r, {
+                default: () => s
             });
-            const o = r(782),
-                a = r(814),
-                l = r(484),
-                s = r(58),
-                i = {
-                    id: "jupyterlab-server-proxy",
-                    autoStart: !0,
-                    requires: [a.ILauncher, o.ILayoutRestorer],
-                    activate: function(e, t, r) {
-                        return n(this, void 0, void 0, (function*() {
-                            const n = yield fetch(l.PageConfig.getBaseUrl() + "server-proxy/servers-info");
-                            if (!n.ok) return console.log("Could not fetch metadata about registered servers. Make sure jupyter-server-proxy is installed."), void console.log(n);
-                            const {
-                                commands: o,
-                                shell: a
-                            } = e, i = yield n.json(), c = "server-proxy", u = new s.WidgetTracker({
-                                namespace: c
-                            }), d = c + ":open";
-                            r && r.restore(u, {
-                                command: d,
-                                args: e => ({
-                                    url: e.content.url,
-                                    title: e.content.title.label,
-                                    newBrowserTab: !1,
-                                    id: e.content.id
-                                }),
-                                name: e => e.content.id
-                            }), o.addCommand(d, {
-                                label: e => e.title,
-                                execute: e => {
-                                    const t = e.id,
-                                        r = e.title,
-                                        n = e.url;
-                                    if (e.newBrowserTab) return void window.open(n, "_blank");
-                                    let o = u.find((e => e.content.id == t));
-                                    if (o || (o = function(e, t, r) {
-                                            const n = new s.IFrame({
-                                                sandbox: ["allow-same-origin", "allow-scripts", "allow-popups", "allow-forms", "allow-downloads", "allow-modals"]
-                                            });
-                                            n.title.label = r, n.title.closable = !0, n.url = t, n.addClass("jp-ServerProxy"), n.id = e;
-                                            const o = new s.MainAreaWidget({
-                                                content: n
-                                            });
-                                            return o.addClass("jp-ServerProxy"), o
-                                        }(t, n, r)), u.has(o) || u.add(o), !o.isAttached) return a.add(o), o;
-                                    a.activateById(o.id)
-                                }
-                            });
-                            for (let e of i.server_processes) {
-                                if (!e.launcher_entry.enabled) continue;
-                                const r = l.PageConfig.getBaseUrl() + e.launcher_entry.path_info,
-                                    n = e.launcher_entry.title,
-                                    o = e.new_browser_tab,
-                                    a = {
-                                        command: d,
-                                        args: {
-                                            url: r,
-                                            title: n + (o ? " [↗]" : ""),
-                                            newBrowserTab: o,
-                                            id: c + ":" + e.name
-                                        },
-                                        category: "Notebook"
-                                    };
-                                e.launcher_entry.icon_url && (a.kernelIconUrl = e.launcher_entry.icon_url), t.add(a)
-                            }
-                        }))
+            var n = t(687),
+                o = t(467),
+                a = t(142),
+                l = t(33);
+            const s = {
+                id: "@jupyterhub/jupyter-server-proxy:add-launcher-entries",
+                autoStart: !0,
+                requires: [o.ILauncher, n.ILayoutRestorer],
+                activate: async function(e, r, t) {
+                    const n = await fetch(a.PageConfig.getBaseUrl() + "server-proxy/servers-info");
+                    if (!n.ok) return console.log("Could not fetch metadata about registered servers. Make sure jupyter-server-proxy is installed."), void console.log(n);
+                    const o = await n.json(),
+                        s = "server-proxy",
+                        i = new l.WidgetTracker({
+                            namespace: s
+                        }),
+                        c = s + ":open";
+                    t && t.restore(i, {
+                        command: c,
+                        args: e => ({
+                            url: e.content.url,
+                            title: e.content.title.label,
+                            newBrowserTab: !1,
+                            id: e.content.id
+                        }),
+                        name: e => e.content.id
+                    });
+                    const {
+                        commands: d,
+                        shell: u
+                    } = e;
+                    d.addCommand(c, {
+                        label: e => e.title,
+                        execute: e => {
+                            const r = e.id,
+                                t = e.title,
+                                n = e.url;
+                            if (e.newBrowserTab) return void window.open(n, "_blank");
+                            let o = i.find((e => e.content.id == r));
+                            if (o || (o = function(e, r, t) {
+                                    const n = new l.IFrame({
+                                        sandbox: ["allow-same-origin", "allow-scripts", "allow-popups", "allow-forms", "allow-downloads", "allow-modals"]
+                                    });
+                                    n.title.label = t, n.title.closable = !0, n.url = r, n.addClass("jp-ServerProxy"), n.id = e;
+                                    const o = new l.MainAreaWidget({
+                                        content: n
+                                    });
+                                    return o.addClass("jp-ServerProxy"), o
+                                }(r, n, t)), i.has(o) || i.add(o), !o.isAttached) return u.add(o), o;
+                            u.activateById(o.id)
+                        }
+                    });
+                    for (let e of o.server_processes) {
+                        if (!e.launcher_entry.enabled) continue;
+                        const t = a.PageConfig.getBaseUrl() + e.launcher_entry.path_info,
+                            n = e.launcher_entry.title,
+                            o = e.new_browser_tab,
+                            l = {
+                                command: c,
+                                args: {
+                                    url: t,
+                                    title: n + (o ? " [↗]" : ""),
+                                    newBrowserTab: o,
+                                    id: s + ":" + e.name
+                                },
+                                category: "Notebook"
+                            };
+                        e.launcher_entry.icon_url && (l.kernelIconUrl = e.launcher_entry.icon_url), r.add(l)
                     }
-                };
-            t.default = i
+                }
+            }
         }
     }
 ]);
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/labextension/static/remoteEntry.e84826446ca2e8c10352.js` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/static/remoteEntry.6bef4394de3b3e455a6a.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,113 +1,124 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, p, f, d, c, h, v = {
-            576: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, p, s, f, d, h, c, v = {
+            16: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
-                            var n = t.S.default,
-                                o = "default";
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[o] = e, t.I(o, r)
+                            var n = "default",
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
         y = {};
 
-    function g(e) {
+    function b(e) {
         var r = y[e];
         if (void 0 !== r) return r.exports;
         var t = y[e] = {
             exports: {}
         };
-        return v[e].call(t.exports, t, t.exports, g), t.exports
+        return v[e](t, t.exports, b), t.exports
     }
-    g.m = v, g.c = y, g.d = (e, r) => {
-        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
+    b.m = v, b.c = y, b.n = e => {
+        var r = e && e.__esModule ? () => e.default : () => e;
+        return b.d(r, {
+            a: r
+        }), r
+    }, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".f25cbf5a25d42e5d9003.js?v=f25cbf5a25d42e5d9003", g.g = function() {
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + ".d5fa5a0c0d3b0516bea8.js?v=d5fa5a0c0d3b0516bea8", b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/server-proxy:", g.l = (t, n, o, a) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterhub/jupyter-server-proxy:", b.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var p = l[s];
-                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
-                        i = p;
+                for (var l = document.getElementsByTagName("script"), p = 0; p < l.length; p++) {
+                    var s = l[p];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, b.nc && i.setAttribute("nonce", b.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 d = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
+    }, b.r = e => {
+        "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
+            value: "Module"
+        }), Object.defineProperty(e, "__esModule", {
+            value: !0
+        })
     }, (() => {
-        g.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        g.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                g.o(g.S, t) || (g.S[t] = {});
-                var a = g.S[t],
-                    i = "@jupyterlab/server-proxy",
+                b.o(b.S, t) || (b.S[t] = {});
+                var a = b.S[t],
+                    i = "@jupyterhub/jupyter-server-proxy",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
-                        get: () => g.e(568).then((() => () => g(568))),
+                        get: () => b.e(568).then((() => () => b(568))),
                         from: i,
                         eager: !1
                     })
-                })("@jupyterlab/server-proxy", "3.2.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("@jupyterhub/jupyter-server-proxy", "4.0.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        g.g.importScripts && (e = g.g.location + "");
-        var r = g.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -144,112 +155,112 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, p, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (p = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
-                if ("u" == p) {
+                var p, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(p = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
                     if (!l || "u" != f) return !1
                 } else if (l)
-                    if (f == p)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (p != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? p > e[u] : p < e[u]) return !1;
+                            p != e[u] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || p < f != o) return !1;
+                    if (u <= n || s < f != o) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var d = [],
-            c = d.pop.bind(d);
+            h = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            var c = e[i];
+            d.push(1 == c ? h() | h() : 2 == c ? h() & h() : c ? a(c, r) : !h())
         }
-        return !!c()
+        return !!h()
     }, i = (e, r) => {
-        var t = g.S[e];
-        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", p = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), p(e[t][o])
-    }, p = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
-        var a = g.I(r);
-        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), d = {}, c = {
-        782: () => f("default", "@jupyterlab/application", [1, 3, 4, 6]),
-        814: () => f("default", "@jupyterlab/launcher", [1, 3, 4, 6]),
-        484: () => f("default", "@jupyterlab/coreutils", [1, 5, 4, 6]),
-        58: () => f("default", "@jupyterlab/apputils", [1, 3, 4, 6])
-    }, h = {
-        568: [782, 814, 484, 58]
-    }, g.f.consumes = (e, r) => {
-        g.o(h, e) && h[e].forEach((e => {
-            if (g.o(d, e)) return r.push(d[e]);
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
+        var a = b.I(r);
+        return a && a.then ? a.then(e.bind(e, r, b.S[r], t, n, o)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), p(r, 0, t, n)))), d = {}, h = {
+        687: () => f("default", "@jupyterlab/application", [1, 3, 6, 3]),
+        467: () => f("default", "@jupyterlab/launcher", [1, 3, 6, 3]),
+        142: () => f("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
+        33: () => f("default", "@jupyterlab/apputils", [1, 3, 6, 3])
+    }, c = {
+        568: [687, 467, 142, 33]
+    }, b.f.consumes = (e, r) => {
+        b.o(c, e) && c[e].forEach((e => {
+            if (b.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    d[e] = 0, g.m[e] = t => {
-                        delete g.c[e], t.exports = r()
+                    d[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete d[e], g.m[e] = t => {
-                        throw delete g.c[e], r
+                    delete d[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
+                var o = h[e]();
                 o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
-            800: 0
+            964: 0
         };
-        g.f.j = (r, t) => {
-            var n = g.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var a = g.p + g.u(r),
+                    var a = b.p + b.u(r),
                         i = new Error;
-                    g.l(a, (t => {
-                        if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    b.l(a, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) g.o(i, n) && (g.m[n] = i[n]);
-                    u && u(g)
+                    for (n in i) b.o(i, n) && (b.m[n] = i[n]);
+                    u && u(b)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], g.o(e, o) && e[o] && e[o][0](), e[a[l]] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
-            t = self.webpackChunk_jupyterlab_server_proxy = self.webpackChunk_jupyterlab_server_proxy || [];
+            t = self.webpackChunk_jupyterhub_jupyter_server_proxy = self.webpackChunk_jupyterhub_jupyter_server_proxy || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var b = g(576);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/server-proxy"] = b
+    var g = b(16);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterhub/jupyter-server-proxy"] = g
 })();
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/utils.py` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 from traitlets import TraitType
 
+
 def call_with_asked_args(callback, args):
     """
     Call callback with only the args it wants from args
 
     Example
     >>> def cb(a):
     ...    return a * 5
 
     >>> print(call_with_asked_args(cb, {'a': 4, 'b': 8}))
     20
     """
     # FIXME: support default args
     # FIXME: support kwargs
-    # co_varnames contains both args and local variables, in order. 
+    # co_varnames contains both args and local variables, in order.
     # We only pick the local variables
-    asked_arg_names = callback.__code__.co_varnames[:callback.__code__.co_argcount]
+    asked_arg_names = callback.__code__.co_varnames[: callback.__code__.co_argcount]
     asked_arg_values = []
     missing_args = []
     for asked_arg_name in asked_arg_names:
         if asked_arg_name in args:
             asked_arg_values.append(args[asked_arg_name])
         else:
             missing_args.append(asked_arg_name)
     if missing_args:
         raise TypeError(
-            '{}() missing required positional argument: {}'.format(
-                callback.__code__.co_name,
-                ', '.join(missing_args)
+            "{}() missing required positional argument: {}".format(
+                callback.__code__.co_name, ", ".join(missing_args)
             )
         )
     return callback(*asked_arg_values)
 
+
 # copy-pasted from the ipython/traitlets source code, see
 # https://github.com/ipython/traitlets/blob/a1425327460c4a3ae970aeaef17e0c22da4c53c6/traitlets/traitlets.py#L3232-L3246
 class Callable(TraitType):
     """A trait which is callable.
     Notes
     -----
     Classes are callable, as are instances
     with a __call__() method."""
 
-    info_text = 'a callable'
+    info_text = "a callable"
 
     def validate(self, obj, value):
         if callable(value):
             return value
         else:
             self.error(obj, value)
```

### Comparing `jupyter-server-proxy-3.2.2/jupyter_server_proxy/websocket.py` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/websocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,113 @@
 """
 Authenticated HTTP proxy for Jupyter Notebooks
 
 Some original inspiration from https://github.com/senko/tornado-proxy
 """
 
 import inspect
-import socket
-import os
-from urllib.parse import urlunparse, urlparse
-
-from tornado import gen, web, httpclient, httputil, process, websocket, ioloop, version_info
-
-from jupyter_server.utils import url_path_join
-from jupyter_server.base.handlers import JupyterHandler, utcnow
 
 from jupyter_server.utils import ensure_async
+from tornado import httpclient, httputil, ioloop, version_info, websocket
 
 
 class PingableWSClientConnection(websocket.WebSocketClientConnection):
     """A WebSocketClientConnection with an on_ping callback."""
+
     def __init__(self, **kwargs):
-        if 'on_ping_callback' in kwargs:
-            self._on_ping_callback = kwargs['on_ping_callback']
-            del(kwargs['on_ping_callback'])
+        if "on_ping_callback" in kwargs:
+            self._on_ping_callback = kwargs["on_ping_callback"]
+            del kwargs["on_ping_callback"]
         super().__init__(**kwargs)
 
     def on_ping(self, data):
         if self._on_ping_callback:
             self._on_ping_callback(data)
 
 
-def pingable_ws_connect(request=None,on_message_callback=None,
-                        on_ping_callback=None, subprotocols=None):
+def pingable_ws_connect(
+    request=None,
+    on_message_callback=None,
+    on_ping_callback=None,
+    subprotocols=None,
+    resolver=None,
+):
     """
     A variation on websocket_connect that returns a PingableWSClientConnection
     with on_ping_callback.
     """
     # Copy and convert the headers dict/object (see comments in
     # AsyncHTTPClient.fetch)
     request.headers = httputil.HTTPHeaders(request.headers)
-    request = httpclient._RequestProxy(
-        request, httpclient.HTTPRequest._DEFAULTS)
+    request = httpclient._RequestProxy(request, httpclient.HTTPRequest._DEFAULTS)
 
     # for tornado 4.5.x compatibility
     if version_info[0] == 4:
-        conn = PingableWSClientConnection(io_loop=ioloop.IOLoop.current(),
+        conn = PingableWSClientConnection(
+            io_loop=ioloop.IOLoop.current(),
             compression_options={},
             request=request,
             on_message_callback=on_message_callback,
-            on_ping_callback=on_ping_callback)
+            on_ping_callback=on_ping_callback,
+        )
     else:
-        conn = PingableWSClientConnection(request=request,
+        # resolver= parameter requires tornado >= 6.3. Only pass it if needed
+        # (for Unix socket support), so older versions of tornado can still
+        # work otherwise.
+        kwargs = {"resolver": resolver} if resolver else {}
+        conn = PingableWSClientConnection(
+            request=request,
             compression_options={},
             on_message_callback=on_message_callback,
             on_ping_callback=on_ping_callback,
-            max_message_size=getattr(websocket, '_default_max_message_size', 10 * 1024 * 1024),
-            subprotocols=subprotocols)
+            max_message_size=getattr(
+                websocket, "_default_max_message_size", 10 * 1024 * 1024
+            ),
+            subprotocols=subprotocols,
+            **kwargs,
+        )
 
     return conn.connect_future
 
+
 # from https://stackoverflow.com/questions/38663666/how-can-i-serve-a-http-page-and-a-websocket-on-the-same-url-in-tornado
 class WebSocketHandlerMixin(websocket.WebSocketHandler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # since my parent doesn't keep calling the super() constructor,
         # I need to do it myself
         bases = inspect.getmro(type(self))
         assert WebSocketHandlerMixin in bases
         meindex = bases.index(WebSocketHandlerMixin)
         try:
             nextparent = bases[meindex + 1]
         except IndexError:
-            raise Exception("WebSocketHandlerMixin should be followed "
-                            "by another parent to make sense")
+            raise Exception(
+                "WebSocketHandlerMixin should be followed "
+                "by another parent to make sense"
+            )
 
         # undisallow methods --- t.ws.WebSocketHandler disallows methods,
         # we need to re-enable these methods
         def wrapper(method):
             def undisallow(*args2, **kwargs2):
                 getattr(nextparent, method)(self, *args2, **kwargs2)
+
             return undisallow
 
-        for method in ["write", "redirect", "set_header", "set_cookie",
-                       "set_status", "flush", "finish"]:
+        for method in [
+            "write",
+            "redirect",
+            "set_header",
+            "set_cookie",
+            "set_status",
+            "flush",
+            "finish",
+        ]:
             setattr(self, method, wrapper(method))
         nextparent.__init__(self, *args, **kwargs)
 
     async def get(self, *args, **kwargs):
-        if self.request.headers.get("Upgrade", "").lower() != 'websocket':
+        if self.request.headers.get("Upgrade", "").lower() != "websocket":
             return await self.http_get(*args, **kwargs)
         else:
             await ensure_async(super().get(*args, **kwargs))
-
-
-def setup_handlers(web_app):
-    web_app.add_handlers('.*', [
-        (url_path_join(web_app.settings['base_url'], r'/proxy/(\d+)(.*)'), LocalProxyHandler)
-    ])
-
-# vim: set et ts=4 sw=4:
```

### Comparing `jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/lib/index.js` & `jupyter_server_proxy-4.0.0/labextension/src/index.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,304 +1,261 @@
-00000000: 2275 7365 2073 7472 6963 7422 3b0a 7661  "use strict";.va
-00000010: 7220 5f5f 6177 6169 7465 7220 3d20 2874  r __awaiter = (t
-00000020: 6869 7320 2626 2074 6869 732e 5f5f 6177  his && this.__aw
-00000030: 6169 7465 7229 207c 7c20 6675 6e63 7469  aiter) || functi
-00000040: 6f6e 2028 7468 6973 4172 672c 205f 6172  on (thisArg, _ar
-00000050: 6775 6d65 6e74 732c 2050 2c20 6765 6e65  guments, P, gene
-00000060: 7261 746f 7229 207b 0a20 2020 2066 756e  rator) {.    fun
-00000070: 6374 696f 6e20 6164 6f70 7428 7661 6c75  ction adopt(valu
-00000080: 6529 207b 2072 6574 7572 6e20 7661 6c75  e) { return valu
-00000090: 6520 696e 7374 616e 6365 6f66 2050 203f  e instanceof P ?
-000000a0: 2076 616c 7565 203a 206e 6577 2050 2866   value : new P(f
-000000b0: 756e 6374 696f 6e20 2872 6573 6f6c 7665  unction (resolve
-000000c0: 2920 7b20 7265 736f 6c76 6528 7661 6c75  ) { resolve(valu
-000000d0: 6529 3b20 7d29 3b20 7d0a 2020 2020 7265  e); }); }.    re
-000000e0: 7475 726e 206e 6577 2028 5020 7c7c 2028  turn new (P || (
-000000f0: 5020 3d20 5072 6f6d 6973 6529 2928 6675  P = Promise))(fu
-00000100: 6e63 7469 6f6e 2028 7265 736f 6c76 652c  nction (resolve,
-00000110: 2072 656a 6563 7429 207b 0a20 2020 2020   reject) {.     
-00000120: 2020 2066 756e 6374 696f 6e20 6675 6c66     function fulf
-00000130: 696c 6c65 6428 7661 6c75 6529 207b 2074  illed(value) { t
-00000140: 7279 207b 2073 7465 7028 6765 6e65 7261  ry { step(genera
-00000150: 746f 722e 6e65 7874 2876 616c 7565 2929  tor.next(value))
-00000160: 3b20 7d20 6361 7463 6820 2865 2920 7b20  ; } catch (e) { 
-00000170: 7265 6a65 6374 2865 293b 207d 207d 0a20  reject(e); } }. 
-00000180: 2020 2020 2020 2066 756e 6374 696f 6e20         function 
-00000190: 7265 6a65 6374 6564 2876 616c 7565 2920  rejected(value) 
-000001a0: 7b20 7472 7920 7b20 7374 6570 2867 656e  { try { step(gen
-000001b0: 6572 6174 6f72 5b22 7468 726f 7722 5d28  erator["throw"](
-000001c0: 7661 6c75 6529 293b 207d 2063 6174 6368  value)); } catch
-000001d0: 2028 6529 207b 2072 656a 6563 7428 6529   (e) { reject(e)
-000001e0: 3b20 7d20 7d0a 2020 2020 2020 2020 6675  ; } }.        fu
-000001f0: 6e63 7469 6f6e 2073 7465 7028 7265 7375  nction step(resu
-00000200: 6c74 2920 7b20 7265 7375 6c74 2e64 6f6e  lt) { result.don
-00000210: 6520 3f20 7265 736f 6c76 6528 7265 7375  e ? resolve(resu
-00000220: 6c74 2e76 616c 7565 2920 3a20 6164 6f70  lt.value) : adop
-00000230: 7428 7265 7375 6c74 2e76 616c 7565 292e  t(result.value).
-00000240: 7468 656e 2866 756c 6669 6c6c 6564 2c20  then(fulfilled, 
-00000250: 7265 6a65 6374 6564 293b 207d 0a20 2020  rejected); }.   
-00000260: 2020 2020 2073 7465 7028 2867 656e 6572       step((gener
-00000270: 6174 6f72 203d 2067 656e 6572 6174 6f72  ator = generator
-00000280: 2e61 7070 6c79 2874 6869 7341 7267 2c20  .apply(thisArg, 
-00000290: 5f61 7267 756d 656e 7473 207c 7c20 5b5d  _arguments || []
-000002a0: 2929 2e6e 6578 7428 2929 3b0a 2020 2020  )).next());.    
-000002b0: 7d29 3b0a 7d3b 0a4f 626a 6563 742e 6465  });.};.Object.de
-000002c0: 6669 6e65 5072 6f70 6572 7479 2865 7870  fineProperty(exp
-000002d0: 6f72 7473 2c20 225f 5f65 734d 6f64 756c  orts, "__esModul
-000002e0: 6522 2c20 7b20 7661 6c75 653a 2074 7275  e", { value: tru
-000002f0: 6520 7d29 3b0a 636f 6e73 7420 6170 706c  e });.const appl
-00000300: 6963 6174 696f 6e5f 3120 3d20 7265 7175  ication_1 = requ
-00000310: 6972 6528 2240 6a75 7079 7465 726c 6162  ire("@jupyterlab
-00000320: 2f61 7070 6c69 6361 7469 6f6e 2229 3b0a  /application");.
-00000330: 636f 6e73 7420 6c61 756e 6368 6572 5f31  const launcher_1
-00000340: 203d 2072 6571 7569 7265 2822 406a 7570   = require("@jup
-00000350: 7974 6572 6c61 622f 6c61 756e 6368 6572  yterlab/launcher
-00000360: 2229 3b0a 636f 6e73 7420 636f 7265 7574  ");.const coreut
-00000370: 696c 735f 3120 3d20 7265 7175 6972 6528  ils_1 = require(
-00000380: 2240 6a75 7079 7465 726c 6162 2f63 6f72  "@jupyterlab/cor
-00000390: 6575 7469 6c73 2229 3b0a 636f 6e73 7420  eutils");.const 
-000003a0: 6170 7075 7469 6c73 5f31 203d 2072 6571  apputils_1 = req
-000003b0: 7569 7265 2822 406a 7570 7974 6572 6c61  uire("@jupyterla
-000003c0: 622f 6170 7075 7469 6c73 2229 3b0a 6675  b/apputils");.fu
-000003d0: 6e63 7469 6f6e 206e 6577 5365 7276 6572  nction newServer
-000003e0: 5072 6f78 7957 6964 6765 7428 6964 2c20  ProxyWidget(id, 
-000003f0: 7572 6c2c 2074 6578 7429 207b 0a20 2020  url, text) {.   
-00000400: 2063 6f6e 7374 2063 6f6e 7465 6e74 203d   const content =
-00000410: 206e 6577 2061 7070 7574 696c 735f 312e   new apputils_1.
-00000420: 4946 7261 6d65 287b 0a20 2020 2020 2020  IFrame({.       
-00000430: 2073 616e 6462 6f78 3a20 5b27 616c 6c6f   sandbox: ['allo
-00000440: 772d 7361 6d65 2d6f 7269 6769 6e27 2c20  w-same-origin', 
-00000450: 2761 6c6c 6f77 2d73 6372 6970 7473 272c  'allow-scripts',
-00000460: 2027 616c 6c6f 772d 706f 7075 7073 272c   'allow-popups',
-00000470: 2027 616c 6c6f 772d 666f 726d 7327 2c20   'allow-forms', 
-00000480: 2761 6c6c 6f77 2d64 6f77 6e6c 6f61 6473  'allow-downloads
-00000490: 272c 2027 616c 6c6f 772d 6d6f 6461 6c73  ', 'allow-modals
-000004a0: 275d 2c0a 2020 2020 7d29 3b0a 2020 2020  '],.    });.    
-000004b0: 636f 6e74 656e 742e 7469 746c 652e 6c61  content.title.la
-000004c0: 6265 6c20 3d20 7465 7874 3b0a 2020 2020  bel = text;.    
-000004d0: 636f 6e74 656e 742e 7469 746c 652e 636c  content.title.cl
-000004e0: 6f73 6162 6c65 203d 2074 7275 653b 0a20  osable = true;. 
-000004f0: 2020 2063 6f6e 7465 6e74 2e75 726c 203d     content.url =
-00000500: 2075 726c 3b0a 2020 2020 636f 6e74 656e   url;.    conten
-00000510: 742e 6164 6443 6c61 7373 2827 6a70 2d53  t.addClass('jp-S
-00000520: 6572 7665 7250 726f 7879 2729 3b0a 2020  erverProxy');.  
-00000530: 2020 636f 6e74 656e 742e 6964 203d 2069    content.id = i
-00000540: 643b 0a20 2020 2063 6f6e 7374 2077 6964  d;.    const wid
-00000550: 6765 7420 3d20 6e65 7720 6170 7075 7469  get = new apputi
-00000560: 6c73 5f31 2e4d 6169 6e41 7265 6157 6964  ls_1.MainAreaWid
-00000570: 6765 7428 7b20 636f 6e74 656e 7420 7d29  get({ content })
-00000580: 3b0a 2020 2020 7769 6467 6574 2e61 6464  ;.    widget.add
-00000590: 436c 6173 7328 276a 702d 5365 7276 6572  Class('jp-Server
-000005a0: 5072 6f78 7927 293b 0a20 2020 2072 6574  Proxy');.    ret
-000005b0: 7572 6e20 7769 6467 6574 3b0a 7d0a 6675  urn widget;.}.fu
-000005c0: 6e63 7469 6f6e 2061 6374 6976 6174 6528  nction activate(
-000005d0: 6170 702c 206c 6175 6e63 6865 722c 2072  app, launcher, r
-000005e0: 6573 746f 7265 7229 207b 0a20 2020 2072  estorer) {.    r
-000005f0: 6574 7572 6e20 5f5f 6177 6169 7465 7228  eturn __awaiter(
-00000600: 7468 6973 2c20 766f 6964 2030 2c20 766f  this, void 0, vo
-00000610: 6964 2030 2c20 6675 6e63 7469 6f6e 2a20  id 0, function* 
-00000620: 2829 207b 0a20 2020 2020 2020 2063 6f6e  () {.        con
-00000630: 7374 2072 6573 706f 6e73 6520 3d20 7969  st response = yi
-00000640: 656c 6420 6665 7463 6828 636f 7265 7574  eld fetch(coreut
-00000650: 696c 735f 312e 5061 6765 436f 6e66 6967  ils_1.PageConfig
-00000660: 2e67 6574 4261 7365 5572 6c28 2920 2b20  .getBaseUrl() + 
-00000670: 2773 6572 7665 722d 7072 6f78 792f 7365  'server-proxy/se
-00000680: 7276 6572 732d 696e 666f 2729 3b0a 2020  rvers-info');.  
-00000690: 2020 2020 2020 6966 2028 2172 6573 706f        if (!respo
-000006a0: 6e73 652e 6f6b 2920 7b0a 2020 2020 2020  nse.ok) {.      
-000006b0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
-000006c0: 6728 2743 6f75 6c64 206e 6f74 2066 6574  g('Could not fet
-000006d0: 6368 206d 6574 6164 6174 6120 6162 6f75  ch metadata abou
-000006e0: 7420 7265 6769 7374 6572 6564 2073 6572  t registered ser
-000006f0: 7665 7273 2e20 4d61 6b65 2073 7572 6520  vers. Make sure 
-00000700: 6a75 7079 7465 722d 7365 7276 6572 2d70  jupyter-server-p
-00000710: 726f 7879 2069 7320 696e 7374 616c 6c65  roxy is installe
-00000720: 642e 2729 3b0a 2020 2020 2020 2020 2020  d.');.          
-00000730: 2020 636f 6e73 6f6c 652e 6c6f 6728 7265    console.log(re
-00000740: 7370 6f6e 7365 293b 0a20 2020 2020 2020  sponse);.       
-00000750: 2020 2020 2072 6574 7572 6e3b 0a20 2020       return;.   
-00000760: 2020 2020 207d 0a20 2020 2020 2020 2063       }.        c
-00000770: 6f6e 7374 207b 2063 6f6d 6d61 6e64 732c  onst { commands,
-00000780: 2073 6865 6c6c 207d 203d 2061 7070 3b0a   shell } = app;.
-00000790: 2020 2020 2020 2020 636f 6e73 7420 6461          const da
-000007a0: 7461 203d 2079 6965 6c64 2072 6573 706f  ta = yield respo
-000007b0: 6e73 652e 6a73 6f6e 2829 3b0a 2020 2020  nse.json();.    
-000007c0: 2020 2020 636f 6e73 7420 6e61 6d65 7370      const namesp
-000007d0: 6163 6520 3d20 2773 6572 7665 722d 7072  ace = 'server-pr
-000007e0: 6f78 7927 3b0a 2020 2020 2020 2020 636f  oxy';.        co
-000007f0: 6e73 7420 7472 6163 6b65 7220 3d20 6e65  nst tracker = ne
-00000800: 7720 6170 7075 7469 6c73 5f31 2e57 6964  w apputils_1.Wid
-00000810: 6765 7454 7261 636b 6572 287b 0a20 2020  getTracker({.   
-00000820: 2020 2020 2020 2020 206e 616d 6573 7061           namespa
-00000830: 6365 0a20 2020 2020 2020 207d 293b 0a20  ce.        });. 
-00000840: 2020 2020 2020 2063 6f6e 7374 2063 6f6d         const com
-00000850: 6d61 6e64 203d 206e 616d 6573 7061 6365  mand = namespace
-00000860: 202b 2027 3a27 202b 2027 6f70 656e 273b   + ':' + 'open';
-00000870: 0a20 2020 2020 2020 2069 6620 2872 6573  .        if (res
-00000880: 746f 7265 7229 207b 0a20 2020 2020 2020  torer) {.       
-00000890: 2020 2020 2076 6f69 6420 7265 7374 6f72       void restor
-000008a0: 6572 2e72 6573 746f 7265 2874 7261 636b  er.restore(track
-000008b0: 6572 2c20 7b0a 2020 2020 2020 2020 2020  er, {.          
-000008c0: 2020 2020 2020 636f 6d6d 616e 643a 2063        command: c
-000008d0: 6f6d 6d61 6e64 2c0a 2020 2020 2020 2020  ommand,.        
-000008e0: 2020 2020 2020 2020 6172 6773 3a20 7769          args: wi
-000008f0: 6467 6574 203d 3e20 287b 0a20 2020 2020  dget => ({.     
-00000900: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00000910: 726c 3a20 7769 6467 6574 2e63 6f6e 7465  rl: widget.conte
-00000920: 6e74 2e75 726c 2c0a 2020 2020 2020 2020  nt.url,.        
-00000930: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00000940: 653a 2077 6964 6765 742e 636f 6e74 656e  e: widget.conten
-00000950: 742e 7469 746c 652e 6c61 6265 6c2c 0a20  t.title.label,. 
-00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000970: 2020 206e 6577 4272 6f77 7365 7254 6162     newBrowserTab
-00000980: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00000990: 2020 2020 2020 2020 2020 2020 2069 643a               id:
-000009a0: 2077 6964 6765 742e 636f 6e74 656e 742e   widget.content.
-000009b0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-000009c0: 2020 207d 292c 0a20 2020 2020 2020 2020     }),.         
-000009d0: 2020 2020 2020 206e 616d 653a 2077 6964         name: wid
-000009e0: 6765 7420 3d3e 2077 6964 6765 742e 636f  get => widget.co
-000009f0: 6e74 656e 742e 6964 0a20 2020 2020 2020  ntent.id.       
-00000a00: 2020 2020 207d 293b 0a20 2020 2020 2020       });.       
-00000a10: 207d 0a20 2020 2020 2020 2063 6f6d 6d61   }.        comma
-00000a20: 6e64 732e 6164 6443 6f6d 6d61 6e64 2863  nds.addCommand(c
-00000a30: 6f6d 6d61 6e64 2c20 7b0a 2020 2020 2020  ommand, {.      
-00000a40: 2020 2020 2020 6c61 6265 6c3a 2061 7267        label: arg
-00000a50: 7320 3d3e 2061 7267 735b 2774 6974 6c65  s => args['title
-00000a60: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
-00000a70: 6578 6563 7574 653a 2061 7267 7320 3d3e  execute: args =>
-00000a80: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000a90: 2020 2063 6f6e 7374 2069 6420 3d20 6172     const id = ar
-00000aa0: 6773 5b27 6964 275d 3b0a 2020 2020 2020  gs['id'];.      
-00000ab0: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00000ac0: 7469 746c 6520 3d20 6172 6773 5b27 7469  title = args['ti
-00000ad0: 746c 6527 5d3b 0a20 2020 2020 2020 2020  tle'];.         
-00000ae0: 2020 2020 2020 2063 6f6e 7374 2075 726c         const url
-00000af0: 203d 2061 7267 735b 2775 726c 275d 3b0a   = args['url'];.
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 636f 6e73 7420 6e65 7742 726f 7773 6572  const newBrowser
-00000b20: 5461 6220 3d20 6172 6773 5b27 6e65 7742  Tab = args['newB
-00000b30: 726f 7773 6572 5461 6227 5d3b 0a20 2020  rowserTab'];.   
-00000b40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000b50: 286e 6577 4272 6f77 7365 7254 6162 2920  (newBrowserTab) 
-00000b60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000b70: 2020 2020 2020 7769 6e64 6f77 2e6f 7065        window.ope
-00000b80: 6e28 7572 6c2c 2027 5f62 6c61 6e6b 2729  n(url, '_blank')
-00000b90: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000ba0: 2020 2020 2020 7265 7475 726e 3b0a 2020        return;.  
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 6c65 7420 7769 6467 6574 203d 2074 7261  let widget = tra
-00000be0: 636b 6572 2e66 696e 6428 2877 6964 6765  cker.find((widge
-00000bf0: 7429 203d 3e20 7b20 7265 7475 726e 2077  t) => { return w
-00000c00: 6964 6765 742e 636f 6e74 656e 742e 6964  idget.content.id
-00000c10: 203d 3d20 6964 3b20 7d29 3b0a 2020 2020   == id; });.    
-00000c20: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00000c30: 2177 6964 6765 7429 207b 0a20 2020 2020  !widget) {.     
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00000c50: 6964 6765 7420 3d20 6e65 7753 6572 7665  idget = newServe
-00000c60: 7250 726f 7879 5769 6467 6574 2869 642c  rProxyWidget(id,
-00000c70: 2075 726c 2c20 7469 746c 6529 3b0a 2020   url, title);.  
-00000c80: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ca0: 6966 2028 2174 7261 636b 6572 2e68 6173  if (!tracker.has
-00000cb0: 2877 6964 6765 7429 2920 7b0a 2020 2020  (widget)) {.    
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 766f 6964 2074 7261 636b 6572 2e61 6464  void tracker.add
-00000ce0: 2877 6964 6765 7429 3b0a 2020 2020 2020  (widget);.      
-00000cf0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000d00: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00000d10: 2177 6964 6765 742e 6973 4174 7461 6368  !widget.isAttach
-00000d20: 6564 2920 7b0a 2020 2020 2020 2020 2020  ed) {.          
-00000d30: 2020 2020 2020 2020 2020 7368 656c 6c2e            shell.
-00000d40: 6164 6428 7769 6467 6574 293b 0a20 2020  add(widget);.   
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2072 6574 7572 6e20 7769 6467 6574 3b0a   return widget;.
-00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d80: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000d90: 2020 656c 7365 207b 0a20 2020 2020 2020    else {.       
-00000da0: 2020 2020 2020 2020 2020 2020 2073 6865               she
-00000db0: 6c6c 2e61 6374 6976 6174 6542 7949 6428  ll.activateById(
-00000dc0: 7769 6467 6574 2e69 6429 3b0a 2020 2020  widget.id);.    
-00000dd0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000de0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000df0: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
-00000e00: 666f 7220 286c 6574 2073 6572 7665 725f  for (let server_
-00000e10: 7072 6f63 6573 7320 6f66 2064 6174 612e  process of data.
-00000e20: 7365 7276 6572 5f70 726f 6365 7373 6573  server_processes
-00000e30: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00000e40: 6966 2028 2173 6572 7665 725f 7072 6f63  if (!server_proc
-00000e50: 6573 732e 6c61 756e 6368 6572 5f65 6e74  ess.launcher_ent
-00000e60: 7279 2e65 6e61 626c 6564 2920 7b0a 2020  ry.enabled) {.  
-00000e70: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00000e80: 6e74 696e 7565 3b0a 2020 2020 2020 2020  ntinue;.        
-00000e90: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00000ea0: 2020 636f 6e73 7420 7572 6c20 3d20 636f    const url = co
-00000eb0: 7265 7574 696c 735f 312e 5061 6765 436f  reutils_1.PageCo
-00000ec0: 6e66 6967 2e67 6574 4261 7365 5572 6c28  nfig.getBaseUrl(
-00000ed0: 2920 2b20 7365 7276 6572 5f70 726f 6365  ) + server_proce
-00000ee0: 7373 2e6c 6175 6e63 6865 725f 656e 7472  ss.launcher_entr
-00000ef0: 792e 7061 7468 5f69 6e66 6f3b 0a20 2020  y.path_info;.   
-00000f00: 2020 2020 2020 2020 2063 6f6e 7374 2074           const t
-00000f10: 6974 6c65 203d 2073 6572 7665 725f 7072  itle = server_pr
-00000f20: 6f63 6573 732e 6c61 756e 6368 6572 5f65  ocess.launcher_e
-00000f30: 6e74 7279 2e74 6974 6c65 3b0a 2020 2020  ntry.title;.    
-00000f40: 2020 2020 2020 2020 636f 6e73 7420 6e65          const ne
-00000f50: 7742 726f 7773 6572 5461 6220 3d20 7365  wBrowserTab = se
-00000f60: 7276 6572 5f70 726f 6365 7373 2e6e 6577  rver_process.new
-00000f70: 5f62 726f 7773 6572 5f74 6162 3b0a 2020  _browser_tab;.  
-00000f80: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00000f90: 6964 203d 206e 616d 6573 7061 6365 202b  id = namespace +
-00000fa0: 2027 3a27 202b 2073 6572 7665 725f 7072   ':' + server_pr
-00000fb0: 6f63 6573 732e 6e61 6d65 3b0a 2020 2020  ocess.name;.    
-00000fc0: 2020 2020 2020 2020 636f 6e73 7420 6c61          const la
-00000fd0: 756e 6368 6572 5f69 7465 6d20 3d20 7b0a  uncher_item = {.
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 636f 6d6d 616e 643a 2063 6f6d 6d61 6e64  command: command
-00001000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001010: 2020 6172 6773 3a20 7b0a 2020 2020 2020    args: {.      
-00001020: 2020 2020 2020 2020 2020 2020 2020 7572                ur
-00001030: 6c3a 2075 726c 2c0a 2020 2020 2020 2020  l: url,.        
-00001040: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-00001050: 653a 2074 6974 6c65 202b 2028 6e65 7742  e: title + (newB
-00001060: 726f 7773 6572 5461 6220 3f20 2720 5be2  rowserTab ? ' [.
-00001070: 8697 5d27 203a 2027 2729 2c0a 2020 2020  ..]' : ''),.    
-00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001090: 6e65 7742 726f 7773 6572 5461 623a 206e  newBrowserTab: n
-000010a0: 6577 4272 6f77 7365 7254 6162 2c0a 2020  ewBrowserTab,.  
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010c0: 2020 6964 3a20 6964 0a20 2020 2020 2020    id: id.       
-000010d0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000010e0: 2020 2020 2020 2020 2020 2020 6361 7465              cate
-000010f0: 676f 7279 3a20 274e 6f74 6562 6f6f 6b27  gory: 'Notebook'
-00001100: 0a20 2020 2020 2020 2020 2020 207d 3b0a  .            };.
-00001110: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00001120: 7365 7276 6572 5f70 726f 6365 7373 2e6c  server_process.l
-00001130: 6175 6e63 6865 725f 656e 7472 792e 6963  auncher_entry.ic
-00001140: 6f6e 5f75 726c 2920 7b0a 2020 2020 2020  on_url) {.      
-00001150: 2020 2020 2020 2020 2020 6c61 756e 6368            launch
-00001160: 6572 5f69 7465 6d2e 6b65 726e 656c 4963  er_item.kernelIc
-00001170: 6f6e 5572 6c20 3d20 7365 7276 6572 5f70  onUrl = server_p
-00001180: 726f 6365 7373 2e6c 6175 6e63 6865 725f  rocess.launcher_
-00001190: 656e 7472 792e 6963 6f6e 5f75 726c 3b0a  entry.icon_url;.
-000011a0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000011b0: 2020 2020 2020 2020 2020 6c61 756e 6368            launch
-000011c0: 6572 2e61 6464 286c 6175 6e63 6865 725f  er.add(launcher_
-000011d0: 6974 656d 293b 0a20 2020 2020 2020 207d  item);.        }
-000011e0: 0a20 2020 207d 293b 0a7d 0a2f 2a2a 0a20  .    });.}./**. 
-000011f0: 2a20 496e 6974 6961 6c69 7a61 7469 6f6e  * Initialization
-00001200: 2064 6174 6120 666f 7220 7468 6520 6a75   data for the ju
-00001210: 7079 7465 726c 6162 2d73 6572 7665 722d  pyterlab-server-
-00001220: 7072 6f78 7920 6578 7465 6e73 696f 6e2e  proxy extension.
-00001230: 0a20 2a2f 0a63 6f6e 7374 2065 7874 656e  . */.const exten
-00001240: 7369 6f6e 203d 207b 0a20 2020 2069 643a  sion = {.    id:
-00001250: 2027 6a75 7079 7465 726c 6162 2d73 6572   'jupyterlab-ser
-00001260: 7665 722d 7072 6f78 7927 2c0a 2020 2020  ver-proxy',.    
-00001270: 6175 746f 5374 6172 743a 2074 7275 652c  autoStart: true,
-00001280: 0a20 2020 2072 6571 7569 7265 733a 205b  .    requires: [
-00001290: 6c61 756e 6368 6572 5f31 2e49 4c61 756e  launcher_1.ILaun
-000012a0: 6368 6572 2c20 6170 706c 6963 6174 696f  cher, applicatio
-000012b0: 6e5f 312e 494c 6179 6f75 7452 6573 746f  n_1.ILayoutResto
-000012c0: 7265 725d 2c0a 2020 2020 6163 7469 7661  rer],.    activa
-000012d0: 7465 3a20 6163 7469 7661 7465 0a7d 3b0a  te: activate.};.
-000012e0: 6578 706f 7274 732e 6465 6661 756c 7420  exports.default 
-000012f0: 3d20 6578 7465 6e73 696f 6e3b 0a         = extension;.
+00000000: 696d 706f 7274 207b 0a20 204a 7570 7974  import {.  Jupyt
+00000010: 6572 4672 6f6e 7445 6e64 2c0a 2020 4a75  erFrontEnd,.  Ju
+00000020: 7079 7465 7246 726f 6e74 456e 6450 6c75  pyterFrontEndPlu
+00000030: 6769 6e2c 0a20 2049 4c61 796f 7574 5265  gin,.  ILayoutRe
+00000040: 7374 6f72 6572 2c0a 7d20 6672 6f6d 2022  storer,.} from "
+00000050: 406a 7570 7974 6572 6c61 622f 6170 706c  @jupyterlab/appl
+00000060: 6963 6174 696f 6e22 3b0a 696d 706f 7274  ication";.import
+00000070: 207b 2049 4c61 756e 6368 6572 207d 2066   { ILauncher } f
+00000080: 726f 6d20 2240 6a75 7079 7465 726c 6162  rom "@jupyterlab
+00000090: 2f6c 6175 6e63 6865 7222 3b0a 696d 706f  /launcher";.impo
+000000a0: 7274 207b 2050 6167 6543 6f6e 6669 6720  rt { PageConfig 
+000000b0: 7d20 6672 6f6d 2022 406a 7570 7974 6572  } from "@jupyter
+000000c0: 6c61 622f 636f 7265 7574 696c 7322 3b0a  lab/coreutils";.
+000000d0: 696d 706f 7274 207b 2049 4672 616d 652c  import { IFrame,
+000000e0: 204d 6169 6e41 7265 6157 6964 6765 742c   MainAreaWidget,
+000000f0: 2057 6964 6765 7454 7261 636b 6572 207d   WidgetTracker }
+00000100: 2066 726f 6d20 2240 6a75 7079 7465 726c   from "@jupyterl
+00000110: 6162 2f61 7070 7574 696c 7322 3b0a 0a66  ab/apputils";..f
+00000120: 756e 6374 696f 6e20 6e65 7753 6572 7665  unction newServe
+00000130: 7250 726f 7879 5769 6467 6574 280a 2020  rProxyWidget(.  
+00000140: 6964 3a20 7374 7269 6e67 2c0a 2020 7572  id: string,.  ur
+00000150: 6c3a 2073 7472 696e 672c 0a20 2074 6578  l: string,.  tex
+00000160: 743a 2073 7472 696e 672c 0a29 3a20 4d61  t: string,.): Ma
+00000170: 696e 4172 6561 5769 6467 6574 3c49 4672  inAreaWidget<IFr
+00000180: 616d 653e 207b 0a20 2063 6f6e 7374 2063  ame> {.  const c
+00000190: 6f6e 7465 6e74 203d 206e 6577 2049 4672  ontent = new IFr
+000001a0: 616d 6528 7b0a 2020 2020 7361 6e64 626f  ame({.    sandbo
+000001b0: 783a 205b 0a20 2020 2020 2022 616c 6c6f  x: [.      "allo
+000001c0: 772d 7361 6d65 2d6f 7269 6769 6e22 2c0a  w-same-origin",.
+000001d0: 2020 2020 2020 2261 6c6c 6f77 2d73 6372        "allow-scr
+000001e0: 6970 7473 222c 0a20 2020 2020 2022 616c  ipts",.      "al
+000001f0: 6c6f 772d 706f 7075 7073 222c 0a20 2020  low-popups",.   
+00000200: 2020 2022 616c 6c6f 772d 666f 726d 7322     "allow-forms"
+00000210: 2c0a 2020 2020 2020 2261 6c6c 6f77 2d64  ,.      "allow-d
+00000220: 6f77 6e6c 6f61 6473 222c 0a20 2020 2020  ownloads",.     
+00000230: 2022 616c 6c6f 772d 6d6f 6461 6c73 222c   "allow-modals",
+00000240: 0a20 2020 205d 2c0a 2020 7d29 3b0a 2020  .    ],.  });.  
+00000250: 636f 6e74 656e 742e 7469 746c 652e 6c61  content.title.la
+00000260: 6265 6c20 3d20 7465 7874 3b0a 2020 636f  bel = text;.  co
+00000270: 6e74 656e 742e 7469 746c 652e 636c 6f73  ntent.title.clos
+00000280: 6162 6c65 203d 2074 7275 653b 0a20 2063  able = true;.  c
+00000290: 6f6e 7465 6e74 2e75 726c 203d 2075 726c  ontent.url = url
+000002a0: 3b0a 2020 636f 6e74 656e 742e 6164 6443  ;.  content.addC
+000002b0: 6c61 7373 2822 6a70 2d53 6572 7665 7250  lass("jp-ServerP
+000002c0: 726f 7879 2229 3b0a 2020 636f 6e74 656e  roxy");.  conten
+000002d0: 742e 6964 203d 2069 643b 0a20 2063 6f6e  t.id = id;.  con
+000002e0: 7374 2077 6964 6765 7420 3d20 6e65 7720  st widget = new 
+000002f0: 4d61 696e 4172 6561 5769 6467 6574 287b  MainAreaWidget({
+00000300: 2063 6f6e 7465 6e74 207d 293b 0a20 2077   content });.  w
+00000310: 6964 6765 742e 6164 6443 6c61 7373 2822  idget.addClass("
+00000320: 6a70 2d53 6572 7665 7250 726f 7879 2229  jp-ServerProxy")
+00000330: 3b0a 2020 7265 7475 726e 2077 6964 6765  ;.  return widge
+00000340: 743b 0a7d 0a0a 2f2a 2a0a 202a 2054 6865  t;.}../**. * The
+00000350: 2061 6374 6976 6174 6520 6675 6e63 7469   activate functi
+00000360: 6f6e 2069 7320 7265 6769 7374 6572 6564  on is registered
+00000370: 2074 6f20 6265 2063 616c 6c65 6420 6f6e   to be called on
+00000380: 2061 6374 6976 6174 696f 6e20 6f66 2074   activation of t
+00000390: 6865 0a20 2a20 6a75 7079 7465 726c 6162  he. * jupyterlab
+000003a0: 2065 7874 656e 7369 6f6e 2e0a 202a 0a20   extension.. *. 
+000003b0: 2a20 7265 663a 2068 7474 7073 3a2f 2f6a  * ref: https://j
+000003c0: 7570 7974 6572 6c61 622e 7265 6164 7468  upyterlab.readth
+000003d0: 6564 6f63 732e 696f 2f65 6e2f 7374 6162  edocs.io/en/stab
+000003e0: 6c65 2f65 7874 656e 7369 6f6e 2f65 7874  le/extension/ext
+000003f0: 656e 7369 6f6e 5f64 6576 2e68 746d 6c0a  ension_dev.html.
+00000400: 202a 2f0a 6173 796e 6320 6675 6e63 7469   */.async functi
+00000410: 6f6e 2061 6374 6976 6174 6528 0a20 2061  on activate(.  a
+00000420: 7070 3a20 4a75 7079 7465 7246 726f 6e74  pp: JupyterFront
+00000430: 456e 642c 0a20 206c 6175 6e63 6865 723a  End,.  launcher:
+00000440: 2049 4c61 756e 6368 6572 2c0a 2020 7265   ILauncher,.  re
+00000450: 7374 6f72 6572 3a20 494c 6179 6f75 7452  storer: ILayoutR
+00000460: 6573 746f 7265 722c 0a29 3a20 5072 6f6d  estorer,.): Prom
+00000470: 6973 653c 766f 6964 3e20 7b0a 2020 2f2f  ise<void> {.  //
+00000480: 2046 6574 6368 2063 6f6e 6669 6775 7265   Fetch configure
+00000490: 6420 7365 7276 6572 2070 726f 6365 7373  d server process
+000004a0: 6573 2066 726f 6d20 7b62 6173 655f 7572  es from {base_ur
+000004b0: 6c7d 2f73 6572 7665 722d 7072 6f78 792f  l}/server-proxy/
+000004c0: 7365 7276 6572 732d 696e 666f 0a20 2063  servers-info.  c
+000004d0: 6f6e 7374 2072 6573 706f 6e73 6520 3d20  onst response = 
+000004e0: 6177 6169 7420 6665 7463 6828 0a20 2020  await fetch(.   
+000004f0: 2050 6167 6543 6f6e 6669 672e 6765 7442   PageConfig.getB
+00000500: 6173 6555 726c 2829 202b 2022 7365 7276  aseUrl() + "serv
+00000510: 6572 2d70 726f 7879 2f73 6572 7665 7273  er-proxy/servers
+00000520: 2d69 6e66 6f22 2c0a 2020 293b 0a20 2069  -info",.  );.  i
+00000530: 6620 2821 7265 7370 6f6e 7365 2e6f 6b29  f (!response.ok)
+00000540: 207b 0a20 2020 2063 6f6e 736f 6c65 2e6c   {.    console.l
+00000550: 6f67 280a 2020 2020 2020 2243 6f75 6c64  og(.      "Could
+00000560: 206e 6f74 2066 6574 6368 206d 6574 6164   not fetch metad
+00000570: 6174 6120 6162 6f75 7420 7265 6769 7374  ata about regist
+00000580: 6572 6564 2073 6572 7665 7273 2e20 4d61  ered servers. Ma
+00000590: 6b65 2073 7572 6520 6a75 7079 7465 722d  ke sure jupyter-
+000005a0: 7365 7276 6572 2d70 726f 7879 2069 7320  server-proxy is 
+000005b0: 696e 7374 616c 6c65 642e 222c 0a20 2020  installed.",.   
+000005c0: 2029 3b0a 2020 2020 636f 6e73 6f6c 652e   );.    console.
+000005d0: 6c6f 6728 7265 7370 6f6e 7365 293b 0a20  log(response);. 
+000005e0: 2020 2072 6574 7572 6e3b 0a20 207d 0a20     return;.  }. 
+000005f0: 2063 6f6e 7374 2064 6174 6120 3d20 6177   const data = aw
+00000600: 6169 7420 7265 7370 6f6e 7365 2e6a 736f  ait response.jso
+00000610: 6e28 293b 0a0a 2020 636f 6e73 7420 6e61  n();..  const na
+00000620: 6d65 7370 6163 6520 3d20 2273 6572 7665  mespace = "serve
+00000630: 722d 7072 6f78 7922 3b0a 2020 636f 6e73  r-proxy";.  cons
+00000640: 7420 7472 6163 6b65 7220 3d20 6e65 7720  t tracker = new 
+00000650: 5769 6467 6574 5472 6163 6b65 723c 4d61  WidgetTracker<Ma
+00000660: 696e 4172 6561 5769 6467 6574 3c49 4672  inAreaWidget<IFr
+00000670: 616d 653e 3e28 7b0a 2020 2020 6e61 6d65  ame>>({.    name
+00000680: 7370 6163 652c 0a20 207d 293b 0a20 2063  space,.  });.  c
+00000690: 6f6e 7374 2063 6f6d 6d61 6e64 203d 206e  onst command = n
+000006a0: 616d 6573 7061 6365 202b 2022 3a22 202b  amespace + ":" +
+000006b0: 2022 6f70 656e 223b 0a0a 2020 6966 2028   "open";..  if (
+000006c0: 7265 7374 6f72 6572 2920 7b0a 2020 2020  restorer) {.    
+000006d0: 766f 6964 2072 6573 746f 7265 722e 7265  void restorer.re
+000006e0: 7374 6f72 6528 7472 6163 6b65 722c 207b  store(tracker, {
+000006f0: 0a20 2020 2020 2063 6f6d 6d61 6e64 3a20  .      command: 
+00000700: 636f 6d6d 616e 642c 0a20 2020 2020 2061  command,.      a
+00000710: 7267 733a 2028 7769 6467 6574 2920 3d3e  rgs: (widget) =>
+00000720: 2028 7b0a 2020 2020 2020 2020 7572 6c3a   ({.        url:
+00000730: 2077 6964 6765 742e 636f 6e74 656e 742e   widget.content.
+00000740: 7572 6c2c 0a20 2020 2020 2020 2074 6974  url,.        tit
+00000750: 6c65 3a20 7769 6467 6574 2e63 6f6e 7465  le: widget.conte
+00000760: 6e74 2e74 6974 6c65 2e6c 6162 656c 2c0a  nt.title.label,.
+00000770: 2020 2020 2020 2020 6e65 7742 726f 7773          newBrows
+00000780: 6572 5461 623a 2066 616c 7365 2c0a 2020  erTab: false,.  
+00000790: 2020 2020 2020 6964 3a20 7769 6467 6574        id: widget
+000007a0: 2e63 6f6e 7465 6e74 2e69 642c 0a20 2020  .content.id,.   
+000007b0: 2020 207d 292c 0a20 2020 2020 206e 616d     }),.      nam
+000007c0: 653a 2028 7769 6467 6574 2920 3d3e 2077  e: (widget) => w
+000007d0: 6964 6765 742e 636f 6e74 656e 742e 6964  idget.content.id
+000007e0: 2c0a 2020 2020 7d29 3b0a 2020 7d0a 0a20  ,.    });.  }.. 
+000007f0: 2063 6f6e 7374 207b 2063 6f6d 6d61 6e64   const { command
+00000800: 732c 2073 6865 6c6c 207d 203d 2061 7070  s, shell } = app
+00000810: 3b0a 2020 636f 6d6d 616e 6473 2e61 6464  ;.  commands.add
+00000820: 436f 6d6d 616e 6428 636f 6d6d 616e 642c  Command(command,
+00000830: 207b 0a20 2020 206c 6162 656c 3a20 2861   {.    label: (a
+00000840: 7267 7329 203d 3e20 6172 6773 5b22 7469  rgs) => args["ti
+00000850: 746c 6522 5d20 6173 2073 7472 696e 672c  tle"] as string,
+00000860: 0a20 2020 2065 7865 6375 7465 3a20 2861  .    execute: (a
+00000870: 7267 7329 203d 3e20 7b0a 2020 2020 2020  rgs) => {.      
+00000880: 636f 6e73 7420 6964 203d 2061 7267 735b  const id = args[
+00000890: 2269 6422 5d20 6173 2073 7472 696e 673b  "id"] as string;
+000008a0: 0a20 2020 2020 2063 6f6e 7374 2074 6974  .      const tit
+000008b0: 6c65 203d 2061 7267 735b 2274 6974 6c65  le = args["title
+000008c0: 225d 2061 7320 7374 7269 6e67 3b0a 2020  "] as string;.  
+000008d0: 2020 2020 636f 6e73 7420 7572 6c20 3d20      const url = 
+000008e0: 6172 6773 5b22 7572 6c22 5d20 6173 2073  args["url"] as s
+000008f0: 7472 696e 673b 0a20 2020 2020 2063 6f6e  tring;.      con
+00000900: 7374 206e 6577 4272 6f77 7365 7254 6162  st newBrowserTab
+00000910: 203d 2061 7267 735b 226e 6577 4272 6f77   = args["newBrow
+00000920: 7365 7254 6162 225d 2061 7320 626f 6f6c  serTab"] as bool
+00000930: 6561 6e3b 0a20 2020 2020 2069 6620 286e  ean;.      if (n
+00000940: 6577 4272 6f77 7365 7254 6162 2920 7b0a  ewBrowserTab) {.
+00000950: 2020 2020 2020 2020 7769 6e64 6f77 2e6f          window.o
+00000960: 7065 6e28 7572 6c2c 2022 5f62 6c61 6e6b  pen(url, "_blank
+00000970: 2229 3b0a 2020 2020 2020 2020 7265 7475  ");.        retu
+00000980: 726e 3b0a 2020 2020 2020 7d0a 2020 2020  rn;.      }.    
+00000990: 2020 6c65 7420 7769 6467 6574 203d 2074    let widget = t
+000009a0: 7261 636b 6572 2e66 696e 6428 2877 6964  racker.find((wid
+000009b0: 6765 7429 203d 3e20 7b0a 2020 2020 2020  get) => {.      
+000009c0: 2020 7265 7475 726e 2077 6964 6765 742e    return widget.
+000009d0: 636f 6e74 656e 742e 6964 203d 3d20 6964  content.id == id
+000009e0: 3b0a 2020 2020 2020 7d29 3b0a 2020 2020  ;.      });.    
+000009f0: 2020 6966 2028 2177 6964 6765 7429 207b    if (!widget) {
+00000a00: 0a20 2020 2020 2020 2077 6964 6765 7420  .        widget 
+00000a10: 3d20 6e65 7753 6572 7665 7250 726f 7879  = newServerProxy
+00000a20: 5769 6467 6574 2869 642c 2075 726c 2c20  Widget(id, url, 
+00000a30: 7469 746c 6529 3b0a 2020 2020 2020 7d0a  title);.      }.
+00000a40: 2020 2020 2020 6966 2028 2174 7261 636b        if (!track
+00000a50: 6572 2e68 6173 2877 6964 6765 7429 2920  er.has(widget)) 
+00000a60: 7b0a 2020 2020 2020 2020 766f 6964 2074  {.        void t
+00000a70: 7261 636b 6572 2e61 6464 2877 6964 6765  racker.add(widge
+00000a80: 7429 3b0a 2020 2020 2020 7d0a 2020 2020  t);.      }.    
+00000a90: 2020 6966 2028 2177 6964 6765 742e 6973    if (!widget.is
+00000aa0: 4174 7461 6368 6564 2920 7b0a 2020 2020  Attached) {.    
+00000ab0: 2020 2020 7368 656c 6c2e 6164 6428 7769      shell.add(wi
+00000ac0: 6467 6574 293b 0a20 2020 2020 2020 2072  dget);.        r
+00000ad0: 6574 7572 6e20 7769 6467 6574 3b0a 2020  eturn widget;.  
+00000ae0: 2020 2020 7d20 656c 7365 207b 0a20 2020      } else {.   
+00000af0: 2020 2020 2073 6865 6c6c 2e61 6374 6976       shell.activ
+00000b00: 6174 6542 7949 6428 7769 6467 6574 2e69  ateById(widget.i
+00000b10: 6429 3b0a 2020 2020 2020 7d0a 2020 2020  d);.      }.    
+00000b20: 7d2c 0a20 207d 293b 0a0a 2020 666f 7220  },.  });..  for 
+00000b30: 286c 6574 2073 6572 7665 725f 7072 6f63  (let server_proc
+00000b40: 6573 7320 6f66 2064 6174 612e 7365 7276  ess of data.serv
+00000b50: 6572 5f70 726f 6365 7373 6573 2920 7b0a  er_processes) {.
+00000b60: 2020 2020 6966 2028 2173 6572 7665 725f      if (!server_
+00000b70: 7072 6f63 6573 732e 6c61 756e 6368 6572  process.launcher
+00000b80: 5f65 6e74 7279 2e65 6e61 626c 6564 2920  _entry.enabled) 
+00000b90: 7b0a 2020 2020 2020 636f 6e74 696e 7565  {.      continue
+00000ba0: 3b0a 2020 2020 7d0a 0a20 2020 2063 6f6e  ;.    }..    con
+00000bb0: 7374 2075 726c 203d 0a20 2020 2020 2050  st url =.      P
+00000bc0: 6167 6543 6f6e 6669 672e 6765 7442 6173  ageConfig.getBas
+00000bd0: 6555 726c 2829 202b 2073 6572 7665 725f  eUrl() + server_
+00000be0: 7072 6f63 6573 732e 6c61 756e 6368 6572  process.launcher
+00000bf0: 5f65 6e74 7279 2e70 6174 685f 696e 666f  _entry.path_info
+00000c00: 3b0a 2020 2020 636f 6e73 7420 7469 746c  ;.    const titl
+00000c10: 6520 3d20 7365 7276 6572 5f70 726f 6365  e = server_proce
+00000c20: 7373 2e6c 6175 6e63 6865 725f 656e 7472  ss.launcher_entr
+00000c30: 792e 7469 746c 653b 0a20 2020 2063 6f6e  y.title;.    con
+00000c40: 7374 206e 6577 4272 6f77 7365 7254 6162  st newBrowserTab
+00000c50: 203d 2073 6572 7665 725f 7072 6f63 6573   = server_proces
+00000c60: 732e 6e65 775f 6272 6f77 7365 725f 7461  s.new_browser_ta
+00000c70: 623b 0a20 2020 2063 6f6e 7374 2069 6420  b;.    const id 
+00000c80: 3d20 6e61 6d65 7370 6163 6520 2b20 223a  = namespace + ":
+00000c90: 2220 2b20 7365 7276 6572 5f70 726f 6365  " + server_proce
+00000ca0: 7373 2e6e 616d 653b 0a20 2020 2063 6f6e  ss.name;.    con
+00000cb0: 7374 206c 6175 6e63 6865 725f 6974 656d  st launcher_item
+00000cc0: 3a20 494c 6175 6e63 6865 722e 4949 7465  : ILauncher.IIte
+00000cd0: 6d4f 7074 696f 6e73 203d 207b 0a20 2020  mOptions = {.   
+00000ce0: 2020 2063 6f6d 6d61 6e64 3a20 636f 6d6d     command: comm
+00000cf0: 616e 642c 0a20 2020 2020 2061 7267 733a  and,.      args:
+00000d00: 207b 0a20 2020 2020 2020 2075 726c 3a20   {.        url: 
+00000d10: 7572 6c2c 0a20 2020 2020 2020 2074 6974  url,.        tit
+00000d20: 6c65 3a20 7469 746c 6520 2b20 286e 6577  le: title + (new
+00000d30: 4272 6f77 7365 7254 6162 203f 2022 205b  BrowserTab ? " [
+00000d40: e286 975d 2220 3a20 2222 292c 0a20 2020  ...]" : ""),.   
+00000d50: 2020 2020 206e 6577 4272 6f77 7365 7254       newBrowserT
+00000d60: 6162 3a20 6e65 7742 726f 7773 6572 5461  ab: newBrowserTa
+00000d70: 622c 0a20 2020 2020 2020 2069 643a 2069  b,.        id: i
+00000d80: 642c 0a20 2020 2020 207d 2c0a 2020 2020  d,.      },.    
+00000d90: 2020 6361 7465 676f 7279 3a20 224e 6f74    category: "Not
+00000da0: 6562 6f6f 6b22 2c0a 2020 2020 7d3b 0a0a  ebook",.    };..
+00000db0: 2020 2020 6966 2028 7365 7276 6572 5f70      if (server_p
+00000dc0: 726f 6365 7373 2e6c 6175 6e63 6865 725f  rocess.launcher_
+00000dd0: 656e 7472 792e 6963 6f6e 5f75 726c 2920  entry.icon_url) 
+00000de0: 7b0a 2020 2020 2020 6c61 756e 6368 6572  {.      launcher
+00000df0: 5f69 7465 6d2e 6b65 726e 656c 4963 6f6e  _item.kernelIcon
+00000e00: 5572 6c20 3d20 7365 7276 6572 5f70 726f  Url = server_pro
+00000e10: 6365 7373 2e6c 6175 6e63 6865 725f 656e  cess.launcher_en
+00000e20: 7472 792e 6963 6f6e 5f75 726c 3b0a 2020  try.icon_url;.  
+00000e30: 2020 7d0a 2020 2020 6c61 756e 6368 6572    }.    launcher
+00000e40: 2e61 6464 286c 6175 6e63 6865 725f 6974  .add(launcher_it
+00000e50: 656d 293b 0a20 207d 0a7d 0a0a 2f2a 2a0a  em);.  }.}../**.
+00000e60: 202a 2044 6174 6120 746f 2072 6567 6973   * Data to regis
+00000e70: 7465 7220 7468 6520 6578 7465 6e73 696f  ter the extensio
+00000e80: 6e20 7769 7468 206a 7570 7974 6572 6c61  n with jupyterla
+00000e90: 6220 7768 6963 6820 616c 736f 2063 6c61  b which also cla
+00000ea0: 7269 6669 6573 2077 6861 7473 0a20 2a20  rifies whats. * 
+00000eb0: 7265 7175 6972 6564 2062 7920 7468 6520  required by the 
+00000ec0: 6578 7465 6e73 696f 6e20 616e 6420 7061  extension and pa
+00000ed0: 7373 6564 2074 6f20 6f75 7220 7072 6f76  ssed to our prov
+00000ee0: 6964 6564 2061 6374 6976 6174 6520 6675  ided activate fu
+00000ef0: 6e63 7469 6f6e 2e0a 202a 0a20 2a20 7265  nction.. *. * re
+00000f00: 663a 2068 7474 7073 3a2f 2f6a 7570 7974  f: https://jupyt
+00000f10: 6572 6c61 622e 7265 6164 7468 6564 6f63  erlab.readthedoc
+00000f20: 732e 696f 2f65 6e2f 7374 6162 6c65 2f65  s.io/en/stable/e
+00000f30: 7874 656e 7369 6f6e 2f65 7874 656e 7369  xtension/extensi
+00000f40: 6f6e 5f64 6576 2e68 746d 6c23 6170 706c  on_dev.html#appl
+00000f50: 6963 6174 696f 6e2d 706c 7567 696e 730a  ication-plugins.
+00000f60: 202a 2f0a 636f 6e73 7420 6578 7465 6e73   */.const extens
+00000f70: 696f 6e3a 204a 7570 7974 6572 4672 6f6e  ion: JupyterFron
+00000f80: 7445 6e64 506c 7567 696e 3c76 6f69 643e  tEndPlugin<void>
+00000f90: 203d 207b 0a20 2069 643a 2022 406a 7570   = {.  id: "@jup
+00000fa0: 7974 6572 6875 622f 6a75 7079 7465 722d  yterhub/jupyter-
+00000fb0: 7365 7276 6572 2d70 726f 7879 3a61 6464  server-proxy:add
+00000fc0: 2d6c 6175 6e63 6865 722d 656e 7472 6965  -launcher-entrie
+00000fd0: 7322 2c0a 2020 6175 746f 5374 6172 743a  s",.  autoStart:
+00000fe0: 2074 7275 652c 0a20 2072 6571 7569 7265   true,.  require
+00000ff0: 733a 205b 494c 6175 6e63 6865 722c 2049  s: [ILauncher, I
+00001000: 4c61 796f 7574 5265 7374 6f72 6572 5d2c  LayoutRestorer],
+00001010: 0a20 2061 6374 6976 6174 653a 2061 6374  .  activate: act
+00001020: 6976 6174 652c 0a7d 3b0a 0a65 7870 6f72  ivate,.};..expor
+00001030: 7420 6465 6661 756c 7420 6578 7465 6e73  t default extens
+00001040: 696f 6e3b 0a                             ion;.
```

### Comparing `jupyter-server-proxy-3.2.2/jupyterlab-server-proxy/package.json` & `jupyter_server_proxy-4.0.0/jupyter_server_proxy/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7976102941176472%*

 * *Differences: {"'description'": "'A JupyterLab extension accompanying the PyPI package jupyter-server-proxy "*

 * *                  "adding launcher items for configured server processes.'",*

 * * "'devDependencies'": "{'rimraf': '^3.0.2', 'typescript': '~4.8.4', 'yarn-deduplicate': '^6.0.0', "*

 * *                      "'npm-run-all': '^4.1.5'}",*

 * * "'files'": "{insert: [(0, 'LICENSE')], delete: [1]}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.6bef4394de3b3e455a6a.js'), "*

 * *                 "('extension', '. […]*

```diff
@@ -6,54 +6,62 @@
     "bugs": {
         "url": "https://github.com/jupyterhub/jupyter-server-proxy/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^2.0 || ^3.0",
         "@jupyterlab/launcher": "^2.0 || ^3.0"
     },
-    "description": "Jupyter server extension to supervise and proxy web services",
+    "description": "A JupyterLab extension accompanying the PyPI package jupyter-server-proxy adding launcher items for configured server processes.",
     "devDependencies": {
         "@jupyterlab/builder": "^3.2.4",
-        "rimraf": "^2.6.1",
-        "typescript": "~3.7.0"
+        "npm-run-all": "^4.1.5",
+        "rimraf": "^3.0.2",
+        "typescript": "~4.8.4",
+        "yarn-deduplicate": "^6.0.0"
     },
     "files": [
-        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "LICENSE",
+        "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterhub/jupyter-server-proxy",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.6bef4394de3b3e455a6a.js"
+        },
         "extension": true,
         "outputDir": "../jupyter_server_proxy/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "@jupyterlab/server-proxy",
+    "name": "@jupyterhub/jupyter-server-proxy",
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterhub/jupyter-server-proxy.git"
     },
+    "resolutions": {
+        "loader-utils": ">=2.0.3"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
+        "build:lib": "tsc -b",
+        "build:prod": "jlpm clean && jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
         "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
         "clean:labextension": "rimraf jupyter_server_proxy/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
+        "deduplicate": "yarn-deduplicate -s fewer --fail",
         "install:extension": "jupyter labextension develop --overwrite .",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "jlpm build:lib -w --preserveWatchOutput"
     },
     "types": "lib/index.d.ts",
-    "version": "3.2.2"
+    "version": "4.0.0"
 }
```

