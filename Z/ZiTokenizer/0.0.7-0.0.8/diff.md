# Comparing `tmp/ZiTokenizer-0.0.7.tar.gz` & `tmp/ZiTokenizer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZiTokenizer-0.0.7.tar", last modified: Wed Apr 12 14:39:54 2023, max compression
+gzip compressed data, was "ZiTokenizer-0.0.8.tar", last modified: Thu Apr 20 17:49:59 2023, max compression
```

## Comparing `ZiTokenizer-0.0.7.tar` & `ZiTokenizer-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:54.251252 ZiTokenizer-0.0.7/
--rw-rw-rw-   0        0        0     1545 2023-04-12 14:39:54.250252 ZiTokenizer-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:54.236256 ZiTokenizer-0.0.7/ZiTokenizer/
--rw-rw-rw-   0        0        0     8129 2023-04-11 15:45:51.000000 ZiTokenizer-0.0.7/ZiTokenizer/He2Zi.py
--rw-rw-rw-   0        0        0     7243 2023-04-06 17:19:17.000000 ZiTokenizer-0.0.7/ZiTokenizer/UnicodeTokenizer.py
--rw-rw-rw-   0        0        0     6038 2023-04-11 16:10:04.000000 ZiTokenizer-0.0.7/ZiTokenizer/ZiCutter.py
--rw-rw-rw-   0        0        0     2808 2023-04-11 01:27:10.000000 ZiTokenizer-0.0.7/ZiTokenizer/ZiSegmenter.py
--rw-rw-rw-   0        0        0     7143 2023-04-11 16:09:58.000000 ZiTokenizer-0.0.7/ZiTokenizer/ZiTokenizer.py
--rw-rw-rw-   0        0        0        0 2023-04-06 16:52:46.000000 ZiTokenizer-0.0.7/ZiTokenizer/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-03-10 17:35:16.000000 ZiTokenizer-0.0.7/ZiTokenizer/glance.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:39:54.248755 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/
--rw-rw-rw-   0        0        0     1545 2023-04-12 14:39:54.000000 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-12 14:39:54.000000 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:39:54.000000 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-12 14:39:54.000000 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-12 14:39:54.000000 ZiTokenizer-0.0.7/ZiTokenizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:39:54.251735 ZiTokenizer-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1644 2023-04-07 15:19:50.000000 ZiTokenizer-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:49:59.749883 ZiTokenizer-0.0.8/
+-rw-rw-rw-   0        0        0     1411 2023-04-20 17:49:59.749883 ZiTokenizer-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 17:49:59.742884 ZiTokenizer-0.0.8/ZiTokenizer/
+-rw-rw-rw-   0        0        0     9065 2023-04-19 12:27:35.000000 ZiTokenizer-0.0.8/ZiTokenizer/He2Zi.py
+-rw-rw-rw-   0        0        0     7390 2023-04-20 15:58:46.000000 ZiTokenizer-0.0.8/ZiTokenizer/UnicodeTokenizer.py
+-rw-rw-rw-   0        0        0     3527 2023-04-20 16:07:24.000000 ZiTokenizer-0.0.8/ZiTokenizer/ZiCutter.py
+-rw-rw-rw-   0        0        0     2808 2023-04-11 01:27:10.000000 ZiTokenizer-0.0.8/ZiTokenizer/ZiSegmenter.py
+-rw-rw-rw-   0        0        0     6903 2023-04-20 16:22:42.000000 ZiTokenizer-0.0.8/ZiTokenizer/ZiTokenizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-06 16:52:46.000000 ZiTokenizer-0.0.8/ZiTokenizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:49:59.747882 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/
+-rw-rw-rw-   0        0        0     1411 2023-04-20 17:49:59.000000 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-04-20 17:49:59.000000 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:49:59.000000 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-20 17:49:59.000000 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-20 17:49:59.000000 ZiTokenizer-0.0.8/ZiTokenizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 17:49:59.749883 ZiTokenizer-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1644 2023-04-20 16:51:06.000000 ZiTokenizer-0.0.8/setup.py
```

### Comparing `ZiTokenizer-0.0.7/PKG-INFO` & `ZiTokenizer-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 Metadata-Version: 2.1
 Name: ZiTokenizer
-Version: 0.0.7
+Version: 0.0.8
 Summary: ZiTokenizer: tokenize world text as Zi
 Home-page: https://github.com/laohur/ZiCutter
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: UnicodeTokenizer,ZiCutter,ZiTokenizer,Tokenizer,Unicode,laohur
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # ZiTokenizer
 
-ZiTokenizer: tokenize word as Zi
+Tokineze all languages text into Zi.
+
+support 300+ languages from wikipedia, including global 
 
-word => prefix + root + suffix
 
-support 325 languages + global, including global 
 ## use
 * pip install ZiTokenizer
-* toeknize language frequency and count word frequency (https://github.com/laohur/UnicodeTokenizer/blob/master/test/count_lang/count_word.py)
+
 ```python
 from ZiTokenizer.ZiTokenizer import ZiTokenizer
 
 # use
-tokenizer = ZiTokenizer(lang="global")  # lang='ar', 'en', 'fr', 'ru', 'zh' ...
-line = "'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)熵😀'\x0000熇"
-tokens = tokenizer.tokenize(line)
-print(' '.join(tokens)) # ' 〇 ㎡ [ ค ณ-- จ-- ะ --จ ด-- พ ธ แต ง-- งา-- น-- เม อไ-- ร --ค --ะ ] ##s ht pays - g [ ran ] d - blanc - eleve » ( 白 高 大 夏 國 ) ⿰ 火 商 ##g ce ' 00 ⿰ 火 高
-
-# build 
-tokenizer = ZiTokenizer(mydir) # mydir include "word_frequency.tsv"
-tokenizer.build(min_ratio=1.5e-6, min_freq=3)
-tokenizer = ZiTokenizer(dir=mydir)
+tokenizer = ZiTokenizer()  
+line = "'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏2022２０１９\U0010ffff"
+indexs = tokenizer.encode(line)
+tokens = tokenizer.decode(indexs)
+line2=tokenizer.tokens2line(tokens)
 
+# build
+demo/unit.py
 ```
+
+## UnicodeTokenizer
+basic tokeinzer
+
+## ZiCutter
+汉字拆字
+> '瞼' -> ['⿰', '目', '僉']
+
+## ZiSegmenter
+word => prefix + root + suffix
+> 'modernbritishdo' -> ['mod--', 'er--', 'n--', 'british', '--do']
+
+## languages
+default using "golabl" vocob, others from https://laohur.github.io/ZiTokenizer/index.html
+> tokenizer = ZiTokenizer(vocab_dir)
```

### Comparing `ZiTokenizer-0.0.7/ZiTokenizer/UnicodeTokenizer.py` & `ZiTokenizer-0.0.8/ZiTokenizer/UnicodeTokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 # -*- coding: utf-8 -*-
 
 import unicodedata
 
+
 class UnicodeTokenizer:
-    def __init__(self,  do_lower_case=True, never_split=[], highUnicodePoint=10000):
+    def __init__(self,  do_lower_case=True, never_split=[], highUnicodePoint=10000, split_digit=False):
         self.do_lower_case = do_lower_case
         self.highUnicodePoint = highUnicodePoint
+        self.split_digit = split_digit
         self.never_split = set(x for x in never_split)
 
-    
-    def split_blank(self,line):
-        tokens=[x.strip() for x in line.split() if x.strip()]
+    def split_blank(self, line):
+        tokens = [x.strip() for x in line.split() if x.strip()]
         return tokens
 
-    def split_marks(self,line,marks):
+    def split_marks(self, line, marks):
         tokens = []
         for i, x in enumerate(line):
             if i == 0:
                 tokens.append(x)
             elif marks[i] or marks[i-1]:
                 tokens.append(x)
             else:
                 tokens[-1] += x
         return tokens
-        
+
     def normalize(self, line,  normal_type="NFD"):
         l = unicodedata.normalize(normal_type, line)
         return l
-    
-    def split_highUnicodePoint(self,line):
+
+    def split_highUnicodePoint(self, line):
         marks = [ord(x) >= self.highUnicodePoint for x in line]
         return self.split_marks(line, marks)
 
-    def split_category(self,line):
+    def split_category(self, line):
         if len(line) == 1:
             return [line]
         elif len(line) == 0:
             return []
         categorys = [unicodedata.category(x) for x in line]
         names = [unicodedata.name(x).split()[0] if categorys[i][0] in 'LN' else None for i, x in enumerate(line)]
         tokens = []
         for i, x in enumerate(line):
             if i == 0:
                 tokens.append(x)
             elif categorys[i][0] == categorys[i-1][0] == 'L':
-                if names[i]==names[i-1]:
+                if names[i] == names[i-1]:
                     tokens[-1] += x
                 else:
                     tokens.append(x)
-            elif categorys[i][0] == categorys[i-1][0] == 'N':
+            elif not self.split_digit and categorys[i][0] == categorys[i-1][0] == 'N':
                 if names[i] == names[i-1]:
                     tokens[-1] += x
                 else:
                     tokens.append(x)
             else:
-                if categorys[i]!='Mn':
+                if categorys[i] != 'Mn':
                     tokens.append(x)
-                if categorys[i-1]=='Mn':
+                if categorys[i-1] == 'Mn':
                     tokens.append('')
 
-        return [x.strip() for x in tokens if x.strip()]
+        tokens = [x.strip() for x in tokens if x.strip()]
+        return tokens
 
     def split_word(self, x):
-        tokens=[]
+        tokens = []
         if self.do_lower_case:
             x = self.normalize(x.lower())
         us = self.split_blank(x)
         for u in us:
             vs = self.split_highUnicodePoint(u)
             for v in vs:
                 w = self.split_category(v)
@@ -78,54 +80,54 @@
         tokens = []
         for x in words:
             if x in self.never_split:
                 tokens.append(x)
             else:
                 tokens += self.split_word(x)
         return tokens
-    
-    def detokenize(self,tokens):
-        l=tokens[0]
-        for i,x in enumerate(tokens):
-            if i==0:
+
+    def detokenize(self, tokens):
+        l = tokens[0]
+        for i, x in enumerate(tokens):
+            if i == 0:
                 continue
-            a=tokens[i-1][-1]
-            b=x[0]
-            if max(ord(a), ord(b))<self.highUnicodePoint and unicodedata.category(a)[0]==unicodedata.category(b)[0] and unicodedata.category(a)[0] in 'LN':
-                l+=' '
-            l+=x
+            a = tokens[i-1][-1]
+            b = x[0]
+            if max(ord(a), ord(b)) < self.highUnicodePoint and unicodedata.category(a)[0] == unicodedata.category(b)[0] and unicodedata.category(a)[0] in 'LN':
+                l += ' '
+            l += x
         return l
 
 
 def test_UnicodeTokenizer():
-    doc = ["'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏２０１９\U0010ffff",
+    doc = ["'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏2022２０１９\U0010ffff",
            "대한민국의Ⅷ首先8.88设置 st。art_new_word=True 和 output=[açaí]，output 就是最终 no such name",
            "的输出คุณจะจัดพิธีแต่งงานเมื่อไรคะ탑승 수속해야pneumonoultramicroscopicsilicovolcanoconiosis",
            "하는데 카운터가 어디에 있어요ꆃꎭꆈꌠꊨꏦꏲꅉꆅꉚꅉꋍꂷꂶꌠلأحياء تمارين تتطلب من [MASK] [PAD] [CLS][SEP]",
            '''est 𗴂𗹭𘜶𗴲𗂧, ou "phiow-bjij-lhjij-lhjij", ce que l'on peut traduire par « pays-grand-blanc-élevé » (白高大夏國).''',
            'วรรณพงษ์เป็นนักศึกษาชั้นปีที่หนึ่ง เรียนสาขาวิทยาการคอมพิวเตอร์และสารสนเทศคณะวิทยาศาสตร์ประยุกต์และวิศวกรรมศาสตร์อยู่ที่มหาวิทยาลัยขอนแก่นวิทยาเขตหนองคายยืมคืนทรัพยากรห้องสมุดเอกสารสัมมนาคอมพิวเตอร์ปัญญาประดิษฐ์กับการพัฒนาเกมแมวกินปลาหิวววไหมหลักสูตรใหม่สดสดทนได้',
            'ສົມເດັດພະເຈົ້າຢູ່ຫົວບໍຣົມໂກດຊົງທຳນຸບຳລຸງບ້ານເມືອງແລະພະສາດສະໜາຈົນກ່າວໄດ້ວ່າກຸງສີອະຍຸທະຢາໃນສະໄໝພະອົງນັ້ນເປັນຍຸກທີ່ບ້ານເມືອງດີ ມີຂຸນນາງຄົນສຳຄັນທີ່ເຕີບໂຕໃນເວລາຕໍ່ມາ ໃນລາຊະການຂອງພະອົງຫຼາຍຄົນ ເຊັ່ນ ສົມເດັດພະເຈົ້າກຸງທົນບຸລີ, ພະບາດສົມເດັດພະພຸດທະຍອດຟ້າຈຸລາໂລກມະຫາລາດ ເປັນຕົ້ນ ໃນທາງດ້ານວັນນະຄະດີກໍມີກະວີຄົນສຳຄັນ ເຊັ່ນ ເຈົ້າຟ້າທຳມາທິເບດໄຊຍະເຊດສຸລິຍະວົງ ກົມມະຂຸນເສນາພິທັກ ຫຼືເຈົ້າຟ້າກຸ້ງ ເຊິ່ງເປັນພະໂອລົດ ເປັນຕົ້ນ'
            ]
-    unicodeTokenizer=UnicodeTokenizer()    
+    unicodeTokenizer = UnicodeTokenizer()
     for line in doc:
         tokens = unicodeTokenizer.tokenize(line)
         print(tokens)
 
+
 if __name__ == "__main__":
     from logzero import logger
 
-
-    line = "대한민국의'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏２０１９\U0010ffff"
+    line = "대한민국의'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏2022２０１９\U0010ffff"
     # line = "art_new_word=True"
-    tokenizer=UnicodeTokenizer()
+    tokenizer = UnicodeTokenizer()
     logger.info((tokenizer.split_blank(line)))
     # line = "=True"
 
-    tokenizer = UnicodeTokenizer()
-    tokens=tokenizer.tokenize(line)
+    tokenizer = UnicodeTokenizer(split_digit=True)
+    tokens = tokenizer.tokenize(line)
     logger.info(tokens)
     logger.info(tokenizer.detokenize(tokens))
     import timeit
     # re=timeit.timeit("''.join(chr(x) for x in range(int(1e6))) ")
     # logger.info(re)
 
     import time
@@ -136,8 +138,8 @@
     t1 = time.time()
     logger.info(t1-t0)
 
     test_UnicodeTokenizer()
 
 """
  '〇㎡[ค ณ จะจ ด พ ธ แ ต ง งานเม อ ไรคะ]ⅷpays-g[ran]d-blanc-e l eve»(白高大夏國)😀熇'00𧭏２０１９􏿿
-"""
+"""
```

### Comparing `ZiTokenizer-0.0.7/ZiTokenizer/ZiSegmenter.py` & `ZiTokenizer-0.0.8/ZiTokenizer/ZiSegmenter.py`

 * *Files identical despite different names*

### Comparing `ZiTokenizer-0.0.7/ZiTokenizer/ZiTokenizer.py` & `ZiTokenizer-0.0.8/ZiTokenizer/ZiTokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 import os
 import random
 import math
 
 from logzero import logger
 
 from .UnicodeTokenizer import UnicodeTokenizer
-from .ZiCutter import ZiCutter 
-from .glance import load_frequency, describe
+from .ZiCutter import ZiCutter
 from .ZiSegmenter import ZiSegmenter
 
 
 class ZiTokenizer:
-    def __init__(self, dir=None, do_lower_case=True, max_split=3, never_split=[]) -> None:
+    def __init__(self, dir=None, do_lower_case=True, max_split=3, unk_k=10, split_digit=False, never_split=[]) -> None:
         self.do_lower_case = do_lower_case
         self.max_split = max_split
+        self.split_digit = split_digit
         self.dir = dir
         self.never_split = set(x for x in never_split)
         self.token2index = collections.OrderedDict()
+        self.UNKs = [f"##{x}" for x in range(unk_k)]  # 10
+        if dir == None:
+            dir = "languages/global"
         if dir:
             self.load(dir)
 
-    def load(self,folder):
-        vocab=[]
+    def load(self, folder):
+        vocab = []
         root_words = []
         prefixs = []
         suffixs = []
-        vocab_path = os.path.join(folder,"vocab.txt")
+        vocab_path = os.path.join(folder, "vocab.txt")
         assert os.path.exists(vocab_path)
         vocab = open(vocab_path).read().splitlines()
         for i, x in enumerate(vocab):
-            # if i==3680:
-            #     d=0
-            # assert x.strip()                
             if len(x) > 1:
                 if x[:2] == '--':
                     suffixs.append(x[2:])
                     continue
                 if x[-2:] == '--':
                     prefixs.append(x[:-2])
                     continue
@@ -47,65 +47,63 @@
 
         self.vocab = vocab
         for i, x in enumerate(vocab):
             self.token2index[x] = i
 
         root_words = set(root_words)
         never_split = self.never_split | root_words
-        self.unicodeTokenizer = UnicodeTokenizer(do_lower_case=self.do_lower_case,never_split=never_split)
-        self.ziCutter = ZiCutter(self.dir)
+        self.unicodeTokenizer = UnicodeTokenizer(do_lower_case=self.do_lower_case, never_split=never_split, split_digit=self.split_digit)
+        self.ziCutter = ZiCutter(folder)
         self.ziSegmenter = ZiSegmenter(
-            root_words=root_words, prefixs= prefixs, suffixs= suffixs, max_split=self.max_split)
+            root_words=root_words, prefixs=prefixs, suffixs=suffixs, max_split=self.max_split)
+
+    def cutRare(self, token) -> str:
+        point = sum(ord(x) for x in token) % 10
+        return f"##{point}"
 
     def token_word(self, word):
         [heads, root, tails] = self.ziSegmenter.token_word(word)
         if root:
             for i in range(len(heads)):
                 heads[i] += '--'
             for i in range(len(tails)):
                 tails[i] = '--' + tails[i]
             tokens = heads+[root]+tails
             return tokens
-        token=self.ziCutter.cutWord(word)
-        if token.startswith('##'):
-            tokens = [token ]
+        ids = self.ziCutter.cutHanzi(word)
+        if ids == word:
+            tokens = [self.cutRare(word)]
         else:
-            tokens=list(token)
+            tokens = list(ids)
         return tokens
 
-    def build(self,word_freq_path,folder, min_ratio=1.5e-6, min_freq=3):
-        assert os.path.exists(word_freq_path)
-        logger.warning(f" building from {word_freq_path}")
-        word_freq = load_frequency(
-            word_freq_path, do_lower_case=self.do_lower_case)
-        if not word_freq:
-            logger.error(f"no word_freq")
-            return
-        total = describe(word_freq)
+    def build(self, word_freq, total, folder, min_ratio=1.5e-6, min_freq=2, vocab_size=-1):
         bottom = max(min_freq, (total*min_ratio))
-        bottom_char=max(min_freq, bottom/4)
+        bottom_word = bottom
         logger.info(
-            f"min_ratio:{min_ratio} min_freq:{min_freq} bottom:{bottom:.2f} bottom_char:{bottom_char:.2f}")
-        hot = [k for k, v in word_freq if v >= bottom]
-        hot=set(hot)
-        # hot=set()
-        # for k,v in word_freq:
-        #     if v/total/(len(hot)+1)>=min_ratio/2**15:
-        #         hot.add(k)
-        chars = [k for k, v in word_freq if v/len(k) >= bottom_char and k not in hot]
-        # chars = [k for k, v in word_freq if len(k)==1 and v>= bottom_char and k not in hot]
-        # chars=[]
+            f"min_ratio:{min_ratio} min_freq:{min_freq} bottom:{bottom:.2f} vocab_size:{vocab_size}")
+        hot = set()
+        for k, v in word_freq:
+            if v >= bottom:
+                hot.add(k)
+                bottom_word = v
+            else:
+                break
+            if 0 < vocab_size < len(hot):
+                break
+        bottom_char = max(min_freq, bottom_word/4)
+        logger.info(f"  bottom_word:{bottom_word:.2f} bottom_char:{bottom_char:.2f}")
+        chars = [k for k, v in word_freq if len(k) == 1 and v >= bottom_char and k not in hot]
         root_words = self.never_split | hot | set(chars)
         logger.info(
             f" words:{len(word_freq)} hot:{len(hot)} chars:{len(chars)} root_words:{len(root_words)}")
+
         ziCutter = ZiCutter(folder)
-        ziCutter.build(folder,root_words)
+        ziCutter.build(folder, root_words)
         root_words |= set(ziCutter.vocab)
-        # for x in root_words:
-        #     assert x.strip()
         ziSegmenter = ZiSegmenter(root_words=root_words)
 
         logger.info("  === token_root ===  ")
         sample = random.choices(word_freq, k=5)
         for k, v in sample:
             [prefix, root, suffix] = ziSegmenter.token_root(k)
             row = [k, v, prefix, root, suffix]
@@ -121,32 +119,26 @@
             if not root:
                 continue
             if prefix:
                 prefix_counter[prefix] += v
             if suffix:
                 suffix_counter[suffix] += v
         del word_freq
-        prefixs = [k for k, v in prefix_counter.items() if v  >= bottom ]
+        prefixs = [k for k, v in prefix_counter.items() if v >= bottom_word]
         del prefix_counter
-        # for x in prefixs:
-        #     assert x.strip()
-        suffixs = [k for k, v in suffix_counter.items() if v  >= bottom ]
+        suffixs = [k for k, v in suffix_counter.items() if v >= bottom_word]
         del suffix_counter
-        # for x in suffixs:
-        #     assert x.strip()
         logger.info(
             f"root_words:{len(root_words)} prefixs:{len(prefixs)} suffixs:{len(suffixs)}")
 
         prefixs = [x+'--' for x in prefixs]
         root_words = [x for x in root_words]
         suffixs = ['--'+x for x in suffixs]
-        vocab = sorted(root_words)+sorted(prefixs)+sorted(suffixs)
-        # for x in vocab:
-        #     assert x.strip()        
-        vocab_path = os.path.join(folder,"vocab.txt")
+        vocab = self.UNKs + sorted(root_words)+sorted(prefixs)+sorted(suffixs)
+        vocab_path = os.path.join(folder, "vocab.txt")
         with open(vocab_path, 'w') as f:
             for x in vocab:
                 f.write(x+'\n')
         logger.info(f"save  vocab { len(vocab) }  -->{vocab_path} ")
         self.load(folder)
 
     def tokenize(self, line):
@@ -176,21 +168,24 @@
         indexs = self.tokens2indexs(tokens)
         return indexs
 
     def tokens2words(self, tokens):
         ts = tokens[:1]
         for i in range(1, len(tokens)):
             x = tokens[i]
-            if len(ts[-1]) > 1 and ts[-1][-2:] == '--':  # prefix
+            if ts[-1].endswith('--'):  # prefix
                 ts[-1] = ts[-1][:-2]+x
-                continue
-            if len(x) > 1 and x[:2] == '--':  # suffix
-                ts[-1] += x[1:]
-                continue
-            ts.append(x)
+            elif x.startswith('--'):  # suffix
+                ts[-1] += x[2:]
+            else:
+                ts.append(x)
         return ts
 
     def decode(self, indexs):
         tokens = self.indexs2tokens(indexs)
         ts = self.tokens2words(tokens)
-        words=self.ziCutter.combineWord(ts)
+        words = self.ziCutter.combineHanzi(ts)
         return words
+
+    def tokens2line(self, tokens):
+        line = self.unicodeTokenizer.detokenize(tokens)
+        return line
```

### Comparing `ZiTokenizer-0.0.7/ZiTokenizer.egg-info/PKG-INFO` & `ZiTokenizer-0.0.8/ZiTokenizer.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 Metadata-Version: 2.1
 Name: ZiTokenizer
-Version: 0.0.7
+Version: 0.0.8
 Summary: ZiTokenizer: tokenize world text as Zi
 Home-page: https://github.com/laohur/ZiCutter
 Author: laohur
 Author-email: laohur@gmail.com
 License: [Anti-996 License](https: // github.com/996icu/996.ICU/blob/master/LICENSE)
 Keywords: UnicodeTokenizer,ZiCutter,ZiTokenizer,Tokenizer,Unicode,laohur
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # ZiTokenizer
 
-ZiTokenizer: tokenize word as Zi
+Tokineze all languages text into Zi.
+
+support 300+ languages from wikipedia, including global 
 
-word => prefix + root + suffix
 
-support 325 languages + global, including global 
 ## use
 * pip install ZiTokenizer
-* toeknize language frequency and count word frequency (https://github.com/laohur/UnicodeTokenizer/blob/master/test/count_lang/count_word.py)
+
 ```python
 from ZiTokenizer.ZiTokenizer import ZiTokenizer
 
 # use
-tokenizer = ZiTokenizer(lang="global")  # lang='ar', 'en', 'fr', 'ru', 'zh' ...
-line = "'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)熵😀'\x0000熇"
-tokens = tokenizer.tokenize(line)
-print(' '.join(tokens)) # ' 〇 ㎡ [ ค ณ-- จ-- ะ --จ ด-- พ ธ แต ง-- งา-- น-- เม อไ-- ร --ค --ะ ] ##s ht pays - g [ ran ] d - blanc - eleve » ( 白 高 大 夏 國 ) ⿰ 火 商 ##g ce ' 00 ⿰ 火 高
-
-# build 
-tokenizer = ZiTokenizer(mydir) # mydir include "word_frequency.tsv"
-tokenizer.build(min_ratio=1.5e-6, min_freq=3)
-tokenizer = ZiTokenizer(dir=mydir)
+tokenizer = ZiTokenizer()  
+line = "'〇㎡[คุณจะจัดพิธีแต่งงานเมื่อไรคะัีิ์ื็ํึ]Ⅷpays-g[ran]d-blanc-élevé » (白高大夏國)😀熇'\x0000𧭏2022２０１９\U0010ffff"
+indexs = tokenizer.encode(line)
+tokens = tokenizer.decode(indexs)
+line2=tokenizer.tokens2line(tokens)
 
+# build
+demo/unit.py
 ```
+
+## UnicodeTokenizer
+basic tokeinzer
+
+## ZiCutter
+汉字拆字
+> '瞼' -> ['⿰', '目', '僉']
+
+## ZiSegmenter
+word => prefix + root + suffix
+> 'modernbritishdo' -> ['mod--', 'er--', 'n--', 'british', '--do']
+
+## languages
+default using "golabl" vocob, others from https://laohur.github.io/ZiTokenizer/index.html
+> tokenizer = ZiTokenizer(vocab_dir)
```

### Comparing `ZiTokenizer-0.0.7/setup.py` & `ZiTokenizer-0.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = f.read()
 
 
 setup(
     name="ZiTokenizer",
     packages=find_packages(),
     # py_modules = ['ZiTokenizer.UnicodeTokenizer', 'ZiTokenizer.ZiCutter', 'ZiTokenizer.ZiTokenizer', 'ZiTokenizer.ZiSegmenter'],
-    version='0.0.7',
+    version='0.0.8',
     description='ZiTokenizer: tokenize world text as Zi',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.0',
     install_requires=[
         "logzero",
         # "UnicodeTokenizer",
```

