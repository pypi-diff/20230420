# Comparing `tmp/digocli-0.0.2.tar.gz` & `tmp/digocli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digocli-0.0.2.tar", last modified: Thu Apr 20 11:51:57 2023, max compression
+gzip compressed data, was "digocli-0.0.3.tar", last modified: Thu Apr 20 11:54:29 2023, max compression
```

## Comparing `digocli-0.0.2.tar` & `digocli-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.656442 digocli-0.0.2/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1432 2023-04-20 11:51:57.656145 digocli-0.0.2/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 digocli-0.0.2/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.632360 digocli-0.0.2/digocli.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1432 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1396 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       47 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       79 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-20 11:51:57.000000 digocli-0.0.2/digocli.egg-info/top_level.txt
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.634044 digocli-0.0.2/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 digocli-0.0.2/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 digocli-0.0.2/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.635396 digocli-0.0.2/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 digocli-0.0.2/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-20 11:51:49.000000 digocli-0.0.2/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.635912 digocli-0.0.2/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 digocli-0.0.2/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.636905 digocli-0.0.2/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        7 2023-04-14 08:49:35.000000 digocli-0.0.2/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.638214 digocli-0.0.2/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 digocli-0.0.2/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 digocli-0.0.2/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2529 2023-04-20 11:50:51.000000 digocli-0.0.2/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.644611 digocli-0.0.2/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 digocli-0.0.2/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      770 2023-04-18 03:48:11.000000 digocli-0.0.2/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      422 2023-04-18 03:48:11.000000 digocli-0.0.2/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      358 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      366 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 digocli-0.0.2/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.646232 digocli-0.0.2/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 digocli-0.0.2/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      897 2023-04-20 07:03:15.000000 digocli-0.0.2/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 digocli-0.0.2/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.652234 digocli-0.0.2/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      111 2023-04-18 03:48:11.000000 digocli-0.0.2/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 digocli-0.0.2/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2842 2023-04-20 11:36:51.000000 digocli-0.0.2/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       29 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/query_meta_info.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       41 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 digocli-0.0.2/openxlab/model/handler/update_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.653300 digocli-0.0.2/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 digocli-0.0.2/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 digocli-0.0.2/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.654726 digocli-0.0.2/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 digocli-0.0.2/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 digocli-0.0.2/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:51:57.655398 digocli-0.0.2/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 digocli-0.0.2/openxlab/xlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 digocli-0.0.2/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 11:51:57.656548 digocli-0.0.2/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1170 2023-04-20 10:36:44.000000 digocli-0.0.2/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.958324 digocli-0.0.3/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1432 2023-04-20 11:54:29.958047 digocli-0.0.3/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 digocli-0.0.3/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.946121 digocli-0.0.3/digocli.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1432 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1396 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       47 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       79 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-20 11:54:29.000000 digocli-0.0.3/digocli.egg-info/top_level.txt
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.946668 digocli-0.0.3/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 digocli-0.0.3/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 digocli-0.0.3/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.947150 digocli-0.0.3/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 digocli-0.0.3/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-20 11:54:13.000000 digocli-0.0.3/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.947430 digocli-0.0.3/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 digocli-0.0.3/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.947875 digocli-0.0.3/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        7 2023-04-14 08:49:35.000000 digocli-0.0.3/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.949013 digocli-0.0.3/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 digocli-0.0.3/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 digocli-0.0.3/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2473 2023-04-20 11:54:06.000000 digocli-0.0.3/openxlab/model/clients/openapi_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.951661 digocli-0.0.3/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 digocli-0.0.3/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      770 2023-04-18 03:48:11.000000 digocli-0.0.3/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      422 2023-04-18 03:48:11.000000 digocli-0.0.3/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      358 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      366 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      390 2023-04-14 09:06:08.000000 digocli-0.0.3/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.952595 digocli-0.0.3/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 digocli-0.0.3/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      897 2023-04-20 07:03:15.000000 digocli-0.0.3/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 digocli-0.0.3/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.955895 digocli-0.0.3/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      111 2023-04-18 03:48:11.000000 digocli-0.0.3/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 digocli-0.0.3/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2842 2023-04-20 11:36:51.000000 digocli-0.0.3/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       29 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/query_meta_info.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       41 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       32 2023-04-13 03:08:33.000000 digocli-0.0.3/openxlab/model/handler/update_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.956504 digocli-0.0.3/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 digocli-0.0.3/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 digocli-0.0.3/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.957227 digocli-0.0.3/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 digocli-0.0.3/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 digocli-0.0.3/openxlab/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-20 11:54:29.957610 digocli-0.0.3/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 digocli-0.0.3/openxlab/xlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 digocli-0.0.3/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-20 11:54:29.958424 digocli-0.0.3/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1170 2023-04-20 10:36:44.000000 digocli-0.0.3/setup.py
```

### Comparing `digocli-0.0.2/PKG-INFO` & `digocli-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digocli
-Version: 0.0.2
+Version: 0.0.3
 Summary: digocli
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `digocli-0.0.2/README.md` & `digocli-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/digocli.egg-info/PKG-INFO` & `digocli-0.0.3/digocli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digocli
-Version: 0.0.2
+Version: 0.0.3
 Summary: digocli
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `digocli-0.0.2/digocli.egg-info/SOURCES.txt` & `digocli-0.0.3/digocli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/cli.py` & `digocli-0.0.3/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/demo_cmd/__init__.py` & `digocli-0.0.3/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/model/clients/openapi_client.py` & `digocli-0.0.3/openxlab/model/clients/openapi_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         """
         get file(model file|meta file|log file|readme file) download url
         """
         client_from = os.environ.get('CLIENT_FROM', '0')
         payload = {"repositoryName": repository, "fileName": file, "clientFrom": client_from}
         path = paths['file_download_path']
         response_dto = self.http_post_response_dto(path, payload)
-        print(f"response_dto.data:{response_dto.data}")
         if response_dto.msg_code != '10000':
             raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
         if response_dto.data['msgCode'] != '10000':
             raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
                              f"traceId:{response_dto.data['traceId']}")
         return response_dto.data['data']['url']
```

### Comparing `digocli-0.0.2/openxlab/model/commands/__init__.py` & `digocli-0.0.3/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/model/commands/download.py` & `digocli-0.0.3/openxlab/model/commands/download.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/model/common/constants.py` & `digocli-0.0.3/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/model/common/response_dto.py` & `digocli-0.0.3/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/model/handler/download_file.py` & `digocli-0.0.3/openxlab/model/handler/download_file.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/types/command_type.py` & `digocli-0.0.3/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/openxlab/utils/file.py` & `digocli-0.0.3/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `digocli-0.0.2/setup.py` & `digocli-0.0.3/setup.py`

 * *Files identical despite different names*

