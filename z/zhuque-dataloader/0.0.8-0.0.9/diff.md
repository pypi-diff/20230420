# Comparing `tmp/zhuque-dataloader-0.0.8.tar.gz` & `tmp/zhuque-dataloader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.0.8.tar", last modified: Thu Apr 20 07:00:37 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.0.9.tar", last modified: Thu Apr 20 07:39:14 2023, max compression
```

## Comparing `zhuque-dataloader-0.0.8.tar` & `zhuque-dataloader-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 07:00:37.612336 zhuque-dataloader-0.0.8/
--rw-rw-rw-   0        0        0      192 2023-04-20 07:00:37.611364 zhuque-dataloader-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    13656 2023-04-20 06:59:52.000000 zhuque-dataloader-0.0.8/loader.py
--rw-rw-rw-   0        0        0       42 2023-04-20 07:00:37.612336 zhuque-dataloader-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-04-20 07:00:35.000000 zhuque-dataloader-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 07:00:37.609337 zhuque-dataloader-0.0.8/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-20 07:00:37.000000 zhuque-dataloader-0.0.8/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 07:00:37.000000 zhuque-dataloader-0.0.8/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 07:00:37.000000 zhuque-dataloader-0.0.8/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 07:00:37.000000 zhuque-dataloader-0.0.8/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 07:39:14.711729 zhuque-dataloader-0.0.9/
+-rw-rw-rw-   0        0        0      192 2023-04-20 07:39:14.711729 zhuque-dataloader-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13686 2023-04-20 07:09:37.000000 zhuque-dataloader-0.0.9/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 07:39:14.712730 zhuque-dataloader-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-20 07:39:10.000000 zhuque-dataloader-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 07:39:14.708729 zhuque-dataloader-0.0.9/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-20 07:39:14.000000 zhuque-dataloader-0.0.9/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-20 07:39:14.000000 zhuque-dataloader-0.0.9/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 07:39:14.000000 zhuque-dataloader-0.0.9/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 07:39:14.000000 zhuque-dataloader-0.0.9/zhuque_dataloader.egg-info/top_level.txt
```

### Comparing `zhuque-dataloader-0.0.8/loader.py` & `zhuque-dataloader-0.0.9/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,24 +152,25 @@
     from graphscope.dataset.ogbn_arxiv import load_ogbn_arxiv
     from graphscope.dataset.ogbn_mag import load_ogbn_mag
     from graphscope.dataset.ogbn_proteins import load_ogbn_proteins
 
 
     sess = None
     ogb_name = dataloader['ogbName']
+    ogb_root = dataloader['ogbRoot']
     normal_ogb_name = ogb_name.replace("-", "_")
     if normal_ogb_name not in OGB_GS_LOAD_MAP.keys():
         raise Exception(normal_ogb_name + ' is not supported in GraphScope,\n'
                        'supported list contains: \nogbl_collab\nogbl_ddi \nogbn_arxiv\nogbn_mag\nogbn_proteins\n')
     try:
         sess = gs.session(addr='127.0.0.1:59001', mount_dataset='/dataset')
         print(sess)
         params = []
         params.append('sess')
-        params.append('\'/FILES/INPUT/' + data_name + '\'')
+        params.append('\'/FILES' + ogb_root + '\'')
         obj_str = OGB_GS_LOAD_MAP.get(normal_ogb_name) + construct_param(params)
         # graph = load_ogbn_mag(sess, '/FILES/INPUT/ogbn_mag_small')
         print(obj_str)
         return eval(obj_str)
     except:
         print('load ogb graph in GraphScope error')
         raise Exception('load ogb graph in GraphScope error')
```

### Comparing `zhuque-dataloader-0.0.8/setup.py` & `zhuque-dataloader-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhuque-dataloader',
-    version='0.0.8',
+    version='0.0.9',
     description='zhuque graph platform dataloader component',
     author='yanrisheng',
     author_email='yanrs@zhejianglab.com',
     packages=find_packages(),
     py_modules=['loader'],
     requires=[],  # 定义依赖
     license='GPL 3.0'
```

