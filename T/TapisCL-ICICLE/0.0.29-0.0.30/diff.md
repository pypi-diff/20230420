# Comparing `tmp/TapisCL-ICICLE-0.0.29.tar.gz` & `tmp/TapisCL-ICICLE-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.29.tar", last modified: Wed Apr 19 04:52:39 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.30.tar", last modified: Thu Apr 20 00:23:50 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.29.tar` & `TapisCL-ICICLE-0.0.30.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.517221 TapisCL-ICICLE-0.0.29/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/LICENSE
--rw-rw-rw-   0        0        0    44210 2023-04-19 04:52:39.516220 TapisCL-ICICLE-0.0.29/PKG-INFO
--rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.29/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.509058 TapisCL-ICICLE-0.0.29/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10959 2023-04-19 04:50:36.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     9161 2023-04-19 04:39:15.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5592 2023-04-19 04:46:55.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10424 2023-04-19 04:49:26.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    19567 2023-04-19 04:33:11.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.515224 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-04-19 04:51:53.000000 TapisCL-ICICLE-0.0.29/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 04:52:39.517221 TapisCL-ICICLE-0.0.29/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.385810 TapisCL-ICICLE-0.0.30/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/LICENSE
+-rw-rw-rw-   0        0        0    44210 2023-04-20 00:23:50.384784 TapisCL-ICICLE-0.0.30/PKG-INFO
+-rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.30/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.371774 TapisCL-ICICLE-0.0.30/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    11005 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     9563 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5620 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     2059 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10588 2023-04-20 00:11:27.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    19567 2023-04-19 04:33:11.000000 TapisCL-ICICLE-0.0.30/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:23:50.383781 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-20 00:23:50.000000 TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-04-20 00:22:41.000000 TapisCL-ICICLE-0.0.30/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 00:23:50.385810 TapisCL-ICICLE-0.0.30/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.29/LICENSE` & `TapisCL-ICICLE-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/PKG-INFO` & `TapisCL-ICICLE-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.29
+Version: 0.0.30
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.29/README.md` & `TapisCL-ICICLE-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,19 @@
             if response.schema_type == 'FormRequest' and not response.arguments_list:
                 form = self.expression_input()
                 filled_form = schemas.FormResponse(arguments_list=form)
             elif response.schema_type == 'FormRequest':
                 form = self.fillout_form(response.arguments_list)
                 filled_form = schemas.FormResponse(arguments_list=form)
             elif response.schema_type == 'AuthRequest':
-                if not response.secure_input:
-                    username = input("Username: ")
+                if response.secure_input or not response.requires_username:
+                    username = self.username
                     password = getpass("Password: ")
-                else:
-                    username = None
+                else: 
+                    username = input("Username: ")
                     password = getpass("Password: ")
                 filled_form = schemas.AuthData(username=username, password=password)
             elif response.schema_type == "ConfirmationRequest":
                 print(response.message)
                 while True:
                     decision = str(input("(y/n)"))
                     if decision == 'y':
@@ -221,15 +221,15 @@
             command = self.command_operator(kwargs, exit_=1) # operate with args, send them over
             self.json_send(command.dict())
             response = self.special_forms_ops()
             if response.schema_type == 'ResponseData':
                 self.print_response(response.response_message)
             os._exit(0)
 
-        title = pyfiglet.figlet_format("---------\nTapiconsole\n---------", font="slant") # print the title when CLI is accessed
+        title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
         print(title)
         
         while True: # open the CLI if no arguments provided on startup
             try:
                 time.sleep(0.01)
                 kwargs = self.process_command(str(input(f"[{self.username}@{self.url}] "))) # ask for and process user input
                 try:
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,24 +107,31 @@
 
 class Auth(BaseRequirementDecorator):
     """
     used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
     the client, and checks those credentials against the stored credentials in the server.
     """
     def __call__(self, obj, *args, **kwargs):
+        no_username = False
         if BaseRequirementDecorator.connection:
             if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
                 return self.function(obj, **kwargs)
             fields = list(helpers.get_parameters(self.function))
-            auth_request = schemas.AuthRequest()
+            if kwargs['username']:
+                no_username = True
+                auth_request = schemas.AuthRequest(requires_username=False)
+            else:
+                auth_request = schemas.AuthRequest()
             self.json_send_explicit(BaseRequirementDecorator.connection, auth_request.dict())
             auth_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
-            if 'username' in fields and 'password' in fields:
+            if 'username' in fields and 'password' in fields and not no_username:
                 kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
                 return self.function(obj, **kwargs)
+            elif 'password' in fields and no_username:
+                kwargs['password'] = auth_data.password
             username, password = auth_data.username, auth_data.password
             if username != BaseRequirementDecorator.username:
                 raise exceptions.InvalidCredentialsReceived(self.function, 'username')
             elif password != BaseRequirementDecorator.password:    
                 raise exceptions.InvalidCredentialsReceived(self.function, 'password')
 
         return self.function(obj, **kwargs)
@@ -180,15 +187,17 @@
         while True:
             for frame in self.animation_frames:
                 sys.stdout.write(f'\rloading ' + frame)
                 sys.stdout.flush()
                 time.sleep(0.5)
     
     def __call__(self, obj, *args, **kwargs):
-        if BaseRequirementDecorator.username:
+        if not BaseRequirementDecorator.username:
             animation_thread = helpers.KillableThread(target=self.animation)
             animation_thread.start()
             result = self.function(obj, *args, **kwargs)
+            sys.stdout.flush()
             animation_thread.kill()
+            sys.stdout.flush()
         else:
             result = self.function(obj, *args, **kwargs)
         return result
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,16 @@
                 self.recursive_dict_print(value, depth=depth + 1)
             elif isinstance(value, (list, tuple, set)):
                 print(("  " * depth) + f"{key}:")
                 for data in value:
                     print(("  " * (depth + 1)) + data)
             else: 
                 print(("  " * depth) + f"{key}: {str(value).strip()}")
-        print("\n")
+        if depth == 1:
+            print("\n")
 
 
 if __name__ == "__main__":
     class Silly:
         def z(self, y=True, x=False):
             return None
     x = OperationsHelper()
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 class AuthRequest(BaseModel):
     """
     Request auth credentials from the client
     """
     schema_type: str = 'AuthRequest'
+    requires_username: bool = True
     secure_input: bool = False
 
 
 class ConfirmationRequest(BaseModel):
     """
     ask the client for confirmation to carry out an action
     """
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 try:
     from . import exceptions
     from . import socketOpts as SO
     from . import helpers
     from . import schemas
     from . import decorators
+    from . import args
 except:
     import exceptions
     import socketOpts as SO
     import helpers
     import schemas
     import decorators
+    import args
 
 class Server(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
     """
     Receives commands from the client and executes Tapis operations
     """
     def __init__(self, IP: str, PORT: int):
         # logger setup
@@ -202,17 +204,19 @@
         checks if the timeout has been exceeded
         """
         if time.time() > self.end_time: 
             raise exceptions.TimeoutError
 
     def help(self, command: str):
         """
-        @help: returns help information. To get specific help information for tapis services, you can run <service> -c help
+        @help: returns help information. To get specific help information for tapis services, you can run <service> -c help. enter -c args to see detailed command usage
         """
-        if command in self.help:
+        if command == "args":
+            return args.Args.argparser_args
+        elif command in self.help:
             return self.help[command]
         return self.help
 
     def run_command(self, command_data: dict):
         """
         process and run command based on received kwargs
         """
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.30/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.29
+Version: 0.0.30
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.30/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.29/pyproject.toml` & `TapisCL-ICICLE-0.0.30/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.29"
+version = "0.0.30"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

