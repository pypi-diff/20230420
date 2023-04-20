# Comparing `tmp/zhuque-dataloader-0.0.5.tar.gz` & `tmp/zhuque-dataloader-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.0.5.tar", last modified: Wed Apr 19 09:42:41 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.0.6.tar", last modified: Thu Apr 20 02:38:10 2023, max compression
```

## Comparing `zhuque-dataloader-0.0.5.tar` & `zhuque-dataloader-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:42:41.992579 zhuque-dataloader-0.0.5/
--rw-rw-rw-   0        0        0      192 2023-04-19 09:42:41.991579 zhuque-dataloader-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    13435 2023-04-19 07:33:46.000000 zhuque-dataloader-0.0.5/loader.py
--rw-rw-rw-   0        0        0       42 2023-04-19 09:42:41.992579 zhuque-dataloader-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-04-19 09:42:21.000000 zhuque-dataloader-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:42:41.989579 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 09:42:41.000000 zhuque-dataloader-0.0.5/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 02:38:10.552078 zhuque-dataloader-0.0.6/
+-rw-rw-rw-   0        0        0      192 2023-04-20 02:38:10.551078 zhuque-dataloader-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13446 2023-04-20 02:37:19.000000 zhuque-dataloader-0.0.6/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 02:38:10.552078 zhuque-dataloader-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-20 02:37:50.000000 zhuque-dataloader-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 02:38:10.548077 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/top_level.txt
```

### Comparing `zhuque-dataloader-0.0.5/loader.py` & `zhuque-dataloader-0.0.6/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,16 +157,16 @@
     if normal_ogb_name not in OGB_GS_LOAD_MAP.keys():
         raise Exception(normal_ogb_name + ' is not supported in GraphScope,\n'
                        'supported list contains: \nogbl_collab\nogbl_ddi \nogbn_arxiv\nogbn_mag\nogbn_proteins\n')
     try:
         sess = gs.session(addr='127.0.0.1:59001', mount_dataset='/dataset')
         print(sess)
         params = []
-        params.append(sess)
-        params.append('/FILES/INPUT/' + data_name)
+        params.append('sess')
+        params.append('\'/FILES/INPUT/' + data_name + '\'')
         obj_str = OGB_GS_LOAD_MAP.get(normal_ogb_name) + construct_param(params)
         # graph = load_ogbn_mag(sess, '/FILES/INPUT/ogbn_mag_small')
         print(obj_str)
         return eval(obj_str)
     except:
         print('load ogb graph in GraphScope error')
         raise Exception('load ogb graph in GraphScope error')
```

### Comparing `zhuque-dataloader-0.0.5/setup.py` & `zhuque-dataloader-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhuque-dataloader',
-    version='0.0.5',
+    version='0.0.6',
     description='zhuque graph platform dataloader component',
     author='yanrisheng',
     author_email='yanrs@zhejianglab.com',
     packages=find_packages(),
     py_modules=['loader'],
     requires=[],  # 定义依赖
     license='GPL 3.0'
```

