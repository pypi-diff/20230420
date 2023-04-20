# Comparing `tmp/zhuque-dataloader-0.0.6.tar.gz` & `tmp/zhuque-dataloader-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhuque-dataloader-0.0.6.tar", last modified: Thu Apr 20 02:38:10 2023, max compression
+gzip compressed data, was "zhuque-dataloader-0.0.7.tar", last modified: Thu Apr 20 03:01:53 2023, max compression
```

## Comparing `zhuque-dataloader-0.0.6.tar` & `zhuque-dataloader-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 02:38:10.552078 zhuque-dataloader-0.0.6/
--rw-rw-rw-   0        0        0      192 2023-04-20 02:38:10.551078 zhuque-dataloader-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    13446 2023-04-20 02:37:19.000000 zhuque-dataloader-0.0.6/loader.py
--rw-rw-rw-   0        0        0       42 2023-04-20 02:38:10.552078 zhuque-dataloader-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      519 2023-04-20 02:37:50.000000 zhuque-dataloader-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 02:38:10.548077 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/
--rw-rw-rw-   0        0        0      192 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 02:38:10.000000 zhuque-dataloader-0.0.6/zhuque_dataloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 03:01:53.143324 zhuque-dataloader-0.0.7/
+-rw-rw-rw-   0        0        0      192 2023-04-20 03:01:53.141323 zhuque-dataloader-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13650 2023-04-20 03:01:21.000000 zhuque-dataloader-0.0.7/loader.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:01:53.144323 zhuque-dataloader-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-20 03:01:34.000000 zhuque-dataloader-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:01:53.139323 zhuque-dataloader-0.0.7/zhuque_dataloader.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-04-20 03:01:53.000000 zhuque-dataloader-0.0.7/zhuque_dataloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-20 03:01:53.000000 zhuque-dataloader-0.0.7/zhuque_dataloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:01:53.000000 zhuque-dataloader-0.0.7/zhuque_dataloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 03:01:53.000000 zhuque-dataloader-0.0.7/zhuque_dataloader.egg-info/top_level.txt
```

### Comparing `zhuque-dataloader-0.0.6/loader.py` & `zhuque-dataloader-0.0.7/loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,19 +143,22 @@
     train_data, valid_data, test_data = load_pickle_data(ogb_root, normal_graph_name, True)
     return train_data, valid_data, test_data
 
 
 # 加载ogb格式数据集 在graphscope框架
 def load_graph_ogb_gs(data_name, dataloader):
     import graphscope as gs
-    from graphscope.dataset import (
-        ogbl_collab, ogbl_ddi, ogbn_arxiv, ogbn_mag, ogbn_proteins
-    )
-    sess = None
+    from graphscope.dataset.ogbl_collab import load_ogbl_collab
+    from graphscope.dataset.ogbl_ddi import load_ogbl_ddi
+    from graphscope.dataset.ogbn_arxiv import load_ogbn_arxiv
+    from graphscope.dataset.ogbn_mag import load_ogbn_mag
+    from graphscope.dataset.ogbn_proteins import load_ogbn_proteins
+
 
+    sess = None
     ogb_name = dataloader['ogbName']
     normal_ogb_name = ogb_name.replace("-", "_")
     if normal_ogb_name not in OGB_GS_LOAD_MAP.keys():
         raise Exception(normal_ogb_name + ' is not supported in GraphScope,\n'
                        'supported list contains: \nogbl_collab\nogbl_ddi \nogbn_arxiv\nogbn_mag\nogbn_proteins\n')
     try:
         sess = gs.session(addr='127.0.0.1:59001', mount_dataset='/dataset')
```

### Comparing `zhuque-dataloader-0.0.6/setup.py` & `zhuque-dataloader-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='zhuque-dataloader',
-    version='0.0.6',
+    version='0.0.7',
     description='zhuque graph platform dataloader component',
     author='yanrisheng',
     author_email='yanrs@zhejianglab.com',
     packages=find_packages(),
     py_modules=['loader'],
     requires=[],  # 定义依赖
     license='GPL 3.0'
```

