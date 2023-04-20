# Comparing `tmp/tmctl-0.1.0.tar.gz` & `tmp/tmctl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmctl-0.1.0.tar", last modified: Thu Apr 13 08:35:17 2023, max compression
+gzip compressed data, was "tmctl-0.2.0.tar", last modified: Thu Apr 20 09:44:12 2023, max compression
```

## Comparing `tmctl-0.1.0.tar` & `tmctl-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.691391 tmctl-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 08:35:17.691391 tmctl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:35:17.691391 tmctl-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 08:35:03.000000 tmctl-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.687390 tmctl-0.1.0/tmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27802 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-13 08:35:03.000000 tmctl-0.1.0/tmctl/tmctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:35:17.691391 tmctl-0.1.0/tmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 08:35:17.000000 tmctl-0.1.0/tmctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 09:44:12.042519 tmctl-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:44:12.042519 tmctl-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-20 09:43:51.000000 tmctl-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/tmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/tmctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/tmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/top_level.txt
```

### Comparing `tmctl-0.1.0/tmctl/controller.py` & `tmctl-0.2.0/tmctl/controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -271,15 +271,15 @@
                                     "target_path": target_path,
                                 },
                             )
 
                         if response.status:
                             self.print(response.data)
                         else:
-                            logging.warning("catalog submit failed")
+                            logging.warning("file submit failed")
 
 
 class Catalog(AdminClient):
     def __init__(self, common_option: CommonOption):
         super(Catalog, self).__init__(common_option, "/v1/catalogs")
 
     def list(self):
@@ -361,14 +361,15 @@
                 cluster = clusters[0]
                 health_check = self._health_check_status(cluster["id"])
 
                 if health_check:
                     if force:
                         self.off(name=name, refresh=refresh, timeout=timeout)
                     else:
+                        print("Cluster is on. please off the cluster first.")
                         logging.warning("Cluster is on. please off the cluster first.")
                         return
 
             super().delete(name)
 
     def _health_check_status(self, cluster_id):
         response = self._send_get(f"/v1/clusters/{cluster_id}/gateway/health")
@@ -817,7 +818,141 @@
                             },
                         )
 
                         if response.status:
                             self.print(response.data[0])
                         else:
                             logging.warning("chart submit failed")
+
+
+class MountFile(AdminClient):
+    def __init__(self, url):
+        super(MountFile, self).__init__(url, "/v1/mounts")
+
+    def get(self, mount_path):
+        response = self._send_get(f"{self._base_url}", {"mount_path": mount_path})
+
+        if response.status:
+            for each in response.data:
+                self.print(each)
+
+    def delete(self, mount_path: str, model_id: int = None):
+        delete_response = None
+        identifier = model_id or mount_path
+        return_value = None
+
+        if model_id:
+            delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+        elif mount_path:
+            response = self._send_get(
+                f"{self._base_url}", params={"mount_path": mount_path}
+            )
+
+            if response.status:
+                models = response.data
+                if models:
+                    model = models[0]
+
+                    model_id = model["id"]
+
+                    delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+
+        if delete_response:
+            return_value = f"identifier: {identifier} is successfully deleted!"
+        else:
+            return_value = f"identifier: {identifier} does not be successfully deleted!"
+
+        return return_value
+
+    def download(self, mount_path, path=None):
+        path = path or "./"
+        response = self._send_get(f"{self._base_url}", {"mount_path": mount_path})
+
+        if response.status:
+            mount_file = response.data[0]
+
+            binary = self._send_download(
+                f"{self._base_url}/{mount_file['id']}/download"
+            )
+
+            if binary:
+                file_path = os.path.join(path, mount_file["file_name"])
+                with open(file_path, "wb") as _f:
+                    _f.write(binary)
+
+                self.print("download success.")
+            else:
+                self.print("empty binary")
+        else:
+            self.print("cannot download file")
+
+    def submit(self, path):
+        yamls = self._yaml_load_all(path)
+
+        for each in yamls:
+            version = each.get("version", None)
+            action_type = each.get("type", None)
+
+            if version in ["v1/mount"]:
+                file_config = each.get("mount", None) or {}
+                source_path = file_config.get("source_path", None)
+                mount_path = file_config.get("mount_path", None)
+                target_path = file_config.get("target_path", None)
+                refresh = file_config.get("refresh", None) or False
+
+                if not refresh:
+                    if not source_path:
+                        print("invalid path", source_path)
+                        break
+
+                    file_exists = os.path.exists(source_path)
+
+                    if not file_exists:
+                        print("invalid currnet source fil path", source_path)
+                        break
+
+                    if not mount_path:
+                        print("invalid mount_path", mount_path)
+                        break
+
+                if action_type == "create":
+                    response = None
+                    if refresh:
+                        response = self._send_post(
+                            "/v1/mounts",
+                            form_data={
+                                "mount_path": mount_path,
+                                "target_path": target_path,
+                                "refresh": True,
+                            },
+                        )
+                    else:
+                        response = self._send_binary_post(
+                            "/v1/mounts",
+                            source_path,
+                            form_data={
+                                "mount_path": mount_path,
+                                "target_path": target_path,
+                            },
+                        )
+
+                    if response.status:
+                        self.print(response.data)
+                    else:
+                        logging.warning("mount file create failed")
+                elif action_type == "update":
+                    mount_file_id = file_config.get("id", None)
+
+                    if mount_file_id:
+                        response = self._send_binary_post(
+                            f"/v1/mounts/{mount_file_id}",
+                            source_path,
+                            form_data={
+                                "mount_path": mount_path,
+                                "target_path": target_path,
+                            },
+                        )
+
+                        if response.status:
+                            self.print(response.data)
+                        else:
+                            logging.warning("mount file update failed")
```

### Comparing `tmctl-0.1.0/tmctl/tmctl.py` & `tmctl-0.2.0/tmctl/tmctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 import fire
 import logging
 import yaml
 
-from .controller import CommonOption, Catalog, Cluster, File, HelmChart
+from .controller import CommonOption, Catalog, Cluster, File, HelmChart, MountFile
 
 
 class TMCtl(object):
     """Class Documentation"""
 
     def __init__(
         self, url=None, output=None, indent=4, log_level="WARNING", verbose=False
@@ -22,14 +22,15 @@
 
         common_option = CommonOption(admin_url=admin_url, output=output, indent=indent)
 
         self.catalog = Catalog(common_option)
         self.cluster = Cluster(common_option)
         self.helm_chart = HelmChart(common_option)
         self.file = File(common_option)
+        self.mount = MountFile(common_option)
 
         log_config = self._config.get("logging", None) or {}
         self._init_logging(log_config, log_level, verbose)
 
     def _init_config(self):
         config = None
         try:
```

