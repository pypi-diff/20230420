# Comparing `tmp/pulumi_aws_static_website-0.3.0.tar.gz` & `tmp/pulumi_aws_static_website-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aws_static_website-0.3.0.tar", last modified: Thu Jan 26 21:32:26 2023, max compression
+gzip compressed data, was "pulumi_aws_static_website-0.4.0.tar", last modified: Thu Apr 20 00:01:08 2023, max compression
```

## Comparing `pulumi_aws_static_website-0.3.0.tar` & `pulumi_aws_static_website-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:32:26.190485 pulumi_aws_static_website-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-01-26 21:32:26.190485 pulumi_aws_static_website-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:32:26.190485 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/
--rw-------   0 runner    (1001) docker     (123)      717 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/__init__.py
--rw-------   0 runner    (1001) docker     (123)     4196 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     7647 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     2817 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/provider.py
--rw-------   0 runner    (1001) docker     (123)       55 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/py.typed
--rw-------   0 runner    (1001) docker     (123)    17932 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/website.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 21:32:26.190485 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-26 21:32:26.000000 pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 21:32:26.190485 pulumi_aws_static_website-0.3.0/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2179 2023-01-26 21:32:25.000000 pulumi_aws_static_website-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:01:08.706551 pulumi_aws_static_website-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 00:01:08.706551 pulumi_aws_static_website-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:01:08.706551 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/
+-rw-------   0 runner    (1001) docker     (123)      825 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     4208 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     8061 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     2766 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/provider.py
+-rw-------   0 runner    (1001) docker     (123)     4535 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/public_bucket_policy.py
+-rw-------   0 runner    (1001) docker     (123)       55 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/py.typed
+-rw-------   0 runner    (1001) docker     (123)    17881 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:01:08.706551 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:01:08.706551 pulumi_aws_static_website-0.4.0/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2210 2023-04-20 00:01:08.000000 pulumi_aws_static_website-0.4.0/setup.py
```

### Comparing `pulumi_aws_static_website-0.3.0/PKG-INFO` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_aws_static_website
-Version: 0.3.0
+Name: pulumi-aws-static-website
+Version: 0.4.0
 Summary: A Pulumi component to deploy a static website to AWS
 Home-page: https://pulumi.com
 License: UNKNOWN
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-static-website
 Keywords: pulumi aws category/cloud kind/component web
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi AWS Static Website Component
 
 This component makes it easy to deploy a static website to s3 along with an optional CloudFront distribution using any of the supported Pulumi programming languages including markup languages like YAML and JSON.
 
 ## Example Usage
```

### Comparing `pulumi_aws_static_website-0.3.0/README.md` & `pulumi_aws_static_website-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/__init__.py` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .provider import *
+from .public_bucket_policy import *
 from .website import *
 from ._inputs import *
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "aws-static-website",
   "mod": "index",
   "fqn": "pulumi_aws_static_website",
   "classes": {
+   "aws-static-website:index:PublicBucketPolicy": "PublicBucketPolicy",
    "aws-static-website:index:Website": "Website"
   }
  }
 ]
 """,
     resource_packages="""
 [
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/_inputs.py` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 import pulumi_aws
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/_utilities.py` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +241,10 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/provider.py` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -50,20 +51,17 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
         super(Provider, __self__).__init__(
             'aws-static-website',
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website/website.py` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website/website.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 import pulumi_aws
@@ -297,20 +298,17 @@
                  price_class: Optional[pulumi.Input[str]] = None,
                  site_path: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  target_domain: Optional[pulumi.Input[str]] = None,
                  with_cdn: Optional[pulumi.Input[bool]] = None,
                  with_logs: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = WebsiteArgs.__new__(WebsiteArgs)
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/PKG-INFO` & `pulumi_aws_static_website-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-aws-static-website
-Version: 0.3.0
+Name: pulumi_aws_static_website
+Version: 0.4.0
 Summary: A Pulumi component to deploy a static website to AWS
 Home-page: https://pulumi.com
 License: UNKNOWN
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-static-website
 Keywords: pulumi aws category/cloud kind/component web
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pulumi AWS Static Website Component
 
 This component makes it easy to deploy a static website to s3 along with an optional CloudFront distribution using any of the supported Pulumi programming languages including markup languages like YAML and JSON.
 
 ## Example Usage
```

### Comparing `pulumi_aws_static_website-0.3.0/pulumi_aws_static_website.egg-info/SOURCES.txt` & `pulumi_aws_static_website-0.4.0/pulumi_aws_static_website.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 pulumi_aws_static_website/__init__.py
 pulumi_aws_static_website/_inputs.py
 pulumi_aws_static_website/_utilities.py
 pulumi_aws_static_website/provider.py
+pulumi_aws_static_website/public_bucket_policy.py
 pulumi_aws_static_website/pulumi-plugin.json
 pulumi_aws_static_website/py.typed
 pulumi_aws_static_website/website.py
 pulumi_aws_static_website.egg-info/PKG-INFO
 pulumi_aws_static_website.egg-info/SOURCES.txt
 pulumi_aws_static_website.egg-info/dependency_links.txt
 pulumi_aws_static_website.egg-info/not-zip-safe
```

### Comparing `pulumi_aws_static_website-0.3.0/setup.py` & `pulumi_aws_static_website-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.3.0"
-PLUGIN_VERSION = "0.3.0"
+VERSION = "0.4.0"
+PLUGIN_VERSION = "0.4.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'aws-static-website', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "aws-static-website Pulumi Package - Development Version"
 
 
 setup(name='pulumi_aws_static_website',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi component to deploy a static website to AWS",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

