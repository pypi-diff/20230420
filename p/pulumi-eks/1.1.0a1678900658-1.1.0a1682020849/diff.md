# Comparing `tmp/pulumi_eks-1.1.0a1678900658.tar.gz` & `tmp/pulumi_eks-1.1.0a1682020849.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-1.1.0a1678900658.tar", last modified: Wed Mar 15 17:23:33 2023, max compression
+gzip compressed data, was "pulumi_eks-1.1.0a1682020849.tar", last modified: Thu Apr 20 20:07:52 2023, max compression
```

## Comparing `pulumi_eks-1.1.0a1678900658.tar` & `pulumi_eks-1.1.0a1682020849.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:23:33.253365 pulumi_eks-1.1.0a1678900658/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-15 17:23:33.253365 pulumi_eks-1.1.0a1678900658/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:23:33.253365 pulumi_eks-1.1.0a1678900658/pulumi_eks/
--rw-------   0 runner    (1001) docker     (123)     1150 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (123)    84174 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     7641 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (123)    90165 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (123)     4911 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (123)    30269 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (123)    45902 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (123)     8456 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (123)    48814 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (123)    38594 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (123)     2766 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (123)       40 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (123)    37707 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:23:33.253365 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-15 17:23:33.000000 pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 17:23:33.253365 pulumi_eks-1.1.0a1678900658/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2144 2023-03-15 17:23:32.000000 pulumi_eks-1.1.0a1678900658/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:07:52.458609 pulumi_eks-1.1.0a1682020849/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-20 20:07:52.458609 pulumi_eks-1.1.0a1682020849/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:07:52.458609 pulumi_eks-1.1.0a1682020849/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (123)     1150 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    84186 2023-04-20 20:07:51.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     8055 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)    90114 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (123)     4860 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (123)    30218 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (123)    45851 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (123)     8405 2023-04-20 20:07:51.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (123)    48763 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (123)    38606 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (123)     2715 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (123)       40 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (123)    37656 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:07:52.458609 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:07:52.458609 pulumi_eks-1.1.0a1682020849/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2175 2023-04-20 20:07:52.000000 pulumi_eks-1.1.0a1682020849/setup.py
```

### Comparing `pulumi_eks-1.1.0a1678900658/PKG-INFO` & `pulumi_eks-1.1.0a1682020849/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 1.1.0a1678900658
+Version: 1.1.0a1682020849
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![npm version](https://badge.fury.io/js/@pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks)
@@ -81,8 +81,9 @@
         Please follow the [code of conduct][code-of-conduct].
         
         [contributing]: CONTRIBUTING.md
         [code-of-conduct]: CODE-OF-CONDUCT.md
         
 Keywords: pulumi aws eks
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 1.1.0a1678900658 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 1.1.0a1682020849 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. Home-page: https://pulumi.com
 License: Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-
 eks Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml) [![Slack](http://www.pulumi.com/images/docs/badges/
 slack.svg)](https://slack.pulumi.com) [![npm version](https://badge.fury.io/js/
 @pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks) [![Python version]
@@ -32,9 +32,9 @@
 www.pulumi.com/blog/easily-create-and-manage-aws-eks-kubernetes-clusters-with-
 pulumi/) * [Reference Documentation](https://www.pulumi.com/registry/packages/
 eks/api-docs/) * [Examples](./examples) * [Crosswalk for AWS - EKS Guide]
 (https://www.pulumi.com/docs/guides/crosswalk/aws/eks/) ## Contributing If you
 are interested in contributing, please see the [contributing docs]
 [contributing]. ## Code of Conduct Please follow the [code of conduct][code-of-
 conduct]. [contributing]: CONTRIBUTING.md [code-of-conduct]: CODE-OF-CONDUCT.md
-Keywords: pulumi aws eks Platform: UNKNOWN Description-Content-Type: text/
-markdown
+Keywords: pulumi aws eks Platform: UNKNOWN Requires-Python: >=3.7 Description-
+Content-Type: text/markdown
```

### Comparing `pulumi_eks-1.1.0a1678900658/README.md` & `pulumi_eks-1.1.0a1682020849/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/__init__.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/_inputs.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from .vpc_cni import VpcCni
 import pulumi_aws
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/_utilities.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/_utilities.py`

 * *Files 10% similar despite different names*

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

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/cluster.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -1260,20 +1261,17 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  use_default_vpc_cni: Optional[bool] = None,
                  user_mappings: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['UserMappingArgs']]]]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  vpc_cni_options: Optional[pulumi.InputType['VpcCniOptionsArgs']] = None,
                  vpc_id: Optional[pulumi.Input[str]] = None,
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
             __props__ = ClusterArgs.__new__(ClusterArgs)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/cluster_creation_role_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 import pulumi_aws
 
@@ -80,20 +81,17 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  profile: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
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
             __props__ = ClusterCreationRoleProviderArgs.__new__(ClusterCreationRoleProviderArgs)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/managed_node_group.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/managed_node_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 from .cluster import Cluster
@@ -484,20 +485,17 @@
                  remote_access: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupRemoteAccessArgs']]] = None,
                  scaling_config: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupScalingConfigArgs']]] = None,
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupTaintArgs']]]]] = None,
                  version: Optional[pulumi.Input[str]] = None,
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
             __props__ = ManagedNodeGroupArgs.__new__(ManagedNodeGroupArgs)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 from .cluster import Cluster
@@ -707,20 +708,17 @@
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
                  node_user_data_override: Optional[pulumi.Input[str]] = None,
                  spot_price: Optional[pulumi.Input[str]] = None,
                  taints: Optional[Mapping[str, pulumi.InputType['TaintArgs']]] = None,
                  version: Optional[pulumi.Input[str]] = None,
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
             __props__ = NodeGroupArgs.__new__(NodeGroupArgs)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group_security_group.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group_security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 import pulumi_aws
 
@@ -125,20 +126,17 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_security_group: Optional[pulumi.Input['pulumi_aws.ec2.SecurityGroup']] = None,
                  eks_cluster: Optional[pulumi.Input['pulumi_aws.eks.Cluster']] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  vpc_id: Optional[pulumi.Input[str]] = None,
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
             __props__ = NodeGroupSecurityGroupArgs.__new__(NodeGroupSecurityGroupArgs)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/node_group_v2.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/node_group_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from ._inputs import *
 from .cluster import Cluster
@@ -745,20 +746,17 @@
                  node_subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_user_data: Optional[pulumi.Input[str]] = None,
                  node_user_data_override: Optional[pulumi.Input[str]] = None,
                  spot_price: Optional[pulumi.Input[str]] = None,
                  taints: Optional[Mapping[str, pulumi.InputType['TaintArgs']]] = None,
                  version: Optional[pulumi.Input[str]] = None,
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
             __props__ = NodeGroupV2Args.__new__(NodeGroupV2Args)
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/outputs.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from .vpc_cni import VpcCni
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/provider.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
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
             'eks',
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks/vpc_cni.py` & `pulumi_eks-1.1.0a1682020849/pulumi_eks/vpc_cni.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-eks. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['VpcCniArgs', 'VpcCni']
@@ -546,20 +547,17 @@
                  node_port_support: Optional[pulumi.Input[bool]] = None,
                  security_context_privileged: Optional[pulumi.Input[bool]] = None,
                  veth_prefix: Optional[pulumi.Input[str]] = None,
                  warm_eni_target: Optional[pulumi.Input[int]] = None,
                  warm_ip_target: Optional[pulumi.Input[int]] = None,
                  warm_prefix_target: Optional[pulumi.Input[int]] = None,
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
             __props__ = VpcCniArgs.__new__(VpcCniArgs)
 
             __props__.__dict__["cni_configure_rpfilter"] = cni_configure_rpfilter
             __props__.__dict__["cni_custom_network_cfg"] = cni_custom_network_cfg
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-eks
-Version: 1.1.0a1678900658
+Version: 1.1.0a1682020849
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![npm version](https://badge.fury.io/js/@pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks)
@@ -81,8 +81,9 @@
         Please follow the [code of conduct][code-of-conduct].
         
         [contributing]: CONTRIBUTING.md
         [code-of-conduct]: CODE-OF-CONDUCT.md
         
 Keywords: pulumi aws eks
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-eks Version: 1.1.0a1678900658 Summary:
+Metadata-Version: 2.1 Name: pulumi-eks Version: 1.1.0a1682020849 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. Home-page: https://pulumi.com
 License: Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-
 eks Description: [![Build Status](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml/badge.svg)](https://github.com/pulumi/pulumi-eks/actions/
 workflows/master.yml) [![Slack](http://www.pulumi.com/images/docs/badges/
 slack.svg)](https://slack.pulumi.com) [![npm version](https://badge.fury.io/js/
 @pulumi%2Feks.svg)](https://badge.fury.io/js/@pulumi%2Feks) [![Python version]
@@ -32,9 +32,9 @@
 www.pulumi.com/blog/easily-create-and-manage-aws-eks-kubernetes-clusters-with-
 pulumi/) * [Reference Documentation](https://www.pulumi.com/registry/packages/
 eks/api-docs/) * [Examples](./examples) * [Crosswalk for AWS - EKS Guide]
 (https://www.pulumi.com/docs/guides/crosswalk/aws/eks/) ## Contributing If you
 are interested in contributing, please see the [contributing docs]
 [contributing]. ## Code of Conduct Please follow the [code of conduct][code-of-
 conduct]. [contributing]: CONTRIBUTING.md [code-of-conduct]: CODE-OF-CONDUCT.md
-Keywords: pulumi aws eks Platform: UNKNOWN Description-Content-Type: text/
-markdown
+Keywords: pulumi aws eks Platform: UNKNOWN Requires-Python: >=3.7 Description-
+Content-Type: text/markdown
```

### Comparing `pulumi_eks-1.1.0a1678900658/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-1.1.0a1682020849/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-1.1.0a1678900658/setup.py` & `pulumi_eks-1.1.0a1682020849/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.0a1678900658"
-PLUGIN_VERSION = "1.1.0-alpha.1678900658+cf16a765"
+VERSION = "1.1.0a1682020849"
+PLUGIN_VERSION = "1.1.0-alpha.1682020849+210d6b17"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'eks', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "eks Pulumi Package - Development Version"
 
 
 setup(name='pulumi_eks',
+      python_requires='>=3.7',
       version=VERSION,
       description="Pulumi Amazon Web Services (AWS) EKS Components.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

