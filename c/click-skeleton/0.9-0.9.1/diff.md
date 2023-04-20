# Comparing `tmp/click-skeleton-0.9.tar.gz` & `tmp/click-skeleton-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-skeleton-0.9.tar", last modified: Sat Dec 19 16:50:09 2020, max compression
+gzip compressed data, was "click-skeleton-0.9.1.tar", last modified: Fri Jan 22 20:49:02 2021, max compression
```

## Comparing `click-skeleton-0.9.tar` & `click-skeleton-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      629 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/__init__.py
--rw-r--r--   0        0        0     3472 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/advanced_group.py
--rw-r--r--   0        0        0     9215 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/backtrace.py
--rw-r--r--   0        0        0     2315 2020-12-19 16:27:22.000000 click-skeleton-0.9/click_skeleton/completion.py
--rw-r--r--   0        0        0     2977 2020-12-19 15:15:57.990000 click-skeleton-0.9/click_skeleton/core.py
--rw-r--r--   0        0        0     1159 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/decorators.py
--rw-r--r--   0        0        0     2723 2020-12-19 16:36:28.640000 click-skeleton-0.9/click_skeleton/doc.py
--rw-r--r--   0        0        0      133 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/exceptions.py
--rw-r--r--   0        0        0     2749 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/expanded_path.py
--rw-r--r--   0        0        0     3070 2020-12-19 15:15:57.990000 click-skeleton-0.9/click_skeleton/helpers.py
--rw-r--r--   0        0        0     1275 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/importdir.py
--rw-r--r--   0        0        0        0 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/py.typed
--rw-r--r--   0        0        0      949 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/testing.py
--rw-r--r--   0        0        0      526 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/version.py
--rw-r--r--   0        0        0     4010 2020-10-05 02:57:21.150000 click-skeleton-0.9/click_skeleton/version_checker.py
--rw-r--r--   0        0        0     1408 2020-12-19 16:48:44.570000 click-skeleton-0.9/pyproject.toml
--rw-r--r--   0        0        0      931 2020-12-19 16:50:09.134518 click-skeleton-0.9/setup.py
--rw-r--r--   0        0        0      909 2020-12-19 16:50:09.134795 click-skeleton-0.9/PKG-INFO
+-rw-r--r--   0        0        0      629 2020-11-04 22:49:38.504005 click-skeleton-0.9.1/click_skeleton/__init__.py
+-rw-r--r--   0        0        0     3634 2021-01-22 20:48:54.899698 click-skeleton-0.9.1/click_skeleton/advanced_group.py
+-rw-r--r--   0        0        0     9215 2020-11-04 22:49:38.504762 click-skeleton-0.9.1/click_skeleton/backtrace.py
+-rw-r--r--   0        0        0     2315 2021-01-22 19:45:32.133418 click-skeleton-0.9.1/click_skeleton/completion.py
+-rw-r--r--   0        0        0     2977 2020-12-15 15:58:44.966390 click-skeleton-0.9.1/click_skeleton/core.py
+-rw-r--r--   0        0        0     1159 2020-11-04 22:49:38.505430 click-skeleton-0.9.1/click_skeleton/decorators.py
+-rw-r--r--   0        0        0     2723 2021-01-22 19:45:32.134734 click-skeleton-0.9.1/click_skeleton/doc.py
+-rw-r--r--   0        0        0      133 2020-11-04 22:49:38.506119 click-skeleton-0.9.1/click_skeleton/exceptions.py
+-rw-r--r--   0        0        0     2749 2020-11-04 22:49:38.506246 click-skeleton-0.9.1/click_skeleton/expanded_path.py
+-rw-r--r--   0        0        0     3070 2020-11-04 22:49:38.506621 click-skeleton-0.9.1/click_skeleton/helpers.py
+-rw-r--r--   0        0        0     1275 2020-11-04 22:49:38.506811 click-skeleton-0.9.1/click_skeleton/importdir.py
+-rw-r--r--   0        0        0        0 2020-11-04 22:49:38.507126 click-skeleton-0.9.1/click_skeleton/py.typed
+-rw-r--r--   0        0        0      949 2020-11-04 22:49:38.507298 click-skeleton-0.9.1/click_skeleton/testing.py
+-rw-r--r--   0        0        0      526 2020-11-04 22:49:38.507452 click-skeleton-0.9.1/click_skeleton/version.py
+-rw-r--r--   0        0        0     4010 2020-11-04 22:49:38.507644 click-skeleton-0.9.1/click_skeleton/version_checker.py
+-rw-r--r--   0        0        0     1410 2021-01-22 20:48:54.926679 click-skeleton-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      933 2021-01-22 20:49:02.192898 click-skeleton-0.9.1/setup.py
+-rw-r--r--   0        0        0      911 2021-01-22 20:49:02.193237 click-skeleton-0.9.1/PKG-INFO
```

### Comparing `click-skeleton-0.9/click_skeleton/__init__.py` & `click-skeleton-0.9.1/click_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/advanced_group.py` & `click-skeleton-0.9.1/click_skeleton/advanced_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,38 +20,42 @@
     - click aliases for commands
     - colored help message
     - auto help command
     '''
     def __init__(self, *args: Any, aliases: Optional[str] = None, **kwargs: Any):
         kwargs['help_headers_color'] = 'yellow'
         kwargs['help_options_color'] = 'green'
-        # super(AdvancedGroup, self).__init__(*args, aliases=aliases, **kwargs)
         super().__init__(*args, **kwargs)
-        # print(f"{self} : {args} | {kwargs}")
         self.aliases = aliases if aliases is not None else []
 
         @click.command('help')
         @click.argument('command', nargs=-1)
         @click.pass_context
         def _help(ctx: Optional[click.Context], command: Sequence[click.Command]) -> None:
             '''Print help'''
             # we accept many commands, but only show help of the first one
             if not ctx:
                 raise RuntimeError('no click context available')
             if command:
                 first_command = command[0]
                 command_obj = self.get_command(ctx, first_command)
-                print(command_obj.get_help(ctx))
+                click.echo(command_obj.get_help(ctx))
             else:
                 if not ctx.parent:
                     raise RuntimeError('no click context parent available')
-                print(ctx.parent.get_help())
+                click.echo(ctx.parent.get_help())
 
         self.add_command(_help, 'help')
 
+    def parse_args(self, ctx: click.Context, args: Any) -> Any:
+        if any([help_option_name in args for help_option_name in ctx.help_option_names]):
+            click.echo(ctx.get_help(), color=ctx.color)
+            ctx.exit()
+        return super().parse_args(ctx, args)
+
     def add_group(self, cmd: "AdvancedGroup", name: str) -> None:
         """Registers another :class:`Group` with this group.  If the name
         is not provided, the name of the group is used.
         """
         self.add_command(cmd, name)
 
         if not cmd.aliases:
```

### Comparing `click-skeleton-0.9/click_skeleton/backtrace.py` & `click-skeleton-0.9.1/click_skeleton/backtrace.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/completion.py` & `click-skeleton-0.9.1/click_skeleton/completion.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/core.py` & `click-skeleton-0.9.1/click_skeleton/core.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/decorators.py` & `click-skeleton-0.9.1/click_skeleton/decorators.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/doc.py` & `click-skeleton-0.9.1/click_skeleton/doc.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/expanded_path.py` & `click-skeleton-0.9.1/click_skeleton/expanded_path.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/helpers.py` & `click-skeleton-0.9.1/click_skeleton/helpers.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/importdir.py` & `click-skeleton-0.9.1/click_skeleton/importdir.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/testing.py` & `click-skeleton-0.9.1/click_skeleton/testing.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/version.py` & `click-skeleton-0.9.1/click_skeleton/version.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/click_skeleton/version_checker.py` & `click-skeleton-0.9.1/click_skeleton/version_checker.py`

 * *Files identical despite different names*

### Comparing `click-skeleton-0.9/pyproject.toml` & `click-skeleton-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "click-skeleton"
-version = "0.9"
+version = "0.9.1"
 description = "Click app skeleton"
 authors = ["Adrien Pensart"]
 
 [tool.poetry.dependencies]
 python = ">=3.6,<=3.9"
 click-completion = "^0.5.0"
 click-didyoumean = "^0.0.3"
@@ -21,16 +21,16 @@
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^2.10.1"
 pylint = "^2.6.0"
 coverage-badge = "^1.0.1"
 flake8 = "^3.8.3"
 dephell = "^0.8.3"
-mypy = "^0.790"
 restructuredtext-lint = "^1.3.2"
+mypy = "^0.800"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov-report term-missing:skip-covered --cov-report html --durations=0 --cov click_skeleton -s"
 
 [tool.pylint.master]
 jobs = 4
```

### Comparing `click-skeleton-0.9/setup.py` & `click-skeleton-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'pytest-click>=1.0.2,<2.0.0',
  'pytest>=6.0.1,<7.0.0',
  'requests>=2.24.0,<3.0.0',
  'semver>=2.10.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'click-skeleton',
-    'version': '0.9',
+    'version': '0.9.1',
     'description': 'Click app skeleton',
     'long_description': None,
     'author': 'Adrien Pensart',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `click-skeleton-0.9/PKG-INFO` & `click-skeleton-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-skeleton
-Version: 0.9
+Version: 0.9.1
 Summary: Click app skeleton
 Author: Adrien Pensart
 Requires-Python: >=3.6,<=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

