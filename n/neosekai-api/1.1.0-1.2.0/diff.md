# Comparing `tmp/neosekai_api-1.1.0-py3-none-any.whl.zip` & `tmp/neosekai_api-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6845 bytes, number of entries: 11
+Zip file size: 6860 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      219 b- defN 23-Apr-12 07:51 neosekai_api/__init__.py
--rw-rw-rw-  2.0 fat     2573 b- defN 23-Apr-14 12:03 neosekai_api/chapter.py
--rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-14 10:50 neosekai_api/constants.py
--rw-rw-rw-  2.0 fat      294 b- defN 23-Apr-05 08:07 neosekai_api/helper.py
+-rw-rw-rw-  2.0 fat     2543 b- defN 23-Apr-20 09:23 neosekai_api/chapter.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Apr-20 09:24 neosekai_api/constants.py
+-rw-rw-rw-  2.0 fat      332 b- defN 23-Apr-20 09:21 neosekai_api/helper.py
 -rw-rw-rw-  2.0 fat     4735 b- defN 23-Apr-14 11:29 neosekai_api/novel.py
 -rw-rw-rw-  2.0 fat      135 b- defN 23-Apr-14 11:41 neosekai_api/test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3165 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      883 b- defN 23-Apr-14 14:58 neosekai_api-1.1.0.dist-info/RECORD
-11 files, 13219 bytes uncompressed, 5349 bytes compressed:  59.5%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3165 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      883 b- defN 23-Apr-20 09:28 neosekai_api-1.2.0.dist-info/RECORD
+11 files, 13227 bytes uncompressed, 5364 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: neosekai_api/novel.py
 Comment: 
 
 Filename: neosekai_api/test.py
 Comment: 
 
-Filename: neosekai_api-1.1.0.dist-info/LICENSE
+Filename: neosekai_api-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: neosekai_api-1.1.0.dist-info/METADATA
+Filename: neosekai_api-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: neosekai_api-1.1.0.dist-info/WHEEL
+Filename: neosekai_api-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: neosekai_api-1.1.0.dist-info/top_level.txt
+Filename: neosekai_api-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: neosekai_api-1.1.0.dist-info/RECORD
+Filename: neosekai_api-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neosekai_api/chapter.py

```diff
@@ -8,43 +8,36 @@
     '''
     NovelChapter object
 
     :params _url : The Mangadex Chapter URL
     '''
 
     def __init__(self, _url: str) -> None:
-        self.url = self.__urlformatter(_url)
+        self.url = _url
         self.__response_object = requests.get(self.url, timeout=10)
+        self.details = self.chapter_details()
         self.volume = self.details['volume']
         self.name = self.details['chapter_name']
         self.release_date = self.details['release_date']
 
-    def __urlformatter(self, _url):
-        """
-        formats url to standard form to be used in the program
-        """
-        __url = ''
-        if 'https://' not in _url:
-            __url = 'https://' + _url
-        else:
-            return __url
 
     def chapter_details(self):
         """
         returns chapter details : 
 
         - chapter volume
         - chapter name
         - url
         - chapter release date
 
         In the given order in JSON format
-
         """
-        novel_url = self.url[:self.url.index('/', 43)]
+        novel_url_ = self.url.split('neosekaitranslations.com/novel/')[-1]
+        novel_name = novel_url_[:novel_url_.index('/')]
+        novel_url = f"https://www.neosekaitranslations.com/novel/{novel_name}/"
         novel = Novel(novel_url)
         index_page = novel.get_index_page()
         for i in index_page:
             if index_page[i]['url'] == self.url:
                 return index_page[i]
 
     def get_chapter_content(self, fancy=True):
@@ -68,15 +61,15 @@
         div = soup.find('div', attrs={'class': 'text-left'})
         paras = div.find_all('p')
         content = {}
         n = 1
         for i in paras:
             if i.span != None:
                 content[str(n)] = {'type': 'text',
-                                   'content': i.span.text.strip()}
+                                   'content': i.span.text.strip() if fancy else heavy_translate(i.span.text.strip())}
                 n += 1
             elif i.img != None:
                 content[str(n)] = {'type': 'img', 'content': i.img['src']}
                 n += 1
             else:
                 continue
         if fancy:
```

## neosekai_api/constants.py

```diff
@@ -1 +1 @@
-VERSION = '1.1.0'
+VERSION = '1.2.0'
```

## neosekai_api/helper.py

```diff
@@ -1,6 +1,6 @@
 def heavy_translate(string:str):
     '''
     returns string translated of any 'fancy' quotations or ellipses
     '''
-    transl_table = dict([ (ord(x), ord(y)) for x,y in zip( u"‘’´“”–-―　",  u"'''\"\"--- ") ] )
-    return string.translate(transl_table).replace('…', '...')
+    transl_table = dict([ (ord(x), ord(y)) for x,y in zip( u"‘’´“”–-―　–※₩└♪─◇一◆",  u"'''\"\"--- -*   -*-*") ] )
+    return string.translate(transl_table).replace('…', '...')
```

## Comparing `neosekai_api-1.1.0.dist-info/LICENSE` & `neosekai_api-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neosekai_api-1.1.0.dist-info/METADATA` & `neosekai_api-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosekai-api
-Version: 1.1.0
+Version: 1.2.0
 Summary: An Unoffical Python API for neosekaitranslations.com
 Home-page: https://github.com/john-erinjery/neosekai-api/
 Author: John Erinjery
 Author-email: jancyvinod415@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
```

