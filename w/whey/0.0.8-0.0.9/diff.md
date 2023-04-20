# Comparing `tmp/whey-0.0.8.tar.gz` & `tmp/whey-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whey-0.0.8.tar", last modified: Sun Mar 28 12:09:40 2021, max compression
+gzip compressed data, was "whey-0.0.9.tar", last modified: Tue Apr  6 09:47:08 2021, max compression
```

## Comparing `whey-0.0.8.tar` & `whey-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 12:09:40.984547 whey-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-03-28 12:09:08.000000 whey-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-03-28 12:09:08.000000 whey-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8663 2021-03-28 12:09:40.984547 whey-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5791 2021-03-28 12:09:08.000000 whey-0.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-03-28 12:09:08.000000 whey-0.0.8/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2021-03-28 12:09:08.000000 whey-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-03-28 12:09:08.000000 whey-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2021-03-28 12:09:40.984547 whey-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-03-28 12:09:08.000000 whey-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 12:09:40.980548 whey-0.0.8/whey/
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-03-28 12:09:08.000000 whey-0.0.8/whey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2021-03-28 12:09:08.000000 whey-0.0.8/whey/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21561 2021-03-28 12:09:08.000000 whey-0.0.8/whey/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 12:09:40.984547 whey-0.0.8/whey/config/
--rw-r--r--   0 runner    (1001) docker     (121)     3488 2021-03-28 12:09:08.000000 whey-0.0.8/whey/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17073 2021-03-28 12:09:08.000000 whey-0.0.8/whey/config/pep621.py
--rw-r--r--   0 runner    (1001) docker     (121)    12369 2021-03-28 12:09:08.000000 whey-0.0.8/whey/config/whey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2021-03-28 12:09:08.000000 whey-0.0.8/whey/foreman.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-28 12:09:08.000000 whey-0.0.8/whey/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-28 12:09:40.980548 whey-0.0.8/whey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8663 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      439 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      244 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-28 12:09:40.000000 whey-0.0.8/whey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-04-06 09:46:38.000000 whey-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      136 2021-04-06 09:46:38.000000 whey-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-04-06 09:47:08.739432 whey-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5570 2021-04-06 09:46:38.000000 whey-0.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2021-04-06 09:46:38.000000 whey-0.0.9/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2021-04-06 09:46:38.000000 whey-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-04-06 09:46:38.000000 whey-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1717 2021-04-06 09:47:08.739432 whey-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2021-04-06 09:46:38.000000 whey-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.735432 whey-0.0.9/whey/
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-04-06 09:46:38.000000 whey-0.0.9/whey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3358 2021-04-06 09:46:38.000000 whey-0.0.9/whey/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21561 2021-04-06 09:46:38.000000 whey-0.0.9/whey/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/whey/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17073 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/pep621.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12588 2021-04-06 09:46:38.000000 whey-0.0.9/whey/config/whey.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2021-04-06 09:46:38.000000 whey-0.0.9/whey/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-06 09:46:38.000000 whey-0.0.9/whey/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-06 09:47:08.739432 whey-0.0.9/whey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8410 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      439 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-04-06 09:47:08.000000 whey-0.0.9/whey.egg-info/top_level.txt
```

### Comparing `whey-0.0.8/LICENSE` & `whey-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `whey-0.0.8/PKG-INFO` & `whey-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple Python wheel builder for simple projects.
 Home-page: https://github.com/repo-helper/whey
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: MIT License
 Project-URL: Documentation, https://whey.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/repo-helper/whey/issues
@@ -45,15 +45,15 @@
         	* - PyPI
         	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
         	* - Anaconda
         	  - |conda-version| |conda-platform|
         	* - Activity
         	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
         	* - QA
-        	  - |codefactor| |actions_flake8| |actions_mypy| |pre_commit_ci|
+        	  - |codefactor| |actions_flake8| |actions_mypy|
         	* - Other
         	  - |license| |language| |requires|
         
         .. |docs| image:: https://img.shields.io/readthedocs/whey/latest?logo=read-the-docs
         	:target: https://whey.readthedocs.io/en/latest
         	:alt: Documentation Build Status
         
@@ -120,33 +120,29 @@
         .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
         	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
         	:alt: License
         
         .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
         	:alt: GitHub top language
         
-        .. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.8
+        .. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.9
         	:target: https://github.com/repo-helper/whey/pulse
         	:alt: GitHub commits since tagged version
         
         .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
         	:target: https://github.com/repo-helper/whey/commit/master
         	:alt: GitHub last commit
         
         .. |maintained| image:: https://img.shields.io/maintenance/yes/2021
         	:alt: Maintenance
         
         .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey
         	:target: https://pypi.org/project/whey/
         	:alt: PyPI - Downloads
         
-        .. |pre_commit_ci| image:: https://results.pre-commit.ci/badge/github/repo-helper/whey/master.svg
-        	:target: https://results.pre-commit.ci/latest/github/repo-helper/whey/master
-        	:alt: pre-commit.ci status
-        
         .. end shields
         
         Installation
         --------------
         
         .. start installation
```

### Comparing `whey-0.0.8/README.rst` & `whey-0.0.9/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	* - PyPI
 	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
 	* - Anaconda
 	  - |conda-version| |conda-platform|
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
-	  - |codefactor| |actions_flake8| |actions_mypy| |pre_commit_ci|
+	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
 .. |docs| image:: https://img.shields.io/readthedocs/whey/latest?logo=read-the-docs
 	:target: https://whey.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
@@ -109,33 +109,29 @@
 .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.8
+.. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.9
 	:target: https://github.com/repo-helper/whey/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
 	:target: https://github.com/repo-helper/whey/commit/master
 	:alt: GitHub last commit
 
 .. |maintained| image:: https://img.shields.io/maintenance/yes/2021
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey
 	:target: https://pypi.org/project/whey/
 	:alt: PyPI - Downloads
 
-.. |pre_commit_ci| image:: https://results.pre-commit.ci/badge/github/repo-helper/whey/master.svg
-	:target: https://results.pre-commit.ci/latest/github/repo-helper/whey/master
-	:alt: pre-commit.ci status
-
 .. end shields
 
 Installation
 --------------
 
 .. start installation
```

### Comparing `whey-0.0.8/__pkginfo__.py` & `whey-0.0.9/__pkginfo__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,26 +7,14 @@
 #  In any case, this program is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 #
 # This script based on https://github.com/rocky/python-uncompyle6/blob/master/__pkginfo__.py
 #
 
-# stdlib
-import pathlib
-
 __all__ = [
-		"__copyright__",
 		"__version__",
-		"repo_root",
-		"install_requires",
 		"extras_require",
 		]
 
-__copyright__ = """
-2021 Dominic Davis-Foster <dominic@davis-foster.co.uk>
-"""
-
-__version__ = "0.0.8"
-repo_root = pathlib.Path(__file__).parent
-install_requires = (repo_root / "requirements.txt").read_text(encoding="utf-8").split('\n')
+__version__ = "0.0.9"
 extras_require = {"readme": ["readme-renderer[md]>=27.0"], "all": ["readme-renderer[md]>=27.0"]}
```

### Comparing `whey-0.0.8/pyproject.toml` & `whey-0.0.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whey"
-version = "0.0.8"
+version = "0.0.9"
 description = "A simple Python wheel builder for simple projects."
 readme = "README.rst"
 keywords = [ "pep517", "pep621", "build", "sdist", "wheel", "packaging", "distribution",]
 dynamic = [ "requires-python", "classifiers", "dependencies",]
 
 [[project.authors]]
 email = "dominic@davis-foster.co.uk"
@@ -27,24 +27,15 @@
 [project.scripts]
 whey = "whey.__main__:main"
 
 [project.optional-dependencies]
 readme = [ "readme-renderer[md]>=27.0",]
 all = [ "readme-renderer[md]>=27.0",]
 
-[tool.whey]
-base-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Build Tools",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed",
-]
-python-versions = [ "3.6", "3.7", "3.8", "3.9",]
-python-implementations = [ "CPython", "PyPy",]
-platforms = [ "Windows", "macOS", "Linux",]
+[tool.mkrecipe]
+conda-channels = [ "conda-forge", "domdfcoding",]
+extras = "all"
 license-key = "MIT"
 
 [project.entry-points."whey.builder"]
 whey_sdist = "whey.builder:SDistBuilder"
 whey_wheel = "whey.builder:WheelBuilder"
```

### Comparing `whey-0.0.8/setup.cfg` & `whey-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = whey
+version = 0.0.8
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = pep517, pep621, build, sdist, wheel, packaging, distribution
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
```

### Comparing `whey-0.0.8/whey/__init__.py` & `whey-0.0.9/whey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from whey.foreman import Foreman
 
 __all__ = ["build_sdist", "build_wheel", "SDistBuilder", "WheelBuilder", "Foreman"]
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.0.8"
+__version__: str = "0.0.9"
 __email__: str = "dominic@davis-foster.co.uk"
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
 	"""
 	:pep:`517` hook to build a wheel binary distribution.
```

### Comparing `whey-0.0.8/whey/__main__.py` & `whey-0.0.9/whey/__main__.py`

 * *Files identical despite different names*

### Comparing `whey-0.0.8/whey/builder.py` & `whey-0.0.9/whey/builder.py`

 * *Files identical despite different names*

### Comparing `whey-0.0.8/whey/config/__init__.py` & `whey-0.0.9/whey/config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 #
 #  __init__.py
 """
-:pep:`621` configuration parser.
+``pyproject.toml`` configuration parsing.
 """
 #
 #  Copyright © 2021 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
```

### Comparing `whey-0.0.8/whey/config/pep621.py` & `whey-0.0.9/whey/config/pep621.py`

 * *Files identical despite different names*

### Comparing `whey-0.0.8/whey/config/whey.py` & `whey-0.0.9/whey/config/whey.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 
 		:param config: The unparsed TOML config for the ``[tool.whey]`` table.
 		"""
 
 		parsed_builders = get_default_builders()
 		builders = config["builders"]
 
-		entry_points: Dict[str, importlib_metadata.EntryPoint] = dict(get_entry_points())  # type: ignore
+		entry_points: Dict[str, importlib_metadata.EntryPoint] = {ep.name: ep for ep in get_entry_points()}
 
 		self.assert_type(builders, dict, ["tool", "whey", "builders"])
 
 		for builder_type in ["binary", "sdist", "wheel"]:
 			if builder_type in builders:
 				entry_point_name = builders[builder_type]
 				if entry_point_name not in entry_points:
@@ -333,16 +333,19 @@
 
 	validate_classifiers(parsed_classifiers)
 
 	return natsorted(parsed_classifiers)
 
 
 def get_entry_points() -> Iterable[importlib_metadata.EntryPoint]:
-	"""
-	Returns an iterable over :class:`~.EntryPoint` objects in the ``whey.builder`` group.
-	"""
+	r"""
+	Returns an iterable over `EntryPoint <https://docs.python.org/3/library/importlib.metadata.html#entry-points>`_
+	objects in the ``whey.builder`` group.
+
+	:rtype: :class:`Iterable <typing.Iterable>`\[`EntryPoint <https://docs.python.org/3/library/importlib.metadata.html#entry-points>`_\]
+	"""  # noqa: D400
 
 	eps = itertools.chain.from_iterable(dist.entry_points for dist in importlib_metadata.distributions())
 
 	for entry_point in eps:
 		if entry_point.group == "whey.builder":
 			yield entry_point
```

### Comparing `whey-0.0.8/whey/foreman.py` & `whey-0.0.9/whey/foreman.py`

 * *Files identical despite different names*

### Comparing `whey-0.0.8/whey.egg-info/PKG-INFO` & `whey-0.0.9/whey.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whey
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple Python wheel builder for simple projects.
 Home-page: https://github.com/repo-helper/whey
 Author: Dominic Davis-Foster
 Author-email: dominic@davis-foster.co.uk
 License: MIT License
 Project-URL: Documentation, https://whey.readthedocs.io/en/latest
 Project-URL: Issue Tracker, https://github.com/repo-helper/whey/issues
@@ -45,15 +45,15 @@
         	* - PyPI
         	  - |pypi-version| |supported-versions| |supported-implementations| |wheel|
         	* - Anaconda
         	  - |conda-version| |conda-platform|
         	* - Activity
         	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
         	* - QA
-        	  - |codefactor| |actions_flake8| |actions_mypy| |pre_commit_ci|
+        	  - |codefactor| |actions_flake8| |actions_mypy|
         	* - Other
         	  - |license| |language| |requires|
         
         .. |docs| image:: https://img.shields.io/readthedocs/whey/latest?logo=read-the-docs
         	:target: https://whey.readthedocs.io/en/latest
         	:alt: Documentation Build Status
         
@@ -120,33 +120,29 @@
         .. |license| image:: https://img.shields.io/github/license/repo-helper/whey
         	:target: https://github.com/repo-helper/whey/blob/master/LICENSE
         	:alt: License
         
         .. |language| image:: https://img.shields.io/github/languages/top/repo-helper/whey
         	:alt: GitHub top language
         
-        .. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.8
+        .. |commits-since| image:: https://img.shields.io/github/commits-since/repo-helper/whey/v0.0.9
         	:target: https://github.com/repo-helper/whey/pulse
         	:alt: GitHub commits since tagged version
         
         .. |commits-latest| image:: https://img.shields.io/github/last-commit/repo-helper/whey
         	:target: https://github.com/repo-helper/whey/commit/master
         	:alt: GitHub last commit
         
         .. |maintained| image:: https://img.shields.io/maintenance/yes/2021
         	:alt: Maintenance
         
         .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/whey
         	:target: https://pypi.org/project/whey/
         	:alt: PyPI - Downloads
         
-        .. |pre_commit_ci| image:: https://results.pre-commit.ci/badge/github/repo-helper/whey/master.svg
-        	:target: https://results.pre-commit.ci/latest/github/repo-helper/whey/master
-        	:alt: pre-commit.ci status
-        
         .. end shields
         
         Installation
         --------------
         
         .. start installation
```

