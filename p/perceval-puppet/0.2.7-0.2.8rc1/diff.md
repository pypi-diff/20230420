# Comparing `tmp/perceval_puppet-0.2.7.tar.gz` & `tmp/perceval_puppet-0.2.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_puppet-0.2.7.tar", max compression
+gzip compressed data, was "perceval_puppet-0.2.8rc1.tar", max compression
```

## Comparing `perceval_puppet-0.2.7.tar` & `perceval_puppet-0.2.8rc1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0       50 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/LICENSE
--rw-r--r--   0        0        0      798 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/NEWS
--rw-r--r--   0        0        0     2197 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/perceval/backends/puppet/__init__.py
--rw-r--r--   0        0        0       86 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/perceval/backends/puppet/_version.py
--rw-r--r--   0        0        0    10849 2023-02-03 08:17:27.000249 perceval_puppet-0.2.7/perceval/backends/puppet/puppetforge.py
--rw-r--r--   0        0        0     1397 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/__init__.py
--rw-r--r--   0        0        0     1888 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/base.py
--rw-r--r--   0        0        0      192 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_empty.json
--rw-r--r--   0        0        0    15963 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_modules.json
--rw-r--r--   0        0        0     1028 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_modules_next.json
--rw-r--r--   0        0        0    22968 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_releases_ceph.json
--rw-r--r--   0        0        0     1810 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_releases_nomad.json
--rw-r--r--   0        0        0      318 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_user_norisnetwork.json
--rw-r--r--   0        0        0      302 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
--rwxr-xr-x   0        0        0     1017 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/run_tests.py
--rw-r--r--   0        0        0    18656 2023-02-03 08:17:27.004249 perceval_puppet-0.2.7/tests/test_puppetforge.py
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 perceval_puppet-0.2.7/setup.py
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 perceval_puppet-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       50 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/LICENSE
+-rw-r--r--   0        0        0      798 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/NEWS
+-rw-r--r--   0        0        0     2197 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-20 15:35:36.624819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/_version.py
+-rw-r--r--   0        0        0    10849 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/perceval/backends/puppet/puppetforge.py
+-rw-r--r--   0        0        0     1402 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1888 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/base.py
+-rw-r--r--   0        0        0      192 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_empty.json
+-rw-r--r--   0        0        0    15963 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules.json
+-rw-r--r--   0        0        0     1028 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules_next.json
+-rw-r--r--   0        0        0    22968 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_ceph.json
+-rw-r--r--   0        0        0     1810 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_nomad.json
+-rw-r--r--   0        0        0      318 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_user_norisnetwork.json
+-rw-r--r--   0        0        0      302 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
+-rwxr-xr-x   0        0        0     1017 2023-04-20 15:35:36.628819 perceval_puppet-0.2.8rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    18656 2023-04-20 15:35:36.632819 perceval_puppet-0.2.8rc1/tests/test_puppetforge.py
+-rw-r--r--   0        0        0     3423 1970-01-01 00:00:00.000000 perceval_puppet-0.2.8rc1/PKG-INFO
```

### Comparing `perceval_puppet-0.2.7/LICENSE` & `perceval_puppet-0.2.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/NEWS` & `perceval_puppet-0.2.8rc1/NEWS`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/README.md` & `perceval_puppet-0.2.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/perceval/backends/puppet/puppetforge.py` & `perceval_puppet-0.2.8rc1/perceval/backends/puppet/puppetforge.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/pyproject.toml` & `perceval_puppet-0.2.8rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-puppet"
-version = "0.2.7"
+version = "0.2.8-rc.1"
 description = "Bundle of Perceval backends for Puppet, Inc. ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_puppet-0.2.7/tests/base.py` & `perceval_puppet-0.2.8rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_modules.json` & `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_modules_next.json` & `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_modules_next.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_releases_ceph.json` & `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_ceph.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/data/puppetforge/puppetforge_releases_nomad.json` & `perceval_puppet-0.2.8rc1/tests/data/puppetforge/puppetforge_releases_nomad.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/run_tests.py` & `perceval_puppet-0.2.8rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/tests/test_puppetforge.py` & `perceval_puppet-0.2.8rc1/tests/test_puppetforge.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.7/setup.py` & `perceval_puppet-0.2.8rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,103 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: perceval-puppet
+Version: 0.2.8rc1
+Summary: Bundle of Perceval backends for Puppet, Inc. ecosystem.
+Home-page: https://chaoss.github.io/grimoirelab/
+License: GPL-3.0+
+Keywords: development,grimoirelab
+Author: GrimoireLab Developers
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: grimoirelab-toolkit (>=0.3)
+Requires-Dist: perceval (>=0.19)
+Requires-Dist: requests (>=2.7.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-perceval-puppet/issues
+Project-URL: Repository, https://github.com/chaoss/grimoirelab-perceval-puppet
+Description-Content-Type: text/markdown
+
+# perceval-puppet [![Build Status](https://github.com/chaoss/grimoirelab-perceval-puppet/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-perceval-puppet/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-perceval-puppet.svg)](https://coveralls.io/r/chaoss/grimoirelab-perceval-puppet?branch=master)  [![PyPI version](https://badge.fury.io/py/perceval-puppet.svg)](https://badge.fury.io/py/perceval-puppet)
+
+Bundle of Perceval backends for Puppet ecosystem.
+
+## Backends
+
+The backends currently managed by this package support the next repositories:
+
+* Puppet Forge
+
+## Requirements
+
+ * Python >= 3.7
+
+You will also need some other libraries for running the tool, you can find the
+whole list of dependencies in [pyproject.toml](pyproject.toml) file.
+
+## Installation
+
+There are several ways to install perceval-puppet on your system: packages or source 
+code using Poetry or pip.
+
+### PyPI
+
+perceval-puppet can be installed using pip, a tool for installing Python packages. 
+To do it, run the next command:
+```
+$ pip install perceval-puppet
+```
+
+### Source code
+
+To install from the source code you will need to clone the repository first:
+```
+$ git clone https://github.com/chaoss/grimoirelab-perceval-puppet
+$ cd grimoirelab-perceval-puppet
+```
+
+Then use pip or Poetry to install the package along with its dependencies.
+
+#### Pip
+To install the package from local directory run the following command:
+```
+$ pip install .
+```
+In case you are a developer, you should install perceval-puppet in editable mode:
+```
+$ pip install -e .
+```
+
+#### Poetry
+We use [poetry](https://python-poetry.org/) for dependency management and 
+packaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).
+Once you have installed it, you can install perceval-puppet and the dependencies in 
+a project isolated environment using:
+```
+$ poetry install
+```
+To spaw a new shell within the virtual environment use:
+```
+$ poetry shell
+```
+
+## Examples
+
+### Puppet Forge
+
+```
+$ perceval puppetforge
+```
 
-packages = \
-['perceval', 'perceval.backends.puppet', 'tests']
+## License
 
-package_data = \
-{'': ['*'], 'tests': ['data/puppetforge/*']}
+Licensed under GNU General Public License (GPL), version 3 or later.
 
-install_requires = \
-['grimoirelab-toolkit>=0.3', 'perceval>=0.19', 'requests>=2.7.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'perceval-puppet',
-    'version': '0.2.7',
-    'description': 'Bundle of Perceval backends for Puppet, Inc. ecosystem.',
-    'long_description': '# perceval-puppet [![Build Status](https://github.com/chaoss/grimoirelab-perceval-puppet/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-perceval-puppet/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-perceval-puppet.svg)](https://coveralls.io/r/chaoss/grimoirelab-perceval-puppet?branch=master)  [![PyPI version](https://badge.fury.io/py/perceval-puppet.svg)](https://badge.fury.io/py/perceval-puppet)\n\nBundle of Perceval backends for Puppet ecosystem.\n\n## Backends\n\nThe backends currently managed by this package support the next repositories:\n\n* Puppet Forge\n\n## Requirements\n\n * Python >= 3.7\n\nYou will also need some other libraries for running the tool, you can find the\nwhole list of dependencies in [pyproject.toml](pyproject.toml) file.\n\n## Installation\n\nThere are several ways to install perceval-puppet on your system: packages or source \ncode using Poetry or pip.\n\n### PyPI\n\nperceval-puppet can be installed using pip, a tool for installing Python packages. \nTo do it, run the next command:\n```\n$ pip install perceval-puppet\n```\n\n### Source code\n\nTo install from the source code you will need to clone the repository first:\n```\n$ git clone https://github.com/chaoss/grimoirelab-perceval-puppet\n$ cd grimoirelab-perceval-puppet\n```\n\nThen use pip or Poetry to install the package along with its dependencies.\n\n#### Pip\nTo install the package from local directory run the following command:\n```\n$ pip install .\n```\nIn case you are a developer, you should install perceval-puppet in editable mode:\n```\n$ pip install -e .\n```\n\n#### Poetry\nWe use [poetry](https://python-poetry.org/) for dependency management and \npackaging. You can install it following its [documentation](https://python-poetry.org/docs/#installation).\nOnce you have installed it, you can install perceval-puppet and the dependencies in \na project isolated environment using:\n```\n$ poetry install\n```\nTo spaw a new shell within the virtual environment use:\n```\n$ poetry shell\n```\n\n## Examples\n\n### Puppet Forge\n\n```\n$ perceval puppetforge\n```\n\n## License\n\nLicensed under GNU General Public License (GPL), version 3 or later.\n',
-    'author': 'GrimoireLab Developers',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://chaoss.github.io/grimoirelab/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

