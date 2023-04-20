# Comparing `tmp/snk-0.5.0.tar.gz` & `tmp/snk-0.6.0.tar.gz`

## Comparing `snk-0.5.0.tar` & `snk-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.5.0/Dockerfile
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.5.0/snk/__about__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.5.0/snk/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.5.0/snk/errors.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 snk-0.5.0/snk/main.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 snk-0.5.0/snk/nest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/__init__.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/config.py
--rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/options.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/pipeline.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.5.0/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_nest.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_pipline_cli.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.5.0/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/.snk
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/Snakefile
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk-0.5.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 snk-0.5.0/README.md
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 snk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 snk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.0/Dockerfile
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 snk-0.6.0/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.0/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.0/snk/__about__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.6.0/snk/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.6.0/snk/errors.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 snk-0.6.0/snk/main.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 snk-0.6.0/snk/nest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/config.py
+-rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/options.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/pipeline.py
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.0/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_nest.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/Snakefile
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.0/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.0/PKG-INFO
```

### Comparing `snk-0.5.0/snk/main.py` & `snk-0.6.0/snk/main.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/snk/nest.py` & `snk-0.6.0/snk/nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/snk/cli/config.py` & `snk-0.6.0/snk/cli/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,23 @@
             snk_config = cls(**snk_config_dict)
             snk_config.resources = [snk_config_path.parent / resource for resource in snk_config.resources]
             snk_config.validate_resources(snk_config.resources)
             return snk_config
         return cls()
     
     def validate_resources(self, resources):
+        """
+    Validate resources.
+    Args:
+      resources (List[Path]): List of resources to validate.
+    Raises:
+      FileNotFoundError: If a resource is not found.
+    Notes:
+      This function does not modify the resources list.
+    """
         for resource in resources:
             assert resource.exists(), FileNotFoundError(f"Could not find resource: {resource}")
 
     def add_resources(self, resources: List[Path], pipeline_dir_path: Path = None):
         """
         Add and validate resources. 
         It takes a list of resources, and if the resource is not absolute, it appends the
@@ -44,14 +53,23 @@
             if pipeline_dir_path and not resource.is_absolute():
                 resource = pipeline_dir_path / resource
             processed.append(resource)
         self.validate_resources(processed)
         self.resources.extend(processed)
 
     def to_yaml(self, path: Path) -> None:
+        """
+        Write SNK config to YAML file.
+        Args:
+            path (Path): Path to write the YAML file to.
+        Returns:
+            None
+        Side Effects:
+            Writes the SNK config to the specified path.
+        """
         with open(path, 'w') as f:
             yaml.dump(vars(self), f)
                              
     
 
 def get_config_from_pipeline_dir(pipeline_dir_path: Path):
     """Search possible config locations"""
```

### Comparing `snk-0.5.0/snk/cli/main.py` & `snk-0.6.0/snk/cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,28 +30,49 @@
         if part not in d:
             d[part] = dict()
         d = d[part]
     d[parts[-1]] = value
     return resultDict
 
 def serialise(d):
+    """
+    Serialises a data structure into a string.
+    Args:
+      d (any): The data structure to serialise.
+    Returns:
+      any: The serialised data structure.
+    Examples:
+      >>> serialise({'a': 1, 'b': 2})
+      {'a': '1', 'b': '2'}
+    """
     if isinstance(d, Path) or isinstance(d, datetime):
         return str(d)
 
     if isinstance(d, list):
         return [serialise(x) for x in d]
 
     if isinstance(d, dict):
         for k, v in d.items():
             d.update({k: serialise(v)})
 
     # return anything else, like a string or number
     return d
 
 def parse_config_args(args: List[str], options):
+    """
+    Parses a list of arguments and a list of options.
+    Args:
+      args (List[str]): A list of arguments.
+      options (List[dict]): A list of options.
+    Returns:
+      (List[str], List[dict]): A tuple of parsed arguments and config.
+    Examples:
+      >>> parse_config_args(['-name', 'John', '-age', '20'], [{'name': 'name', 'default': '', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'default': '', 'help': '', 'type': 'int', 'required': True}])
+      (['John', '20'], [{'name': 'name', 'John'}, {'age': 20}])
+    """
     names = [op['name'] for op in options]
     config = []
     parsed = []
     flag=None
     for arg in args:
         if flag:
             name = flag.lstrip('-')
@@ -72,14 +93,25 @@
             flag = arg
             continue
         parsed.append(arg)
     return parsed, config
 
 
 def build_dynamic_cli_options(snakemake_config, snk_config: SnkConfig):
+    """
+    Builds a list of options from a snakemake config and a snk config.
+    Args:
+      snakemake_config (dict): A snakemake config.
+      snk_config (SnkConfig): A snk config.
+    Returns:
+      List[dict]: A list of options.
+    Examples:
+      >>> build_dynamic_cli_options({'name': 'John', 'age': 20}, {'annotations': {'name:name': 'name', 'name:help': '', 'name:type': 'str', 'name:required': True, 'age:name': 'age', 'age:help': '', 'age:type': 'int', 'age:required': True}})
+      [{'name': 'name', 'original_key': 'name', 'default': 'John', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'original_key': 'age', 'default': 20, 'help': '', 'type': 'int', 'required': True}]
+    """
     flat_config = flatten(snakemake_config)
     options = []
     flat_snk_annotations = flatten(snk_config.annotations)
     for op in flat_config:
         name = flat_snk_annotations.get(f"{op}:name", op.replace(':', '_'))
         help = flat_snk_annotations.get(f"{op}:help", "")
         # TODO be smarter here 
@@ -98,14 +130,23 @@
             }
         )
     # TODO: find annotations missing from config and add them to options
     return options
 
 
 class CLI:
+    """
+    Constructor for the CLI class.
+    Args:
+      pipeline_dir_path (Path): Path to the pipeline directory.
+    Side Effects:
+      Initializes the CLI class.
+    Examples:
+      >>> CLI(Path('/path/to/pipeline'))
+    """
     def __init__(self, pipeline_dir_path: Path) -> None:
         self.pipeline = Pipeline(path=pipeline_dir_path)
         self.app = typer.Typer()
         self.snakemake_config = load_pipeline_snakemake_config(pipeline_dir_path)
         self.snk_config: SnkConfig = SnkConfig.from_path(pipeline_dir_path / '.snk')
         self.options = build_dynamic_cli_options(self.snakemake_config, self.snk_config)
         self.snakefile = self._find_snakefile()
@@ -144,50 +185,102 @@
                 "allow_extra_args": True, 
                 "ignore_unknown_options": True, 
                 "help_option_names": ["-h", "--help"]
             }
         )
 
     def __call__(self):
+        """
+    Invoke the CLI.
+    Side Effects:
+      Invokes the CLI.
+    Examples:
+      >>> CLI(Path('/path/to/pipeline'))()
+    """
         self.app()
 
     def register_command(self, command: Callable, **command_kwargs) -> None:
+        """
+    Register a command to the CLI.
+    Args:
+      command (Callable): The command to register.
+    Side Effects:
+      Registers the command to the CLI.
+    Examples:
+      >>> CLI.register_command(my_command)
+    """
         self.app.command(**command_kwargs)(command)
 
     def register_callback(self, command: Callable, **command_kwargs) -> None:
+        """
+    Register a callback to the CLI.
+    Args:
+      command (Callable): The callback to register.
+    Side Effects:
+      Registers the callback to the CLI.
+    Examples:
+      >>> CLI.register_callback(my_callback)
+    """
         self.app.callback(**command_kwargs)(command)
 
     def create_logo(self, font="small"):
+        """
+    Create a logo for the CLI.
+    Args:
+      font (str): The font to use for the logo.
+    Returns:
+      str: The logo.
+    Examples:
+      >>> CLI.create_logo()
+    """
         logo = text2art(self.name, font=font)        
         doc  = f"""\b{logo}\bA Snakemake pipeline CLI generated with snk"""
         return doc
 
     def _print_snakemake_help(value: bool):
+        """
+    Print the snakemake help and exit.
+    Args:
+      value (bool): If True, print the snakemake help and exit.
+    Side Effects:
+      Prints the snakemake help and exits.
+    Examples:
+      >>> CLI._print_snakemake_help(True)
+    """
         if value:
             snakemake.main("-h")
     
     def _find_snakefile(self):
-            """Search possible snakefile locations"""
+            """
+    Search possible snakefile locations.
+    Returns:
+      Path: The path to the snakefile.
+    Examples:
+      >>> CLI._find_snakefile()
+    """
             for path in snakemake.SNAKEFILE_CHOICES:
                 if (self.pipeline.path / path).exists():
                     return self.pipeline.path / path 
             raise FileNotFoundError("Snakefile not found!")
     
     @contextmanager
     def copy_resources(self, resources: List[Path], cleanup: bool):
         """
-        It copies the resources to the current working directory, and then removes them when the
-        function exits
-        
-        :param resources: A list of paths to the resources you want to copy
-        :type resources: List[Path]
-        :param cleanup_resources: If True, the resources will be removed after the test
-        :type cleanup_resources: bool
-        :return: A generator object.
-        """
+    Copy resources to the current working directory.
+    Args:
+      resources (List[Path]): A list of paths to the resources to copy.
+      cleanup (bool): If True, the resources will be removed after the function exits.
+    Side Effects:
+      Copies the resources to the current working directory.
+    Returns:
+      Generator: A generator object.
+    Examples:
+      >>> with CLI.copy_resources(resources, cleanup=True):
+      ...     # do something
+    """
         copied_resources = []
 
         def copy_resource(src, dst):
             if src.is_dir():
                 shutil.copytree(src, dst)
             else:
                 shutil.copy(src, dst)
@@ -230,14 +323,30 @@
             cleanup_snakemake: Optional[bool] = typer.Option(True, help="Delete .snakemake folder once the pipeline sucessfully completes."),
             cores:  int = typer.Option(None, help="Set the number of cores to use. If None will use all cores."),
             verbose: Optional[bool] = typer.Option(False, "--verbose", "-v", help="Run pipeline in verbose mode.",),
             help_snakemake: Optional[bool] = typer.Option(
                 False, "--help-snakemake", "-hs", help="Print the snakemake help and exit.", is_eager=True, callback=_print_snakemake_help, show_default=False
             ),
         ):
+        """
+    Run the pipeline.
+    Args:
+      target (str): File to generate. If None will run the pipeline 'all' rule.
+      configfile (Path): Path to snakemake config file. Overrides existing config and defaults.
+      resource (List[Path]): Additional resources to copy to workdir at run time.
+      cleanup_resources (bool): Delete resources once the pipeline sucessfully completes.
+      cleanup_snakemake (bool): Delete .snakemake folder once the pipeline sucessfully completes.
+      cores (int): Set the number of cores to use. If None will use all cores.
+      verbose (bool): Run pipeline in verbose mode.
+      help_snakemake (bool): Print the snakemake help and exit.
+    Side Effects:
+      Runs the pipeline.
+    Examples:
+      >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
+    """
         args = []
         if not cores:
             cores = 'all'
         args.extend([
             "--use-conda",
             f"--conda-prefix={self.conda_prefix_dir}",
             f"--cores={cores}",
@@ -282,34 +391,62 @@
         self.snk_config.add_resources(resource, self.pipeline.path)
         with self.copy_resources(self.snk_config.resources, cleanup=cleanup_resources):
                 snakemake.main(args)
         if cleanup_snakemake:
             shutil.rmtree(".snakemake")
 
     def info(self):
+        """
+    Display information about current pipeline install.
+    Returns:
+      str: A JSON string containing information about the current pipeline install.
+    Examples:
+      >>> CLI.info()
+    """
         import json
         info_dict = {}
         info_dict['name'] = self.pipeline.path.name
         info_dict['version'] = self.pipeline.version
         info_dict['pipeline_dir_path'] = str(self.pipeline.path)
         typer.echo(json.dumps(info_dict, indent=2))
 
     def config(self):
+        """
+    Access the pipeline configuration.
+    Side Effects:
+      Prints the pipeline configuration.
+    Examples:
+      >>> CLI.config()
+    """
         config_path = get_config_from_pipeline_dir(self.pipeline.path)
         if not config_path:
             typer.secho("Could not find config...", fg='red')
             raise typer.Exit(1)
         with open(config_path) as f:
             code = f.read()
             syntax = Syntax(code, 'yaml')
             console = Console()
             console.print(syntax)
     
     def env(
         name: Optional[str] = typer.Argument(None)
     ):
+        """
+    Access the pipeline conda environments.
+    Args:
+      name (str): The name of the environment.
+    Examples:
+      >>> CLI.env(name='my_env')
+    """
         raise NotImplementedError
 
     def script(
         name: Optional[str] = typer.Argument(None)
     ):
+        """
+    Access the pipeline scripts.
+    Args:
+      name (str): The name of the script.
+    Examples:
+      >>> CLI.script(name='my_script')
+    """
         raise NotImplementedError
```

### Comparing `snk-0.5.0/tests/.DS_Store` & `snk-0.6.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/conftest.py` & `snk-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/test_nest.py` & `snk-0.6.0/tests/test_nest.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/test_pipline_cli.py` & `snk-0.6.0/tests/test_pipline_cli.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/utils.py` & `snk-0.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/data/artic_v4.1.bed` & `snk-0.6.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/data/config.yaml` & `snk-0.6.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/tests/data/cov.fasta` & `snk-0.6.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/LICENSE.txt` & `snk-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.5.0/README.md` & `snk-0.6.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+---
+title: Home
+---
 # snk
 
 [![PyPI - Version](https://img.shields.io/pypi/v/snk.svg)](https://pypi.org/project/snk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snk.svg)](https://pypi.org/project/snk)
-
+[![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [About](#about)
 - [License](#license)
```

### Comparing `snk-0.5.0/pyproject.toml` & `snk-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 [tool.hatch.version]
 path = "snk/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
+  "write-the",
+  "openai"
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=snk --cov=tests"
 test = "cov --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
```

### Comparing `snk-0.5.0/PKG-INFO` & `snk-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.5.0
+Version: 0.6.0
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # snk
 
 [![PyPI - Version](https://img.shields.io/pypi/v/snk.svg)](https://pypi.org/project/snk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/snk.svg)](https://pypi.org/project/snk)
-
+[![write-the - docs](https://badgen.net/badge/write-the/docs/blue?icon=https://raw.githubusercontent.com/Wytamma/write-the/master/images/write-the-icon.svg)](https://write-the.wytamma.com/)
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [About](#about)
 - [License](#license)
```

