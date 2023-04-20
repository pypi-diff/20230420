# Comparing `tmp/openapi_readme-0.2.1.tar.gz` & `tmp/openapi_readme-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_readme-0.2.1.tar", max compression
+gzip compressed data, was "openapi_readme-0.2.2.tar", max compression
```

## Comparing `openapi_readme-0.2.1.tar` & `openapi_readme-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-10-21 14:13:36.329262 openapi_readme-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     1892 2022-10-22 08:23:57.605488 openapi_readme-0.2.1/README.md
--rw-r--r--   0        0        0        0 2022-10-21 08:37:08.347794 openapi_readme-0.2.1/openapi_readme/__init__.py
--rw-r--r--   0        0        0     4115 2022-10-22 08:38:10.895753 openapi_readme-0.2.1/openapi_readme/main.py
--rw-r--r--   0        0        0     1308 2022-10-22 08:38:10.895753 openapi_readme-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 openapi_readme-0.2.1/setup.py
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 openapi_readme-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-21 14:13:36.329262 openapi_readme-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1965 2023-04-20 11:23:36.904701 openapi_readme-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2022-10-21 08:37:08.347794 openapi_readme-0.2.2/openapi_readme/__init__.py
+-rw-r--r--   0        0        0     4504 2023-04-20 11:51:18.263740 openapi_readme-0.2.2/openapi_readme/main.py
+-rw-r--r--   0        0        0     1354 2023-04-20 11:51:18.263740 openapi_readme-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 openapi_readme-0.2.2/setup.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 openapi_readme-0.2.2/PKG-INFO
```

### Comparing `openapi_readme-0.2.1/LICENSE.txt` & `openapi_readme-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openapi_readme-0.2.1/README.md` & `openapi_readme-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 there is a lot to do with extra functionality and refactoring.
 
 - [Usage](#usage)
 - [Options Summary](#options-summary)
 - [Options in Detail](#options-in-detail)
   - [--route-level](#--route-level)
   - [--inject](#--inject)
+- [TODO](#todo)
 
 ## Usage
 
 ```console
 openapi-readme [OPTIONS]
 ```
 
@@ -58,8 +59,12 @@
 
 ### Next section
 The document continues unaffected after the injection.
 ```
 
 Existing (previously injected) Schemas will be **replaced** by this new data.
 
-<!-- openapi-schema -->
+## TODO
+
+Future improvement plans
+
+- Take more info from the `openapi.json` file
```

### Comparing `openapi_readme-0.2.1/openapi_readme/main.py` & `openapi_readme-0.2.2/openapi_readme/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from pathlib import Path
+from typing import Optional
 
 try:
     from importlib import metadata
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata
 
 import typer
@@ -12,15 +13,15 @@
 
 path_to_pyproject_dir = Path(__file__).parent.parent
 __version__ = get_version(__name__, path_to_pyproject_dir, default_return=None)
 
 if __version__ is None:
     __version__ = metadata.version("openapi-readme")
 
-app = typer.Typer()
+app = typer.Typer(pretty_exceptions_show_locals=False)
 
 OPENAPI_FILENAME = "openapi.json"
 README_FILENAME = "README.md"
 
 
 def get_api_data(filename: str) -> dict:
     """Return a python dictionary containing the API data from schema file."""
@@ -36,22 +37,28 @@
 
 
 def process_path(route: str, route_data: dict, route_level: int) -> str:
     """Process the specific API route."""
     output = [""]
 
     for verb, verb_data in route_data.items():
-        first_line, *desc = verb_data["description"].splitlines()
+        description = verb_data.get("description", "")
         heading_level = "#" * route_level
         output.append(f"{heading_level} **`{verb.upper()}`** _{route}_\n")
-        output.append(f"> {verb_data['summary']} : _{first_line}_".strip())
-
-        if desc:
-            for line in desc:
-                output.append(f"> {line}".strip())
+        if description:
+            first_line, *desc = description.splitlines()
+            output.append(f"> {verb_data['summary']} : _{first_line}_".strip())
+            if desc:
+                for line in desc:
+                    output.append(f"> {line}".strip())
+        else:
+            # output.append(f"{heading_level} **`{verb.upper()}`** _{route}_\n")
+            output.append(
+                f"> {verb_data['summary']} : _No Description Given_".strip()
+            )
 
     return "\n".join(output) + "\n"
 
 
 def get_markdown(route_level: int) -> str:
     """Return the full OpenAPI Markdown as a string."""
     schema_path = Path(".") / OPENAPI_FILENAME
@@ -61,27 +68,28 @@
         output += process_path(route, data, route_level)
 
     return output
 
 
 def print_header() -> None:
     print(
-        "\n[cyan][underline]openapi-readme[/underline] "
-        f"version [bold]{__version__}[/bold] (c) Grant Ramsay 2022.",
+        "[cyan][underline]openapi-readme[/underline] "
+        f"version [bold]{__version__}[/bold] (c) Grant Ramsay 2023.\n",
     )
 
 
 @app.command()
 def main(
     route_level: int = typer.Option(4, help="Number of heading levels to use."),
     inject: bool = typer.Option(
-        False, help="Inject generated output into a README file."
+        False,
+        "--inject",
+        help="Inject generated output into a README file.",
     ),
 ) -> None:
-
     output = get_markdown(route_level)
 
     if inject:
         print_header()
         try:
             with open(README_FILENAME, "r+") as f:
                 contents = f.readlines()
```

### Comparing `openapi_readme-0.2.1/pyproject.toml` & `openapi_readme-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-readme"
-version = "0.2.1"
+version = "0.2.2"
 description = "Generate Markdown from an openapi JSON file."
 authors = ["Grant Ramsay <grant@gnramsay.com>"]
 readme = "README.md"
 packages = [{ include = "openapi_readme" }]
 license = "MIT"
 repository = "https://github.com/seapagan/openapi-readme"
 homepage = "https://github.com/seapagan/openapi-readme"
@@ -25,20 +25,21 @@
 "Pull Requests" = "https://github.com/seapagan/openapi-readme/pulls"
 "Bug Tracker" = "https://github.com/seapagan/openapi-readme/issues"
 
 [tool.poetry.scripts]
 openapi-readme = "openapi_readme.main:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-typer = { extras = ["all"], version = "^0.6.1" }
+python = "^3.8.1,<4.0"
+typer = { extras = ["all"], version = ">=0.6.1,<0.8.0" }
 pydantic = "^1.10.2"
 single-source = "^0.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^5.0.4"
-black = "^22.10.0"
+flake8 = ">=5.0.4,<7.0.0"
+black = ">=22.10,<24.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openapi_readme-0.2.1/setup.py` & `openapi_readme-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.2,<2.0.0',
  'single-source>=0.3.0,<0.4.0',
- 'typer[all]>=0.6.1,<0.7.0']
+ 'typer[all]>=0.6.1,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['openapi-readme = openapi_readme.main:app']}
 
 setup_kwargs = {
     'name': 'openapi-readme',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Generate Markdown from an openapi JSON file.',
-    'long_description': '# OpenAPI Readme Generator  <!-- omit in toc -->\n\nGenerates Markdown suitable for a README file from a local `openapi.json` file.\n\nThis tool is still under development, progress so far is only a days work so\nthere is a lot to do with extra functionality and refactoring.\n\n- [Usage](#usage)\n- [Options Summary](#options-summary)\n- [Options in Detail](#options-in-detail)\n  - [--route-level](#--route-level)\n  - [--inject](#--inject)\n\n## Usage\n\n```console\nopenapi-readme [OPTIONS]\n```\n\nRun this in the same directory as your `openapi.json` file. By default the\nMarkdown output will be printed to the console, but you can redirect it out to\na file too.\n\nThe particular styling of the generated Markdown is currently hardcoded, though\nplans are afoot to implement some sort of themeing.\n\n## Options Summary\n\n- `--route-level INTEGER`: Number of heading levels to use.  [default: 4]\n- `--inject / --no-inject`: Inject generated output into a README file.  [default: False]\n- `--install-completion`: Install completion for the current shell.\n- `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n- `--help`: Show this message and exit.\n\n## Options in Detail\n\n### --route-level\n\nSpecify the heading level for each Route in the generated documentation. This\ndefaults to **4** if not specified, ie:\n\n```Markdown\n#### **`GET`** _/user/list_\n```\n\n### --inject\n\nInjects the new Markdown directly into a `README.md` file in the current\ndirectory, if it is found.\nYou need to add the placeholder comment `<!--\nopenapi-schema -->` to your markdown where you want it to be injected:\n\n```Markdown\nThis is some preceeding text\n\n### API Schema description\n<!-- openapi-schema -->\n\n### Next section\nThe document continues unaffected after the injection.\n```\n\nExisting (previously injected) Schemas will be **replaced** by this new data.\n\n<!-- openapi-schema -->\n',
+    'long_description': '# OpenAPI Readme Generator  <!-- omit in toc -->\n\nGenerates Markdown suitable for a README file from a local `openapi.json` file.\n\nThis tool is still under development, progress so far is only a days work so\nthere is a lot to do with extra functionality and refactoring.\n\n- [Usage](#usage)\n- [Options Summary](#options-summary)\n- [Options in Detail](#options-in-detail)\n  - [--route-level](#--route-level)\n  - [--inject](#--inject)\n- [TODO](#todo)\n\n## Usage\n\n```console\nopenapi-readme [OPTIONS]\n```\n\nRun this in the same directory as your `openapi.json` file. By default the\nMarkdown output will be printed to the console, but you can redirect it out to\na file too.\n\nThe particular styling of the generated Markdown is currently hardcoded, though\nplans are afoot to implement some sort of themeing.\n\n## Options Summary\n\n- `--route-level INTEGER`: Number of heading levels to use.  [default: 4]\n- `--inject / --no-inject`: Inject generated output into a README file.  [default: False]\n- `--install-completion`: Install completion for the current shell.\n- `--show-completion`: Show completion for the current shell, to copy it or customize the installation.\n- `--help`: Show this message and exit.\n\n## Options in Detail\n\n### --route-level\n\nSpecify the heading level for each Route in the generated documentation. This\ndefaults to **4** if not specified, ie:\n\n```Markdown\n#### **`GET`** _/user/list_\n```\n\n### --inject\n\nInjects the new Markdown directly into a `README.md` file in the current\ndirectory, if it is found.\nYou need to add the placeholder comment `<!--\nopenapi-schema -->` to your markdown where you want it to be injected:\n\n```Markdown\nThis is some preceeding text\n\n### API Schema description\n<!-- openapi-schema -->\n\n### Next section\nThe document continues unaffected after the injection.\n```\n\nExisting (previously injected) Schemas will be **replaced** by this new data.\n\n## TODO\n\nFuture improvement plans\n\n- Take more info from the `openapi.json` file\n',
     'author': 'Grant Ramsay',
     'author_email': 'grant@gnramsay.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seapagan/openapi-readme',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `openapi_readme-0.2.1/PKG-INFO` & `openapi_readme-0.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: openapi-readme
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate Markdown from an openapi JSON file.
 Home-page: https://github.com/seapagan/openapi-readme
 License: MIT
 Author: Grant Ramsay
 Author-email: grant@gnramsay.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
-Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/openapi-readme/issues
 Project-URL: Pull Requests, https://github.com/seapagan/openapi-readme/pulls
 Project-URL: Repository, https://github.com/seapagan/openapi-readme
 Description-Content-Type: text/markdown
 
 # OpenAPI Readme Generator  <!-- omit in toc -->
 
@@ -40,14 +38,15 @@
 there is a lot to do with extra functionality and refactoring.
 
 - [Usage](#usage)
 - [Options Summary](#options-summary)
 - [Options in Detail](#options-in-detail)
   - [--route-level](#--route-level)
   - [--inject](#--inject)
+- [TODO](#todo)
 
 ## Usage
 
 ```console
 openapi-readme [OPTIONS]
 ```
 
@@ -92,9 +91,13 @@
 
 ### Next section
 The document continues unaffected after the injection.
 ```
 
 Existing (previously injected) Schemas will be **replaced** by this new data.
 
-<!-- openapi-schema -->
+## TODO
+
+Future improvement plans
+
+- Take more info from the `openapi.json` file
```

