# Comparing `tmp/whey-pth-0.0.4.tar.gz` & `tmp/whey-pth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whey-pth-0.0.4.tar", last modified: Tue Jun 15 12:27:02 2021, max compression
+gzip compressed data, was "whey-pth-0.0.5.tar", last modified: Thu Apr 20 14:10:15 2023, max compression
```

## Comparing `whey-pth-0.0.4.tar` & `whey-pth-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-15 12:27:02.696322 whey-pth-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-06-15 12:26:39.000000 whey-pth-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      144 2021-06-15 12:26:39.000000 whey-pth-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6588 2021-06-15 12:27:02.696322 whey-pth-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2021-06-15 12:26:39.000000 whey-pth-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-06-15 12:26:39.000000 whey-pth-0.0.4/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2021-06-15 12:26:39.000000 whey-pth-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-15 12:26:39.000000 whey-pth-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2021-06-15 12:27:02.696322 whey-pth-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      649 2021-06-15 12:26:39.000000 whey-pth-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-15 12:27:02.696322 whey-pth-0.0.4/whey_pth/
--rw-r--r--   0 runner    (1001) docker     (121)     5337 2021-06-15 12:26:39.000000 whey-pth-0.0.4/whey_pth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-15 12:26:39.000000 whey-pth-0.0.4/whey_pth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-15 12:27:02.696322 whey-pth-0.0.4/whey_pth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6588 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-06-15 12:27:02.000000 whey-pth-0.0.4/whey_pth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-20 14:09:44.000000 whey-pth-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-20 14:09:44.000000 whey-pth-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8323 2023-04-20 14:10:15.795812 whey-pth-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5417 2023-04-20 14:09:44.000000 whey-pth-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5110 2023-04-20 14:09:44.000000 whey-pth-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 14:09:44.000000 whey-pth-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-04-20 14:10:15.795812 whey-pth-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-20 14:09:44.000000 whey-pth-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.791812 whey-pth-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    12145 2023-04-20 14:09:44.000000 whey-pth-0.0.5/tests/test_whey_pth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/whey_pth/
+-rw-r--r--   0 runner    (1001) docker     (122)     5307 2023-04-20 14:09:44.000000 whey-pth-0.0.5/whey_pth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-20 14:09:44.000000 whey-pth-0.0.5/whey_pth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 14:10:15.795812 whey-pth-0.0.5/whey_pth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8323 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-20 14:10:15.000000 whey-pth-0.0.5/whey_pth.egg-info/top_level.txt
```

### Comparing `whey-pth-0.0.4/LICENSE` & `whey-pth-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `whey-pth-0.0.4/README.rst` & `whey-pth-0.0.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/repo-helper/whey-pth/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/repo-helper/whey-pth/workflows/mypy/badge.svg
 	:target: https://github.com/repo-helper/whey-pth/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://requires.io/github/repo-helper/whey-pth/requirements.svg?branch=master
-	:target: https://requires.io/github/repo-helper/whey-pth/requirements/?branch=master
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/repo-helper/whey-pth/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/repo-helper/whey-pth/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/repo-helper/whey-pth/master?logo=coveralls
 	:target: https://coveralls.io/github/repo-helper/whey-pth?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/repo-helper/whey-pth?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey-pth
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.4
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey-pth/v0.0.5
 	:target: https://github.com/repo-helper/whey-pth/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey-pth
 	:target: https://github.com/repo-helper/whey-pth/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2021
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey-pth
 	:target: https://pypi.org/project/whey-pth/
 	:alt: PyPI - Downloads
 
 .. end shields
@@ -143,7 +143,21 @@
 	* Then install
 
 	.. code-block:: bash
 
 		$ conda install whey-pth
 
 .. end installation
+
+-----
+
+To enable ``whey-pth``, add the following lines to your ``pyproject.toml`` file:
+
+.. code-block:: TOML
+
+	[tool.whey.builders]
+	wheel = "whey_pth_wheel"
+
+The ``whey-pth``-specific configuration is defined in the ``tool.whey-pth`` table.
+See `the documentation`_ for more details.
+
+.. _the documentation: https://whey-pth.readthedocs.io/en/latest/
```

### Comparing `whey-pth-0.0.4/setup.py` & `whey-pth-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 import sys
 
 # 3rd party
 from setuptools import setup
 
 sys.path.append('.')
 
-# this package
-from __pkginfo__ import *  # pylint: disable=wildcard-import
+extras_require = {}
 
 repo_root = pathlib.Path(__file__).parent
 install_requires = (repo_root / "requirements.txt").read_text(encoding="UTF-8").split('\n')
 
 setup(
 		description="Extension to whey to support .pth files.",
 		extras_require=extras_require,
 		install_requires=install_requires,
+		name="whey-pth",
 		py_modules=[],
-		version=__version__,
 		)
 
 shutil.rmtree("whey_pth.egg-info", ignore_errors=True)
```

### Comparing `whey-pth-0.0.4/whey_pth/__init__.py` & `whey-pth-0.0.5/whey_pth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import dom_toml
 from dom_toml.parser import TOML_TYPES, AbstractConfigParser, BadConfigError
 from whey.builder import WheelBuilder
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.0.4"
+__version__: str = "0.0.5"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["PthWheelBuilder", "WheyPthParser"]
 
 
 class PthWheelBuilder(WheelBuilder):
 	"""
@@ -53,15 +53,14 @@
 	:param build_dir: The (temporary) build directory.
 	:default build_dir: :file:`{<project_dir>}/build/wheel`
 	:param out_dir: The output directory.
 	:default out_dir: :file:`{<project_dir>}/dist`
 	:param verbose: Enable verbose output.
 
 	.. autosummary-widths:: 5/16
-		:html: 3/10
 	"""
 
 	def write_pth_files(self):
 		"""
 		Write ``.pth`` files, and their associated files, into the build directory.
 
 		.. latex:clearpage::
@@ -88,15 +87,14 @@
 
 
 class WheyPthParser(AbstractConfigParser):
 	"""
 	Parser for the ``[tool.whey-pth]`` table from ``pyproject.toml``.
 
 	.. autosummary-widths:: 1/2
-		:html: 45/100
 	"""
 
 	factories = {"additional-wheel-files": list}
 
 	def parse_name(self, config: Dict[str, TOML_TYPES]) -> str:
 		"""
 		Parse the ``name`` key, giving the desired name of the ``.pth`` file.
```

