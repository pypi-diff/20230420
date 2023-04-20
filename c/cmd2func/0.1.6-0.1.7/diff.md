# Comparing `tmp/cmd2func-0.1.6.tar.gz` & `tmp/cmd2func-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmd2func-0.1.6.tar", last modified: Tue Mar 28 02:26:37 2023, max compression
+gzip compressed data, was "cmd2func-0.1.7.tar", last modified: Thu Apr 20 02:01:12 2023, max compression
```

## Comparing `cmd2func-0.1.6.tar` & `cmd2func-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 02:26:37.335834 cmd2func-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-28 02:26:25.000000 cmd2func-0.1.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-28 02:26:25.000000 cmd2func-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 02:26:25.000000 cmd2func-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-28 02:26:37.335834 cmd2func-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-03-28 02:26:25.000000 cmd2func-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 02:26:37.331834 cmd2func-0.1.6/cmd2func/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-28 02:26:25.000000 cmd2func-0.1.6/cmd2func/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 02:26:37.331834 cmd2func-0.1.6/cmd2func.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 02:26:37.000000 cmd2func-0.1.6/cmd2func.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 02:26:37.335834 cmd2func-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-28 02:26:25.000000 cmd2func-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:01:12.207554 cmd2func-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-20 02:00:58.000000 cmd2func-0.1.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-20 02:00:58.000000 cmd2func-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-20 02:00:58.000000 cmd2func-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 02:01:12.207554 cmd2func-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-20 02:00:58.000000 cmd2func-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:01:12.207554 cmd2func-0.1.7/cmd2func/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-20 02:00:58.000000 cmd2func-0.1.7/cmd2func/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 02:01:12.207554 cmd2func-0.1.7/cmd2func.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 02:01:12.000000 cmd2func-0.1.7/cmd2func.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 02:01:12.207554 cmd2func-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-20 02:00:58.000000 cmd2func-0.1.7/setup.py
```

### Comparing `cmd2func-0.1.6/CONTRIBUTING.md` & `cmd2func-0.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cmd2func-0.1.6/LICENSE` & `cmd2func-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cmd2func-0.1.6/PKG-INFO` & `cmd2func-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd2func
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convert command to callable Python object.
 Home-page: https://github.com/Nanguage/cmd2func
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: cmd2func
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmd2func-0.1.6/README.md` & `cmd2func-0.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -175,7 +175,28 @@
 
 out = StringIO()
 t = Tee(sys.stdout, out)
 func = cmd2func("python -c 'print({a} + {b})'", out_stream=t)
 func(1, 2)  # will print "3"
 assert out.getvalue().strip() == "3"
 ```
+
+#### Steamable command line runner
+
+`cmd2func.runner.ProcessRunner` is a streamable command line runner, which can be used to run command line in a streaming way.
+
+```Python
+from cmd2func.runner import ProcessRunner
+
+# run command line and print the output line by line
+runner = ProcessRunner("python -c 'print(1 + 2)'")
+for (src, line) in runner.steam:
+    if src == 'stdout':
+        print(line)
+
+# run command line and capture the output and error
+from io import StringIO
+runner = ProcessRunner("python -c 'print(1 + 2)'")
+out, err = StringIO(), StringIO()
+runner.write_stream_until_stop(out, err)
+print(out.getvalue().strip())  # will print '3'
+```
```

### Comparing `cmd2func-0.1.6/cmd2func/cmd.py` & `cmd2func-0.1.7/cmd2func/cmd.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.1.6/cmd2func/config.py` & `cmd2func-0.1.7/cmd2func/config.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.1.6/cmd2func/core.py` & `cmd2func-0.1.7/cmd2func/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,31 +64,66 @@
 class Cmd2Func(object):
     def __init__(
             self, cmd_or_func: T.Union[str, StrFunc, StrGenFunc],
             config: T.Optional[CLIConfig] = None,
             print_cmd=True,
             out_stream=sys.stdout,
             err_stream=sys.stderr,
+            conda_env: T.Optional[str] = None,
             popen_kwargs: T.Optional[dict] = None,):
+        """Convert a command to a function.
+
+        Args:
+            cmd_or_func: The command string or a function that returns the
+                command string or a generator that yields the command string.
+            config: The config of the command. If not provided, it will be
+                inferred from the command string. This is only used when
+                cmd_or_func is a command string. default: None.
+            print_cmd: Whether to print the command string before running it.
+                default: True.
+            out_stream: The stream to print the output of the command.
+                default: sys.stdout.
+            err_stream: The stream to print the error of the command.
+                default: sys.stderr.
+            conda_env: The conda environment to run the command.
+                default: None.
+            popen_kwargs: The keyword arguments for subprocess.Popen.
+                default: None.
+
+        Attributes:
+            lastest_cmd_str: The lastest command string that is run.
+        """
         self.get_cmd_str: T.Union[StrFunc, StrGenFunc]
         if isinstance(cmd_or_func, str):
             self.formater = CommandFormater(cmd_or_func, config)
             self.get_cmd_str = self.formater.get_cmd_str
             self.__signature__ = self.formater.signature
         else:
             self.get_cmd_str = cmd_or_func
             functools.update_wrapper(self, cmd_or_func)
 
         self.is_print_cmd = print_cmd
         self.out_stream = out_stream
         self.err_stream = err_stream
+        self.conda_env = conda_env
         self.kwargs_popen = popen_kwargs or dict()
+        self.lastest_cmd_str: T.Optional[str] = None
+
+    def process_cmd_str(self, cmd_str: str) -> str:
+        if self.conda_env is not None:
+            cmd_str = "conda run --no-capture-output " + \
+                f"-n {self.conda_env} {cmd_str}"
+        return cmd_str
 
     def run_cmd(self, cmd_str: str) -> int:
         """Run the command and return the return code."""
+        cmd_str = self.process_cmd_str(cmd_str)
+        self.lastest_cmd_str = cmd_str
+        if self.is_print_cmd:
+            print(f"Run command: {cmd_str}")
         runner = ProcessRunner(cmd_str)
         runner.run(**self.kwargs_popen)
         ret_code = runner.write_stream_until_stop(
             self.out_stream, self.err_stream)
         return ret_code
 
     def iter_and_run(self, generator: CmdGen) -> T.Any:
@@ -100,33 +135,34 @@
             except StopIteration as e:
                 return e.value
 
     def __call__(self, *args, **kwargs) -> T.Union[int, T.Any]:
         cmd_or_gen = self.get_cmd_str(*args, **kwargs)
         if isinstance(cmd_or_gen, str):
             cmd_str = cmd_or_gen
-            if self.is_print_cmd:
-                print(f"Run command: {cmd_str}")
             return self.run_cmd(cmd_str)
         else:
             return self.iter_and_run(cmd_or_gen)
 
 
 def cmd2func(
         cmd_or_func: T.Union[str, StrFunc, StrGenFunc, None] = None,
         config: T.Optional[CLIConfig] = None,
         print_cmd=True,
         out_stream=sys.stdout,
         err_stream=sys.stderr,
+        conda_env: T.Optional[str] = None,
         popen_kwargs: T.Optional[dict] = None,
         ) -> Cmd2Func:
-    """Convert a command string to a function."""
     if cmd_or_func is None:
         return functools.partial(  # type: ignore
             cmd2func, config=config, print_cmd=print_cmd,
             out_stream=out_stream, err_stream=err_stream,
-            popen_kwargs=popen_kwargs)
+            conda_env=conda_env, popen_kwargs=popen_kwargs)
     else:
         return Cmd2Func(
             cmd_or_func, config, print_cmd, out_stream, err_stream,
-            popen_kwargs
+            conda_env, popen_kwargs
         )
+
+
+cmd2func.__doc__ = Cmd2Func.__init__.__doc__
```

### Comparing `cmd2func-0.1.6/cmd2func/runner.py` & `cmd2func-0.1.7/cmd2func/runner.py`

 * *Files identical despite different names*

### Comparing `cmd2func-0.1.6/cmd2func.egg-info/PKG-INFO` & `cmd2func-0.1.7/cmd2func.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd2func
-Version: 0.1.6
+Version: 0.1.7
 Summary: Convert command to callable Python object.
 Home-page: https://github.com/Nanguage/cmd2func
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT license
 Keywords: cmd2func
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cmd2func-0.1.6/setup.py` & `cmd2func-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,30 @@
         for line in f.readlines():
             m = re.match("__version__ = '([^']+)'", line)
             if m:
                 return m.group(1)
         raise IOError("Version information can not found.")
 
 
-def get_install_requirements():
-    requirements = [
-        "funcdesc>=0.1.2",
-        "typing_extensions",
-        "pyYAML",
-    ]
+def get_requirements_from_file(filename):
+    requirements = []
+    with open(filename) as f:
+        for line in f.readlines():
+            line = line.strip()
+            if len(line) == 0:
+                continue
+            if line and not line.startswith('#'):
+                requirements.append(line)
     return requirements
 
 
+def get_install_requires():
+    return get_requirements_from_file('requirements.txt')
+
+
 requires_test = ['pytest', 'pytest-cov', 'flake8', 'mypy']
 packages_for_dev = ["pip", "setuptools", "wheel", "twine", "ipdb"]
 
 requires_dev = packages_for_dev + requires_test
 
 setup(
     author="Weize Xu",
@@ -44,15 +51,15 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     description="Convert command to callable Python object.",
-    install_requires=get_install_requirements(),
+    install_requires=get_install_requires(),
     license="MIT license",
     long_description=get_long_description(),
     include_package_data=True,
     keywords='cmd2func',
     name='cmd2func',
     packages=find_packages(include=['cmd2func', 'cmd2func.*']),
     url='https://github.com/Nanguage/cmd2func',
```

