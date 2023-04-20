# Comparing `tmp/EmoTFIDF-1.1.4.tar.gz` & `tmp/EmoTFIDF-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmoTFIDF-1.1.4.tar", last modified: Wed Apr 19 10:40:23 2023, max compression
+gzip compressed data, was "EmoTFIDF-1.1.5.tar", last modified: Thu Apr 20 08:56:37 2023, max compression
```

## Comparing `EmoTFIDF-1.1.4.tar` & `EmoTFIDF-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-19 10:40:23.057296 EmoTFIDF-1.1.4/
-drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-19 10:40:23.056827 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/requires.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-19 10:40:23.000000 EmoTFIDF-1.1.4/EmoTFIDF.egg-info/top_level.txt
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.4/LICENSE
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-19 10:40:23.057073 EmoTFIDF-1.1.4/PKG-INFO
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.4/README.md
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4840 2023-04-19 10:39:31.000000 EmoTFIDF-1.1.4/emotfidf.py
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-19 10:40:23.057357 EmoTFIDF-1.1.4/setup.cfg
--rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-19 10:40:07.000000 EmoTFIDF-1.1.4/setup.py
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-20 08:56:37.768392 EmoTFIDF-1.1.5/
+drwxr-xr-x   0 mohamedmostafa   (501) staff       (20)        0 2023-04-20 08:56:37.767973 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-20 08:56:37.000000 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)      197 2023-04-20 08:56:37.000000 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        1 2023-04-20 08:56:37.000000 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        5 2023-04-20 08:56:37.000000 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/requires.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)        9 2023-04-20 08:56:37.000000 EmoTFIDF-1.1.5/EmoTFIDF.egg-info/top_level.txt
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1091 2023-04-15 10:32:28.000000 EmoTFIDF-1.1.5/LICENSE
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     2421 2023-04-20 08:56:37.768197 EmoTFIDF-1.1.5/PKG-INFO
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1915 2023-04-18 10:48:25.000000 EmoTFIDF-1.1.5/README.md
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     4930 2023-04-20 08:55:09.000000 EmoTFIDF-1.1.5/emotfidf.py
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)       38 2023-04-20 08:56:37.768446 EmoTFIDF-1.1.5/setup.cfg
+-rw-r--r--   0 mohamedmostafa   (501) staff       (20)     1386 2023-04-20 08:56:07.000000 EmoTFIDF-1.1.5/setup.py
```

### Comparing `EmoTFIDF-1.1.4/EmoTFIDF.egg-info/PKG-INFO` & `EmoTFIDF-1.1.5/EmoTFIDF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.4/LICENSE` & `EmoTFIDF-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.4/PKG-INFO` & `EmoTFIDF-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmoTFIDF
-Version: 1.1.4
+Version: 1.1.5
 Summary: A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion2- Integrating TFIDF to add a contextNote that lexicon license is for research purposes only.
 Home-page: https://github.com/mmsa/emotfidf
 Author: mmsa12
 Author-email: mmsa12@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EmoTFIDF-1.1.4/README.md` & `EmoTFIDF-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `EmoTFIDF-1.1.4/emotfidf.py` & `EmoTFIDF-1.1.5/emotfidf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,24 @@
     # get emotions
     em_list = []
     em_dict = dict()
     em_frequencies = Counter()
     lexicon_keys = self.lexicon.keys()
     for word in self.words:
         if word in lexicon_keys:
-            emotions_found = list(set(self.lexicon[word]))
-            emotions_found = list(filter(None, emotions_found))
-            if emotions_found is not None:
-                if 'negative' in emotions_found:
-                    emotions_found.remove('negative')
-                elif 'positive' in emotions_found:
-                    emotions_found.remove('positive')
-                em_list.extend(emotions_found)
-                em_dict.update({word: self.lexicon[word]})
+            if isinstance(self.lexicon[word], list):
+                emotions_found = list(set(self.lexicon[word]))
+                emotions_found = list(filter(None, emotions_found))
+                if emotions_found is not None:
+                    if 'negative' in emotions_found:
+                        emotions_found.remove('negative')
+                    elif 'positive' in emotions_found:
+                        emotions_found.remove('positive')
+                    em_list.extend(emotions_found)
+                    em_dict.update({word: self.lexicon[word]})
     for word in em_list:
         em_frequencies[word] += 1
     sum_values = sum(em_frequencies.values())
     em_percent = {'fear': 0.0, 'anger': 0.0, 'anticipation': 0.0, 'trust': 0.0, 'surprise': 0.0,'sadness': 0.0, 'disgust': 0.0, 'joy': 0.0}
     for key in em_frequencies.keys():
         em_percent.update({key: float(em_frequencies[key]) / float(sum_values)})
     self.em_list = em_list
```

### Comparing `EmoTFIDF-1.1.4/setup.py` & `EmoTFIDF-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         nltk.download('wordnet')
         nltk.download('punkt')
         nltk.download('stopwords')
 
 
 setuptools.setup(
     name="EmoTFIDF",
-    version="1.1.4",
+    version="1.1.5",
     author="mmsa12",
     author_email="mmsa12@gmail.com",
     description="A library to extract emotions using two methods, 1- Using lexicon based, counting frequency of emotion"
                 "2- Integrating TFIDF to add a context"
                 "Note that lexicon license is for research purposes only.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

