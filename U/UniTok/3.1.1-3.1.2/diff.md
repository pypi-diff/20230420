# Comparing `tmp/UniTok-3.1.1.tar.gz` & `tmp/UniTok-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniTok-3.1.1.tar", last modified: Tue Apr 18 12:51:16 2023, max compression
+gzip compressed data, was "UniTok-3.1.2.tar", last modified: Thu Apr 20 07:37:51 2023, max compression
```

## Comparing `UniTok-3.1.1.tar` & `UniTok-3.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.194331 UniTok-3.1.1/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:51:16.194217 UniTok-3.1.1/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.1/README.md
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.190647 UniTok-3.1.1/UniTok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.1/UniTok/__init__.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.192128 UniTok-3.1.1/UniTok/analysis/
--rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.1/UniTok/analysis/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.1/UniTok/analysis/lengths.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.1/UniTok/analysis/plot.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.1/UniTok/cols.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     3782 2023-04-18 12:51:00.000000 UniTok-3.1.1/UniTok/column.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.1/UniTok/global_setting.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     4444 2023-04-18 12:50:20.000000 UniTok-3.1.1/UniTok/meta.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.193904 UniTok-3.1.1/UniTok/tok/
--rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.1/UniTok/tok/__init__.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      911 2023-03-26 10:24:07.000000 UniTok-3.1.1/UniTok/tok/bert_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.1/UniTok/tok/ent_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.1/UniTok/tok/id_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.1/UniTok/tok/number_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.1/UniTok/tok/seq_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.1/UniTok/tok/split_tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.1/UniTok/tok/tok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8829 2023-04-18 12:49:58.000000 UniTok-3.1.1/UniTok/unidep.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.1/UniTok/unitok.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     8552 2023-04-18 12:29:04.000000 UniTok-3.1.1/UniTok/vocab.py
--rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.1/UniTok/vocabs.py
-drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-18 12:51:16.191414 UniTok-3.1.1/UniTok.egg-info/
--rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/PKG-INFO
--rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/SOURCES.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/dependency_links.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/requires.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-18 12:51:16.000000 UniTok-3.1.1/UniTok.egg-info/top_level.txt
--rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-18 12:51:16.194363 UniTok-3.1.1/setup.cfg
--rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-18 12:51:12.000000 UniTok-3.1.1/setup.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 07:37:51.356479 UniTok-3.1.2/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-20 07:37:51.356279 UniTok-3.1.2/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6303 2023-03-28 09:24:03.000000 UniTok-3.1.2/README.md
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 07:37:51.352716 UniTok-3.1.2/UniTok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      397 2023-03-26 13:47:19.000000 UniTok-3.1.2/UniTok/__init__.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 07:37:51.354065 UniTok-3.1.2/UniTok/analysis/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       86 2023-03-26 13:40:47.000000 UniTok-3.1.2/UniTok/analysis/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      884 2023-03-26 13:40:47.000000 UniTok-3.1.2/UniTok/analysis/lengths.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1299 2023-03-26 13:36:04.000000 UniTok-3.1.2/UniTok/analysis/plot.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      109 2023-03-26 12:27:16.000000 UniTok-3.1.2/UniTok/cols.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     3782 2023-04-18 12:51:00.000000 UniTok-3.1.2/UniTok/column.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      190 2022-09-06 07:19:54.000000 UniTok-3.1.2/UniTok/global_setting.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     4444 2023-04-18 12:50:20.000000 UniTok-3.1.2/UniTok/meta.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 07:37:51.355978 UniTok-3.1.2/UniTok/tok/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      284 2023-03-28 08:56:34.000000 UniTok-3.1.2/UniTok/tok/__init__.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      975 2023-04-20 07:37:34.000000 UniTok-3.1.2/UniTok/tok/bert_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      490 2023-03-28 08:56:34.000000 UniTok-3.1.2/UniTok/tok/ent_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      178 2023-03-26 10:26:04.000000 UniTok-3.1.2/UniTok/tok/id_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1429 2023-03-27 10:44:39.000000 UniTok-3.1.2/UniTok/tok/number_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      379 2023-03-26 14:01:30.000000 UniTok-3.1.2/UniTok/tok/seq_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      721 2023-03-26 10:27:50.000000 UniTok-3.1.2/UniTok/tok/split_tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1628 2023-03-26 13:37:00.000000 UniTok-3.1.2/UniTok/tok/tok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8829 2023-04-18 12:49:58.000000 UniTok-3.1.2/UniTok/unidep.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6491 2023-04-18 12:49:05.000000 UniTok-3.1.2/UniTok/unitok.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     8607 2023-04-20 07:37:12.000000 UniTok-3.1.2/UniTok/vocab.py
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     1448 2023-04-18 12:43:49.000000 UniTok-3.1.2/UniTok/vocabs.py
+drwxr-xr-x   0 jyonnliu   (501) staff       (20)        0 2023-04-20 07:37:51.353445 UniTok-3.1.2/UniTok.egg-info/
+-rw-r--r--   0 jyonnliu   (501) staff       (20)     6584 2023-04-20 07:37:51.000000 UniTok-3.1.2/UniTok.egg-info/PKG-INFO
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      582 2023-04-20 07:37:51.000000 UniTok-3.1.2/UniTok.egg-info/SOURCES.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        1 2023-04-20 07:37:51.000000 UniTok-3.1.2/UniTok.egg-info/dependency_links.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       51 2023-04-20 07:37:51.000000 UniTok-3.1.2/UniTok.egg-info/requires.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)        7 2023-04-20 07:37:51.000000 UniTok-3.1.2/UniTok.egg-info/top_level.txt
+-rw-r--r--   0 jyonnliu   (501) staff       (20)       38 2023-04-20 07:37:51.356514 UniTok-3.1.2/setup.cfg
+-rw-r--r--   0 jyonnliu   (501) staff       (20)      724 2023-04-20 07:37:43.000000 UniTok-3.1.2/setup.py
```

### Comparing `UniTok-3.1.1/PKG-INFO` & `UniTok-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.1
+Version: 3.1.2
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.1/README.md` & `UniTok-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/analysis/lengths.py` & `UniTok-3.1.2/UniTok/analysis/lengths.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/analysis/plot.py` & `UniTok-3.1.2/UniTok/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/column.py` & `UniTok-3.1.2/UniTok/column.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/meta.py` & `UniTok-3.1.2/UniTok/meta.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/tok/bert_tok.py` & `UniTok-3.1.2/UniTok/tok/bert_tok.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,8 +26,12 @@
 
     def t(self, obj) -> [int, list]:
         if pd.notnull(obj):
             ts = self.tokenizer.tokenize(obj)
             ids = self.tokenizer.convert_tokens_to_ids(ts)
         else:
             ids = []
+
+        for index in ids:
+            self.vocab.count(index)
+
         return ids
```

### Comparing `UniTok-3.1.1/UniTok/tok/number_tok.py` & `UniTok-3.1.2/UniTok/tok/number_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/tok/split_tok.py` & `UniTok-3.1.2/UniTok/tok/split_tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/tok/tok.py` & `UniTok-3.1.2/UniTok/tok/tok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/unidep.py` & `UniTok-3.1.2/UniTok/unidep.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/unitok.py` & `UniTok-3.1.2/UniTok/unitok.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok/vocab.py` & `UniTok-3.1.2/UniTok/vocab.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,20 @@
         extend vocab with iterable object
         :return: index list
         """
         return [self.append(obj) for obj in objs]
 
     def append(self, obj):
         index = self._append(obj)
+        self.count(index)
+        return index
+
+    def count(self, index):
         if self._count_mode and index > -1:
             self._counter[index] = self._counter.get(index, 0) + 1
-        return index
 
     def _append(self, obj):
         """
         append object to vocab
         :return: object index
         """
         if obj in self.o2i:
```

### Comparing `UniTok-3.1.1/UniTok/vocabs.py` & `UniTok-3.1.2/UniTok/vocabs.py`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/UniTok.egg-info/PKG-INFO` & `UniTok-3.1.2/UniTok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UniTok
-Version: 3.1.1
+Version: 3.1.2
 Summary: Unified Tokenizer
 Home-page: https://github.com/Jyonn/UnifiedTokenizer
 Author: Jyonn Liu
 Author-email: i@6-79.cn
 License: MIT Licence
 Keywords: token,tokenizer,bert
 Platform: any
```

### Comparing `UniTok-3.1.1/UniTok.egg-info/SOURCES.txt` & `UniTok-3.1.2/UniTok.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UniTok-3.1.1/setup.py` & `UniTok-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='UniTok',
-    version='3.1.1',
+    version='3.1.2',
     keywords=['token', 'tokenizer', 'bert'],
     description='Unified Tokenizer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT Licence',
     url='https://github.com/Jyonn/UnifiedTokenizer',
     author='Jyonn Liu',
```

