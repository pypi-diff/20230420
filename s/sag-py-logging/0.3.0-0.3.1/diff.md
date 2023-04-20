# Comparing `tmp/sag-py-logging-0.3.0.tar.gz` & `tmp/sag-py-logging-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-0.3.0.tar", last modified: Tue Apr 11 06:18:13 2023, max compression
+gzip compressed data, was "sag-py-logging-0.3.1.tar", last modified: Thu Apr 20 09:27:54 2023, max compression
```

## Comparing `sag-py-logging-0.3.0.tar` & `sag-py-logging-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.028520 sag-py-logging-0.3.0/sag_py_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/log_config_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/sag_py_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/sag_py_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 06:18:13.000000 sag-py-logging-0.3.0/sag_py_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:18:13.032520 sag-py-logging-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 06:18:03.000000 sag-py-logging-0.3.0/tests/test_log_config_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.340401 sag-py-logging-0.3.1/sag_py_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/log_config_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/sag_py_logging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.340401 sag-py-logging-0.3.1/sag_py_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-20 09:27:54.000000 sag-py-logging-0.3.1/sag_py_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:27:54.344401 sag-py-logging-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-20 09:27:33.000000 sag-py-logging-0.3.1/tests/test_log_config_processors.py
```

### Comparing `sag-py-logging-0.3.0/LICENSE.txt` & `sag-py-logging-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/PKG-INFO` & `sag-py-logging-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.0
+Version: 0.3.1
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -63,22 +63,22 @@
 
 placeholder_container = { "host": "myhost.com", ...}
 
 # For toml config with jinja templating
 init_logging(
     "./log_config.toml",
     loader=TomlLoader(),
-    processors=[JinjaProcessor(placeholder_container.__dict__)]
+    processors=[JinjaProcessor(placeholder_container)]
 )
 
 # For json config with format templating
 init_logging(
     "./log_config.json",
     loader=JsonLoader(),
-    processors=[FormatProcessor(placeholder_container.__dict__)]
+    processors=[FormatProcessor(placeholder_container)]
 )
 
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
 ### The configuration
@@ -135,21 +135,27 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(ConsoleExtraFieldFilter())
 ```
 
 If you init logging by config file the filter is added like that:
 ```json
 {
+    "formatters": {
+        "myformatter": {
+            "format": "s%(asctime)s - %(name)s - %(message)s - %(stringified_extra)s",
+        },
+    },
+    "filters": {
+        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
+    },
     "handlers": {
         "myhandler": {
+            "formatter": "myformatter",
             "filters": ["console_extra_field_filter"]
         }
-    },
-    "filters": {
-        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
     }
 }
 ```
 
 Afterwards you can use the field "stringified_extra" in your format string.
 
 If you for example log the following:
@@ -161,12 +167,33 @@
 
 ```
 Watch out! {"keyOne": "valueOne", "keyTwo": 2}
 ```
 
 Note: Internally json.dumps is used to convert the object/data to a string
 
-## How to publish
 
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
+
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-logging-0.3.0/README.md` & `sag-py-logging-0.3.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 
 placeholder_container = { "host": "myhost.com", ...}
 
 # For toml config with jinja templating
 init_logging(
     "./log_config.toml",
     loader=TomlLoader(),
-    processors=[JinjaProcessor(placeholder_container.__dict__)]
+    processors=[JinjaProcessor(placeholder_container)]
 )
 
 # For json config with format templating
 init_logging(
     "./log_config.json",
     loader=JsonLoader(),
-    processors=[FormatProcessor(placeholder_container.__dict__)]
+    processors=[FormatProcessor(placeholder_container)]
 )
 
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
 ### The configuration
@@ -110,21 +110,27 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(ConsoleExtraFieldFilter())
 ```
 
 If you init logging by config file the filter is added like that:
 ```json
 {
+    "formatters": {
+        "myformatter": {
+            "format": "s%(asctime)s - %(name)s - %(message)s - %(stringified_extra)s",
+        },
+    },
+    "filters": {
+        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
+    },
     "handlers": {
         "myhandler": {
+            "formatter": "myformatter",
             "filters": ["console_extra_field_filter"]
         }
-    },
-    "filters": {
-        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
     }
 }
 ```
 
 Afterwards you can use the field "stringified_extra" in your format string.
 
 If you for example log the following:
@@ -136,12 +142,33 @@
 
 ```
 Watch out! {"keyOne": "valueOne", "keyTwo": 2}
 ```
 
 Note: Internally json.dumps is used to convert the object/data to a string
 
-## How to publish
 
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
+
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-logging-0.3.0/sag_py_logging/console_extra_field_filter.py` & `sag-py-logging-0.3.1/sag_py_logging/console_extra_field_filter.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/sag_py_logging/log_config_initializer.py` & `sag-py-logging-0.3.1/sag_py_logging/log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/sag_py_logging/log_config_loader.py` & `sag-py-logging-0.3.1/sag_py_logging/log_config_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,17 +18,16 @@
         return self.json.loads(string_config)
 
 
 class TomlLoader(LogLoader):
     def __init__(self) -> None:
         try:
             import tomli
+
+            self.tomli = tomli
         except ImportError as e:
             raise ModuleNotFoundError(
                 "Module 'tomli' not installed.  Please run " "'python -m pip install sag-py-logging[toml]'"
             ) from e
-        import tomli
-
-        self.tomli = tomli
 
     def __call__(self, string_config: str) -> Dict[str, Any]:
         return self.tomli.loads(string_config)
```

### Comparing `sag-py-logging-0.3.0/sag_py_logging/log_config_processors.py` & `sag-py-logging-0.3.1/sag_py_logging/log_config_processors.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/sag_py_logging.egg-info/PKG-INFO` & `sag-py-logging-0.3.1/sag_py_logging.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.0
+Version: 0.3.1
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
@@ -63,22 +63,22 @@
 
 placeholder_container = { "host": "myhost.com", ...}
 
 # For toml config with jinja templating
 init_logging(
     "./log_config.toml",
     loader=TomlLoader(),
-    processors=[JinjaProcessor(placeholder_container.__dict__)]
+    processors=[JinjaProcessor(placeholder_container)]
 )
 
 # For json config with format templating
 init_logging(
     "./log_config.json",
     loader=JsonLoader(),
-    processors=[FormatProcessor(placeholder_container.__dict__)]
+    processors=[FormatProcessor(placeholder_container)]
 )
 
 ```
 
 Init logging returns the log configuration as dictionary if needed for further processing.
 
 ### The configuration
@@ -135,21 +135,27 @@
 console_handler = logging.StreamHandler(sys.stdout)
 console_handler.addFilter(ConsoleExtraFieldFilter())
 ```
 
 If you init logging by config file the filter is added like that:
 ```json
 {
+    "formatters": {
+        "myformatter": {
+            "format": "s%(asctime)s - %(name)s - %(message)s - %(stringified_extra)s",
+        },
+    },
+    "filters": {
+        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
+    },
     "handlers": {
         "myhandler": {
+            "formatter": "myformatter",
             "filters": ["console_extra_field_filter"]
         }
-    },
-    "filters": {
-        "console_extra_field_filter": {"()": "sag_py_logging.console_extra_field_filter.ConsoleExtraFieldFilter"}
     }
 }
 ```
 
 Afterwards you can use the field "stringified_extra" in your format string.
 
 If you for example log the following:
@@ -161,12 +167,33 @@
 
 ```
 Watch out! {"keyOne": "valueOne", "keyTwo": 2}
 ```
 
 Note: Internally json.dumps is used to convert the object/data to a string
 
-## How to publish
 
+## How to start developing
+
+### With vscode
+
+Just install vscode with dev containers extension. All required extensions and configurations are prepared automatically.
+
+### With pycharm
+
+* Install latest pycharm
+* Install pycharm plugin BlackConnect
+* Install pycharm plugin Mypy
+* Configure the python interpreter/venv
+* pip install requirements-dev.txt
+* pip install black[d]
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger when saving changed files
+* Ctl+Alt+S => Check Tools => BlackConnect => Trigger on code reformat
+* Ctl+Alt+S => Click Tools => BlackConnect => "Load from pyproject.yaml" (ensure line length is 120)
+* Ctl+Alt+S => Click Tools => BlackConnect => Configure path to the blackd.exe at the "local instance" config (e.g. C:\Python310\Scripts\blackd.exe)
+* Ctl+Alt+S => Click Tools => Actions on save => Reformat code
+* Restart pycharm
+
+## How to publish
 * Update the version in setup.py and commit your change
 * Create a tag with the same version number
 * Let github do the rest
```

### Comparing `sag-py-logging-0.3.0/sag_py_logging.egg-info/SOURCES.txt` & `sag-py-logging-0.3.1/sag_py_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/setup.py` & `sag-py-logging-0.3.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 with open("requirements.txt", "r") as fin:
     REQS = fin.read().splitlines()
 
+with open("requirements-dev.txt", "r") as fin:
+    REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
+
+JINJA_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require jinia" in item]
+TOMLI_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require tomli" in item]
+
 setuptools.setup(
     name="sag-py-logging",
-    version="0.3.0",
+    version="0.3.1",
     description="Initialize logging from a configuration json",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
@@ -25,14 +31,14 @@
         "Topic :: Software Development",
     ],
     keywords="logging, extra, fields",
     packages=setuptools.find_packages(exclude=["tests"]),
     package_data={"sag_py_logging": ["py.typed"]},
     python_requires=">=3.8",
     install_requires=REQS,
-    extras_require={"dev": ["pytest"], "jinja": ["Jinja2>=3.1.2"], "toml": ["tomli>=2.0.1"]},
+    extras_require={"dev": REQS_DEV, "jinja": JINJA_EXTRA, "toml": TOMLI_EXTRA},
     project_urls={
         "Documentation": "https://github.com/SamhammerAG/sag_py_logging",
         "Bug Reports": "https://github.com/SamhammerAG/sag_py_logging/issues",
         "Source": "https://github.com/SamhammerAG/sag_py_logging",
     },
 )
```

### Comparing `sag-py-logging-0.3.0/tests/test_console_extra_field_filter.py` & `sag-py-logging-0.3.1/tests/test_console_extra_field_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from logging import INFO, LogRecord
 from typing import cast
 
 import pytest
 
-from sag_py_logging import ConsoleExtraFieldFilter, ExtraFieldsLogRecord
+from sag_py_logging.console_extra_field_filter import ConsoleExtraFieldFilter
+from sag_py_logging.models import ExtraFieldsLogRecord
 
 
 @pytest.fixture()
 def log_record() -> LogRecord:
     return LogRecord(name="", level=INFO, pathname="", lineno=0, msg="Hello, world!", args=(), exc_info=None)
```

### Comparing `sag-py-logging-0.3.0/tests/test_log_config_initializer.py` & `sag-py-logging-0.3.1/tests/test_log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.0/tests/test_log_config_loader.py` & `sag-py-logging-0.3.1/tests/test_log_config_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,26 +39,26 @@
     json_loader = JsonLoader()
 
     # Act
     actual = json_loader(test_json)
 
     # Assert
     assert actual["version"] == 1
-    assert actual["disable_existing_loggers"] == True
+    assert actual["disable_existing_loggers"] is True
     assert actual["root"]["handlers"][0] == "myhandler"
     assert actual["root"]["level"] == "INFO"
     assert actual["handlers"]["myhandler"]["formatter"] == "handler_formatter"
 
 
 def test__toml_loader(test_toml: str) -> None:
     # Arrange
     toml_loader = TomlLoader()
 
     # Act
     actual = toml_loader(test_toml)
 
     # Assert
     assert actual["version"] == 1
-    assert actual["disable_existing_loggers"] == True
+    assert actual["disable_existing_loggers"] is True
     assert actual["root"]["handlers"][0] == "myhandler"
     assert actual["root"]["level"] == "INFO"
     assert actual["handlers"]["myhandler"]["formatter"] == "handler_formatter"
```

### Comparing `sag-py-logging-0.3.0/tests/test_log_config_processors.py` & `sag-py-logging-0.3.1/tests/test_log_config_processors.py`

 * *Files identical despite different names*

