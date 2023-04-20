# Comparing `tmp/UniTok-3.1.3.tar.gz` & `tmp/UniTok-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.3.tar", last modified: Thu Apr 20 08:18:26 2023, max compression
+gzip compressed data, was "UniTok-3.1.4.tar", last modified: Thu Apr 20 08:27:09 2023, max compression
```

## Comparing `UniTok-3.1.3.tar` & `UniTok-3.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:18:26.912251 UniTok-3.1.3/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6582 2023-04-20 08:18:26.912096 UniTok-3.1.3/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.3/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:18:26.906106 UniTok-3.1.3/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.3/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:18:26.907644 UniTok-3.1.3/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.3/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.3/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.3/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.3/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3782 2023-04-18 12:51:00.000000 UniTok-3.1.3/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.3/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4288 2023-04-20 08:16:56.000000 UniTok-3.1.3/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:18:26.910854 UniTok-3.1.3/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.3/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      975 2023-04-20 07:37:34.000000 UniTok-3.1.3/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.3/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.3/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.3/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.3/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.3/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.3/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8843 2023-04-20 08:17:34.000000 UniTok-3.1.3/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.3/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8607 2023-04-20 07:37:12.000000 UniTok-3.1.3/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.3/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:18:26.906785 UniTok-3.1.3/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6582 2023-04-20 08:18:26.000000 UniTok-3.1.3/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-20 08:18:26.000000 UniTok-3.1.3/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-20 08:18:26.000000 UniTok-3.1.3/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-20 08:18:26.000000 UniTok-3.1.3/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-20 08:18:26.000000 UniTok-3.1.3/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-20 08:18:26.912289 UniTok-3.1.3/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-20 08:17:51.000000 UniTok-3.1.3/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:27:09.790900 UniTok-3.1.4/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6582 2023-04-20 08:27:09.790776 UniTok-3.1.4/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.4/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:27:09.787313 UniTok-3.1.4/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.4/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:27:09.788519 UniTok-3.1.4/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.4/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.4/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.4/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.4/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3782 2023-04-18 12:51:00.000000 UniTok-3.1.4/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.4/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4288 2023-04-20 08:16:56.000000 UniTok-3.1.4/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:27:09.790477 UniTok-3.1.4/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.4/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      975 2023-04-20 07:37:34.000000 UniTok-3.1.4/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.4/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.4/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.4/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.4/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.4/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.4/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8838 2023-04-20 08:26:57.000000 UniTok-3.1.4/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.4/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8607 2023-04-20 07:37:12.000000 UniTok-3.1.4/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.4/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 08:27:09.787929 UniTok-3.1.4/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6582 2023-04-20 08:27:09.000000 UniTok-3.1.4/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-20 08:27:09.000000 UniTok-3.1.4/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-20 08:27:09.000000 UniTok-3.1.4/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-20 08:27:09.000000 UniTok-3.1.4/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-20 08:27:09.000000 UniTok-3.1.4/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-20 08:27:09.790946 UniTok-3.1.4/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-20 08:27:01.000000 UniTok-3.1.4/setup.py
```

### Comparing `UniTok-3.1.3/PKG-INFO` & `UniTok-3.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.3
+Version: 3.1.4
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.3/README.md` & `UniTok-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/analysis/lengths.py` & `UniTok-3.1.4/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/analysis/plot.py` & `UniTok-3.1.4/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/column.py` & `UniTok-3.1.4/UniTok/column.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/meta.py` & `UniTok-3.1.4/UniTok/meta.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/tok/bert_tok.py` & `UniTok-3.1.4/UniTok/tok/bert_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/tok/number_tok.py` & `UniTok-3.1.4/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/tok/split_tok.py` & `UniTok-3.1.4/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/tok/tok.py` & `UniTok-3.1.4/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/unidep.py` & `UniTok-3.1.4/UniTok/unidep.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         export modified, unioned or filtered depot
         """
 
         os.makedirs(store_dir, exist_ok=True)
         data = dict()
 
         for voc in self.vocabs:
-            self.vocabs[voc.name].save(store_dir)
+            self.vocabs[voc].save(store_dir)
 
         for sample in tqdm.tqdm(self, disable=self.silent):
             for col_name in sample:
                 if col_name not in data:
                     data[col_name] = []
                 data[col_name].append(sample[col_name])
```

### Comparing `UniTok-3.1.3/UniTok/unitok.py` & `UniTok-3.1.4/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/vocab.py` & `UniTok-3.1.4/UniTok/vocab.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok/vocabs.py` & `UniTok-3.1.4/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.4/UniTok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.3
+Version: 3.1.4
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.3/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.4/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.3/setup.py` & `UniTok-3.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.1.3',
+    version='3.1.4',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

