# Comparing `tmp/remove_print_statements-0.5.0.tar.gz` & `tmp/remove_print_statements-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remove_print_statements-0.5.0.tar", max compression
+gzip compressed data, was "remove_print_statements-0.5.1.tar", max compression
```

## Comparing `remove_print_statements-0.5.0.tar` & `remove_print_statements-0.5.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2022-10-29 18:53:10.058441 remove_print_statements-0.5.0/LICENSE
--rw-r--r--   0        0        0     6264 2022-10-29 18:53:10.058441 remove_print_statements-0.5.0/README.md
--rw-r--r--   0        0        0     1862 2022-10-29 18:53:10.062441 remove_print_statements-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     9210 2022-10-29 18:53:10.062441 remove_print_statements-0.5.0/remove_print_statements.py
--rw-r--r--   0        0        0     7253 1970-01-01 00:00:00.000000 remove_print_statements-0.5.0/setup.py
--rw-r--r--   0        0        0     7793 1970-01-01 00:00:00.000000 remove_print_statements-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6273 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/README.md
+-rw-r--r--   0        0        0     1862 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9246 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/remove_print_statements.py
+-rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 remove_print_statements-0.5.1/PKG-INFO
```

### Comparing `remove_print_statements-0.5.0/LICENSE` & `remove_print_statements-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remove_print_statements-0.5.0/README.md` & `remove_print_statements-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 [![test](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml/badge.svg)](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/dhruvmanila/remove-print-statements/branch/main/graph/badge.svg)](https://codecov.io/gh/dhruvmanila/remove-print-statements)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/dhruvmanila/remove-print-statements/main.svg)](https://results.pre-commit.ci/latest/github/dhruvmanila/remove-print-statements/main)
 [![PyPi Status](https://img.shields.io/pypi/v/remove-print-statements.svg?color=blue)](https://pypi.org/project/remove-print-statements/)
 ![Python versions](https://img.shields.io/pypi/pyversions/remove-print-statements.svg)
 [![MIT License](https://img.shields.io/pypi/l/remove-print-statements.svg)](./LICENSE)
 
-A CLI tool (and pre-commit hook) to remove all the `print` statements from your
-Python project.
+A command-line tool (and pre-commit hook) to remove all the `print` statements
+from your Python project.
 
 </div>
 
 Do you use `print` statements for debugging? We all do, and there's nothing wrong
 with it. After the bug has been resolved, we need to manually open all the files
 which we added the print statements in, only if we remember all of them after
 hours of debugging, and remove them. A better way would be to use some sort of
```

### Comparing `remove_print_statements-0.5.0/pyproject.toml` & `remove_print_statements-0.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remove-print-statements"
-version = "0.5.0"
+version = "0.5.1"
 description = "A tool (and pre-commit hook) to remove print statements from your Python project."
 authors = ["Dhruv Manilawala <dhruvmanila@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dhruvmanila/remove-print-statements"
 repository = "https://github.com/dhruvmanila/remove-print-statements"
 keywords = ["python", "codemod", "libCST"]
```

### Comparing `remove_print_statements-0.5.0/remove_print_statements.py` & `remove_print_statements-0.5.1/remove_print_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ContextAwareTransformer,
     TransformFailure,
     TransformSuccess,
     transform_module,
 )
 from libcst.metadata import PositionProvider
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # TODO(dhruvmanila): Remove this block when it's the default.
 # https://github.com/Instagram/LibCST/issues/285#issuecomment-1011427731
 if sys.version_info >= (3, 10):
     os.environ["LIBCST_PARSER_TYPE"] = "native"
 
 
@@ -191,15 +191,15 @@
     Args:
         filename: Name of the file to check
         report: A report instance which will be updated with the given file's stats.
         dry_run: If True, it will not update the file with the transformed code.
         verbose: If True, output all the print statements along with their location.
     """
     try:
-        with open(filename) as f:
+        with open(filename, encoding="utf-8") as f:
             code = f.read()
     except Exception as exc:  # pragma: no cover
         click.secho(f"Could not read file {filename!r}, skipping: {exc}", fg="red")
         report.failure_count += 1
         return
 
     codemod = RemovePrintStatements(
@@ -211,15 +211,15 @@
     if isinstance(result, TransformSuccess):
         if codemod.print_statement_count:
             report.file_count += 1
             report.print_statement_count += codemod.print_statement_count
             if verbose:
                 click.echo(format_verbose_output(filename, codemod.print_statements))
             if not dry_run:
-                with open(filename, "w") as f:
+                with open(filename, "w", encoding="utf-8") as f:
                     f.write(result.code)
     elif isinstance(result, TransformFailure):
         click.secho(
             f"Failed to transform the file {filename!r}: {result.error}", fg="red"
         )
         report.failure_count += 1
```

### Comparing `remove_print_statements-0.5.0/setup.py` & `remove_print_statements-0.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,177 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: remove-print-statements
+Version: 0.5.1
+Summary: A tool (and pre-commit hook) to remove print statements from your Python project.
+Home-page: https://github.com/dhruvmanila/remove-print-statements
+License: MIT
+Keywords: python,codemod,libCST
+Author: Dhruv Manilawala
+Author-email: dhruvmanila@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Typing :: Typed
+Requires-Dist: click (>=8.1.1)
+Requires-Dist: libcst (>=0.4.2,<0.5.0)
+Project-URL: Bug Tracker, https://github.com/dhruvmanila/remove-print-statements/issues
+Project-URL: Repository, https://github.com/dhruvmanila/remove-print-statements
+Description-Content-Type: text/markdown
 
-modules = \
-['remove_print_statements']
-install_requires = \
-['click>=8.1.1', 'libcst>=0.4.2,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['remove-print-statements = remove_print_statements:main']}
-
-setup_kwargs = {
-    'name': 'remove-print-statements',
-    'version': '0.5.0',
-    'description': 'A tool (and pre-commit hook) to remove print statements from your Python project.',
-    'long_description': '<div align="center">\n\n# remove-print-statements\n\n[![test](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml/badge.svg)](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/dhruvmanila/remove-print-statements/branch/main/graph/badge.svg)](https://codecov.io/gh/dhruvmanila/remove-print-statements)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/dhruvmanila/remove-print-statements/main.svg)](https://results.pre-commit.ci/latest/github/dhruvmanila/remove-print-statements/main)\n[![PyPi Status](https://img.shields.io/pypi/v/remove-print-statements.svg?color=blue)](https://pypi.org/project/remove-print-statements/)\n![Python versions](https://img.shields.io/pypi/pyversions/remove-print-statements.svg)\n[![MIT License](https://img.shields.io/pypi/l/remove-print-statements.svg)](./LICENSE)\n\nA CLI tool (and pre-commit hook) to remove all the `print` statements from your\nPython project.\n\n</div>\n\nDo you use `print` statements for debugging? We all do, and there\'s nothing wrong\nwith it. After the bug has been resolved, we need to manually open all the files\nwhich we added the print statements in, only if we remember all of them after\nhours of debugging, and remove them. A better way would be to use some sort of\nfind and replace from the editor or command-line, but that\'s still a lot of\nmanual work. Worst case, it gets pushed and deployed to production.\n\nWho wants to do all the manual work in the age of automation? No one. So,\ninstall this tool and forget about removing the print statements manually\nforever. You could either run this tool manually or add it as a `pre-commit`\nhook. You could even preview the print statements along with it\'s location\nwithout removing it. How nice is that!\n\n## Installation\n\nYou can install `remove-print-statements` from the Python Package Index (PyPI)\nwith `pip` or equivalent.\n\n```\npython -m pip install remove-print-statements\n```\n\nOr with [pre-commit](https://pre-commit.com) in the `repos` section of your\n`.pre-commit-config.yaml` file ([docs](https://pre-commit.com/#plugins)):\n\n```yaml\n- repo: https://github.com/dhruvmanila/remove-print-statements\n  rev: \'\'  # Replace with latest tag on GitHub\n  hooks:\n  - id: remove-print-statements\n    args: [\'--verbose\']   # Show all the print statements to be removed\n```\n\n## Usage\n\nRun it on a given set of files:\n```sh\nremove-print-statements foo.py bar.py ...\n# or use globbing\nremove-print-statements *.py\n```\n\nYou can ignore files as well. To specify multiple files to ignore, use the flag\nmultiple times otherwise it\'s difficult to know the difference between the files\nto ignore and the ones to check.\n```sh\nremove-print-statements *.py --ignore foo.py --ignore bar.py\n```\n\nYou can preview the print statements which would be removed without modifying\nthe source files using both `--dry-run` and `--verbose` flags like so:\n\n```console\n$ remove-print-statements --dry-run --verbose test.py\ntest.py\n  7 print("module")\n  18 print("property")\n  27 print("method")\n  29 print("for loop")\n\n1 file would be transformed, 4 print statements would be removed\n```\n\n`remove-print-statements` is a command-line tool that rewrites the files in\nplace. It focuses on upgrading your code and not on making it look nice. Run\nremove-print-statements before formatters like [Black](https://black.readthedocs.io/en/stable/).\n\n`remove-print-statements` does not have any ability to recurse through\ndirectories. Use the pre-commit integration, globbing, or another technique for\napplying to many files such as [with `git ls-files | xargs`][1].\n\n### Single statement\n\nIf there\'s only a single statement in the body of a function, for/while loop, if\nstatement, etc., which is a print statement, then it will be replaced with the\n`pass` keyword.\n\n```diff\ndef foo():\n-    print()\n+    pass\n\n\nfor _ in range(5):\n-    print()\n+    pass\n\nif __name__ == "__main__":\n-    print()\n+    pass\n```\n\n### Exit status\n\n`remove-print-statements` command returns exit statuses as follows:\n\n| Status       | Description                                      |\n| :----------: | ------------------------------------------------ |\n| 0            | No print statements / changes made successfully |\n| 1            | Files would be updated (dry run)                 |\n| 123          | Some error happened                              |\n\n## Development\n\n[![packaging: poetry](https://img.shields.io/badge/packaging-poetry-299bd7?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=)](https://python-poetry.org/)\n[![code style: black](https://img.shields.io/static/v1?label=code%20style&message=black&color=black)](https://github.com/psf/black)\n[![pre-commit: enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n### Release\n\n1. Run `poetry lock`\n2. Bump version in `pyproject.toml` and `__version__` variable\n3. Commit and push the changes with message `release: <version>`\n4. Publish a new release on GitHub which will trigger an automated workflow to\n   publish on PyPi\n\n## License\n\nremove-print-statements is licensed under the MIT License.\n\nSee [LICENSE](./LICENSE) for details.\n\n<!-- References -->\n\n[1]: https://adamj.eu/tech/2022/03/09/how-to-run-a-command-on-many-files-in-your-git-repository/\n',
-    'author': 'Dhruv Manilawala',
-    'author_email': 'dhruvmanila@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dhruvmanila/remove-print-statements',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+<div align="center">
 
+# remove-print-statements
+
+[![test](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml/badge.svg)](https://github.com/dhruvmanila/remove-print-statements/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/dhruvmanila/remove-print-statements/branch/main/graph/badge.svg)](https://codecov.io/gh/dhruvmanila/remove-print-statements)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/dhruvmanila/remove-print-statements/main.svg)](https://results.pre-commit.ci/latest/github/dhruvmanila/remove-print-statements/main)
+[![PyPi Status](https://img.shields.io/pypi/v/remove-print-statements.svg?color=blue)](https://pypi.org/project/remove-print-statements/)
+![Python versions](https://img.shields.io/pypi/pyversions/remove-print-statements.svg)
+[![MIT License](https://img.shields.io/pypi/l/remove-print-statements.svg)](./LICENSE)
+
+A command-line tool (and pre-commit hook) to remove all the `print` statements
+from your Python project.
+
+</div>
+
+Do you use `print` statements for debugging? We all do, and there's nothing wrong
+with it. After the bug has been resolved, we need to manually open all the files
+which we added the print statements in, only if we remember all of them after
+hours of debugging, and remove them. A better way would be to use some sort of
+find and replace from the editor or command-line, but that's still a lot of
+manual work. Worst case, it gets pushed and deployed to production.
+
+Who wants to do all the manual work in the age of automation? No one. So,
+install this tool and forget about removing the print statements manually
+forever. You could either run this tool manually or add it as a `pre-commit`
+hook. You could even preview the print statements along with it's location
+without removing it. How nice is that!
+
+## Installation
+
+You can install `remove-print-statements` from the Python Package Index (PyPI)
+with `pip` or equivalent.
+
+```
+python -m pip install remove-print-statements
+```
+
+Or with [pre-commit](https://pre-commit.com) in the `repos` section of your
+`.pre-commit-config.yaml` file ([docs](https://pre-commit.com/#plugins)):
+
+```yaml
+- repo: https://github.com/dhruvmanila/remove-print-statements
+  rev: ''  # Replace with latest tag on GitHub
+  hooks:
+  - id: remove-print-statements
+    args: ['--verbose']   # Show all the print statements to be removed
+```
+
+## Usage
+
+Run it on a given set of files:
+```sh
+remove-print-statements foo.py bar.py ...
+# or use globbing
+remove-print-statements *.py
+```
+
+You can ignore files as well. To specify multiple files to ignore, use the flag
+multiple times otherwise it's difficult to know the difference between the files
+to ignore and the ones to check.
+```sh
+remove-print-statements *.py --ignore foo.py --ignore bar.py
+```
+
+You can preview the print statements which would be removed without modifying
+the source files using both `--dry-run` and `--verbose` flags like so:
+
+```console
+$ remove-print-statements --dry-run --verbose test.py
+test.py
+  7 print("module")
+  18 print("property")
+  27 print("method")
+  29 print("for loop")
+
+1 file would be transformed, 4 print statements would be removed
+```
+
+`remove-print-statements` is a command-line tool that rewrites the files in
+place. It focuses on upgrading your code and not on making it look nice. Run
+remove-print-statements before formatters like [Black](https://black.readthedocs.io/en/stable/).
+
+`remove-print-statements` does not have any ability to recurse through
+directories. Use the pre-commit integration, globbing, or another technique for
+applying to many files such as [with `git ls-files | xargs`][1].
+
+### Single statement
+
+If there's only a single statement in the body of a function, for/while loop, if
+statement, etc., which is a print statement, then it will be replaced with the
+`pass` keyword.
+
+```diff
+def foo():
+-    print()
++    pass
+
+
+for _ in range(5):
+-    print()
++    pass
+
+if __name__ == "__main__":
+-    print()
++    pass
+```
+
+### Exit status
+
+`remove-print-statements` command returns exit statuses as follows:
+
+| Status       | Description                                      |
+| :----------: | ------------------------------------------------ |
+| 0            | No print statements / changes made successfully |
+| 1            | Files would be updated (dry run)                 |
+| 123          | Some error happened                              |
+
+## Development
+
+[![packaging: poetry](https://img.shields.io/badge/packaging-poetry-299bd7?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=)](https://python-poetry.org/)
+[![code style: black](https://img.shields.io/static/v1?label=code%20style&message=black&color=black)](https://github.com/psf/black)
+[![pre-commit: enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
+### Release
+
+1. Run `poetry lock`
+2. Bump version in `pyproject.toml` and `__version__` variable
+3. Commit and push the changes with message `release: <version>`
+4. Publish a new release on GitHub which will trigger an automated workflow to
+   publish on PyPi
+
+## License
+
+remove-print-statements is licensed under the MIT License.
+
+See [LICENSE](./LICENSE) for details.
+
+<!-- References -->
+
+[1]: https://adamj.eu/tech/2022/03/09/how-to-run-a-command-on-many-files-in-your-git-repository/
 
-setup(**setup_kwargs)
```

