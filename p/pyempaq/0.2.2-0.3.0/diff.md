# Comparing `tmp/pyempaq-0.2.2.tar.gz` & `tmp/pyempaq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyempaq-0.2.2.tar", last modified: Mon Nov 22 17:44:46 2021, max compression
+gzip compressed data, was "pyempaq-0.3.0.tar", last modified: Wed Apr 19 21:48:06 2023, max compression
```

## Comparing `pyempaq-0.2.2.tar` & `pyempaq-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2021-11-22 17:44:46.281379 pyempaq-0.2.2/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    35149 2021-07-15 22:17:23.000000 pyempaq-0.2.2/LICENSE
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       59 2021-09-26 15:51:02.000000 pyempaq-0.2.2/MANIFEST.in
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    10551 2021-11-22 17:44:46.281379 pyempaq-0.2.2/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     9859 2021-09-27 00:14:47.000000 pyempaq-0.2.2/README.md
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2021-11-22 17:44:46.281379 pyempaq-0.2.2/pyempaq/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      258 2021-07-17 21:32:58.000000 pyempaq-0.2.2/pyempaq/__main__.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     5883 2021-09-21 20:12:14.000000 pyempaq-0.2.2/pyempaq/config_manager.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     5094 2021-09-21 20:12:14.000000 pyempaq-0.2.2/pyempaq/main.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     4209 2021-11-22 17:38:57.000000 pyempaq-0.2.2/pyempaq/unpacker.py
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2021-11-22 17:44:46.281379 pyempaq-0.2.2/pyempaq.egg-info/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    10551 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      325 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/SOURCES.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/dependency_links.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       47 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/entry_points.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       16 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/requires.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        8 2021-11-22 17:44:46.000000 pyempaq-0.2.2/pyempaq.egg-info/top_level.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       16 2021-09-23 10:49:28.000000 pyempaq-0.2.2/requirements.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2021-11-22 17:44:46.281379 pyempaq-0.2.2/setup.cfg
--rwxrwxr-x   0 facundo   (1000) facundo   (1000)     1249 2021-11-22 17:44:34.000000 pyempaq-0.2.2/setup.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    35149 2021-07-15 22:17:23.000000 pyempaq-0.3.0/LICENSE
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       59 2021-09-26 15:51:02.000000 pyempaq-0.3.0/MANIFEST.in
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-19 21:48:06.680242 pyempaq-0.3.0/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12207 2023-04-19 21:19:57.000000 pyempaq-0.3.0/README.md
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/pyempaq/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      267 2023-02-19 18:32:46.000000 pyempaq-0.3.0/pyempaq/__init__.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      258 2021-07-17 21:32:58.000000 pyempaq-0.3.0/pyempaq/__main__.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      488 2023-04-19 21:39:32.000000 pyempaq-0.3.0/pyempaq/_version.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     1485 2022-06-19 15:17:40.000000 pyempaq-0.3.0/pyempaq/common.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     6381 2023-04-17 17:23:34.000000 pyempaq-0.3.0/pyempaq/config_manager.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     9659 2023-04-17 17:23:34.000000 pyempaq-0.3.0/pyempaq/main.py
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)     6526 2023-04-19 21:19:57.000000 pyempaq-0.3.0/pyempaq/unpacker.py
+drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2023-04-19 21:48:06.680242 pyempaq-0.3.0/pyempaq.egg-info/
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)    12899 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/PKG-INFO
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)      383 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       47 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/entry_points.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/requires.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)        8 2023-04-19 21:48:06.000000 pyempaq-0.3.0/pyempaq.egg-info/top_level.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       28 2022-04-15 13:03:12.000000 pyempaq-0.3.0/requirements.txt
+-rw-rw-r--   0 facundo   (1000) facundo   (1000)       38 2023-04-19 21:48:06.680242 pyempaq-0.3.0/setup.cfg
+-rwxrwxr-x   0 facundo   (1000) facundo   (1000)     1776 2023-04-19 21:47:43.000000 pyempaq-0.3.0/setup.py
```

### Comparing `pyempaq-0.2.2/LICENSE` & `pyempaq-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyempaq-0.2.2/PKG-INFO` & `pyempaq-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyempaq
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Python packer to run anywhwere any project with any virtualenv dependencies.
 Home-page: https://github.com/facundobatista/pyempaq
 Author: Facundo Batista
 Author-email: facundo@taniquetil.com.ar
 License: GPL-v3
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyEmpaq
 
 A simple but powerful Python packer to run any project with any virtualenv dependencies anywhwere.
 
@@ -40,18 +40,20 @@
 - [in a terminal](https://github.com/facundobatista/pyempaq/blob/main/examples/simple-command-line.pyz?raw=True): a very small pure terminal example (this, of course, needs to be run in a terminal)
 - [a game](https://github.com/facundobatista/pyempaq/blob/main/examples/arcade-game.pyz?raw=True): a simple game using the [Python Arcade](https://api.arcade.academy/en/latest/) library (actually, it's the [example #6 from their tutorial](https://api.arcade.academy/en/latest/examples/platform_tutorial/step_06.html))
 - [desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/desktop-qt-app.pyz?raw=True): a full-fledged desktop application using PyQt5 (this [Encuentro app](https://encuentro.taniquetil.com.ar/))
 
 ![logo](https://github.com/facundobatista/pyempaq/blob/main/resources/logo-256.png?raw=True)
 
 
-You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install).
+You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install-pyempaq).
 
 PyEmpaq is security friendly, there is nothing obscure or secretly shipped when you distribute your project with it: anybody can just open the `pyz` file (it's just a ZIP) and inspect it.
 
+It's also safe regarding licenses when distributing your packed software. Unlike packing mechanisms that rely on putting inside a big blob, with PyEmpaq you don't have to worry about the licenses of your software dependencies (and the dependencies' dependencies) in regard to distributing them.
+
 
 ### Limitations:
 
 There are some limitations:
 
 - Only Python >= 3.7 is supported
 
@@ -68,15 +70,15 @@
 
 There are two phases: packing and execution. 
 
 The **packing phase** is executed by the project developer, only once, before distribution. It's a simple step where the developer runs PyEmpaq indicating all needed info, and PyEmpaq will produce a single `<projectname>.pyz` file. That's all, and that only file is what is needed for distribution.
 
 In this packing phase, PyEmpaq builds the indicated packed file, putting inside:
 
-- the payload project, with all the indicated modules and binary files (currently *everything from the project*, but this will be improved in the future)
+- the payload project, with all the indicated modules and binary files
 
 - an *unpacker* script from PyEmpaq, which will be run during the execution phase
 
 - few more stuff: some needed infrastructure details for the `.pyz` to run correctly
 
 After packing, the developer will distribute the packed file, final users will download/receive/get it, and execute it.
 
@@ -105,52 +107,81 @@
 
 - `pyempaq .`
 
 - `pyempaq /data/project/`
 
 - `pyempaq ~/repo/proj/config.yaml`
 
-**Note**: [in the future](https://github.com/facundobatista/pyempaq/issues/8) we will be able to control verbosity, we're not there yet.
+You can control verbosity by adding these command line parameters to control logging levels:
+
+- `-v, --verbose` - Show detailed information, typically of interest only when diagnosing problems.
+- `-q, --quiet` - Only events of WARNING level and above will be tracked.
+
+All that said, there is an special option `-V, --version` that if used will just print the version and exit.
+
+> **Note**
+> In the **execution phase**, if you have an environment variable `PYEMPAQ_DEBUG=1` it will show the Pyempaq log lines during the execution.
 
 
 ## The configuration file
 
 All the information that PyEmpaq needs to pack a project comes from a configuration file, which the developer would normally have in the project itself.
 
 The following is the structure of the `pyempaq.yaml` configuration file:
 
 - `name` [mandatory]: the name of the project.
 
-- `basedir` [optional, defaults to where the configuration file is located]: the project's base directory.
+- `basedir` [optional]: the project's base directory; if not included it defaults to where the configuration file is located.
 
 - `exec` [mandatory]: the section where is defined the information to execute the project once unpacked; it holds different subkeys (some subkeys are marked with †: ONE of those keys must be present, but only ONE):
 
     - `script` [†]: the filepath of the python script to run; when unpacking PyEmpaq will do `python3 SCRIPT`.
 
     - `module` [†]: the name of the module to invoke; when unpacking PyEmpaq will do `python3 -m MODULE`.
 
     - `entrypoint` [†]: freeform, as a list of strings; when unpacking PyEmpaq will only insert the proper python3 at the beginning: `python3 STR1 STR2 ...`.
 
-    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed); **note** that this option is [not available yet](https://github.com/facundobatista/pyempaq/issues/14).
+    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed).
+
+- `requirements` [optional]: a list of filepaths pointing to the requirement files with pip-installable dependencies.
 
-- `requirements`: a list of filepaths pointing to the requirement files with pip-installable dependencies.
+- `dependencies` [optional]: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
 
-- `dependencies`: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
+- `include` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to include in the pack (see below); if not included it defaults to `["./**"]` which means all the files and directories in the project.
+
+- `exclude` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to exclude from the pack (see below).
+
+- `unpack-restrictions` [optional]: a section to specify different restrictions to be verified/enforced during unpack.
+
+    - `minimum-python-version` [optional]: a string specifying the minimum version possible to run correctly.
 
 All specified filepaths must exist inside the project and must be relative (to the project's base directory), with the exception of `basedir` itself which can be absolute or relative (to the configuration file location).
 
+Both `include` and `exclude` options use pattern matching according to the rules used by the Unix shell, using `*`, `?`, and character ranges expressed with `[]`. Also `**` will match any files and zero or more directories. For more information or subtleties check the [`glob.glob`](https://docs.python.org/dev/library/glob.html#glob.glob) documentation.
+
+Note that the final user may ignore/bypass any unpack restrictions using the `PYEMPAQ_IGNORE_RESTRICTIONS` environment variable with a value of comma-separated names of which restrictions to ignore.
+
 The following are examples of different configuration files (which were the ones used to build the packed examples mentioned before):
 
 - [the terminal script](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-script.yaml?raw=True)
 
 - [the simple game](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-game.yaml?raw=True)
 
 - [the full desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-desktop-app.yaml?raw=True)
 
 
+## Context of the project being run
+
+When the packed script/module/whatever is run in the unpacking phase, it will be executed inside the virtualenv with the needed requirements/dependencies (freshly created and installed or reused from a previous run).
+
+Also, the following environment variable will be set:
+
+- `PYEMPAQ_PYZ_PATH`: the absolute path to the `.pyz` run by the user
+
+
 ## How to install PyEmpaq
 
 Directly from PyPI:
 
     pip install --user --upgrade --ignore-installed pyempaq
 
 It's handy to install it using `pipx`, if you have it:
@@ -170,14 +201,16 @@
 
 - a `src` and `media`, with stuff to be imported and accessed.
 
 - a `pyempaq.yaml` with the configuration for PyEmpaq.
 
 - a `ep.py` file which is the project's entrypoint; all it does is to inform it started, import the internal module, access the media files, and use the declared dependency, reporting every step.
 
+- a `secrets.txt` file that must not be included in the packed file.
+
 This explores most of the needs of any project. You can try this example, and surely after you will be ready to actually pack any other project you want.
 
 So, let's pack the example source project. As you're working with the PyEmpaq project itself (as you're packing its example), you don't really need to have it installed yet. In that case, if you have `fades` installed is super easy:
 
     fades -r requirements.txt -m pyempaq examples/srcproject/
 
 Otherwise, you would need to create and use a virtual environment:
@@ -201,7 +234,12 @@
     Code access ok .../pyempaq/projectname-20210722013526/orig/src/foo.py
     Media access ok
     Module requests imported .../pyempaq/projectname-20210722013526/venv/lib/python3.8/site-packages/requests/__init__.py
 
 This shows that what you've run actually started, accessed the internal modules and other files, and imported correctly a custom-installed dependency.
 
 
+## How to contribute to the project?
+
+Please check [the how to contribute](https://github.com/facundobatista/pyempaq/blob/main/CONTRIBUTING.md) instructions.
+
+
```

### Comparing `pyempaq-0.2.2/README.md` & `pyempaq-0.3.0/pyempaq.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pyempaq
+Version: 0.3.0
+Summary: A Python packer to run anywhwere any project with any virtualenv dependencies.
+Home-page: https://github.com/facundobatista/pyempaq
+Author: Facundo Batista
+Author-email: facundo@taniquetil.com.ar
+License: GPL-v3
+Platform: UNKNOWN
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Archiving :: Packaging
+Classifier: Topic :: System :: Software Distribution
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyEmpaq
 
 A simple but powerful Python packer to run any project with any virtualenv dependencies anywhwere.
 
 With PyEmpaq you can convert any Python project (see limitations below) into a single `.pyz` file with all the project's content packed inside. 
 
 Packing is super simple, see this demo:
@@ -21,18 +40,20 @@
 - [in a terminal](https://github.com/facundobatista/pyempaq/blob/main/examples/simple-command-line.pyz?raw=True): a very small pure terminal example (this, of course, needs to be run in a terminal)
 - [a game](https://github.com/facundobatista/pyempaq/blob/main/examples/arcade-game.pyz?raw=True): a simple game using the [Python Arcade](https://api.arcade.academy/en/latest/) library (actually, it's the [example #6 from their tutorial](https://api.arcade.academy/en/latest/examples/platform_tutorial/step_06.html))
 - [desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/desktop-qt-app.pyz?raw=True): a full-fledged desktop application using PyQt5 (this [Encuentro app](https://encuentro.taniquetil.com.ar/))
 
 ![logo](https://github.com/facundobatista/pyempaq/blob/main/resources/logo-256.png?raw=True)
 
 
-You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install).
+You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install-pyempaq).
 
 PyEmpaq is security friendly, there is nothing obscure or secretly shipped when you distribute your project with it: anybody can just open the `pyz` file (it's just a ZIP) and inspect it.
 
+It's also safe regarding licenses when distributing your packed software. Unlike packing mechanisms that rely on putting inside a big blob, with PyEmpaq you don't have to worry about the licenses of your software dependencies (and the dependencies' dependencies) in regard to distributing them.
+
 
 ### Limitations:
 
 There are some limitations:
 
 - Only Python >= 3.7 is supported
 
@@ -49,15 +70,15 @@
 
 There are two phases: packing and execution. 
 
 The **packing phase** is executed by the project developer, only once, before distribution. It's a simple step where the developer runs PyEmpaq indicating all needed info, and PyEmpaq will produce a single `<projectname>.pyz` file. That's all, and that only file is what is needed for distribution.
 
 In this packing phase, PyEmpaq builds the indicated packed file, putting inside:
 
-- the payload project, with all the indicated modules and binary files (currently *everything from the project*, but this will be improved in the future)
+- the payload project, with all the indicated modules and binary files
 
 - an *unpacker* script from PyEmpaq, which will be run during the execution phase
 
 - few more stuff: some needed infrastructure details for the `.pyz` to run correctly
 
 After packing, the developer will distribute the packed file, final users will download/receive/get it, and execute it.
 
@@ -86,52 +107,81 @@
 
 - `pyempaq .`
 
 - `pyempaq /data/project/`
 
 - `pyempaq ~/repo/proj/config.yaml`
 
-**Note**: [in the future](https://github.com/facundobatista/pyempaq/issues/8) we will be able to control verbosity, we're not there yet.
+You can control verbosity by adding these command line parameters to control logging levels:
+
+- `-v, --verbose` - Show detailed information, typically of interest only when diagnosing problems.
+- `-q, --quiet` - Only events of WARNING level and above will be tracked.
+
+All that said, there is an special option `-V, --version` that if used will just print the version and exit.
+
+> **Note**
+> In the **execution phase**, if you have an environment variable `PYEMPAQ_DEBUG=1` it will show the Pyempaq log lines during the execution.
 
 
 ## The configuration file
 
 All the information that PyEmpaq needs to pack a project comes from a configuration file, which the developer would normally have in the project itself.
 
 The following is the structure of the `pyempaq.yaml` configuration file:
 
 - `name` [mandatory]: the name of the project.
 
-- `basedir` [optional, defaults to where the configuration file is located]: the project's base directory.
+- `basedir` [optional]: the project's base directory; if not included it defaults to where the configuration file is located.
 
 - `exec` [mandatory]: the section where is defined the information to execute the project once unpacked; it holds different subkeys (some subkeys are marked with †: ONE of those keys must be present, but only ONE):
 
     - `script` [†]: the filepath of the python script to run; when unpacking PyEmpaq will do `python3 SCRIPT`.
 
     - `module` [†]: the name of the module to invoke; when unpacking PyEmpaq will do `python3 -m MODULE`.
 
     - `entrypoint` [†]: freeform, as a list of strings; when unpacking PyEmpaq will only insert the proper python3 at the beginning: `python3 STR1 STR2 ...`.
 
-    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed); **note** that this option is [not available yet](https://github.com/facundobatista/pyempaq/issues/14).
+    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed).
+
+- `requirements` [optional]: a list of filepaths pointing to the requirement files with pip-installable dependencies.
 
-- `requirements`: a list of filepaths pointing to the requirement files with pip-installable dependencies.
+- `dependencies` [optional]: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
 
-- `dependencies`: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
+- `include` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to include in the pack (see below); if not included it defaults to `["./**"]` which means all the files and directories in the project.
+
+- `exclude` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to exclude from the pack (see below).
+
+- `unpack-restrictions` [optional]: a section to specify different restrictions to be verified/enforced during unpack.
+
+    - `minimum-python-version` [optional]: a string specifying the minimum version possible to run correctly.
 
 All specified filepaths must exist inside the project and must be relative (to the project's base directory), with the exception of `basedir` itself which can be absolute or relative (to the configuration file location).
 
+Both `include` and `exclude` options use pattern matching according to the rules used by the Unix shell, using `*`, `?`, and character ranges expressed with `[]`. Also `**` will match any files and zero or more directories. For more information or subtleties check the [`glob.glob`](https://docs.python.org/dev/library/glob.html#glob.glob) documentation.
+
+Note that the final user may ignore/bypass any unpack restrictions using the `PYEMPAQ_IGNORE_RESTRICTIONS` environment variable with a value of comma-separated names of which restrictions to ignore.
+
 The following are examples of different configuration files (which were the ones used to build the packed examples mentioned before):
 
 - [the terminal script](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-script.yaml?raw=True)
 
 - [the simple game](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-game.yaml?raw=True)
 
 - [the full desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-desktop-app.yaml?raw=True)
 
 
+## Context of the project being run
+
+When the packed script/module/whatever is run in the unpacking phase, it will be executed inside the virtualenv with the needed requirements/dependencies (freshly created and installed or reused from a previous run).
+
+Also, the following environment variable will be set:
+
+- `PYEMPAQ_PYZ_PATH`: the absolute path to the `.pyz` run by the user
+
+
 ## How to install PyEmpaq
 
 Directly from PyPI:
 
     pip install --user --upgrade --ignore-installed pyempaq
 
 It's handy to install it using `pipx`, if you have it:
@@ -151,14 +201,16 @@
 
 - a `src` and `media`, with stuff to be imported and accessed.
 
 - a `pyempaq.yaml` with the configuration for PyEmpaq.
 
 - a `ep.py` file which is the project's entrypoint; all it does is to inform it started, import the internal module, access the media files, and use the declared dependency, reporting every step.
 
+- a `secrets.txt` file that must not be included in the packed file.
+
 This explores most of the needs of any project. You can try this example, and surely after you will be ready to actually pack any other project you want.
 
 So, let's pack the example source project. As you're working with the PyEmpaq project itself (as you're packing its example), you don't really need to have it installed yet. In that case, if you have `fades` installed is super easy:
 
     fades -r requirements.txt -m pyempaq examples/srcproject/
 
 Otherwise, you would need to create and use a virtual environment:
@@ -180,7 +232,14 @@
 
     Hello world
     Code access ok .../pyempaq/projectname-20210722013526/orig/src/foo.py
     Media access ok
     Module requests imported .../pyempaq/projectname-20210722013526/venv/lib/python3.8/site-packages/requests/__init__.py
 
 This shows that what you've run actually started, accessed the internal modules and other files, and imported correctly a custom-installed dependency.
+
+
+## How to contribute to the project?
+
+Please check [the how to contribute](https://github.com/facundobatista/pyempaq/blob/main/CONTRIBUTING.md) instructions.
+
+
```

### Comparing `pyempaq-0.2.2/pyempaq/config_manager.py` & `pyempaq-0.3.0/pyempaq/config_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 # base directory to which the different included paths may be relative from
 _BASEDIR = None
 
 # directory where the config is taken from, which is the default for basedir
 _CONFIGDIR = None
 
+# the default include value to get all the project inside
+DEFAULT_INCLUDE_LIST = ["./**"]
+
 
 class ConfigError(Exception):
     """Specific errors found in the config."""
 
     def __init__(self, msg=None, errors=None):
         if msg is None:
             msg = "Problem(s) found in configuration file:"
@@ -96,22 +99,35 @@
 
     script: RelativeFile = None
     module: RelativePath = None
     entrypoint: List[pydantic.StrictStr] = None
     default_args: List[pydantic.StrictStr] = []
 
 
-class Config(ModelConfigDefaults, validate_all=False):
+class UnpackRestrictions(ModelConfigDefaults, alias_generator=lambda s: s.replace("_", "-")):
+    """Restrictions that will be verified/enforced during unpack."""
+
+    minimum_python_version: pydantic.StrictStr = None
+
+
+class Config(
+    ModelConfigDefaults,
+    validate_all=False,
+    alias_generator=lambda s: s.replace("_", "-"),
+):
     """Definition of PyEmpaq's configuration."""
 
     name: str
     basedir: pathlib.Path  # the default for this is managed on YAML load time
     exec: Executor
     requirements: List[RelativeFile] = []
     dependencies: List[str] = []
+    include: List[str] = DEFAULT_INCLUDE_LIST
+    exclude: List[str] = []
+    unpack_restrictions: UnpackRestrictions = None
 
     @pydantic.validator("basedir")
     def ensure_basedir(cls, value):
         """Ensure that the basedir is valid, and store it to be used by other paths."""
         global _BASEDIR
 
         value = value.expanduser()
```

### Comparing `pyempaq-0.2.2/pyempaq.egg-info/PKG-INFO` & `pyempaq-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pyempaq
-Version: 0.2.2
-Summary: A Python packer to run anywhwere any project with any virtualenv dependencies.
-Home-page: https://github.com/facundobatista/pyempaq
-Author: Facundo Batista
-Author-email: facundo@taniquetil.com.ar
-License: GPL-v3
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Archiving :: Packaging
-Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyEmpaq
 
 A simple but powerful Python packer to run any project with any virtualenv dependencies anywhwere.
 
 With PyEmpaq you can convert any Python project (see limitations below) into a single `.pyz` file with all the project's content packed inside. 
 
 Packing is super simple, see this demo:
@@ -40,18 +21,20 @@
 - [in a terminal](https://github.com/facundobatista/pyempaq/blob/main/examples/simple-command-line.pyz?raw=True): a very small pure terminal example (this, of course, needs to be run in a terminal)
 - [a game](https://github.com/facundobatista/pyempaq/blob/main/examples/arcade-game.pyz?raw=True): a simple game using the [Python Arcade](https://api.arcade.academy/en/latest/) library (actually, it's the [example #6 from their tutorial](https://api.arcade.academy/en/latest/examples/platform_tutorial/step_06.html))
 - [desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/desktop-qt-app.pyz?raw=True): a full-fledged desktop application using PyQt5 (this [Encuentro app](https://encuentro.taniquetil.com.ar/))
 
 ![logo](https://github.com/facundobatista/pyempaq/blob/main/resources/logo-256.png?raw=True)
 
 
-You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install).
+You can install `pyempaq` directly from PyPI; see [instructions below](https://github.com/facundobatista/pyempaq#how-to-install-pyempaq).
 
 PyEmpaq is security friendly, there is nothing obscure or secretly shipped when you distribute your project with it: anybody can just open the `pyz` file (it's just a ZIP) and inspect it.
 
+It's also safe regarding licenses when distributing your packed software. Unlike packing mechanisms that rely on putting inside a big blob, with PyEmpaq you don't have to worry about the licenses of your software dependencies (and the dependencies' dependencies) in regard to distributing them.
+
 
 ### Limitations:
 
 There are some limitations:
 
 - Only Python >= 3.7 is supported
 
@@ -68,15 +51,15 @@
 
 There are two phases: packing and execution. 
 
 The **packing phase** is executed by the project developer, only once, before distribution. It's a simple step where the developer runs PyEmpaq indicating all needed info, and PyEmpaq will produce a single `<projectname>.pyz` file. That's all, and that only file is what is needed for distribution.
 
 In this packing phase, PyEmpaq builds the indicated packed file, putting inside:
 
-- the payload project, with all the indicated modules and binary files (currently *everything from the project*, but this will be improved in the future)
+- the payload project, with all the indicated modules and binary files
 
 - an *unpacker* script from PyEmpaq, which will be run during the execution phase
 
 - few more stuff: some needed infrastructure details for the `.pyz` to run correctly
 
 After packing, the developer will distribute the packed file, final users will download/receive/get it, and execute it.
 
@@ -105,52 +88,81 @@
 
 - `pyempaq .`
 
 - `pyempaq /data/project/`
 
 - `pyempaq ~/repo/proj/config.yaml`
 
-**Note**: [in the future](https://github.com/facundobatista/pyempaq/issues/8) we will be able to control verbosity, we're not there yet.
+You can control verbosity by adding these command line parameters to control logging levels:
+
+- `-v, --verbose` - Show detailed information, typically of interest only when diagnosing problems.
+- `-q, --quiet` - Only events of WARNING level and above will be tracked.
+
+All that said, there is an special option `-V, --version` that if used will just print the version and exit.
+
+> **Note**
+> In the **execution phase**, if you have an environment variable `PYEMPAQ_DEBUG=1` it will show the Pyempaq log lines during the execution.
 
 
 ## The configuration file
 
 All the information that PyEmpaq needs to pack a project comes from a configuration file, which the developer would normally have in the project itself.
 
 The following is the structure of the `pyempaq.yaml` configuration file:
 
 - `name` [mandatory]: the name of the project.
 
-- `basedir` [optional, defaults to where the configuration file is located]: the project's base directory.
+- `basedir` [optional]: the project's base directory; if not included it defaults to where the configuration file is located.
 
 - `exec` [mandatory]: the section where is defined the information to execute the project once unpacked; it holds different subkeys (some subkeys are marked with †: ONE of those keys must be present, but only ONE):
 
     - `script` [†]: the filepath of the python script to run; when unpacking PyEmpaq will do `python3 SCRIPT`.
 
     - `module` [†]: the name of the module to invoke; when unpacking PyEmpaq will do `python3 -m MODULE`.
 
     - `entrypoint` [†]: freeform, as a list of strings; when unpacking PyEmpaq will only insert the proper python3 at the beginning: `python3 STR1 STR2 ...`.
 
-    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed); **note** that this option is [not available yet](https://github.com/facundobatista/pyempaq/issues/14).
+    - `default-args` [optional]: the default arguments to be passed to the script/module/entrypoint (if not overriden when the distributed `.pyz` is executed).
+
+- `requirements` [optional]: a list of filepaths pointing to the requirement files with pip-installable dependencies.
+
+- `dependencies` [optional]: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
+
+- `include` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to include in the pack (see below); if not included it defaults to `["./**"]` which means all the files and directories in the project.
+
+- `exclude` [optional]: a list of strings, each one specifying a pattern to decide what files and directories to exclude from the pack (see below).
 
-- `requirements`: a list of filepaths pointing to the requirement files with pip-installable dependencies.
+- `unpack-restrictions` [optional]: a section to specify different restrictions to be verified/enforced during unpack.
 
-- `dependencies`: a list of strings to directly specify packages to be installed by `pip` without needing to have a requirement file.
+    - `minimum-python-version` [optional]: a string specifying the minimum version possible to run correctly.
 
 All specified filepaths must exist inside the project and must be relative (to the project's base directory), with the exception of `basedir` itself which can be absolute or relative (to the configuration file location).
 
+Both `include` and `exclude` options use pattern matching according to the rules used by the Unix shell, using `*`, `?`, and character ranges expressed with `[]`. Also `**` will match any files and zero or more directories. For more information or subtleties check the [`glob.glob`](https://docs.python.org/dev/library/glob.html#glob.glob) documentation.
+
+Note that the final user may ignore/bypass any unpack restrictions using the `PYEMPAQ_IGNORE_RESTRICTIONS` environment variable with a value of comma-separated names of which restrictions to ignore.
+
 The following are examples of different configuration files (which were the ones used to build the packed examples mentioned before):
 
 - [the terminal script](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-script.yaml?raw=True)
 
 - [the simple game](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-game.yaml?raw=True)
 
 - [the full desktop app](https://github.com/facundobatista/pyempaq/blob/main/examples/pyempaq-desktop-app.yaml?raw=True)
 
 
+## Context of the project being run
+
+When the packed script/module/whatever is run in the unpacking phase, it will be executed inside the virtualenv with the needed requirements/dependencies (freshly created and installed or reused from a previous run).
+
+Also, the following environment variable will be set:
+
+- `PYEMPAQ_PYZ_PATH`: the absolute path to the `.pyz` run by the user
+
+
 ## How to install PyEmpaq
 
 Directly from PyPI:
 
     pip install --user --upgrade --ignore-installed pyempaq
 
 It's handy to install it using `pipx`, if you have it:
@@ -170,14 +182,16 @@
 
 - a `src` and `media`, with stuff to be imported and accessed.
 
 - a `pyempaq.yaml` with the configuration for PyEmpaq.
 
 - a `ep.py` file which is the project's entrypoint; all it does is to inform it started, import the internal module, access the media files, and use the declared dependency, reporting every step.
 
+- a `secrets.txt` file that must not be included in the packed file.
+
 This explores most of the needs of any project. You can try this example, and surely after you will be ready to actually pack any other project you want.
 
 So, let's pack the example source project. As you're working with the PyEmpaq project itself (as you're packing its example), you don't really need to have it installed yet. In that case, if you have `fades` installed is super easy:
 
     fades -r requirements.txt -m pyempaq examples/srcproject/
 
 Otherwise, you would need to create and use a virtual environment:
@@ -201,7 +215,10 @@
     Code access ok .../pyempaq/projectname-20210722013526/orig/src/foo.py
     Media access ok
     Module requests imported .../pyempaq/projectname-20210722013526/venv/lib/python3.8/site-packages/requests/__init__.py
 
 This shows that what you've run actually started, accessed the internal modules and other files, and imported correctly a custom-installed dependency.
 
 
+## How to contribute to the project?
+
+Please check [the how to contribute](https://github.com/facundobatista/pyempaq/blob/main/CONTRIBUTING.md) instructions.
```

### Comparing `pyempaq-0.2.2/setup.py` & `pyempaq-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 #!/usr/bin/env python3
 
-# Copyright 2021 Facundo Batista
+# Copyright 2021-2023 Facundo Batista
 # Licensed under the GPL v3 License
 # For further info, check https://github.com/facundobatista/pyempaq
 
 """Setup script for PyEmpaq."""
 
+import re
 from setuptools import setup
 
+
+def get_version():
+    """Retrieve the package version from the file.
+
+    This is done by parsing statically the file, not importing it as a module,
+    because the version is needed in intermediate steps where the package itself
+    is not yet available.
+    """
+    with open('pyempaq/_version.py') as fh:
+        m = re.search(r"VERSION *= *\((.*)\)", fh.read())
+    if m is None:
+        raise ValueError("Unrecognized version in 'pyempaq/_version.py'")
+    return m.groups()[0].replace(', ', '.')
+
+
 with open("requirements.txt", "rt") as fh:
     install_requires = [x.strip() for x in fh]
 
 setup(
     name="pyempaq",
-    version="0.2.2",
+    version=get_version(),
     author="Facundo Batista",
     author_email="facundo@taniquetil.com.ar",
     description="A Python packer to run anywhwere any project with any virtualenv dependencies.",
     long_description=open("README.md", "rt", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/facundobatista/pyempaq",
     license="GPL-v3",
@@ -30,9 +46,9 @@
         "Topic :: System :: Archiving :: Packaging",
         "Topic :: System :: Software Distribution",
     ],
     entry_points={
         "console_scripts": ["pyempaq = pyempaq.main:main"],
     },
     install_requires=install_requires,
-    python_requires=">=3.5",
+    python_requires=">=3.9",
 )
```

