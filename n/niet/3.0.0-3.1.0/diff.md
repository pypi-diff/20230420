# Comparing `tmp/niet-3.0.0.tar.gz` & `tmp/niet-3.1.0.tar.gz`

## Comparing `niet-3.0.0.tar` & `niet-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 niet-3.0.0/.travis.yml
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 niet-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 niet-3.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 niet-3.0.0/ChangeLog.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 niet-3.0.0/Pipfile
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 niet-3.0.0/setup.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 niet-3.0.0/test-requirements.txt
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 niet-3.0.0/tox.ini
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 niet-3.0.0/niet/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 niet-3.0.0/niet/__main__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 niet-3.0.0/niet/output.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 niet-3.0.0/niet/url.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 niet-3.0.0/tests/test_output.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 niet-3.0.0/tests/test_url.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample.json
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 niet-3.0.0/tests/samples/sample_not_indented.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 niet-3.0.0/.gitignore
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 niet-3.0.0/AUTHORS
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 niet-3.0.0/LICENSE
--rw-r--r--   0        0        0    23268 2020-02-02 00:00:00.000000 niet-3.0.0/README.md
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 niet-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    24207 2020-02-02 00:00:00.000000 niet-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 niet-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 niet-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 niet-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 niet-3.1.0/ChangeLog.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 niet-3.1.0/Pipfile
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 niet-3.1.0/setup.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 niet-3.1.0/test-requirements.txt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 niet-3.1.0/tox.ini
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 niet-3.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 niet-3.1.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 niet-3.1.0/niet/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 niet-3.1.0/niet/__main__.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 niet-3.1.0/niet/output.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 niet-3.1.0/niet/url.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 niet-3.1.0/tests/test_output.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 niet-3.1.0/tests/test_url.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.toml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample_not_indented.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 niet-3.1.0/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 niet-3.1.0/AUTHORS
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 niet-3.1.0/LICENSE
+-rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 niet-3.1.0/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 niet-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0    25519 2020-02-02 00:00:00.000000 niet-3.1.0/PKG-INFO
```

### Comparing `niet-3.0.0/CODE_OF_CONDUCT.md` & `niet-3.1.0/CODE_OF_CONDUCT.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 that are not aligned to this Code of Conduct, or to ban temporarily or permanently
 any contributor for other behaviors that they deem inappropriate,
 threatening, offensive, or harmful.
 
 ## Scope
 
 This Code of Conduct applies both within project spaces and in public spaces when an individual
-is representing the project or its community. 
-Examples of representing a project or community include using an official project e-mail address, 
+is representing the project or its community.
+Examples of representing a project or community include using an official project e-mail address,
 posting via an official social media account, or acting as an appointed
 representative at an online or offline event.
 Representation of a project may be further defined and
 clarified by project maintainers.
 
 ## Enforcement
 
@@ -65,8 +65,7 @@
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4, available at [http://contributor-covenant.org/version/1/4][version]
 
 [homepage]: http://contributor-covenant.org
 [version]: http://contributor-covenant.org/version/1/4/
-
```

### Comparing `niet-3.0.0/CONTRIBUTING.md` & `niet-3.1.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,30 @@
 ```shell
 $ git clone https://github.com/openuado/niet
 ```
 
 #### Setup your environment
 
 From there, you can navigate into the directory where you've cloned
-the niet source code
+the niet source code:
 
 ```shell
 $ cd niet
 ```
 
+You can install the development tools by using:
+```
+python3.11 -m pip install --editable ".[dev]"
+```
+
+And enabling `pre-commit` for niet:
+```
+$ pre-commit install
+```
+
 `tox` allow you to use niet directly in a dedicated virtual environment
 already configured (requirements, etc):
 
 ```shell
 $ tox -e venv -- niet -h
 ...
 venv run-test: commands[0] | niet -h
@@ -185,12 +195,12 @@
 You can create your pull request manually directly from github:
 * Include examples, outputs, etc... whenever possible.
 * Include screenshots and animated GIFs in your pull request whenever possible.
 
 ### Deploy niet on PyPi
 
 ```
-python -m pip install build twine
+pip install --editable ".[dev]"
 python -m build
 twine check dist/*
 twine upload dist/*
 ```
```

### Comparing `niet-3.0.0/ChangeLog.md` & `niet-3.1.0/ChangeLog.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 CHANGES
 =======
 
+3.1.0
+-----
+
+* [feature] the toml format is now supported by niet (https://github.com/openuado/niet/pull/77)
+* [fix] replace deprecated pkg_resources by importlib.metadata
+* [CI/CD] move away from travis CI and fix existing github actions
+* [CI/CD] publish to pypi with github actions
+* [CI/CD] introduce black and isort and a couple of new dev tools
+
+3.0.0
+-----
+
+* [packaging] rewrite the way we package niet and move away from pbr
+* [doc] update the contribution guide
+
+2.5.0
+-----
+
+* [fix] return key equal to False and 0 rather than raising an element not found (https://github.com/openuado/niet/issues/72)
+* [requirements] bump PyYAML from version 5.1 to version 5.4.1
+* [doc] improve documentation and error messages
+
+2.4.0
+-----
+
+* fix changelog and integration badges
+
 2.3.0
 -----
 
 * Adding a debug mode to niet
 * [doc] add more examples for the `comma` format
 
 2.2.0
```

### Comparing `niet-3.0.0/niet/__init__.py` & `niet-3.1.0/niet/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #!/usr/bin/python
 import argparse
 import json
 import sys
 import textwrap
+from importlib.metadata import version as getversion
 
+import pkg_resources
+import pytoml as toml
+import yaml
 from jmespath import search
 from jmespath.exceptions import LexerError
 
 import niet.output as output
 import niet.url
 
-import pkg_resources
-
-import yaml
-
-
 VALID_PRINTERS = {
     "json": {
         "cmd": output.print_json,
         "epilog": "Return object in JSON",
     },
     "yaml": {
         "cmd": output.print_yaml,
         "epilog": "Return object in YAML",
     },
+    "toml": {
+        "cmd": output.print_toml,
+        "epilog": "Return object in TOML",
+    },
     "eval": {
         "cmd": output.print_eval,
         "epilog": "Return result in a string evaluable by a shell "
         "eval command as an input",
     },
     "newline": {
         "cmd": output.print_newline,
@@ -55,88 +58,123 @@
 def get_epilog():
     epilog = ""
     indent_max = max(VALID_PRINTERS.keys(), key=len)
     for item in VALID_PRINTERS:
         epilog += "  {item}{indent}\t{epilog}\n".format(
             item=item,
             indent=" " * (len(indent_max) - len(item)),
-            epilog=VALID_PRINTERS[item]["epilog"])
+            epilog=VALID_PRINTERS[item]["epilog"],
+        )
     return epilog
 
 
 class ContentType(argparse.FileType):
-
     def __call__(self, string):
         if niet.url.is_webresource(string):
             return string
         return super().__call__(string)
 
 
 # arguments parsing
 def argparser():
-    epilog = '''output formats:\n{}'''.format(get_epilog())
+    epilog = """output formats:\n{}""".format(get_epilog())
 
     parser = argparse.ArgumentParser(
-        description='Read data from YAML or JSON file',
+        description="Read data from YAML or JSON file",
         formatter_class=argparse.RawDescriptionHelpFormatter,
-        epilog=epilog)
-    parser.add_argument('object', type=str,
-                        help="Path to object separated by dot (.). \
+        epilog=epilog,
+    )
+    parser.add_argument(
+        "object",
+        type=str,
+        help="Path to object separated by dot (.). \
                         Use '.' to get whole file. \
-                        eg: a.b.c")
-    parser.add_argument('file', nargs='?', type=ContentType(),
-                        help="Optional JSON or YAML local filename or \
+                        eg: a.b.c",
+    )
+    parser.add_argument(
+        "file",
+        nargs="?",
+        type=ContentType(),
+        help="Optional JSON or YAML local filename or \
                         distant web resource at raw format. \
-                        If not provided niet read from stdin")
-    parser.add_argument('-f', '--format', type=str,
-                        choices=[key for key in VALID_PRINTERS],
-                        help="output format")
-    parser.add_argument('-i', '--in-place', action='store_true',
-                        help="Perform modification in place. Will so alter \
-                        read file")
-    parser.add_argument('-o', '--output', type=str, metavar="OUTPUT_FILE",
-                        help="Print output in a file instead of stdout \
-                        (surcharged by in-place parameter if set)")
-    parser.add_argument('-s', '--silent', action='store_true',
-                        help="silent mode, doesn't display message when \
-                        element was not found")
-    parser.add_argument('-v', '--version', action='store_true',
-                        help="print the Niet version number and \
-                        exit (also --version)")
-    parser.add_argument('--debug', action='store_true',
-                        help="Activate the debug mode (based on pdb)")
+                        If not provided niet read from stdin",
+    )
+    parser.add_argument(
+        "-f",
+        "--format",
+        type=str,
+        choices=[key for key in VALID_PRINTERS],
+        help="output format",
+    )
+    parser.add_argument(
+        "-i",
+        "--in-place",
+        action="store_true",
+        help="Perform modification in place. Will so alter \
+                        read file",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        metavar="OUTPUT_FILE",
+        help="Print output in a file instead of stdout \
+                        (surcharged by in-place parameter if set)",
+    )
+    parser.add_argument(
+        "-s",
+        "--silent",
+        action="store_true",
+        help="silent mode, doesn't display message when \
+                        element was not found",
+    )
+    parser.add_argument(
+        "-v",
+        "--version",
+        action="store_true",
+        help="print the Niet version number and \
+                        exit (also --version)",
+    )
+    parser.add_argument(
+        "--debug", action="store_true", help="Activate the debug mode (based on pdb)"
+    )
     return parser.parse_args()
 
 
 # Parsing to extract wanted object
 def data_parser(dataset):
     result = None
     try:
         result = json.loads(dataset)
         in_format = "json"
     except ValueError:
         try:
             result = yaml.safe_load(dataset)
             in_format = "yaml"
-        except yaml.constructor.ConstructorError as err:
-            print(str(err))
-        except yaml.parser.ParserError as err:
-            print(str(err))
+        except (yaml.constructor.ConstructorError, yaml.parser.ParserError) as err:
+            try:
+                result = toml.loads(dataset)
+                in_format = "toml"
+            except toml.core.TomlError as err:
+                print(str(err))
     if not isinstance(result, (list, dict)):
-        print(textwrap.dedent("""
+        print(
+            textwrap.dedent(
+                """
                 Oops... An error occur.
                 You face this error because the passed file has been
                 detected as invalid. It have been detected invalid because
                 either the format of this file isn't correct or
                 unsupported.
 
-                Niet only support valid json and yaml input.
+                Niet only support valid json, yaml, and toml input.
                 You can check that your file is valid by using a JSON or
                 YAML linter. https://jsonlint.com/"""
-        ))
+            )
+        )
         sys.exit(1)
     return result, in_format
 
 
 # Load file
 def get(data, keywords, silent=False):
     if keywords == ".":
@@ -156,28 +194,27 @@
         if not silent:
             print("Element not found: {research}".format(research=keywords))
         sys.exit(1)
 
 
 def print_result(res, out_format, in_format, search, out_file):
     if out_format is None:
-        if (isinstance(res, (list, str, int, float)) or in_format is None):
+        if isinstance(res, (list, str, int, float)) or in_format is None:
             out_format = "newline"
         else:
             out_format = in_format
     try:
         if out_format == "eval":
             output = VALID_PRINTERS[out_format]["cmd"](res, search)
         else:
             # we need to pass the search to init the eval var name
             output = VALID_PRINTERS[out_format]["cmd"](res)
     except KeyError:
         print(f"Error : Invalid choice ({out_format}). ")
-        print("Supported formats are: {format}".format(",".join(
-            VALID_PRINTERS)))
+        print("Supported formats are: {format}".format(",".join(VALID_PRINTERS)))
     else:
         if out_file:
             with open(out_file, "w+") as f:
                 f.write(output)
         else:
             print(output)
 
@@ -187,26 +224,26 @@
     if isinstance(infile, str):
         return infile
     with infile:
         return infile.read()
 
 
 def version():
-    installed = pkg_resources.get_distribution('niet').version
-    print("niet version {}".format(installed))
+    print("niet version: {}".format(getversion("niet")))
 
 
 # Main
 def main():
-    if '-v' in sys.argv or '--version' in sys.argv:
+    if "-v" in sys.argv or "--version" in sys.argv:
         version()
         sys.exit(0)
     args = argparser()
     if args.debug:
         import pdb
+
         pdb.set_trace()
     infile = args.file or sys.stdin
     if isinstance(infile, str):
         # NOTE(hberaud): We consider we using a web resource if
         # infile is a string
         infile = niet.url.fetch(infile)
     else:
```

### Comparing `niet-3.0.0/niet/output.py` & `niet-3.1.0/niet/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 import os
 
+import pytoml as toml
 import yaml
 
-IFS = os.getenv('IFS', ' ')
+IFS = os.getenv("IFS", " ")
 
 
 # Output functions
 def print_squote(res):
     if isinstance(res, list):
         res = IFS.join(["'{}'".format(el) for el in res])
-    elif (isinstance(res, str) or isinstance(res, int)):
+    elif isinstance(res, str) or isinstance(res, int):
         res = "".join("'{}'".format(res))
     return res
 
 
 def print_dquote(res):
     if isinstance(res, list):
-        res = IFS.join(["\"{}\"".format(el) for el in res])
-    elif (isinstance(res, str) or isinstance(res, int)):
-        res = "".join("\"{}\"".format(res))
+        res = IFS.join(['"{}"'.format(el) for el in res])
+    elif isinstance(res, str) or isinstance(res, int):
+        res = "".join('"{}"'.format(res))
     return res
 
 
 def print_ifs(res):
     if isinstance(res, list):
         res = IFS.join(["{}".format(el) for el in res])
     return res
@@ -39,19 +40,19 @@
                 result.append(yaml.dump(el))
             return "".join(result)
     else:
         return res
 
 
 def print_newline(res):
-    return _formate_result_with_delimiter(res, delimiter='\n')
+    return _formate_result_with_delimiter(res, delimiter="\n")
 
 
 def print_comma(res):
-    return _formate_result_with_delimiter(res, delimiter=',')
+    return _formate_result_with_delimiter(res, delimiter=",")
 
 
 def _findevalitem(obj, base=""):
     if base.startswith("_"):
         base = base[1:]
     el = []
     for k, v in obj.items():
@@ -86,7 +87,15 @@
 
 def print_yaml(res):
     return yaml.dump(res, default_flow_style=False)
 
 
 def print_json(res):
     return json.dumps(res, indent=4)
+
+
+def print_toml(res):
+    try:
+        return toml.dumps(res)
+    # (hberaud) Catch cases when only the value of a key is captured
+    except AttributeError:
+        return res
```

### Comparing `niet-3.0.0/tests/test_output.py` & `niet-3.1.0/tests/test_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import unittest
 
 import niet.output
 
 
 class TestPrintFunctions(unittest.TestCase):
     def test_squotes(self):
-        output = niet.output.print_squote(['test1', 'test2'])
+        output = niet.output.print_squote(["test1", "test2"])
         self.assertEqual("'test1' 'test2'", output)
 
     def test_dquotes(self):
-        output = niet.output.print_dquote(['test1', 'test2'])
+        output = niet.output.print_dquote(["test1", "test2"])
         self.assertEqual('"test1" "test2"', output)
 
     def test_newline(self):
-        output = niet.output.print_newline(['test1', 'test2'])
-        self.assertEqual('test1\ntest2', output)
+        output = niet.output.print_newline(["test1", "test2"])
+        self.assertEqual("test1\ntest2", output)
         output = niet.output.print_newline([1, 2])
-        self.assertEqual('1\n2', output)
+        self.assertEqual("1\n2", output)
 
     def test_comma(self):
-        output = niet.output.print_comma(['test1', 'test2'])
-        self.assertEqual('test1,test2', output)
+        output = niet.output.print_comma(["test1", "test2"])
+        self.assertEqual("test1,test2", output)
         output = niet.output.print_comma([1, 2])
-        self.assertEqual('1,2', output)
+        self.assertEqual("1,2", output)
```

### Comparing `niet-3.0.0/tests/test_url.py` & `niet-3.1.0/tests/test_url.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # -*- encoding: utf-8 -*-
 import unittest
 
 import niet.url
 
-
 VALID_WEBRESOURCES = [
-    'https://google.com',
-    'http://google.com',
-    'https://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml',  # noqa
-    'http://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml',  # noqa
-    'https://herve.beraud.io',
-    'http://herve.beraud.io',
-    'https://opensource.org/',
-    'http://opensource.org/'
+    "https://google.com",
+    "http://google.com",
+    "https://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml",  # noqa
+    "http://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml",  # noqa
+    "https://herve.beraud.io",
+    "http://herve.beraud.io",
+    "https://opensource.org/",
+    "http://opensource.org/",
 ]
 NONVALID_RESOURCES = [
-    'google.com',
-    'google.com',
-    'raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml',  # noqa
-    'raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml',  # noqa
-    'herve.beraud.io',
-    'herve.beraud.io',
-    'opensource.org/',
-    'opensource.org/'
+    "google.com",
+    "google.com",
+    "raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml",  # noqa
+    "raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml",  # noqa
+    "herve.beraud.io",
+    "herve.beraud.io",
+    "opensource.org/",
+    "opensource.org/",
 ]
 
 
 class TestUrl(unittest.TestCase):
     def test_is_webresource(self):
         for test in VALID_WEBRESOURCES:
             self.assertEqual(True, niet.url.is_webresource(test))
```

### Comparing `niet-3.0.0/LICENSE` & `niet-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niet-3.0.0/README.md` & `niet-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,107 +1,113 @@
 # niet
 
-[![Build Status](https://travis-ci.org/openuado/niet.svg?branch=master)](https://travis-ci.org/openuado/niet)
+![Build](https://github.com/openuado/niet/actions/workflows/python-app.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/niet.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/niet.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/niet.svg)
 [![Downloads](https://pepy.tech/badge/niet)](https://pepy.tech/project/niet)
 [![Downloads](https://pepy.tech/badge/niet/month)](https://pepy.tech/project/niet/month)
 
-Get data from YAML file directly in your shell.
+Get data from YAML, JSON, and TOML file directly in your shell.
 
 ---
 
 > How to easily parse and retrieve data from YAML file in our shell?
 
 The previous question, few years ago, led us to the development of niet.
 
 Indeed, at that time, we needed a way to store and retrieve data for our own
 needs. We created niet to read those data. The goal was to develop a tools
 that will allow us to standardize how we parse YAML locally or in our CI
 pipelines. We wanted something reusable and easily distribuable. Niet was born.
 
+Over the years niet evolved to introduce the support of other formats like
+TOML.
+
 Niet is like [xmllint](http://xmlsoft.org/xmllint.html) or
-[jq](https://stedolan.github.io/jq/) but for YAML and JSON data -
+[jq](https://stedolan.github.io/jq/) but for YAML, JSON and TOML data -
 you can use it to slice and filter and map and transform structured data.
 
 You can easily retrieve data by using simple expressions or using
 xpath advanced features to access non-trivial data.
 
-You can easily convert YAML format into JSON format and vice versa.
+You can easily convert YAML format into JSON, or TOML formats and vice versa.
 
 Niet is writen in Python so you can install it from a package manager (from
 PyPi) or directly by cloning this repository - no specific system rights are
 needed to install it.
 
-## Features
+## Main Features
 - Extract elements by using xpath syntax
-- Extract values from json format
-- Extract values from yaml format
+- Extract values from JSON format
+- Extract values from YAML format
+- Extract values from TOML format
 - Automaticaly detect format (json/yaml)
 - Read data from a web resource
 - Read data from file or pass data from stdin
 - Format output values
 - Format output to be reused by shell `eval`
-- Convert YAML to JSON
-- Convert JSON to YAML
+- Convert YAML to JSON, or TOML
+- Convert JSON to YAML, or TOML
+- Convert TOML to YAML, or JSON
 
 ## Install or Update niet
 
 ```sh
 $ pip install -U niet
 ```
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.9 or higher
 
 ## Supported versions
 
 Since niet 2.0 the support of python 2.7 have been dropped so if
 if you only have python 2.7 at hands then you can use previous version (lower
-to 2.0) but you should consider first that the no support will be given on
+to 2.0) but you should consider first that no support will be given on
 these versions (no bugfix, no new feature, etc). If you report an issue or
 or propose a new feature then they will be addressed only for current or
 higher version.
 
 ## Usage
 
 ### Help and options
 
 ```shell
 $ niet --help
-usage: niet [-h] [-f {json,yaml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
+usage: niet [-h] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
             object [file]
 
 Read data from YAML or JSON file
 
 positional arguments:
   object                Path to object separated by dot (.). Use '.' to get
                         whole file. eg: a.b.c
   file                  Optional JSON or YAML filename. If not provided niet
                         read from stdin
 
 optional arguments:
   -h, --help            show this help message and exit
-  -f {json,yaml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,eval,newline,ifs,squote,dquote,comma}
+  -f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}
                         output format
   -i, --in-place        Perform modification in place. Will so alter read file
   -o OUTPUT_FILE, --output OUTPUT_FILE
                         Print output in a file instead of stdout (surcharged
                         by infile parameter if set)
   -s, --silent          silent mode, doesn't display message when element was
                         not found
   -v, --version         print the Niet version number and exit (also
                         --version)
   --debug               Activate the debug mode (based on pdb)
 
 output formats:
   json          Return object in JSON
   yaml          Return object in YAML
+  toml          Return object in TOML
   eval          Return result in a string evaluable by a shell eval command as an input
   newline       Return all elements of a list in a new line
   ifs           Return all elements of a list separated by IFS env var
   squote        Add single quotes to result
   dquote        Add double quotes to result
   comma         Return all elements separated by commas
 ```
@@ -286,41 +292,42 @@
 ```
 
 Further examples with [`jmespath` identifiers](http://jmespath.org/specification.html#examples).
 
 ### Output
 
 #### Stdout
-By default, niet print the output on stdout. 
+By default, niet print the output on stdout.
 
 #### Save output to a file
 It if possible to pass a filename using -o or --output argument to writes
 directly in a file. This file will be created if not exists or will be
 replaced if already exists.
 
 #### In-file modification
 It is possible to modify directly a file using -i or --in-place argument. This will replace
 the input file by the output of niet command. This can be used to extract some data of a file or
 reindent a file.
 
-### Output formats 
-You can change the output format using the -f or --format optional 
-argument. 
+### Output formats
+You can change the output format using the -f or --format optional
+argument.
 
 By default, niet detect the input format and display complex objects
 in the same format. If the object is a list or a value, newline output
 format will be used.
 
-Output formats are: 
+Output formats are:
   - ifs
   - squote
   - dquote
   - newline
   - yaml
   - json
+  - toml
 
 #### ifs
 Ifs output format print all values of a list or a single value in one line.
 All values are separated by the content of IFS environment variable if defined,
 space otherwise.
 
 Examples (consider the previous [YAML file example](#with-yaml-file)):
@@ -471,28 +478,31 @@
 $ eval $(echo '{"foo-biz": "bar", "fizz": {"buzz": ["zero", "one", "two", "three"]}}' | niet -f eval fizz.buzz)
 $ for el in ${fizz_buzz}; do echo $el; done
 zero
 one
 two
 three
 ```
- 
+
 #### yaml
-Yaml output format force output to be in YAML regardless the input file format.
+YAML output format force output to be in YAML regardless the input file format.
 
 #### json
-Json output format force output to be in JSON regardless the input file format.
+JSON output format force output to be in JSON regardless the input file format.
+
+#### toml
+TOML output format force output to be in TOML regardless the input file format.
 
 ### Read data from a web resource
 
-Niet allow you to read data (json/yaml) from a web resource accessible by using
-the HTTP protocole (introduced in niet 2.1).
+Niet allow you to read data (json/yaml/toml) from a web resource accessible by
+using the HTTP protocole (introduced in niet 2.1).
 
-This can be done by passing an url to niet which refer to a raw content (json
-or yaml).
+This can be done by passing an url to niet which refer to a raw content (json,
+yaml, or toml).
 
 Here is some examples with the [openstack governance's projects data](https://github.com/openstack/governance/blob/master/reference/projects.yaml):
 
 ```sh
 $ # List all the oslo projects repos (https://wiki.openstack.org/wiki/Oslo)
 $ niet "oslo.deliverables.*.repos[0]" \
     https://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml
@@ -599,15 +609,15 @@
     foo: bar
     list:
         - item1
         - item2
         - item3
 ```
 
-### Extract a single value 
+### Extract a single value
 
 Retrieve the project name:
 ```sh
 $ niet project.meta.name tests/samples/sample.yaml
 my-project
 ```
 
@@ -700,32 +710,32 @@
 
 Then parse it after in bash in this example:
 ```shell
 $ niet .meta.name <<< $project
 my-project
 ```
 
-### Transform JSON to YAML
+### Transform JSON into YAML
 
-With niet you can easily convert your JSON to YAML
+With niet you can easily convert your JSON into YAML
 ```shell
 $ niet . tests/samples/sample.json -f yaml
 project:
   foo: bar
   list:
   - item1
   - item2
   - item3
   meta:
     name: my-project
 ```
 
-### Transform YAML to JSON
+### Transform YAML into JSON
 
-With niet you can easily convert your YAML to JSON
+With niet you can easily convert your YAML into JSON
 ```shell
 $ niet . tests/samples/sample.yaml -f json
 {
     "project": {
         "meta": {
             "name": "my-project"
         },
@@ -735,19 +745,63 @@
             "item2",
             "item3"
         ]
     }
 }
 ```
 
+### Transform JSON into TOML
+
+With niet you can easily convert your JSON into TOML
+```shell
+$ niet . tests/samples/sample.json -f toml
+[project]
+foo = "bar"
+list = ["item1", "item2", "item3"]
+test-dash = "value"
+
+[project.meta]
+name = "my-project"
+```
+
+### Transform YAML into TOML
+
+With niet you can easily convert your YAML into TOML
+```shell
+$ niet . tests/samples/sample.yaml -f toml
+[project]
+foo = "bar"
+list = ["item1", "item2", "item3"]
+test-dash = "value"
+
+[project.meta]
+name = "my-project"
+```
+
+### Transform TOML into YAML
+
+With niet you can easily convert your TOML into YAML
+```shell
+niet . tests/samples/sample.toml -f yaml
+project:
+  foo: bar
+  list:
+  - item1
+  - item2
+  - item3
+  meta:
+    name: my-project
+  test-dash: value
+```
+
 ### Indent JSON file
 
 This is an example of how to indent a JSON file :
 ```shell
-$ niet . tests/samples/sample_not_indented.json 
+$ niet . tests/samples/sample_not_indented.json
 {
     "project": {
         "meta": {
             "name": "my-project"
         },
         "foo": "bar",
         "list": [
```

### Comparing `niet-3.0.0/pyproject.toml` & `niet-3.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "niet"
 authors = [
     {name = "Hervé Beraud", email = "herveberaud.pro@gmail.com"},
 ]
-description = "A command-line tool to work with YAML and JSON files."
+description = "A command-line tool to work with YAML, JSON, and TOML files."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 url.Homepage = "https://github.com/openuado/niet"
 url.Source = "https://github.com/openuado/niet"
 url.Tracker = "https://github.com/openuado/niet/issues"
 classifiers = [
@@ -30,18 +30,19 @@
     "Topic :: Software Development",
     "Topic :: Utilities"
 ]
 dynamic = ["version"]
 dependencies = [
     "pyyaml>=5.1",
     "jmespath>=0.9.4",
+    "pytoml", # (hberaud) Remove it when support of python < 3.11 are removed
 ]
 
 [project.optional-dependencies]
-build = ["build", "twine"]
+dev = ["black", "isort", "pip-tools", "build", "twine", "pre-commit", "commitizen"]
 
 [project.scripts]
 niet = "niet.__main__:main"
 
 [options.packages.find]
 where = "niet"
 exclude = "tests*"
```

### Comparing `niet-3.0.0/PKG-INFO` & `niet-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: niet
-Version: 3.0.0
-Summary: A command-line tool to work with YAML and JSON files.
+Version: 3.1.0
+Summary: A command-line tool to work with YAML, JSON, and TOML files.
 Author-email: Hervé Beraud <herveberaud.pro@gmail.com>
 License: MIT
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,120 +15,132 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Requires-Dist: jmespath>=0.9.4
+Requires-Dist: pytoml
 Requires-Dist: pyyaml>=5.1
-Provides-Extra: build
-Requires-Dist: build; extra == 'build'
-Requires-Dist: twine; extra == 'build'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: commitizen; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: pip-tools; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # niet
 
-[![Build Status](https://travis-ci.org/openuado/niet.svg?branch=master)](https://travis-ci.org/openuado/niet)
+![Build](https://github.com/openuado/niet/actions/workflows/python-app.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/niet.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/niet.svg)
 ![PyPI - Status](https://img.shields.io/pypi/status/niet.svg)
 [![Downloads](https://pepy.tech/badge/niet)](https://pepy.tech/project/niet)
 [![Downloads](https://pepy.tech/badge/niet/month)](https://pepy.tech/project/niet/month)
 
-Get data from YAML file directly in your shell.
+Get data from YAML, JSON, and TOML file directly in your shell.
 
 ---
 
 > How to easily parse and retrieve data from YAML file in our shell?
 
 The previous question, few years ago, led us to the development of niet.
 
 Indeed, at that time, we needed a way to store and retrieve data for our own
 needs. We created niet to read those data. The goal was to develop a tools
 that will allow us to standardize how we parse YAML locally or in our CI
 pipelines. We wanted something reusable and easily distribuable. Niet was born.
 
+Over the years niet evolved to introduce the support of other formats like
+TOML.
+
 Niet is like [xmllint](http://xmlsoft.org/xmllint.html) or
-[jq](https://stedolan.github.io/jq/) but for YAML and JSON data -
+[jq](https://stedolan.github.io/jq/) but for YAML, JSON and TOML data -
 you can use it to slice and filter and map and transform structured data.
 
 You can easily retrieve data by using simple expressions or using
 xpath advanced features to access non-trivial data.
 
-You can easily convert YAML format into JSON format and vice versa.
+You can easily convert YAML format into JSON, or TOML formats and vice versa.
 
 Niet is writen in Python so you can install it from a package manager (from
 PyPi) or directly by cloning this repository - no specific system rights are
 needed to install it.
 
-## Features
+## Main Features
 - Extract elements by using xpath syntax
-- Extract values from json format
-- Extract values from yaml format
+- Extract values from JSON format
+- Extract values from YAML format
+- Extract values from TOML format
 - Automaticaly detect format (json/yaml)
 - Read data from a web resource
 - Read data from file or pass data from stdin
 - Format output values
 - Format output to be reused by shell `eval`
-- Convert YAML to JSON
-- Convert JSON to YAML
+- Convert YAML to JSON, or TOML
+- Convert JSON to YAML, or TOML
+- Convert TOML to YAML, or JSON
 
 ## Install or Update niet
 
 ```sh
 $ pip install -U niet
 ```
 
 ## Requirements
 
-- Python 3.6 or higher
+- Python 3.9 or higher
 
 ## Supported versions
 
 Since niet 2.0 the support of python 2.7 have been dropped so if
 if you only have python 2.7 at hands then you can use previous version (lower
-to 2.0) but you should consider first that the no support will be given on
+to 2.0) but you should consider first that no support will be given on
 these versions (no bugfix, no new feature, etc). If you report an issue or
 or propose a new feature then they will be addressed only for current or
 higher version.
 
 ## Usage
 
 ### Help and options
 
 ```shell
 $ niet --help
-usage: niet [-h] [-f {json,yaml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
+usage: niet [-h] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
             object [file]
 
 Read data from YAML or JSON file
 
 positional arguments:
   object                Path to object separated by dot (.). Use '.' to get
                         whole file. eg: a.b.c
   file                  Optional JSON or YAML filename. If not provided niet
                         read from stdin
 
 optional arguments:
   -h, --help            show this help message and exit
-  -f {json,yaml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,eval,newline,ifs,squote,dquote,comma}
+  -f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}
                         output format
   -i, --in-place        Perform modification in place. Will so alter read file
   -o OUTPUT_FILE, --output OUTPUT_FILE
                         Print output in a file instead of stdout (surcharged
                         by infile parameter if set)
   -s, --silent          silent mode, doesn't display message when element was
                         not found
   -v, --version         print the Niet version number and exit (also
                         --version)
   --debug               Activate the debug mode (based on pdb)
 
 output formats:
   json          Return object in JSON
   yaml          Return object in YAML
+  toml          Return object in TOML
   eval          Return result in a string evaluable by a shell eval command as an input
   newline       Return all elements of a list in a new line
   ifs           Return all elements of a list separated by IFS env var
   squote        Add single quotes to result
   dquote        Add double quotes to result
   comma         Return all elements separated by commas
 ```
@@ -313,41 +325,42 @@
 ```
 
 Further examples with [`jmespath` identifiers](http://jmespath.org/specification.html#examples).
 
 ### Output
 
 #### Stdout
-By default, niet print the output on stdout. 
+By default, niet print the output on stdout.
 
 #### Save output to a file
 It if possible to pass a filename using -o or --output argument to writes
 directly in a file. This file will be created if not exists or will be
 replaced if already exists.
 
 #### In-file modification
 It is possible to modify directly a file using -i or --in-place argument. This will replace
 the input file by the output of niet command. This can be used to extract some data of a file or
 reindent a file.
 
-### Output formats 
-You can change the output format using the -f or --format optional 
-argument. 
+### Output formats
+You can change the output format using the -f or --format optional
+argument.
 
 By default, niet detect the input format and display complex objects
 in the same format. If the object is a list or a value, newline output
 format will be used.
 
-Output formats are: 
+Output formats are:
   - ifs
   - squote
   - dquote
   - newline
   - yaml
   - json
+  - toml
 
 #### ifs
 Ifs output format print all values of a list or a single value in one line.
 All values are separated by the content of IFS environment variable if defined,
 space otherwise.
 
 Examples (consider the previous [YAML file example](#with-yaml-file)):
@@ -498,28 +511,31 @@
 $ eval $(echo '{"foo-biz": "bar", "fizz": {"buzz": ["zero", "one", "two", "three"]}}' | niet -f eval fizz.buzz)
 $ for el in ${fizz_buzz}; do echo $el; done
 zero
 one
 two
 three
 ```
- 
+
 #### yaml
-Yaml output format force output to be in YAML regardless the input file format.
+YAML output format force output to be in YAML regardless the input file format.
 
 #### json
-Json output format force output to be in JSON regardless the input file format.
+JSON output format force output to be in JSON regardless the input file format.
+
+#### toml
+TOML output format force output to be in TOML regardless the input file format.
 
 ### Read data from a web resource
 
-Niet allow you to read data (json/yaml) from a web resource accessible by using
-the HTTP protocole (introduced in niet 2.1).
+Niet allow you to read data (json/yaml/toml) from a web resource accessible by
+using the HTTP protocole (introduced in niet 2.1).
 
-This can be done by passing an url to niet which refer to a raw content (json
-or yaml).
+This can be done by passing an url to niet which refer to a raw content (json,
+yaml, or toml).
 
 Here is some examples with the [openstack governance's projects data](https://github.com/openstack/governance/blob/master/reference/projects.yaml):
 
 ```sh
 $ # List all the oslo projects repos (https://wiki.openstack.org/wiki/Oslo)
 $ niet "oslo.deliverables.*.repos[0]" \
     https://raw.githubusercontent.com/openstack/governance/master/reference/projects.yaml
@@ -626,15 +642,15 @@
     foo: bar
     list:
         - item1
         - item2
         - item3
 ```
 
-### Extract a single value 
+### Extract a single value
 
 Retrieve the project name:
 ```sh
 $ niet project.meta.name tests/samples/sample.yaml
 my-project
 ```
 
@@ -727,32 +743,32 @@
 
 Then parse it after in bash in this example:
 ```shell
 $ niet .meta.name <<< $project
 my-project
 ```
 
-### Transform JSON to YAML
+### Transform JSON into YAML
 
-With niet you can easily convert your JSON to YAML
+With niet you can easily convert your JSON into YAML
 ```shell
 $ niet . tests/samples/sample.json -f yaml
 project:
   foo: bar
   list:
   - item1
   - item2
   - item3
   meta:
     name: my-project
 ```
 
-### Transform YAML to JSON
+### Transform YAML into JSON
 
-With niet you can easily convert your YAML to JSON
+With niet you can easily convert your YAML into JSON
 ```shell
 $ niet . tests/samples/sample.yaml -f json
 {
     "project": {
         "meta": {
             "name": "my-project"
         },
@@ -762,19 +778,63 @@
             "item2",
             "item3"
         ]
     }
 }
 ```
 
+### Transform JSON into TOML
+
+With niet you can easily convert your JSON into TOML
+```shell
+$ niet . tests/samples/sample.json -f toml
+[project]
+foo = "bar"
+list = ["item1", "item2", "item3"]
+test-dash = "value"
+
+[project.meta]
+name = "my-project"
+```
+
+### Transform YAML into TOML
+
+With niet you can easily convert your YAML into TOML
+```shell
+$ niet . tests/samples/sample.yaml -f toml
+[project]
+foo = "bar"
+list = ["item1", "item2", "item3"]
+test-dash = "value"
+
+[project.meta]
+name = "my-project"
+```
+
+### Transform TOML into YAML
+
+With niet you can easily convert your TOML into YAML
+```shell
+niet . tests/samples/sample.toml -f yaml
+project:
+  foo: bar
+  list:
+  - item1
+  - item2
+  - item3
+  meta:
+    name: my-project
+  test-dash: value
+```
+
 ### Indent JSON file
 
 This is an example of how to indent a JSON file :
 ```shell
-$ niet . tests/samples/sample_not_indented.json 
+$ niet . tests/samples/sample_not_indented.json
 {
     "project": {
         "meta": {
             "name": "my-project"
         },
         "foo": "bar",
         "list": [
```

