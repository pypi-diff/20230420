# Comparing `tmp/thunno2-2.1.2.tar.gz` & `tmp/thunno2-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.1.2.tar", last modified: Sun Apr 16 13:16:53 2023, max compression
+gzip compressed data, was "thunno2-2.1.3.tar", last modified: Thu Apr 20 18:19:43 2023, max compression
```

## Comparing `thunno2-2.1.2.tar` & `thunno2-2.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.900194 thunno2-2.1.2/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:16:53.900065 thunno2-2.1.2/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-16 13:16:53.900233 thunno2-2.1.2/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.1.2/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.899308 thunno2-2.1.2/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.2/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.1.2/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    46724 2023-04-16 13:00:29.000000 thunno2-2.1.2/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2971 2023-04-15 15:28:56.000000 thunno2-2.1.2/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   245338 2023-04-16 13:14:34.000000 thunno2-2.1.2/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     6066 2023-04-14 19:12:18.000000 thunno2-2.1.2/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    48354 2023-04-16 13:14:16.000000 thunno2-2.1.2/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    25876 2023-04-15 15:28:56.000000 thunno2-2.1.2/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    22512 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    62753 2023-04-16 13:14:34.000000 thunno2-2.1.2/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     3274 2023-04-15 17:55:44.000000 thunno2-2.1.2/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-16 13:16:42.000000 thunno2-2.1.2/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-16 13:16:53.899897 thunno2-2.1.2/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-16 13:16:53.000000 thunno2-2.1.2/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-20 18:19:43.655744 thunno2-2.1.3/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-20 18:19:43.655619 thunno2-2.1.3/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-20 18:19:43.655784 thunno2-2.1.3/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1314 2023-04-16 17:25:02.000000 thunno2-2.1.3/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-20 18:19:43.654894 thunno2-2.1.3/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.1.3/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1393 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    49577 2023-04-20 18:13:59.000000 thunno2-2.1.3/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2950 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245360 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     6508 2023-04-17 19:22:08.000000 thunno2-2.1.3/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    48587 2023-04-20 18:13:59.000000 thunno2-2.1.3/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    26276 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    23076 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1675 2023-04-16 17:25:02.000000 thunno2-2.1.3/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62574 2023-04-20 18:13:59.000000 thunno2-2.1.3/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     3537 2023-04-17 16:14:57.000000 thunno2-2.1.3/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-20 18:19:25.000000 thunno2-2.1.3/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-20 18:19:43.655457 thunno2-2.1.3/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-20 18:19:43.000000 thunno2-2.1.3/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-20 18:19:43.000000 thunno2-2.1.3/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-20 18:19:43.000000 thunno2-2.1.3/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-20 18:19:43.000000 thunno2-2.1.3/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-20 18:19:43.000000 thunno2-2.1.3/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.1.2/PKG-INFO` & `thunno2-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.2
+Version: 2.1.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.2.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.3.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.1.2/setup.py` & `thunno2-2.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 from setuptools import setup, find_packages
 from thunno2 import version
 
-long_description = 'Thunno is a golfing language written in Python. Learn more at https://github.com/Thunno/Thunno2'
+long_description = "Thunno is a golfing language written in Python. Learn more at https://github.com/Thunno/Thunno2"
 
 setup(
-    name='thunno2',
+    name="thunno2",
     version=version.THUNNO_VERSION,
-    license='MIT',
-    description='A golfing language',
-    author='Rujul Nayak',
-    author_email='rujulnayak@outlook.com',
-    url='https://github.com/Thunno/Thunno2',
-    download_url=f'https://github.com/Thunno/Thunno2/archive/refs/tags/v{version.THUNNO_VERSION}.tar.gz',
-    keywords=['golfing', 'code-golf', 'language'],
-    install_requires=[
-    ],
+    license="MIT",
+    description="A golfing language",
+    author="Rujul Nayak",
+    author_email="rujulnayak@outlook.com",
+    url="https://github.com/Thunno/Thunno2",
+    download_url=f"https://github.com/Thunno/Thunno2/archive/refs/tags/v{version.THUNNO_VERSION}.tar.gz",
+    keywords=["golfing", "code-golf", "language"],
+    install_requires=[],
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     long_description=long_description,
-    long_description_content_type='text/x-rst',
+    long_description_content_type="text/x-rst",
     packages=find_packages(),
-    entry_points={
-        'console_scripts': [
-            'thunno2 = thunno2.run:from_cmdline'
-        ]
-    }
+    entry_points={"console_scripts": ["thunno2 = thunno2.run:from_cmdline"]},
 )
```

### Comparing `thunno2-2.1.2/thunno2/codepage.py` & `thunno2-2.1.3/thunno2/codepage.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # This codepage is exactly the same as the Jelly codepage
 # (https://github.com/DennisMitchell/jellylanguage/blob/master/jelly/interpreter.py#L7)
 
 """The 256-character Single Byte Character Set for encoding Thunno 2 programs (https://en.wikipedia.org/wiki/SBCS)"""
 
-CODEPAGE = r'''¡¢£¤¥¦©¬®µ½¿€ÆÇÐÑ×ØŒÞßæçðıȷñ÷øœþ !"#$%&'()*+,-./0123456789:;<=>?''' \
-           r'''@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~¶''' \
-           r'''°¹²³⁴⁵⁶⁷⁸⁹⁺⁻⁼⁽⁾ƁƇƊƑƓƘⱮƝƤƬƲȤɓƈɗƒɠɦƙɱɲƥʠɼʂƭʋȥẠḄḌẸḤỊḲḶṂṆỌṚṢṬỤṾẈỴẒȦḂ''' \
-           r'''ĊḊĖḞĠḢİĿṀṄȮṖṘṠṪẆẊẎŻạḅḍẹḥịḳḷṃṇọṛṣṭ§Äẉỵẓȧḃċḋėḟġḣŀṁṅȯṗṙṡṫẇẋẏż«»‘’“”'''
+CODEPAGE = (
+    r"""¡¢£¤¥¦©¬®µ½¿€ÆÇÐÑ×ØŒÞßæçðıȷñ÷øœþ !"#$%&'()*+,-./0123456789:;<=>?"""
+    r"""@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~¶"""
+    r"""°¹²³⁴⁵⁶⁷⁸⁹⁺⁻⁼⁽⁾ƁƇƊƑƓƘⱮƝƤƬƲȤɓƈɗƒɠɦƙɱɲƥʠɼʂƭʋȥẠḄḌẸḤỊḲḶṂṆỌṚṢṬỤṾẈỴẒȦḂ"""
+    r"""ĊḊĖḞĠḢİĿṀṄȮṖṘṠṪẆẊẎŻạḅḍẹḥịḳḷṃṇọṛṣṭ§Äẉỵẓȧḃċḋėḟġḣŀṁṅȯṗṙṡṫẇẋẏż«»‘’“”"""
+)
 
 assert len(CODEPAGE) == 256
 
 
 def codepage_index(*chars):
     for char in chars:
         if char in CODEPAGE:
             yield CODEPAGE.index(char)
         else:
             yield -1
 
 
 def utf8_to_thunno2(string):
-    ret = ''
+    ret = ""
     for char in string:
         if ord(char) < 256:
             ret += CODEPAGE[ord(char)]
         else:
             ret += char
     return ret
 
 
 def thunno2_to_utf8(string):
-    ret = ''
+    ret = ""
     for char in string:
         if char in CODEPAGE:
             ret += chr(CODEPAGE.index(char))
         else:
             ret += char
     return ret
```

### Comparing `thunno2-2.1.2/thunno2/dictionary.py` & `thunno2-2.1.3/thunno2/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -15241,94 +15241,95 @@
 0003b880: 6875 6e6e 6f32 2069 6d70 6f72 7420 636f  hunno2 import co
 0003b890: 6465 7061 6765 0a66 726f 6d20 7468 756e  depage.from thun
 0003b8a0: 6e6f 3220 696d 706f 7274 2068 656c 7065  no2 import helpe
 0003b8b0: 7273 0a69 6d70 6f72 7420 7374 7269 6e67  rs.import string
 0003b8c0: 2c20 7265 0a0a 6967 6e6f 7265 5f63 6861  , re..ignore_cha
 0003b8d0: 7273 203d 2073 7472 696e 672e 6173 6369  rs = string.asci
 0003b8e0: 695f 6c65 7474 6572 7320 2b20 7374 7269  i_letters + stri
-0003b8f0: 6e67 2e64 6967 6974 7320 2b20 7227 2727  ng.digits + r'''
+0003b8f0: 6e67 2e64 6967 6974 7320 2b20 7222 2222  ng.digits + r"""
 0003b900: 2e2c 213f 3a5c 2227 2528 2920 e280 98e2  .,!?:\"'%() ....
-0003b910: 8099 2727 270a 6469 6374 696f 6e61 7279  ..'''.dictionary
-0003b920: 5f63 6f64 6570 6167 6520 3d20 2727 2e6a  _codepage = ''.j
-0003b930: 6f69 6e28 6368 6172 2066 6f72 2063 6861  oin(char for cha
-0003b940: 7220 696e 2063 6f64 6570 6167 652e 434f  r in codepage.CO
-0003b950: 4445 5041 4745 2069 6620 6368 6172 206e  DEPAGE if char n
-0003b960: 6f74 2069 6e20 6967 6e6f 7265 5f63 6861  ot in ignore_cha
-0003b970: 7273 290a 0a61 7373 6572 7420 6c65 6e28  rs)..assert len(
-0003b980: 6469 6374 696f 6e61 7279 5f63 6f64 6570  dictionary_codep
-0003b990: 6167 6529 203d 3d20 3138 300a 0a0a 6465  age) == 180...de
-0003b9a0: 6620 6469 6374 696f 6e61 7279 5f63 6f6d  f dictionary_com
-0003b9b0: 7072 6573 735f 776f 7264 2877 6f72 6429  press_word(word)
-0003b9c0: 3a0a 2020 2020 6966 2077 6f72 6420 6e6f  :.    if word no
-0003b9d0: 7420 696e 2077 6f72 6473 3a0a 2020 2020  t in words:.    
-0003b9e0: 2020 2020 7265 7475 726e 202d 310a 2020      return -1.  
-0003b9f0: 2020 696e 6465 7820 3d20 776f 7264 732e    index = words.
-0003ba00: 696e 6465 7828 776f 7264 290a 2020 2020  index(word).    
-0003ba10: 6261 7365 5f31 3830 5f6e 756d 203d 2068  base_180_num = h
-0003ba20: 656c 7065 7273 2e6e 756d 6265 725f 746f  elpers.number_to
-0003ba30: 5f62 6173 655f 6469 6769 7473 2869 6e64  _base_digits(ind
-0003ba40: 6578 2c20 3138 3029 0a20 2020 2072 6574  ex, 180).    ret
-0003ba50: 7572 6e20 2727 2e6a 6f69 6e28 6d61 7028  urn ''.join(map(
-0003ba60: 6469 6374 696f 6e61 7279 5f63 6f64 6570  dictionary_codep
-0003ba70: 6167 652e 5f5f 6765 7469 7465 6d5f 5f2c  age.__getitem__,
-0003ba80: 2062 6173 655f 3138 305f 6e75 6d29 292e   base_180_num)).
-0003ba90: 726a 7573 7428 322c 2027 c2a1 2729 0a0a  rjust(2, '..')..
-0003baa0: 0a64 6566 2064 6963 7469 6f6e 6172 795f  .def dictionary_
-0003bab0: 6465 636f 6d70 7265 7373 5f73 7472 696e  decompress_strin
-0003bac0: 6728 7329 3a0a 2020 2020 6261 7365 5f31  g(s):.    base_1
-0003bad0: 3830 5f6e 756d 203d 205b 2a6d 6170 2864  80_num = [*map(d
-0003bae0: 6963 7469 6f6e 6172 795f 636f 6465 7061  ictionary_codepa
-0003baf0: 6765 2e69 6e64 6578 2c20 7329 5d0a 2020  ge.index, s)].  
-0003bb00: 2020 696e 6465 7820 3d20 6865 6c70 6572    index = helper
-0003bb10: 732e 6672 6f6d 5f6c 6973 745f 6f66 5f64  s.from_list_of_d
-0003bb20: 6967 6974 735f 3228 6261 7365 5f31 3830  igits_2(base_180
-0003bb30: 5f6e 756d 2c20 3138 3029 0a20 2020 2072  _num, 180).    r
-0003bb40: 6574 7572 6e20 776f 7264 735b 696e 6465  eturn words[inde
-0003bb50: 785d 0a0a 0a64 6566 2062 6163 6b73 6c61  x]...def backsla
-0003bb60: 7368 6966 7928 7329 3a0a 2020 2020 7220  shify(s):.    r 
-0003bb70: 3d20 2727 0a20 2020 2066 6f72 2063 2069  = ''.    for c i
-0003bb80: 6e20 733a 0a20 2020 2020 2020 2069 6620  n s:.        if 
-0003bb90: 6320 696e 2064 6963 7469 6f6e 6172 795f  c in dictionary_
-0003bba0: 636f 6465 7061 6765 202b 2027 5c5c 273a  codepage + '\\':
-0003bbb0: 0a20 2020 2020 2020 2020 2020 2072 202b  .            r +
-0003bbc0: 3d20 275c 5c27 202b 2063 0a20 2020 2020  = '\\' + c.     
-0003bbd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0003bbe0: 2020 2020 2072 202b 3d20 630a 2020 2020       r += c.    
-0003bbf0: 7265 7475 726e 2072 0a0a 0a64 6566 206f  return r...def o
-0003bc00: 7074 696d 616c 5f64 6963 7469 6f6e 6172  ptimal_dictionar
-0003bc10: 795f 636f 6d70 7265 7373 696f 6e28 7329  y_compression(s)
-0003bc20: 3a0a 2020 2020 7773 203d 2072 652e 6669  :.    ws = re.fi
-0003bc30: 6e64 616c 6c28 2728 5b61 2d7a 5d2a 2928  ndall('([a-z]*)(
-0003bc40: 5b5e 612d 7a5d 2a29 272c 2073 7472 2873  [^a-z]*)', str(s
-0003bc50: 292e 6c6f 7765 7228 2929 0a20 2020 2072  ).lower()).    r
-0003bc60: 6574 203d 2027 270a 2020 2020 666f 7220  et = ''.    for 
-0003bc70: 776f 7264 2c20 6f74 6865 725f 7374 7566  word, other_stuf
-0003bc80: 6620 696e 2077 733a 0a20 2020 2020 2020  f in ws:.       
-0003bc90: 2069 6620 6e6f 7420 2877 6f72 6420 2b20   if not (word + 
-0003bca0: 6f74 6865 725f 7374 7566 6629 3a0a 2020  other_stuff):.  
-0003bcb0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0003bcc0: 7565 0a20 2020 2020 2020 2063 6f6d 7072  ue.        compr
-0003bcd0: 6573 7369 6f6e 7320 3d20 5b5d 0a20 2020  essions = [].   
-0003bce0: 2020 2020 2066 6f72 2078 2069 6e20 6865       for x in he
-0003bcf0: 6c70 6572 732e 616c 6c5f 736c 6963 6573  lpers.all_slices
-0003bd00: 2877 6f72 6429 3a0a 2020 2020 2020 2020  (word):.        
-0003bd10: 2020 2020 636f 6d70 7265 7373 696f 6e73      compressions
-0003bd20: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
-0003bd30: 2020 2020 2020 2020 2027 272e 6a6f 696e           ''.join
-0003bd40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0003bd50: 2020 2020 2020 6469 6374 696f 6e61 7279        dictionary
-0003bd60: 5f63 6f6d 7072 6573 735f 776f 7264 2877  _compress_word(w
-0003bd70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0003bd80: 2020 2020 2020 6966 2064 6963 7469 6f6e        if diction
-0003bd90: 6172 795f 636f 6d70 7265 7373 5f77 6f72  ary_compress_wor
-0003bda0: 6428 7729 2021 3d20 2d31 0a20 2020 2020  d(w) != -1.     
-0003bdb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0003bdc0: 6c73 6520 770a 2020 2020 2020 2020 2020  lse w.          
-0003bdd0: 2020 2020 2020 2020 2020 666f 7220 7720            for w 
-0003bde0: 696e 2078 0a20 2020 2020 2020 2020 2020  in x.           
-0003bdf0: 2020 2020 2029 202b 2062 6163 6b73 6c61       ) + backsla
-0003be00: 7368 6966 7928 6f74 6865 725f 7374 7566  shify(other_stuf
-0003be10: 6629 0a20 2020 2020 2020 2020 2020 2029  f).            )
-0003be20: 0a20 2020 2020 2020 2072 6574 202b 3d20  .        ret += 
-0003be30: 6d69 6e28 636f 6d70 7265 7373 696f 6e73  min(compressions
-0003be40: 2c20 6b65 793d 6c65 6e29 0a20 2020 2072  , key=len).    r
-0003be50: 6574 7572 6e20 7265 740a                 eturn ret.
+0003b910: 8099 2222 220a 6469 6374 696f 6e61 7279  ..""".dictionary
+0003b920: 5f63 6f64 6570 6167 6520 3d20 2222 2e6a  _codepage = "".j
+0003b930: 6f69 6e28 0a20 2020 2063 6861 7220 666f  oin(.    char fo
+0003b940: 7220 6368 6172 2069 6e20 636f 6465 7061  r char in codepa
+0003b950: 6765 2e43 4f44 4550 4147 4520 6966 2063  ge.CODEPAGE if c
+0003b960: 6861 7220 6e6f 7420 696e 2069 676e 6f72  har not in ignor
+0003b970: 655f 6368 6172 730a 290a 0a61 7373 6572  e_chars.)..asser
+0003b980: 7420 6c65 6e28 6469 6374 696f 6e61 7279  t len(dictionary
+0003b990: 5f63 6f64 6570 6167 6529 203d 3d20 3138  _codepage) == 18
+0003b9a0: 300a 0a0a 6465 6620 6469 6374 696f 6e61  0...def dictiona
+0003b9b0: 7279 5f63 6f6d 7072 6573 735f 776f 7264  ry_compress_word
+0003b9c0: 2877 6f72 6429 3a0a 2020 2020 6966 2077  (word):.    if w
+0003b9d0: 6f72 6420 6e6f 7420 696e 2077 6f72 6473  ord not in words
+0003b9e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0003b9f0: 202d 310a 2020 2020 696e 6465 7820 3d20   -1.    index = 
+0003ba00: 776f 7264 732e 696e 6465 7828 776f 7264  words.index(word
+0003ba10: 290a 2020 2020 6261 7365 5f31 3830 5f6e  ).    base_180_n
+0003ba20: 756d 203d 2068 656c 7065 7273 2e6e 756d  um = helpers.num
+0003ba30: 6265 725f 746f 5f62 6173 655f 6469 6769  ber_to_base_digi
+0003ba40: 7473 2869 6e64 6578 2c20 3138 3029 0a20  ts(index, 180). 
+0003ba50: 2020 2072 6574 7572 6e20 2222 2e6a 6f69     return "".joi
+0003ba60: 6e28 6d61 7028 6469 6374 696f 6e61 7279  n(map(dictionary
+0003ba70: 5f63 6f64 6570 6167 652e 5f5f 6765 7469  _codepage.__geti
+0003ba80: 7465 6d5f 5f2c 2062 6173 655f 3138 305f  tem__, base_180_
+0003ba90: 6e75 6d29 292e 726a 7573 7428 322c 2022  num)).rjust(2, "
+0003baa0: c2a1 2229 0a0a 0a64 6566 2064 6963 7469  ..")...def dicti
+0003bab0: 6f6e 6172 795f 6465 636f 6d70 7265 7373  onary_decompress
+0003bac0: 5f73 7472 696e 6728 7329 3a0a 2020 2020  _string(s):.    
+0003bad0: 6261 7365 5f31 3830 5f6e 756d 203d 205b  base_180_num = [
+0003bae0: 2a6d 6170 2864 6963 7469 6f6e 6172 795f  *map(dictionary_
+0003baf0: 636f 6465 7061 6765 2e69 6e64 6578 2c20  codepage.index, 
+0003bb00: 7329 5d0a 2020 2020 696e 6465 7820 3d20  s)].    index = 
+0003bb10: 6865 6c70 6572 732e 6672 6f6d 5f6c 6973  helpers.from_lis
+0003bb20: 745f 6f66 5f64 6967 6974 735f 3228 6261  t_of_digits_2(ba
+0003bb30: 7365 5f31 3830 5f6e 756d 2c20 3138 3029  se_180_num, 180)
+0003bb40: 0a20 2020 2072 6574 7572 6e20 776f 7264  .    return word
+0003bb50: 735b 696e 6465 785d 0a0a 0a64 6566 2062  s[index]...def b
+0003bb60: 6163 6b73 6c61 7368 6966 7928 7329 3a0a  ackslashify(s):.
+0003bb70: 2020 2020 7220 3d20 2222 0a20 2020 2066      r = "".    f
+0003bb80: 6f72 2063 2069 6e20 733a 0a20 2020 2020  or c in s:.     
+0003bb90: 2020 2069 6620 6320 696e 2064 6963 7469     if c in dicti
+0003bba0: 6f6e 6172 795f 636f 6465 7061 6765 202b  onary_codepage +
+0003bbb0: 2022 5c5c 223a 0a20 2020 2020 2020 2020   "\\":.         
+0003bbc0: 2020 2072 202b 3d20 225c 5c22 202b 2063     r += "\\" + c
+0003bbd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0003bbe0: 2020 2020 2020 2020 2020 2072 202b 3d20             r += 
+0003bbf0: 630a 2020 2020 7265 7475 726e 2072 0a0a  c.    return r..
+0003bc00: 0a64 6566 206f 7074 696d 616c 5f64 6963  .def optimal_dic
+0003bc10: 7469 6f6e 6172 795f 636f 6d70 7265 7373  tionary_compress
+0003bc20: 696f 6e28 7329 3a0a 2020 2020 7773 203d  ion(s):.    ws =
+0003bc30: 2072 652e 6669 6e64 616c 6c28 2228 5b61   re.findall("([a
+0003bc40: 2d7a 5d2a 2928 5b5e 612d 7a5d 2a29 222c  -z]*)([^a-z]*)",
+0003bc50: 2073 7472 2873 292e 6c6f 7765 7228 2929   str(s).lower())
+0003bc60: 0a20 2020 2072 6574 203d 2022 220a 2020  .    ret = "".  
+0003bc70: 2020 666f 7220 776f 7264 2c20 6f74 6865    for word, othe
+0003bc80: 725f 7374 7566 6620 696e 2077 733a 0a20  r_stuff in ws:. 
+0003bc90: 2020 2020 2020 2069 6620 6e6f 7420 2877         if not (w
+0003bca0: 6f72 6420 2b20 6f74 6865 725f 7374 7566  ord + other_stuf
+0003bcb0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0003bcc0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+0003bcd0: 2063 6f6d 7072 6573 7369 6f6e 7320 3d20   compressions = 
+0003bce0: 5b5d 0a20 2020 2020 2020 2066 6f72 2078  [].        for x
+0003bcf0: 2069 6e20 6865 6c70 6572 732e 616c 6c5f   in helpers.all_
+0003bd00: 736c 6963 6573 2877 6f72 6429 3a0a 2020  slices(word):.  
+0003bd10: 2020 2020 2020 2020 2020 636f 6d70 7265            compre
+0003bd20: 7373 696f 6e73 2e61 7070 656e 6428 0a20  ssions.append(. 
+0003bd30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0003bd40: 222e 6a6f 696e 280a 2020 2020 2020 2020  ".join(.        
+0003bd50: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+0003bd60: 696f 6e61 7279 5f63 6f6d 7072 6573 735f  ionary_compress_
+0003bd70: 776f 7264 2877 290a 2020 2020 2020 2020  word(w).        
+0003bd80: 2020 2020 2020 2020 2020 2020 6966 2064              if d
+0003bd90: 6963 7469 6f6e 6172 795f 636f 6d70 7265  ictionary_compre
+0003bda0: 7373 5f77 6f72 6428 7729 2021 3d20 2d31  ss_word(w) != -1
+0003bdb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003bdc0: 2020 2020 2065 6c73 6520 770a 2020 2020       else w.    
+0003bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0003bde0: 666f 7220 7720 696e 2078 0a20 2020 2020  for w in x.     
+0003bdf0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0003be00: 2020 2020 2020 2020 2020 2020 202b 2062               + b
+0003be10: 6163 6b73 6c61 7368 6966 7928 6f74 6865  ackslashify(othe
+0003be20: 725f 7374 7566 6629 0a20 2020 2020 2020  r_stuff).       
+0003be30: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
+0003be40: 6574 202b 3d20 6d69 6e28 636f 6d70 7265  et += min(compre
+0003be50: 7373 696f 6e73 2c20 6b65 793d 6c65 6e29  ssions, key=len)
+0003be60: 0a20 2020 2072 6574 7572 6e20 7265 740a  .    return ret.
```

### Comparing `thunno2-2.1.2/thunno2/flags.py` & `thunno2-2.1.3/thunno2/flags.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from thunno2 import interpreter, commands, helpers
 import re
 
 
 def process_input_flags(flags, inputs):
-
-    if 'w' in flags:
+    if "w" in flags:
         commands.ctx.warnings = True
 
-    if 'W' in flags:
+    if "W" in flags:
         inputs = [inputs]
     else:
         inputs = inputs.splitlines()
 
-    if 'E' not in flags:
+    if "E" not in flags:
         new_input = []
         for inp in inputs:
             try:
                 x = eval(inp)
                 if type(x) in (int, float, str, list):
                     new_input.append(x)
                 elif isinstance(x, bool):
@@ -28,163 +27,176 @@
                 else:
                     new_input.append(inp)
             except:
                 new_input.append(inp)
         inputs = new_input[:]
 
     for flag in flags:
-        if flag == 'Z':
+        if flag == "Z":
             commands.ctx.stack.push(0)
-        elif flag == 'T':
+        elif flag == "T":
             commands.ctx.stack.push(10)
-        elif flag == 'H':
+        elif flag == "H":
             commands.ctx.stack.push(100)
 
-    if 'B' in flags:
+    if "B" in flags:
         new_input = []
         for inp in inputs:
             if isinstance(inp, str):
                 new_input.append([ord(c) for c in inp])
             else:
                 new_input.append(inp)
         inputs = new_input[:]
 
-    if '+' in flags:
+    if "+" in flags:
         new_input = []
         for inp in inputs:
             if isinstance(inp, (int, float)):
-                new_input.append(inp + flags.count('+'))
+                new_input.append(inp + flags.count("+"))
             else:
                 new_input.append(inp)
         inputs = new_input[:]
 
-    if '-' in flags:
+    if "-" in flags:
         new_input = []
         for inp in inputs:
             if isinstance(inp, (int, float)):
-                new_input.append(inp - flags.count('-'))
+                new_input.append(inp - flags.count("-"))
             else:
                 new_input.append(inp)
         inputs = new_input[:]
 
     return inputs
 
 
 def process_output_flags(flags, do_print=True):
-
     for flag in flags:
-
-        if 'J' == flag:
+        if "J" == flag:
             commands.ctx.stack.push(helpers.empty_join(next(commands.ctx.stack.rmv(1))))
 
-        if 'j' == flag:
+        if "j" == flag:
             commands.ctx.stack.push(helpers.empty_join(list(commands.ctx.stack)))
 
-        if 'N' == flag:
-            commands.ctx.stack.push(helpers.newline_join(next(commands.ctx.stack.rmv(1))))
+        if "N" == flag:
+            commands.ctx.stack.push(
+                helpers.newline_join(next(commands.ctx.stack.rmv(1)))
+            )
 
-        if 'n' == flag:
+        if "n" == flag:
             commands.ctx.stack.push(helpers.newline_join(list(commands.ctx.stack)))
 
-        if 'Ṡ' == flag:
+        if "Ṡ" == flag:
             commands.ctx.stack.push(helpers.space_join(next(commands.ctx.stack.rmv(1))))
 
-        if 'ṡ' == flag:
+        if "ṡ" == flag:
             commands.ctx.stack.push(helpers.space_join(list(commands.ctx.stack)))
 
-        if 'S' == flag:
-            commands.ctx.stack.push(commands.commands['S']()[0])
+        if "S" == flag:
+            commands.ctx.stack.push(commands.commands["S"]()[0])
 
-        if 's' == flag:
+        if "s" == flag:
             commands.ctx.stack.push(helpers.it_sum(commands.ctx.stack))
 
-        if 'L' == flag:
-            commands.ctx.stack.push(commands.commands['l']()[0])
+        if "L" == flag:
+            commands.ctx.stack.push(commands.commands["l"]()[0])
 
-        if 'l' == flag:
+        if "l" == flag:
             commands.ctx.stack.push(len(commands.ctx.stack))
 
-        if 'h' == flag:
-            commands.ctx.stack.push(commands.commands['h']()[0])
+        if "h" == flag:
+            commands.ctx.stack.push(commands.commands["h"]()[0])
 
-        if 't' == flag:
-            commands.ctx.stack.push(commands.commands['t']()[0])
+        if "t" == flag:
+            commands.ctx.stack.push(commands.commands["t"]()[0])
 
-        if 'B' == flag:
+        if "B" == flag:
             x = (commands.ctx.stack + commands.ctx.other_il + [0])[0]
             if isinstance(x, list):
-                r = ''
+                r = ""
                 for i in x:
                     try:
                         r += chr(int(i))
                     except:
                         pass
                 commands.ctx.stack.push(r)
 
+        if "G" == flag:
+            commands.ctx.stack.push(commands.commands["G"]()[0])
+
+        if "M" == flag:
+            commands.ctx.stack.push(commands.commands["M"]()[0])
+
+        if "b" == flag:
+            commands.ctx.stack.push(commands.commands["ɓ"]()[0])
+
+        if "!" == flag:
+            commands.ctx.stack.push(commands.commands["¬"]()[0])
+
     if do_print:
         do_printing(flags)
 
 
 def do_printing(flags):
-    if (commands.ctx.implicit_print or ('O' in flags)) and not ('o' in flags):
+    if (commands.ctx.implicit_print or ("O" in flags)) and not ("o" in flags):
         print(next(commands.ctx.stack.rmv(1)))
 
 
 def run(flags, code, inputs):
-
-    if 'V' in flags:
-        new_flags = ''.join(f for f in flags if f != 'V')
+    if "V" in flags:
+        new_flags = "".join(f for f in flags if f != "V")
         for line in inputs.splitlines():
             try:
                 x = eval(line)
                 if isinstance(x, tuple):
-                    new_inputs = process_input_flags(new_flags, '\n'.join(map(repr, x)))
+                    new_inputs = process_input_flags(new_flags, "\n".join(map(repr, x)))
                 else:
                     new_inputs = [x]
             except:
                 new_inputs = [line]
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
-            print(line, '--> ', end='')
+            print(line, "--> ", end="")
             interpreter.run(code, n=0, iteration_index=0)
             process_output_flags(new_flags)
         return None
 
-    elif 'C' in flags:
-        new_flags = ''.join(f for f in flags if f != 'C')
+    elif "C" in flags:
+        new_flags = "".join(f for f in flags if f != "C")
         for l in inputs.splitlines():
             m = re.match(r"(.+) ?(?:=>|-+>) ?(.+)", l)
             try:
                 line, output = m[1], m[2]
                 try:
                     x = eval(line)
                     if isinstance(x, tuple):
-                        new_inputs = process_input_flags(new_flags, '\n'.join(map(repr, x)))
+                        new_inputs = process_input_flags(
+                            new_flags, "\n".join(map(repr, x))
+                        )
                     else:
                         new_inputs = [x]
                 except:
                     new_inputs = [line]
                 try:
-                    expected = process_input_flags('', output)[0]
+                    expected = process_input_flags("", output)[0]
                 except:
                     expected = output.strip()
             except Exception as e:
-                print(f'FAIL ❌ (Got error {e})')
+                print(f"FAIL ❌ (Got error {e})")
                 continue
             commands.ctx.og_input_list = new_inputs.copy()
             commands.ctx.other_il = new_inputs.copy()
-            print(line, '--> ', end='')
+            print(line, "--> ", end="")
             interpreter.run(code, n=0, iteration_index=0)
             process_output_flags(new_flags, False)
             actual_output = next(commands.ctx.stack.rmv(1))
-            print(actual_output, end='\t')
+            print(actual_output, end="\t")
             if actual_output == expected:
-                print('PASS ✅')
+                print("PASS ✅")
             else:
-                print(f'FAIL ❌ (Expected {expected})')
+                print(f"FAIL ❌ (Expected {expected})")
         return None
 
     inputs = process_input_flags(flags, inputs)
     commands.ctx.og_input_list = inputs.copy()
     commands.ctx.other_il = inputs.copy()
     interpreter.run(code, n=0, iteration_index=0)
     process_output_flags(flags)
```

### Comparing `thunno2-2.1.2/thunno2/helpers.py` & `thunno2-2.1.3/thunno2/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,52 +171,52 @@
 
 
 def number_to_base(base, num):
     num, base = int(num), int(base)
     if base <= 0:
         return str(num)
     if base == 1:
-        return num * '0'
+        return num * "0"
     return number_to_base_digits(num, base)
 
 
 def ntbs(b, n):
     r = number_to_base_digits(n, b)
     if b <= 64:
-        digits = string.digits + string.ascii_uppercase + string.ascii_lowercase + '+/'
+        digits = string.digits + string.ascii_uppercase + string.ascii_lowercase + "+/"
     else:
         digits = codepage.CODEPAGE * math.ceil(b / 256)
-    return ''.join(map(digits.__getitem__, r))
+    return "".join(map(digits.__getitem__, r))
 
 
 def to_custom_base_string(base, num):
     num = int(num)
     if len(base) == 0:
         return str(num)
     if len(base) == 1:
         return num * base
-    return ''.join(map(base.__getitem__, number_to_base_digits(num, len(base))))
+    return "".join(map(base.__getitem__, number_to_base_digits(num, len(base))))
 
 
 def length_to_base(base, s):
     base = int(base)
     if base <= 0:
         return str(len(s))
     if base == 1:
-        return len(s) * '0'
+        return len(s) * "0"
     return number_to_base_digits(len(s), base)
 
 
 def length_custom_base_string(str2, str1):
     num = len(str1)
     if len(str2) == 0:
         return str(num)
     if len(str2) == 1:
-        return num * '0'
-    return ''.join(map(str2.__getitem__, number_to_base_digits(len(str1), len(str2))))
+        return num * "0"
+    return "".join(map(str2.__getitem__, number_to_base_digits(len(str1), len(str2))))
 
 
 def pass_(*args):
     return args[::-1]
 
 
 def from_list_of_digits_2(num, base):
@@ -237,15 +237,15 @@
 
 
 def ord2(s):
     return [ord(c) for c in s]
 
 
 def digits(num):
-    return [int(d) for d in str(num) if d in '0123456789']
+    return [int(d) for d in str(num) if d in "0123456789"]
 
 
 def is_even(num):
     return int(num % 2 == 0)
 
 
 def eval2(s):
@@ -261,15 +261,15 @@
 
 
 def substrings(s):
     return [s[i:j] for i in range(len(s)) for j in range(i + 1, len(s) + 1)]
 
 
 def max2(num):
-    return max(int(d) for d in str(num) if d in '0123456789')
+    return max(int(d) for d in str(num) if d in "0123456789")
 
 
 def max3(x):
     try:
         return max(x)
     except:
         return x
@@ -310,55 +310,55 @@
             r.append(j)
         return r
     elif len(lst1) > len(lst2):
         r = []
         for i, j in zip(lst2, lst1):
             r.append(i)
             r.append(j)
-        r.extend(lst1[len(lst2):])
+        r.extend(lst1[len(lst2) :])
         return r
     else:
         r = []
         for i, j in zip(lst2, lst1):
             r.append(i)
             r.append(j)
-        r.extend(lst2[len(lst1):])
+        r.extend(lst2[len(lst1) :])
         return r
 
 
 def interleave_str(s1, s2):
     if len(s1) == len(s2):
-        r = ''
+        r = ""
         for i, j in zip(s2, s1):
             r += i + j
         return r
     elif len(s1) > len(s2):
-        r = ''
+        r = ""
         for i, j in zip(s2, s1):
             r += i + j
-        r += s1[len(s2):]
+        r += s1[len(s2) :]
         return r
     else:
-        r = ''
+        r = ""
         for i, j in zip(s2, s1):
             r += i + j
-        r += s2[len(s1):]
+        r += s2[len(s1) :]
         return r
 
 
 def binary_range(num1, num2):
     if num1 < num2:
         return binary_range(num2, num1)[::-1]
     return list(range(num2, num1 + 1))
 
 
 def empty_join(iterable):
     if not isinstance(iterable, list):
         return str(iterable)
-    return ''.join(map(empty_join, iterable))
+    return "".join(map(empty_join, iterable))
 
 
 def safe_len(x):
     try:
         return len(x)
     except:
         return 1
@@ -367,15 +367,15 @@
 def lowered_range(num):
     if num < 0:
         return [-i for i in lowered_range(-num)]
     return list(range(int(num)))
 
 
 def min2(num):
-    return min(int(d) for d in str(num) if d in '0123456789')
+    return min(int(d) for d in str(num) if d in "0123456789")
 
 
 def min3(x):
     try:
         return min(x)
     except:
         return x
@@ -385,64 +385,64 @@
     try:
         return int(x)
     except:
         return str(x)
 
 
 def two_power(n):
-    return 2 ** n
+    return 2**n
 
 
 def is_prime(n):
     i = int(n)
     return int(i >= 2 and all(i % k for k in range(2, i)))
 
 
 def slice1(num, lst):
-    return lst[::int(num)]
+    return lst[:: int(num)]
 
 
 def slice2(lst, num):
-    return lst[::int(num)]
+    return lst[:: int(num)]
 
 
 def not_equal(x, y):
     return int(x != y)
 
 
 def one_range(num):
     if num < 0:
         return [-i for i in one_range(-num)]
     return list(range(1, int(num) + 1))
 
 
 def digit_sum(num):
-    return sum(int(d) for d in str(num) if d in '0123456789')
+    return sum(int(d) for d in str(num) if d in "0123456789")
 
 
 def it_sum(lst):
     if not lst:
         return 0
     if all(isinstance(item, (int, float)) for item in lst):
         return sum(lst)
     if all(isinstance(item, list) for item in lst):
         return sum(lst[1:], lst[0])
-    return ''.join(map(str, lst))
+    return "".join(map(str, lst))
 
 
 def uniquify_lst(lst):
     r = []
     for i in lst:
         if i not in r:
             r.append(i)
     return r
 
 
 def uniquify_str(s):
-    r = ''
+    r = ""
     for c in s:
         if c not in r:
             r += c
     return r
 
 
 def uniquify_num(num):
@@ -450,23 +450,23 @@
 
 
 def indices_where_truthy(l):
     return [i for i, x in enumerate(l) if x]
 
 
 def indices_where_truthy_num(n):
-    return [i for i, x in enumerate(str(n)) if x in '123456789']
+    return [i for i, x in enumerate(str(n)) if x in "123456789"]
 
 
 def rot_13(s):
-    r = ''
+    r = ""
     for c in s:
-        if ord('A') <= ord(c.upper()) <= ord('M'):
+        if ord("A") <= ord(c.upper()) <= ord("M"):
             r += chr(ord(c) + 13)
-        elif ord('N') <= ord(c.upper()) <= ord('Z'):
+        elif ord("N") <= ord(c.upper()) <= ord("Z"):
             r += chr(ord(c) - 13)
         else:
             r += c
     return r
 
 
 def wrap(x):
@@ -502,22 +502,26 @@
 
 def convert_from_base(base, num):
     if base <= 0:
         return num
     elif base == 1:
         return len(str(num))
     if base <= 64:
-        digits = string.digits + string.ascii_uppercase + string.ascii_lowercase + '+/'
+        digits = string.digits + string.ascii_uppercase + string.ascii_lowercase + "+/"
     else:
         digits = codepage.CODEPAGE * math.ceil(base / 256)
-    return from_list_of_digits_2(list(map((lambda c: safe_index(digits, c, 0)), str(num))), base)
+    return from_list_of_digits_2(
+        list(map((lambda c: safe_index(digits, c, 0)), str(num))), base
+    )
 
 
 def convert_from_custom_base(base, num):
-    return from_list_of_digits_2(list(map((lambda c: safe_index(base, c, 0)), str(num))), len(base))
+    return from_list_of_digits_2(
+        list(map((lambda c: safe_index(base, c, 0)), str(num))), len(base)
+    )
 
 
 def nCr(r, n):
     n, r = int(n), int(r)
     f = math.factorial
     return f(n) // f(r) // f(n - r)
 
@@ -535,19 +539,19 @@
 
 
 def duplicate(x):
     return x, x
 
 
 def ten_power(n):
-    return 10 ** n
+    return 10**n
 
 
 def comma_split(s):
-    return s.split(',')
+    return s.split(",")
 
 
 def prime_factors(n):
     n = int(n)
     for i in range(2, n + 1):
         if is_prime(i) and n % i == 0:
             return [i] + prime_factors(n // i)
@@ -572,15 +576,15 @@
         return 0
     for x in reversed(range(1, max(l))):
         if all(y % x == 0 for y in l):
             return x
 
 
 def digits_gcd(n):
-    return gcd([int(i) for i in str(n) if i in '0123456789'])
+    return gcd([int(i) for i in str(n) if i in "0123456789"])
 
 
 def ords_gcd(s):
     return gcd(list(map(ord, s)))
 
 
 def head_extract(x):
@@ -589,17 +593,17 @@
     return x[1:], x[0]
 
 
 def num_head_extract(n):
     r = ()
     for i in head_extract(str(n)):
         try:
-            r += eval(i),
+            r += (eval(i),)
         except:
-            r += i,
+            r += (i,)
     return r
 
 
 def num_ind0(x, y):
     s = str(y)[int(x) % len(str(y))]
     try:
         return int(s)
@@ -626,19 +630,19 @@
 
 
 def decrement(num):
     return num - 1
 
 
 def str_increment(s):
-    return ''.join(chr(ord(c) + 1) for c in s)
+    return "".join(chr(ord(c) + 1) for c in s)
 
 
 def str_decrement(s):
-    return ''.join(chr(ord(c) - 1) for c in s)
+    return "".join(chr(ord(c) - 1) for c in s)
 
 
 def join(joiner, iterable):
     return str(joiner).join(map(str, iterable))
 
 
 def num_join(j, n):
@@ -658,23 +662,23 @@
             pass
     if not l:
         return 0
     return sum(l) / len(l)
 
 
 def num_mean(n):
-    return mean([int(i) for i in str(n) if i in '0123456789'])
+    return mean([int(i) for i in str(n) if i in "0123456789"])
 
 
 def ord_mean(s):
     return mean(map(ord, s))
 
 
 def str_rmv(x, y):
-    return str(y).replace(str(x), '')
+    return str(y).replace(str(x), "")
 
 
 def num_rmv(x, y):
     try:
         return eval(str_rmv(x, y))
     except:
         return str_rmv(x, y)
@@ -688,15 +692,15 @@
 
 
 def swapped_list_rmv(x, y):
     return list_rmv(y, x)
 
 
 def digit_product(num):
-    return math.prod([int(i) for i in str(num) if i in '0123456789'])
+    return math.prod([int(i) for i in str(num) if i in "0123456789"])
 
 
 def product(lst):
     l = []
     for i in lst:
         if isinstance(i, (int, float)):
             l.append(i)
@@ -720,15 +724,15 @@
 def swapped_append(x, y):
     return append(y, x)
 
 
 def _digits(x):
     if isinstance(x, (str, list)):
         return list(x)
-    return [int(i) for i in str(x) if i in '0123456789']
+    return [int(i) for i in str(x) if i in "0123456789"]
 
 
 def append2(x, y):
     return _digits(y) + [x]
 
 
 def string_replace(x, y, z):
@@ -761,22 +765,22 @@
     return x[:-1], x[-1]
 
 
 def num_tail_extract(n):
     r = ()
     for i in tail_extract(str(n)):
         try:
-            r += eval(i),
+            r += (eval(i),)
         except:
-            r += i,
+            r += (i,)
     return r
 
 
 def remove_whitespace(s):
-    return ''.join(s.split())
+    return "".join(s.split())
 
 
 def uninterleave(l):
     return [l[0::2], l[1::2]]
 
 
 def num_uninterleave(n):
@@ -831,15 +835,15 @@
         return x * int(y)
     elif isinstance(y, (str, list)):
         return int(x) * y
     return y * x
 
 
 def string_cartesian_product(a, b):
-    return [''.join(l) for l in itertools.product(b, a)]
+    return ["".join(l) for l in itertools.product(b, a)]
 
 
 def divide(x, y):
     return y / x
 
 
 def split2(a, b):
@@ -847,15 +851,15 @@
         return b
     if not b:
         return [b] * a
     x, y = divmod(len(b), int(a))
     k = 0
     r = []
     while k < len(b):
-        r.append(b[k:k + x + (y > 0)])
+        r.append(b[k : k + x + (y > 0)])
         k += x + (y > 0)
         if y > 0:
             y -= 1
     return r
 
 
 def split1(a, b):
@@ -863,20 +867,20 @@
 
 
 def split3(a, b):
     return b.split(a)
 
 
 def exponentiate(x, y):
-    return y ** x
+    return y**x
 
 
 def append_first1(a, b):
     if not a:
-        return ' ' * b
+        return " " * b
     while len(a) < b:
         a += a[0]
     return a
 
 
 def append_first2(a, b):
     return append_first1(b, a)
@@ -887,15 +891,15 @@
 
 
 def modulo(x, y):
     return y % x
 
 
 def str_format(a, b):
-    return str(b).replace('%', str(a))
+    return str(b).replace("%", str(a))
 
 
 def swapped_format(a, b):
     return str_format(b, a)
 
 
 def integer_divide(x, y):
@@ -969,28 +973,28 @@
     s = split3(a, b)
     if s:
         return s[-1]
     return s
 
 
 def str_format2(a, b):
-    return str(a).replace('%', str(b))
+    return str(a).replace("%", str(b))
 
 
 def swapped_modulo(x, y):
     return x % y
 
 
 def swapped_exponentiate(x, y):
-    return x ** y
+    return x**y
 
 
 def prepend_last1(a, b):
     if not a:
-        return ' ' * b
+        return " " * b
     while len(a) < b:
         a = a[-1] + a
     return a
 
 
 def prepend_last2(a, b):
     return append_first1(b, a)
@@ -1105,15 +1109,15 @@
     if isinstance(x, list):
         r = []
         for i in x:
             a = recursive_flatten(i)
             if isinstance(a, list):
                 r += a
             else:
-                r += a,
+                r += (a,)
         return r
     return x
 
 
 def dyadic_gcd(a, b):
     try:
         return math.gcd(abs(int(a)), abs(int(b)))
@@ -1130,15 +1134,15 @@
 
 
 def longest_common_substring(x, y):
     a, b = substrings(x), substrings(y)
     try:
         return max([i for i in a if i in b], key=len)
     except:
-        return ''
+        return ""
 
 
 def num_head(x):
     return int(str(x)[0])
 
 
 def head(x):
@@ -1188,23 +1192,23 @@
             r.append(indexing_1(i, y))
         except:
             r.append(length_ind1(i, y))
     return r
 
 
 def ljust1(x, n, y):
-    return str(y).ljust(abs(int(n)) or 1, (str(x) + ' ')[0])
+    return str(y).ljust(abs(int(n)) or 1, (str(x) + " ")[0])
 
 
 def ljust2(n, x, y):
-    return str(y).ljust(abs(int(n)) or 1, (str(x) + ' ')[0])
+    return str(y).ljust(abs(int(n)) or 1, (str(x) + " ")[0])
 
 
 def ljust3(x, y, z):
-    return str(z).ljust(len(y) or 1, (str(x) + ' ')[0])
+    return str(z).ljust(len(y) or 1, (str(x) + " ")[0])
 
 
 def mode(it):
     if not it:
         return it
     return max(it, key=it.count)
 
@@ -1214,15 +1218,15 @@
 
 
 def negate(x):
     return -x
 
 
 def rle(s):
-    l = ''
+    l = ""
     r = []
     for c in s:
         if c == l:
             r[-1] += 1
         else:
             r.append(1)
         l = c
@@ -1286,40 +1290,47 @@
     return z
 
 
 def string_repr(s):
     r = repr(s)
     if r[0] == '"':
         return r
-    f = first_char_not_present(r, '\\\'"')
-    return '"' + recursive_replace(f, '\\\\', r[1:-1]).replace("\\'", "'").replace('"', '\\"').replace(f, '\\\\') + '"'
+    f = first_char_not_present(r, "\\'\"")
+    return (
+        '"'
+        + recursive_replace(f, "\\\\", r[1:-1])
+        .replace("\\'", "'")
+        .replace('"', '\\"')
+        .replace(f, "\\\\")
+        + '"'
+    )
 
 
 def list_repr(l):
     x = []
     for i in l:
         if isinstance(i, list):
             x.append(list_repr(i))
         elif isinstance(i, str):
             x.append(string_repr(i))
         else:
             x.append(str(i))
-    return '[' + ', '.join(x) + ']'
+    return "[" + ", ".join(x) + "]"
 
 
 def sort(l):
     return list(sorted(l))
 
 
 def digits_sort(n):
-    return eval(''.join(str_sort(map(str, digits(n)))))
+    return eval("".join(str_sort(map(str, digits(n)))))
 
 
 def str_sort(s):
-    return ''.join(sort(s))
+    return "".join(sort(s))
 
 
 def chunk1(x, y):
     return split2(x, one_range(y))
 
 
 def chunk2(x, y):
@@ -1343,15 +1354,15 @@
         return a
     if isinstance(a, list):
         a[int(b) % len(a)] = c
         return a
     else:
         a = list(a)
         a[b % len(a)] = c
-        return ''.join(map(str, a))
+        return "".join(map(str, a))
 
 
 def swapped_assign(c, a, b):
     return assign(c, b, a)
 
 
 def length_assign(c, b, a):
@@ -1369,15 +1380,15 @@
         else:
             a = assign(c, i, a)
     return a
 
 
 def to_binary(n):
     if n < 0:
-        return '-' + to_binary(abs(n))
+        return "-" + to_binary(abs(n))
     return bin(int(n))[2:]
 
 
 def ord_bin(s):
     return [to_binary(ord(c)) for c in s]
 
 
@@ -1443,15 +1454,15 @@
     for i in l:
         if i != last:
             r.append([i])
         else:
             r[-1].append(i)
         last = i
     if isinstance(l, str):
-        return [*map(''.join, r)]
+        return [*map("".join, r)]
     return r
 
 
 def consecutive_digits(n):
     return group_consecutive(digits(n))
 
 
@@ -1473,15 +1484,15 @@
     while 1:
         if all(n % j == 0 for j in l):
             return n
         n += 1
 
 
 def digits_lcm(n):
-    return lcm([int(i) for i in str(n) if i in '0123456789'])
+    return lcm([int(i) for i in str(n) if i in "0123456789"])
 
 
 def ords_lcm(s):
     return lcm(list(map(ord, s)))
 
 
 def median(lst):
@@ -1497,15 +1508,15 @@
                     l.append(float(i))
                 except:
                     pass
     if not l:
         return []
     if len(l) % 2:
         return sorted(l)[len(l) // 2]
-    s = sorted(l)[len(l) // 2 - 1: len(l) // 2 + 1]
+    s = sorted(l)[len(l) // 2 - 1 : len(l) // 2 + 1]
     return mean(s)
 
 
 def num_median(n):
     return median(digits(n))
 
 
@@ -1551,23 +1562,23 @@
         if i not in r:
             if i not in x:
                 r.append(i)
     return r
 
 
 def rjust1(x, n, y):
-    return str(y).rjust(abs(int(n)) or 1, (str(x) + ' ')[0])
+    return str(y).rjust(abs(int(n)) or 1, (str(x) + " ")[0])
 
 
 def rjust2(n, x, y):
-    return str(y).rjust(abs(int(n)) or 1, (str(x) + ' ')[0])
+    return str(y).rjust(abs(int(n)) or 1, (str(x) + " ")[0])
 
 
 def rjust3(x, y, z):
-    return str(z).rjust(len(y) or 1, (str(x) + ' ')[0])
+    return str(z).rjust(len(y) or 1, (str(x) + " ")[0])
 
 
 def prefixes(l):
     r = []
     for i in range(1, len(l) + 1):
         r.append(l[:i])
     return r
@@ -1597,15 +1608,15 @@
     if not x:
         return x
     return x[:-1]
 
 
 def chunk3(n, l):
     x, y = len(l), abs(int(n))
-    return list(filter(bool, [l[i:i + y] for i in range(0, (x // y + 1) * y, y)]))
+    return list(filter(bool, [l[i : i + y] for i in range(0, (x // y + 1) * y, y)]))
 
 
 def chunk4(l, n):
     return chunk3(n, l)
 
 
 def chunk5(x, y):
@@ -1629,15 +1640,15 @@
 
 
 def num_length_range_0(n):
     return n, lowered_range(len(str(n)))
 
 
 def character_multiply1(s, n):
-    return ''.join(c * n for c in s)
+    return "".join(c * n for c in s)
 
 
 def character_multiply2(n, s):
     return character_multiply1(s, n)
 
 
 def regex_split(x, y):
@@ -1650,28 +1661,28 @@
 
 def exactly_not_equal(x, y):
     return int(y != x)
 
 
 def to_hex(n):
     if n < 0:
-        return '-' + to_hex(abs(n))
+        return "-" + to_hex(abs(n))
     return hex(int(n))[2:]
 
 
 def ord_hex(s):
     return [to_hex(ord(c)) for c in s]
 
 
 def reciprocal(n):
     return 1 / n
 
 
 def remove_non_alphabets(s):
-    return ''.join(c for c in s if c.isalpha())
+    return "".join(c for c in s if c.isalpha())
 
 
 def num_bifurcate(n):
     return n, digit_reverse(n)
 
 
 def bifurcate(x):
@@ -1782,39 +1793,39 @@
 
 
 def combinations_with_replacement4(x, y):
     return combinations_with_replacement1(len(x), y)
 
 
 def square(n):
-    return n ** 2
+    return n**2
 
 
 def chunk_wrap_2(s):
     return chunk3(2, s)
 
 
 def cube(n):
-    return n ** 3
+    return n**3
 
 
 def chunk_wrap_3(s):
     return chunk3(3, s)
 
 
 def fourth(n):
-    return n ** 4
+    return n**4
 
 
 def chunk_wrap_4(s):
     return chunk3(4, s)
 
 
 def fifth(n):
-    return n ** 5
+    return n**5
 
 
 def chunk_wrap_5(s):
     return chunk3(5, s)
 
 
 def halve(n):
@@ -1968,17 +1979,16 @@
 
 def num_to_alphabet(n):
     return chr(64 + (int(n) % 26))
 
 
 def alphabet_to_num(s):
     return [
-        ord(c) - 64 if 'A' <= c <= 'Z' else (
-            ord(c) - 96 if 'a' <= c <= 'z' else 0
-        ) for c in s
+        ord(c) - 64 if "A" <= c <= "Z" else (ord(c) - 96 if "a" <= c <= "z" else 0)
+        for c in s
     ]
 
 
 def nPr(r, n):
     n, r = int(n), int(r)
     f = math.factorial
     return f(n) // f(n - r)
@@ -2046,21 +2056,21 @@
         return [[-i for i in sl] for sl in l]
     return l
 
 
 def newline_join(iterable):
     if not isinstance(iterable, list):
         return str(iterable)
-    return '\n'.join(map(empty_join, iterable))
+    return "\n".join(map(empty_join, iterable))
 
 
 def space_join(iterable):
     if not isinstance(iterable, list):
         return str(iterable)
-    return ' '.join(map(empty_join, iterable))
+    return " ".join(map(empty_join, iterable))
 
 
 def prepend(x, l):
     return [x] + l
 
 
 def swapped_prepend(l, x):
@@ -2068,18 +2078,15 @@
 
 
 def prepend2(x, y):
     return [x] + _digits(y)
 
 
 def transpose_with_filler(f, l):
-    matrix = [
-        [*x] if isinstance(x, (list, str)) else digits(x)
-        for x in l
-    ]
+    matrix = [[*x] if isinstance(x, (list, str)) else digits(x) for x in l]
     transposed = itertools.zip_longest(*matrix, fillvalue=f)
     return list(map(list, transposed))
 
 
 def swapped_transpose_with_filler(l, f):
     return transpose_with_filler(f, l)
 
@@ -2216,24 +2223,24 @@
     elif n > 0:
         return 1
     else:
         return 0
 
 
 def sentence_case(s):
-    r = ''
+    r = ""
     b = True
     for c in s:
         if b:
             r += c.upper()
         else:
             r += c.lower()
-        if c in '?!.':
+        if c in "?!.":
             b = True
-        elif c == ' ' and b == True:
+        elif c == " " and b == True:
             pass
         else:
             b = False
     return r
 
 
 def sum_each(l):
@@ -2253,15 +2260,15 @@
 def num_all_equal(n):
     return all_equal(str(n))
 
 
 def symmetric_set_difference(x, y):
     r = uniquify_lst([i for i in y if i not in x] + [j for j in x if j not in y])
     if (type(x), type(y)) == (str, str):
-        return ''.join(r)
+        return "".join(r)
     return r
 
 
 def range_ssd1(x, y):
     return symmetric_set_difference(digits(x), digits(y))
 
 
@@ -2307,15 +2314,15 @@
 
 def corresponding_filter(x, y):
     r = []
     for i, j in zip(y, x):
         if j:
             r.append(i)
     if isinstance(y, str):
-        return ''.join(r)
+        return "".join(r)
     return r
 
 
 def corresponding_digit_filter_1(x, y):
     return corresponding_filter(digits(x), digits(y))
 
 
@@ -2336,57 +2343,70 @@
 
 
 def num_sort_uniquify(n):
     return list_sort_uniquify(digits(n))
 
 
 def to_roman_numerals(num):
-    ret = ''
+    ret = ""
     if num < 0:
         num = -num
-        ret += '-'
-    symbols = {'M': 1000, 'CM': 900, 'D': 500, 'CD': 400, 'C': 100, 'XC': 90, 'L': 50, 'XL': 40, 'X': 10, 'IX': 9,
-               'V': 5, 'IV': 4, 'I': 1}
+        ret += "-"
+    symbols = {
+        "M": 1000,
+        "CM": 900,
+        "D": 500,
+        "CD": 400,
+        "C": 100,
+        "XC": 90,
+        "L": 50,
+        "XL": 40,
+        "X": 10,
+        "IX": 9,
+        "V": 5,
+        "IV": 4,
+        "I": 1,
+    }
     for s, n in symbols.items():
         while num >= n:
             ret += s
             num -= n
     return ret
 
 
 def from_roman_numerals(s):
     ret = 0
     i = 0
     while i < len(s):
         c = s[i]
-        if c == 'M':
+        if c == "M":
             ret += 1000
-        elif c == 'D':
+        elif c == "D":
             ret += 500
-        elif c == 'L':
+        elif c == "L":
             ret += 50
-        elif c == 'V':
+        elif c == "V":
             ret += 5
-        elif c == 'C':
+        elif c == "C":
             i += 1
-            if s[i] == 'M':
+            if s[i] == "M":
                 ret += 900
             else:
                 ret += 100
                 i -= 1
-        elif c == 'X':
+        elif c == "X":
             i += 1
-            if s[i] == 'C':
+            if s[i] == "C":
                 ret += 90
             else:
                 ret += 10
                 i -= 1
-        elif c == 'I':
+        elif c == "I":
             i += 1
-            if s[i] == 'X':
+            if s[i] == "X":
                 ret += 9
             else:
                 ret += 1
                 i -= 1
         i += 1
     return ret
 
@@ -2402,15 +2422,15 @@
 
 
 def complement(n):
     return 1 - n
 
 
 def is_vowel(s):
-    return [int(c.lower() in 'aeiou') for c in s]
+    return [int(c.lower() in "aeiou") for c in s]
 
 
 def islower(s):
     if not s:
         return 1
     return int(s.islower())
 
@@ -2454,23 +2474,23 @@
 
 
 def shuffle(l):
     return random.sample(l, len(l))
 
 
 def str_shuffle(s):
-    return ''.join(shuffle(s))
+    return "".join(shuffle(s))
 
 
 def range_shuffle(n):
     return shuffle(one_range(n))
 
 
 def spaces(n):
-    return int(n) * ' '
+    return int(n) * " "
 
 
 def suffixes(l):
     r = []
     for i in range(1, len(l) + 1):
         r.append(l[-i:])
     return r
@@ -2549,19 +2569,19 @@
 def listify(x):
     if isinstance(x, (list, str)):
         return list(copy.deepcopy(x))
     return one_range(x)
 
 
 def replace_with_nothing(x, y):
-    return y.replace(x, '')
+    return y.replace(x, "")
 
 
 def replace_with_nothing2(x, y):
-    return x.replace(y, '')
+    return x.replace(y, "")
 
 
 def factorial(n):
     if n < 1:
         return 1
     return math.factorial(int(n))
 
@@ -2570,7 +2590,15 @@
     if not s:
         return [[]]
     r = []
     for i in one_range(len(s)):
         for x in all_slices(s[i:]):
             r.append([s[:i]] + x)
     return r
+
+
+def dump(x):
+    return tuple(x)
+
+
+def num_dump(n):
+    return dump(digits(n))
```

### Comparing `thunno2-2.1.2/thunno2/interpreter.py` & `thunno2-2.1.3/thunno2/interpreter.py`

 * *Files 19% similar despite different names*

```diff
@@ -127,157 +127,176 @@
     Work.
  d. Affirmer understands and acknowledges that Creative Commons is not a
     party to this document and has no duty or obligation with respect to
     this CC0 or use of the Work.
 """
 
 vars_dict = {
-    'x': 1,   # x defaults to 1
-    'y': 2,   # y defaults to 2
-    'ga': []  # global array defaults to []
+    "x": 1,  # x defaults to 1
+    "y": 2,  # y defaults to 2
+    "ga": [],  # global array defaults to []
 }
 
-'''RUN FUNCTION'''
+"""RUN FUNCTION"""
 
 
 def run(code, *, n, iteration_index):
     # while ctx.index < len(code):
     for chars, desc, info in code:
-        if desc == 'command' or desc == 'digraph':
+        if desc == "command" or desc == "digraph":
             if info != Void:
                 values = info()
                 for value in values:
                     ctx.stack.push(value)
         elif desc in (
-            'number', 'string', 'one character', 'two characters', 'three characters', 'list'
+            "number",
+            "string",
+            "one character",
+            "two characters",
+            "three characters",
+            "list",
         ):
             ctx.stack.push(info)
-        elif desc == 'lowercase alphabetic compression':
-            base255_number = decompress(info, '“')
-            decompressed_string = to_custom_base_string(' ' + string.ascii_lowercase, base255_number)
+        elif desc == "lowercase alphabetic compression":
+            base255_number = decompress(info, "“")
+            decompressed_string = to_custom_base_string(
+                " " + string.ascii_lowercase, base255_number
+            )
             ctx.stack.push(decompressed_string)
-        elif desc == 'title case alphabetic compression':
-            base255_number = decompress(info, '”')
-            decompressed_string = to_custom_base_string(' ' + string.ascii_lowercase, base255_number)
+        elif desc == "title case alphabetic compression":
+            base255_number = decompress(info, "”")
+            decompressed_string = to_custom_base_string(
+                " " + string.ascii_lowercase, base255_number
+            )
             ctx.stack.push(decompressed_string.title())
-        elif desc == 'lowercase dictionary compression':
+        elif desc == "lowercase dictionary compression":
             lst = []
             i = 0
             while i < len(info):
                 c = info[i]
                 if c in dictionary.dictionary_codepage:
                     try:
                         i += 1
                         lst.append(dictionary.dictionary_decompress_string(c + info[i]))
                     except:
                         pass
-                elif c == '\\':
+                elif c == "\\":
                     try:
                         i += 1
                         lst.append(info[i])
                     except:
-                        lst.append('\\')
+                        lst.append("\\")
                 else:
                     lst.append(c)
                 i += 1
-            ctx.stack.push(''.join(lst))
-        elif desc == 'title case dictionary compression':
+            ctx.stack.push("".join(lst))
+        elif desc == "title case dictionary compression":
             lst = []
             i = 0
             while i < len(info):
                 c = info[i]
                 if c in dictionary.dictionary_codepage:
                     try:
                         i += 1
-                        lst.append(dictionary.dictionary_decompress_string(c + info[i]).title())
+                        lst.append(
+                            dictionary.dictionary_decompress_string(c + info[i]).title()
+                        )
                     except:
                         pass
-                elif c == '\\':
+                elif c == "\\":
                     try:
                         i += 1
                         lst.append(info[i])
                     except:
-                        lst.append('\\')
+                        lst.append("\\")
                 else:
                     lst.append(c)
                 i += 1
-            ctx.stack.push(''.join(lst))
-        elif desc == 'one word dictionary compression':
+            ctx.stack.push("".join(lst))
+        elif desc == "one word dictionary compression":
             ctx.stack.push(dictionary.dictionary_decompress_string(info).title())
-        elif desc == 'two words dictionary compression':
+        elif desc == "two words dictionary compression":
             ctx.stack.push(
                 dictionary.dictionary_decompress_string(info[:2]).title()
                 + dictionary.dictionary_decompress_string(info[2:]).title()
             )
-        elif desc == 'compressed number' or desc == 'small compressed number':
-            base255_number = decompress(info, '»')
+        elif desc == "compressed number" or desc == "small compressed number":
+            base255_number = decompress(info, "»")
             ctx.stack.push(base255_number)
-        elif desc == 'compressed list':
-            base255_number = decompress(info, '¿')
-            decompressed_string = to_custom_base_string('][0123456789-.,', base255_number)
+        elif desc == "compressed list":
+            base255_number = decompress(info, "¿")
+            decompressed_string = to_custom_base_string(
+                "][0123456789-.,", base255_number
+            )
             try:
                 e = eval(decompressed_string)
                 if isinstance(e, tuple):
                     ctx.stack.push(list(e))
                 else:
                     ctx.stack.push(e)
             except:
                 ctx.stack.push(decompressed_string)
-        elif desc == 'variable get':
+        elif desc == "variable get":
             ctx.stack.push(vars_dict.get(info, 0))
-        elif desc == 'variable set':
+        elif desc == "variable set":
             a = next(ctx.stack.rmv(1))
             vars_dict[info] = a
-        elif desc == 'single function map':
+        elif desc == "single function map":
             a = next(ctx.stack.rmv(1))
             func = info
             if func != Void:
                 x = listify(a)
                 r = []
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 for i in x:
                     ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
                     ctx.stack.push(i)
                     for j in func():
                         r.append(j)
                 ctx.stack.push(r)
-        elif desc == 'outer product':
+        elif desc == "outer product":
             a, b = ctx.stack.rmv(2)
             func = info
             if func != Void:
                 x = listify(a)
                 r = []
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 if isinstance(a, list):
                     if isinstance(b, list):
                         for j in b:
                             r.append([])
                             for i in a:
-                                ctx.stack = Stack([i, j] + copy.deepcopy(list(old_stack).copy()))
+                                ctx.stack = Stack(
+                                    [i, j] + copy.deepcopy(list(old_stack).copy())
+                                )
                                 for k in func():
                                     r[-1].append(k)
                     else:
                         for i in a:
-                            ctx.stack = Stack([i, b] + copy.deepcopy(list(old_stack).copy()))
+                            ctx.stack = Stack(
+                                [i, b] + copy.deepcopy(list(old_stack).copy())
+                            )
                             for k in func():
                                 r.append(k)
                 else:
                     if isinstance(b, list):
                         for i in b:
-                            ctx.stack = Stack([a, i] + copy.deepcopy(list(old_stack).copy()))
+                            ctx.stack = Stack(
+                                [a, i] + copy.deepcopy(list(old_stack).copy())
+                            )
                             for k in func():
                                 r.append(k)
                     else:
                         ctx.stack.push(b)
                         ctx.stack.push(a)
                         k = func()
                         if k:
                             r = k[-1]
                 ctx.stack.push(r)
-        elif desc == 'single function filter':
+        elif desc == "single function filter":
             a = next(ctx.stack.rmv(1))
             func = info
             if func != Void:
                 x = listify(a)
                 r = []
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 for i in x:
@@ -285,15 +304,15 @@
                     ctx.stack.push(i)
                     f = func()
                     if not f:
                         continue
                     if f[-1]:
                         r.append(i)
                 ctx.stack.push(r)
-        elif desc == 'single function sort by':
+        elif desc == "single function sort by":
             a = next(ctx.stack.rmv(1))
             func = info
             if func != Void:
                 x = listify(a)
                 sort_by = []
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 for i in x:
@@ -305,15 +324,15 @@
                     else:
                         sort_by.append((i, f[-1]))
                 try:
                     sorted_list = sorted(sort_by, key=lambda t: t[-1])
                     ctx.stack.push([p for p, q in sorted_list])
                 except:
                     ctx.stack.push(x)
-        elif desc == 'single function group by':
+        elif desc == "single function group by":
             a = next(ctx.stack.rmv(1))
             func = info
             if func != Void:
                 x = listify(a)
                 group_by = []
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 for i in x:
@@ -332,144 +351,144 @@
                                 d[k][1].append(val)
                                 break
                         else:
                             d.append((key, [val]))
                     ctx.stack.push([q for p, q in d])
                 except:
                     ctx.stack.push(x)
-        elif desc == 'context variable':
+        elif desc == "context variable":
             ctx.stack.push(n)
-        elif desc == 'iteration index':
+        elif desc == "iteration index":
             ctx.stack.push(iteration_index)
-        elif desc == 'get x':
-            ctx.stack.push(vars_dict.get('x', 1))
-        elif desc == 'get y':
-            ctx.stack.push(vars_dict.get('y', 2))
-        elif desc == 'set x':
+        elif desc == "get x":
+            ctx.stack.push(vars_dict.get("x", 1))
+        elif desc == "get y":
+            ctx.stack.push(vars_dict.get("y", 2))
+        elif desc == "set x":
             a = next(ctx.stack.rmv(1))
-            vars_dict['x'] = a
-        elif desc == 'set y':
+            vars_dict["x"] = a
+        elif desc == "set y":
             a = next(ctx.stack.rmv(1))
-            vars_dict['y'] = a
-        elif desc == 'set x without popping':
+            vars_dict["y"] = a
+        elif desc == "set x without popping":
             a = (ctx.stack.copy() + ctx.other_il + [0])[0]
-            vars_dict['x'] = a
-        elif desc == 'set y without popping':
+            vars_dict["x"] = a
+        elif desc == "set y without popping":
             a = (ctx.stack.copy() + ctx.other_il + [0])[0]
-            vars_dict['y'] = a
-        elif desc == 'increment x':
+            vars_dict["y"] = a
+        elif desc == "increment x":
             try:
-                vars_dict['x'] = vars_dict.get('x', 1) + 1
+                vars_dict["x"] = vars_dict.get("x", 1) + 1
             except:
                 pass
-        elif desc == 'increment y':
+        elif desc == "increment y":
             try:
-                vars_dict['y'] = vars_dict.get('y', 2) + 1
+                vars_dict["y"] = vars_dict.get("y", 2) + 1
             except:
                 pass
-        elif desc == 'get global array':
-            ctx.stack.push(vars_dict.get('ga', []))
-        elif desc == 'add to global array':
+        elif desc == "get global array":
+            ctx.stack.push(vars_dict.get("ga", []))
+        elif desc == "add to global array":
             a = next(ctx.stack.rmv(1))
-            ga = vars_dict.get('ga', [])
+            ga = vars_dict.get("ga", [])
             if not isinstance(ga, list):
-                vars_dict['ga'] = [ga, a]
-            vars_dict['ga'] = ga + [a]
-        elif desc == 'stack':
+                vars_dict["ga"] = [ga, a]
+            vars_dict["ga"] = ga + [a]
+        elif desc == "stack":
             ctx.stack.push(list(ctx.stack).copy())
-        elif desc == 'constant':
+        elif desc == "constant":
             ctx.stack.push(info)
-        elif desc == 'callable constant':
+        elif desc == "callable constant":
             ctx.stack.push(info())
-        elif desc == 'codepage compression':
+        elif desc == "codepage compression":
             ctx.stack.push(info)
-        elif desc == 'quit':
+        elif desc == "quit":
             raise TerminateProgramException()  # This will hopefully get caught and ignored
-        elif desc == 'next input':
+        elif desc == "next input":
             if ctx.other_il:
                 ctx.stack.push(ctx.other_il[0])
                 ctx.other_il = ctx.other_il[1:] + [ctx.other_il[0]]
-        elif desc == 'input list':
+        elif desc == "input list":
             ctx.stack.push(ctx.og_input_list)
-        elif desc == 'first input':
+        elif desc == "first input":
             try:
                 ctx.stack.push(ctx.og_input_list[0])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'second input':
+        elif desc == "second input":
             try:
                 ctx.stack.push(ctx.og_input_list[1])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'third input':
+        elif desc == "third input":
             try:
                 ctx.stack.push(ctx.og_input_list[2])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'third last input':
+        elif desc == "third last input":
             try:
                 ctx.stack.push(ctx.og_input_list[-3])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'second last input':
+        elif desc == "second last input":
             try:
                 ctx.stack.push(ctx.og_input_list[-2])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'last input':
+        elif desc == "last input":
             try:
                 ctx.stack.push(ctx.og_input_list[-1])
             except:
                 ctx.stack.push(ctx.og_input_list)
-        elif desc == 'print':
+        elif desc == "print":
             print(next(ctx.stack.rmv(1)))
             ctx.implicit_print = False
-        elif desc == 'print without newline':
-            print(next(ctx.stack.rmv(1)), end='')
+        elif desc == "print without newline":
+            print(next(ctx.stack.rmv(1)), end="")
             ctx.implicit_print = False
-        elif desc == 'print without popping':
+        elif desc == "print without popping":
             print((ctx.stack.copy() + ctx.other_il + [0])[0])
-        elif desc == 'map':
+        elif desc == "map":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, n=j, iteration_index=i)
                 r.append(next(ctx.stack.rmv(1)))
             ctx.stack.push(r)
-        elif desc == 'filter':
+        elif desc == "filter":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, n=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 if z:
                     r.append(j)
             ctx.stack.push(r)
-        elif desc == 'sort by':
+        elif desc == "sort by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, n=j, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 r.append((j, z))
             try:
                 sorted_list = sorted(r, key=lambda t: t[-1])
                 ctx.stack.push([p for p, q in sorted_list])
             except:
                 ctx.stack.push(x)
-        elif desc == 'group by':
+        elif desc == "group by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             r = []
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             for i, j in enumerate(x):
                 ctx.stack = Stack([j] + copy.deepcopy(old_stack))
                 run(info, n=j, iteration_index=i)
@@ -483,108 +502,108 @@
                             d[k][1].append(val)
                             break
                     else:
                         d.append((key, [val]))
                 ctx.stack.push([q for p, q in d])
             except:
                 ctx.stack.push(x)
-        elif desc == 'fixed point':
+        elif desc == "fixed point":
             r = [Void]
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             i = 0
             while True:
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 run(info, n=r[-1], iteration_index=i)
                 k = (ctx.stack + ctx.other_il + [0])[0]
                 print(k)
                 r.append(k)
                 if r[-1] == r[-2]:
                     break
                 i += 1
             ctx.stack.push(r[1:])
-        elif desc == 'first n integers':
+        elif desc == "first n integers":
             a = next(ctx.stack.rmv(1))
             try:
                 x = int(a)
             except:
                 x = 1
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             i = 1
             r = []
             while len(r) < x:
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 ctx.stack.push(i)
-                run(info, n=i, iteration_index=i-1)
+                run(info, n=i, iteration_index=i - 1)
                 k = next(ctx.stack.rmv(1))
                 if k:
                     r.append(i)
                 i += 1
             ctx.stack.push(r)
-        elif desc == 'cumulative reduce by':
+        elif desc == "cumulative reduce by":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             if x:
                 r = [x.pop(0)]
                 for i, j in enumerate(x):
                     ctx.stack = Stack(copy.deepcopy(old_stack))
                     ctx.stack.push(r[-1])
                     ctx.stack.push(j)
                     run(info, n=j, iteration_index=i)
                     r.append(next(ctx.stack.rmv(1)))
                 ctx.stack.push(r)
             else:
                 ctx.stack.push([])
-        elif desc == 'for loop':
+        elif desc == "for loop":
             a = next(ctx.stack.rmv(1))
             x = listify(a)
             for i, j in enumerate(x):
                 if not isinstance(a, (int, float)):
                     ctx.stack.push(j)
                 run(info, n=j, iteration_index=i)
-        elif desc == 'while loop':
+        elif desc == "while loop":
             cond, body = info
             i = 0
             while True:
                 old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
                 run(cond, n=0, iteration_index=i)
                 z = next(ctx.stack.rmv(1))
                 ctx.stack = Stack(copy.deepcopy(old_stack))
                 if not z:
                     break
                 run(body, n=0, iteration_index=i)
                 i += 1
-        elif desc == 'if statement':
+        elif desc == "if statement":
             if_true, if_false = info
             a = next(ctx.stack.rmv(1))
             if a:
                 run(if_true, n=0, iteration_index=1)
             else:
                 run(if_false, n=0, iteration_index=0)
-        elif desc == 'execute without popping':
+        elif desc == "execute without popping":
             if info != Void:
                 values = info(pop=False)
                 for value in values:
                     ctx.stack.push(value)
-        elif desc == 'pair apply':
+        elif desc == "pair apply":
             a = next(ctx.stack.rmv(1))
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             r = []
             f1, f2 = info
             ctx.stack.push(a)
             k = f1()
             if k:
                 r.append(k[-1])
             ctx.stack = Stack(copy.deepcopy(old_stack))
             ctx.stack.push(a)
             k = f2()
             if k:
                 r.append(k[-1])
             ctx.stack.push(r)
-        elif desc == 'two function map':
+        elif desc == "two function map":
             a = next(ctx.stack.rmv(1))
             old_stack = Stack(copy.deepcopy(list(ctx.stack).copy()))
             r = []
             f1, f2 = info
             x = listify(a)
             for i in x:
                 ctx.stack = Stack(copy.deepcopy(list(old_stack).copy()))
@@ -593,16 +612,16 @@
                     ctx.stack.push(j)
                 for k in f2():
                     ctx.stack.push(k)
                 r.append(next(ctx.stack.rmv(1)))
             ctx.stack.push(r)
         else:
             if ctx.warnings:
-                print('TRACEBACK: [UNRECOGNISED TOKEN]', file=sys.stderr)
-                print(f'Got {chars!r} (tokenised to {desc!r})')
+                print("TRACEBACK: [UNRECOGNISED TOKEN]", file=sys.stderr)
+                print(f"Got {chars!r} (tokenised to {desc!r})")
     return 0
 
 
 def test(cod, inp=(), stk=(), warn=True):
     ctx.stack = Stack(stk)
     ctx.og_input_list = list(inp)
     ctx.other_il = list(inp)
```

### Comparing `thunno2-2.1.2/thunno2/lexer.py` & `thunno2-2.1.3/thunno2/lexer.py`

 * *Files 17% similar despite different names*

```diff
@@ -125,429 +125,464 @@
     Work.
  d. Affirmer understands and acknowledges that Creative Commons is not a
     party to this document and has no duty or obligation with respect to
     this CC0 or use of the Work.
 """
 
 
-def tokenise(code, expected_end=''):
+def tokenise(code, expected_end=""):
     index = 0
     ret = []
     while index < len(code):
         char = code[index]
         if char in commands:
-            ret.append((char, 'command', commands[char]))
+            ret.append((char, "command", commands[char]))
         elif char in DIGRAPHS:
             index += 1
             try:
                 x = code[index]
-                ret.append((char, 'digraph', get_a_function(char + x)))
+                ret.append((char, "digraph", get_a_function(char + x)))
             except:
                 pass
-        elif char in '0123456789.':
+        elif char in "0123456789.":
             s = char
             index += 1
             try:
-                while code[index] in '0123456789.':
+                while code[index] in "0123456789.":
                     s += code[index]
                     index += 1
             except:
                 pass
             index -= 1
             try:
-                while s[0] == '0':
-                    ret.append(('0', 'number', 0))
+                while s[0] == "0":
+                    ret.append(("0", "number", 0))
                     try:
                         s = s[1:]
                     except:
                         break
-                if s == '.':
-                    ret.append(('.', 'number', 0.5))
+                if s == ".":
+                    ret.append((".", "number", 0.5))
                 else:
                     x = eval(s)
-                    if s.endswith('.'):
+                    if s.endswith("."):
                         x += 0.5
-                    ret.append((s, 'number', x))
+                    ret.append((s, "number", x))
             except:
                 pass
         elif char == '"':
             s = char
             index += 1
             try:
-                while (code[index] != '"') or (code[index - 1] == '\\'):
+                while (code[index] != '"') or (code[index - 1] == "\\"):
                     s += code[index]
                     index += 1
                 s += code[index]
             except:
                 s += '"'
             try:
-                ret.append((s, 'string', eval(s).replace('¶', '\n')))
+                ret.append((s, "string", eval(s).replace("¶", "\n")))
             except:
-                ret.append((s, 'string', s[1:-1].replace('¶', '\n')))
-        elif char == '\'':
+                ret.append((s, "string", s[1:-1].replace("¶", "\n")))
+        elif char == "'":
             index += 1
             try:
                 x = code[index]
-                ret.append(('\'' + x, 'one character', x))
+                ret.append(("'" + x, "one character", x))
             except:
-                ret.append(('\'', 'one character', ''))
-        elif char == '`':
+                ret.append(("'", "one character", ""))
+        elif char == "`":
             index += 2
-            x = code[index - 1: index + 1]
-            if (len(x) != 2) or (x[0] not in dictionary_codepage) or (x[1] not in dictionary_codepage):
-                ret.append(('`' + x, 'two characters', x))
+            x = code[index - 1 : index + 1]
+            if (
+                (len(x) != 2)
+                or (x[0] not in dictionary_codepage)
+                or (x[1] not in dictionary_codepage)
+            ):
+                ret.append(("`" + x, "two characters", x))
             else:
-                ret.append(('`' + x, 'one word dictionary compression', x))
-        elif char == 'ʋ':
+                ret.append(("`" + x, "one word dictionary compression", x))
+        elif char == "ʋ":
             index += 3
-            x = code[index - 2: index + 1]
+            x = code[index - 2 : index + 1]
             try:
                 nxt = code[index + 1]
             except:
-                nxt = ''
+                nxt = ""
             if (len(x) != 3) or (
-                    (
-                            x[0] not in dictionary_codepage
-                    ) or (
-                            x[1] not in dictionary_codepage
-                    ) or (
-                            x[2] not in dictionary_codepage
-                    ) or (
-                            nxt not in dictionary_codepage
-                    )
+                (x[0] not in dictionary_codepage)
+                or (x[1] not in dictionary_codepage)
+                or (x[2] not in dictionary_codepage)
+                or (nxt not in dictionary_codepage)
             ):
-                ret.append(('ʋ' + x, 'three characters', x))
+                ret.append(("ʋ" + x, "three characters", x))
             else:
                 index += 1
-                ret.append(('ʋ' + x + nxt, 'two words dictionary compression', x + nxt))
-        elif char == '[':
+                ret.append(("ʋ" + x + nxt, "two words dictionary compression", x + nxt))
+        elif char == "[":
             s = char
             index += 1
             try:
-                in_string = ''
+                in_string = ""
                 nests = 1
                 while nests:
                     c = code[index]
                     s += c
-                    if in_string == '' and c in ('"', "'"):
+                    if in_string == "" and c in ('"', "'"):
                         in_string = c
-                    elif in_string != '' and c == in_string:
-                        if code[index - 1] != '\\':
-                            in_string = ''
-                    if in_string == '':
-                        if c == '[':
+                    elif in_string != "" and c == in_string:
+                        if code[index - 1] != "\\":
+                            in_string = ""
+                    if in_string == "":
+                        if c == "[":
                             nests += 1
-                        elif c == ']':
+                        elif c == "]":
                             nests -= 1
                     index += 1
             except:
-                s += ']'
+                s += "]"
             try:
-                ret.append((s, 'list', eval(s)))
+                ret.append((s, "list", eval(s)))
             except:
-                ret.append((s, 'list', s))
-        elif char == ']':
-            ret.append((']', 'list', []))
-        elif char == '#':
+                ret.append((s, "list", s))
+        elif char == "]":
+            ret.append(("]", "list", []))
+        elif char == "#":
             index += 1
             try:
-                if code[index] == ' ':
-                    while code[index] not in '¶\n':
+                if code[index] == " ":
+                    while code[index] not in "¶\n":
                         index += 1
-                elif code[index] == '{':
-                    while code[index] != '#' or code[index - 1] != '}':
+                elif code[index] == "{":
+                    while code[index] != "#" or code[index - 1] != "}":
                         index += 1
             except:
                 pass
-        elif char == '“':
-            compressed_string = ''
+        elif char == "“":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'lowercase alphabetic compression', compressed_string))
-        elif char == '”':
-            compressed_string = ''
+            ret.append(
+                (
+                    char + compressed_string + char,
+                    "lowercase alphabetic compression",
+                    compressed_string,
+                )
+            )
+        elif char == "”":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'title case alphabetic compression', compressed_string))
-        elif char == '‘':
-            compressed_string = ''
+            ret.append(
+                (
+                    char + compressed_string + char,
+                    "title case alphabetic compression",
+                    compressed_string,
+                )
+            )
+        elif char == "‘":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'lowercase dictionary compression', compressed_string))
-        elif char == '’':
-            compressed_string = ''
+            ret.append(
+                (
+                    char + compressed_string + char,
+                    "lowercase dictionary compression",
+                    compressed_string,
+                )
+            )
+        elif char == "’":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'title case dictionary compression', compressed_string))
-        elif char == '»':
-            compressed_string = ''
+            ret.append(
+                (
+                    char + compressed_string + char,
+                    "title case dictionary compression",
+                    compressed_string,
+                )
+            )
+        elif char == "»":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'compressed number', compressed_string))
-        elif char == '«':
-            compressed_string = code[index + 1:index + 3]
+            ret.append(
+                (
+                    char + compressed_string + char,
+                    "compressed number",
+                    compressed_string,
+                )
+            )
+        elif char == "«":
+            compressed_string = code[index + 1 : index + 3]
             index += 2
-            ret.append((char + compressed_string, 'small compressed number', compressed_string))
-        elif char == '¿':
-            compressed_string = ''
+            ret.append(
+                (char + compressed_string, "small compressed number", compressed_string)
+            )
+        elif char == "¿":
+            compressed_string = ""
             index += 1
             try:
                 while code[index] != char:
                     compressed_string += code[index]
                     index += 1
             except:
                 pass
-            ret.append((char + compressed_string + char, 'compressed list', compressed_string))
-        elif char == '¡':
+            ret.append(
+                (char + compressed_string + char, "compressed list", compressed_string)
+            )
+        elif char == "¡":
             index += 1
             try:
                 var = code[index]
             except:
-                var = ''
-            ret.append((char + var, 'variable get', var))
-        elif char == '!':
+                var = ""
+            ret.append((char + var, "variable get", var))
+        elif char == "!":
             index += 1
             try:
                 var = code[index]
             except:
-                var = ''
-            ret.append((char + var, 'variable set', var))
-        elif char == '€':
+                var = ""
+            ret.append((char + var, "variable set", var))
+        elif char == "€":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'single function map', func))
-        elif char == 'ȷ':
+            ret.append((char + cmd, "single function map", func))
+        elif char == "ȷ":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'outer product', func))
-        elif char == 'œ':
+            ret.append((char + cmd, "outer product", func))
+        elif char == "œ":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'single function filter', func))
-        elif char == 'þ':
+            ret.append((char + cmd, "single function filter", func))
+        elif char == "þ":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'single function sort by', func))
-        elif char == 'ñ':
+            ret.append((char + cmd, "single function sort by", func))
+        elif char == "ñ":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'single function group by', func))
-        elif char == 'n':
-            ret.append((char, 'context variable', 0))
-        elif char == 'ṅ':
-            ret.append((char, 'iteration index', 0))
-        elif char == 'x':
-            ret.append((char, 'get x', 0))
-        elif char == 'y':
-            ret.append((char, 'get y', 0))
-        elif char == 'X':
-            ret.append((char, 'set x', 0))
-        elif char == 'Y':
-            ret.append((char, 'set y', 0))
-        elif char == 'Ẋ':
-            ret.append((char, 'set x without popping', 0))
-        elif char == 'Ẏ':
-            ret.append((char, 'set y without popping', 0))
-        elif char == 'ẋ':
-            ret.append((char, 'increment x', 0))
-        elif char == 'ẏ':
-            ret.append((char, 'increment y', 0))
-        elif char == 'Ȥ':
-            ret.append((char, 'get global array', 0))
-        elif char == 'ȥ':
-            ret.append((char, 'add to global array', 0))
-        elif char == 'K':
-            ret.append((char, 'stack', 0))
-        elif char == 'k':
+            ret.append((char + cmd, "single function group by", func))
+        elif char == "n":
+            ret.append((char, "context variable", 0))
+        elif char == "ṅ":
+            ret.append((char, "iteration index", 0))
+        elif char == "x":
+            ret.append((char, "get x", 0))
+        elif char == "y":
+            ret.append((char, "get y", 0))
+        elif char == "X":
+            ret.append((char, "set x", 0))
+        elif char == "Y":
+            ret.append((char, "set y", 0))
+        elif char == "Ẋ":
+            ret.append((char, "set x without popping", 0))
+        elif char == "Ẏ":
+            ret.append((char, "set y without popping", 0))
+        elif char == "ẋ":
+            ret.append((char, "increment x", 0))
+        elif char == "ẏ":
+            ret.append((char, "increment y", 0))
+        elif char == "Ȥ":
+            ret.append((char, "get global array", 0))
+        elif char == "ȥ":
+            ret.append((char, "add to global array", 0))
+        elif char == "K":
+            ret.append((char, "stack", 0))
+        elif char == "k":
             index += 1
             try:
                 if code[index] in CONSTANTS:
                     x = code[index]
                     c = CONSTANTS[x]
                     if type(c) == type(lambda: 0):
-                        ret.append((char + x, 'callable constant', c))
+                        ret.append((char + x, "callable constant", c))
                     else:
-                        ret.append((char + x, 'constant', c))
+                        ret.append((char + x, "constant", c))
             except:
                 pass
-        elif char == 'ṇ':
+        elif char == "ṇ":
             index += 1
             try:
                 x = code[index]
-                ret.append((char + x, 'codepage compression', next(codepage_index(x)) + 101))
-            except:
-                pass
-        elif char == 'q':
-            ret.append((char, 'quit', 0))
-        elif char == '$':
-            ret.append((char, 'next input', 0))
-        elif char == '¤':
-            ret.append((char, 'input list', 0))
-        elif char == '°':
-            ret.append((char, 'first input', 0))
-        elif char == '¹':
-            ret.append((char, 'second input', 0))
-        elif char == '⁶':
-            ret.append((char, 'third input', 0))
-        elif char == '⁷':
-            ret.append((char, 'third last input', 0))
-        elif char == '⁸':
-            ret.append((char, 'second last input', 0))
-        elif char == '⁹':
-            ret.append((char, 'last input', 0))
-        elif char == '£':
-            ret.append((char, 'print', 0))
-        elif char == '¢':
-            ret.append((char, 'print without newline', 0))
-        elif char == 'ß':
-            ret.append((char, 'print without popping', 0))
-        elif char == 'ı':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+                ret.append(
+                    (char + x, "codepage compression", next(codepage_index(x)) + 101)
+                )
+            except:
+                pass
+        elif char == "q":
+            ret.append((char, "quit", 0))
+        elif char == "$":
+            ret.append((char, "next input", 0))
+        elif char == "¤":
+            ret.append((char, "input list", 0))
+        elif char == "°":
+            ret.append((char, "first input", 0))
+        elif char == "¹":
+            ret.append((char, "second input", 0))
+        elif char == "⁶":
+            ret.append((char, "third input", 0))
+        elif char == "⁷":
+            ret.append((char, "third last input", 0))
+        elif char == "⁸":
+            ret.append((char, "second last input", 0))
+        elif char == "⁹":
+            ret.append((char, "last input", 0))
+        elif char == "£":
+            ret.append((char, "print", 0))
+        elif char == "¢":
+            ret.append((char, "print without newline", 0))
+        elif char == "ß":
+            ret.append((char, "print without popping", 0))
+        elif char == "ı":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'map', r))
-        elif char == 'æ':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "map", r))
+        elif char == "æ":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'filter', r))
-        elif char == 'Þ':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "filter", r))
+        elif char == "Þ":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'sort by', r))
-        elif char == 'Ñ':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "sort by", r))
+        elif char == "Ñ":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'group by', r))
-        elif char == '¥':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "group by", r))
+        elif char == "¥":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'fixed point', r))
-        elif char == 'Ƙ':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "fixed point", r))
+        elif char == "Ƙ":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'first n integers', r))
-        elif char == 'Ʋ':
-            i, r = tokenise(code[index + 1:], expected_end=';')
+            ret.append((char, "first n integers", r))
+        elif char == "Ʋ":
+            i, r = tokenise(code[index + 1 :], expected_end=";")
             index += i
-            ret.append((char, 'cumulative reduce by', r))
-        elif char == '{':
-            i, r = tokenise(code[index + 1:], expected_end='}')
+            ret.append((char, "cumulative reduce by", r))
+        elif char == "{":
+            i, r = tokenise(code[index + 1 :], expected_end="}")
             index += i
-            ret.append((char, 'for loop', r))
-        elif char == '(':
-            i, r1 = tokenise(code[index + 1:], expected_end=';)')
+            ret.append((char, "for loop", r))
+        elif char == "(":
+            i, r1 = tokenise(code[index + 1 :], expected_end=";)")
             index += i + 1
             r2 = []
             try:
-                if code[index] == ';':
-                    i, r2 = tokenise(code[index + 1:], expected_end=')')
+                if code[index] == ";":
+                    i, r2 = tokenise(code[index + 1 :], expected_end=")")
                     index += i
             except:
                 pass
-            ret.append((char, 'while loop', (r1, r2)))
-        elif char == '?':
-            i, r1 = tokenise(code[index + 1:], expected_end=':;')
+            ret.append((char, "while loop", (r1, r2)))
+        elif char == "?":
+            i, r1 = tokenise(code[index + 1 :], expected_end=":;")
             index += i + 1
             r2 = []
             try:
-                if code[index] == ':':
-                    i, r2 = tokenise(code[index + 1:], expected_end=';')
+                if code[index] == ":":
+                    i, r2 = tokenise(code[index + 1 :], expected_end=";")
                     index += i
             except:
                 pass
-            ret.append((char, 'if statement', (r1, r2)))
-        elif char == 'Ɓ':
+            ret.append((char, "if statement", (r1, r2)))
+        elif char == "Ɓ":
             index += 1
             cmd = code[index]
             if cmd in DIGRAPHS:
                 index += 1
                 cmd += code[index]
             func = get_a_function(cmd)
-            ret.append((char + cmd, 'execute without popping', func))
-        elif char == 'ç':
+            ret.append((char + cmd, "execute without popping", func))
+        elif char == "ç":
             try:
                 index += 1
                 cmd1 = code[index]
                 if cmd1 in DIGRAPHS:
                     index += 1
                     cmd1 += code[index]
                 func1 = get_a_function(cmd1)
             except:
-                func1, cmd1 = Void, ''
+                func1, cmd1 = Void, ""
             try:
                 index += 1
                 cmd2 = code[index]
                 if cmd2 in DIGRAPHS:
                     index += 1
                     cmd2 += code[index]
                 func2 = get_a_function(cmd2)
             except:
-                func2, cmd2 = Void, ''
-            ret.append((char + cmd1 + cmd2, 'pair apply', (func1, func2)))
-        elif char == 'Ç':
+                func2, cmd2 = Void, ""
+            ret.append((char + cmd1 + cmd2, "pair apply", (func1, func2)))
+        elif char == "Ç":
             try:
                 index += 1
                 cmd1 = code[index]
                 if cmd1 in DIGRAPHS:
                     index += 1
                     cmd1 += code[index]
                 func1 = get_a_function(cmd1)
             except:
-                func1, cmd1 = Void, ''
+                func1, cmd1 = Void, ""
             try:
                 index += 1
                 cmd2 = code[index]
                 if cmd2 in DIGRAPHS:
                     index += 1
                     cmd2 += code[index]
                 func2 = get_a_function(cmd2)
             except:
-                func2, cmd2 = Void, ''
-            ret.append((char + cmd1 + cmd2, 'two function map', (func1, func2)))
+                func2, cmd2 = Void, ""
+            ret.append((char + cmd1 + cmd2, "two function map", (func1, func2)))
         elif char in expected_end:
             return index, ret
         index += 1
     return index + 1, ret
```

### Comparing `thunno2-2.1.2/thunno2/run.py` & `thunno2-2.1.3/thunno2/run.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 from thunno2 import lexer, version, flags, tokens
 import sys
 
 
 def from_terminal():
-    print('Thunno', version.THUNNO_VERSION, 'interpreter\n')
-    print('\nFlags:')
+    print("Thunno", version.THUNNO_VERSION, "interpreter\n")
+    print("\nFlags:")
     flags_list = input()
-    code = ''
-    print('\nHeader:')
+    code = ""
+    print("\nHeader:")
     inp = input()
     while inp:
-        code += inp + '\n'
+        code += inp + "\n"
         inp = input()
-    print('\nCode:')
+    print("\nCode:")
     inp = input()
     while inp:
-        code += inp + '\n'
+        code += inp + "\n"
         inp = input()
-    print('\nFooter:')
+    print("\nFooter:")
     inp = input()
     while inp:
-        code += inp + '\n'
+        code += inp + "\n"
         inp = input()
-    inputs = ''
-    print('\nInput:')
+    inputs = ""
+    print("\nInput:")
     inp = input()
     while inp:
-        inputs += inp + '\n'
+        inputs += inp + "\n"
         inp = input()
-    if 'v' in flags_list:
+    if "v" in flags_list:
         transpiled = tokens.transpile(code)
-        print('\nTranspiled:')
+        print("\nTranspiled:")
         print(transpiled)
         print()
         _, tokenised = lexer.tokenise(transpiled)
     else:
         _, tokenised = lexer.tokenise(code)
-    print('\nOutput:')
+    print("\nOutput:")
     flags.run(flags_list, tokenised, inputs)
 
 
 def from_cmdline():
     args = sys.argv[1:]
     if not args:
         from_terminal()
         return None
     filename = args[0]
     flags_list = args[1:]
-    sys.stderr.write('Thunno, v' + version.THUNNO_VERSION + '\n')
+    sys.stderr.write("Thunno, v" + version.THUNNO_VERSION + "\n")
     try:
         with open(filename) as f:
-            if 'v' in ''.join(flags_list):
+            if "v" in "".join(flags_list):
                 transpiled = tokens.transpile(f.read())
-                print('Transpiled:', transpiled, file=sys.stderr)
+                print("Transpiled:", transpiled, file=sys.stderr)
                 _, tokenised = lexer.tokenise(transpiled)
             else:
                 _, tokenised = lexer.tokenise(f.read())
-            flags.run(''.join(flags_list), tokenised, sys.stdin.read())
+            flags.run("".join(flags_list), tokenised, sys.stdin.read())
     except Exception as E:
-        sys.stderr.write('An error occurred: ' + repr(E))
+        sys.stderr.write("An error occurred: " + repr(E))
```

### Comparing `thunno2-2.1.2/thunno2/tests.py` & `thunno2-2.1.3/thunno2/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1210,25 +1210,21 @@
 
 assert_eq(call('Ḍ', 5), 10)
 assert_eq(call('Ḍ', 'abc'), 'abcabc')
 assert_eq(call('Ḍ', [123, 'abc', 456, 'def']), [246, 'abcabc', 912, 'defdef'])
 
 # Ẹ
 
-assert_eq(call('Ẹ', 1, 2), 1)
-assert_eq(call('Ẹ', 2, 2), 0)
-assert_eq(call('Ẹ', [1, 2, 3], [1, 3, 5]), 1)
-
-assert_eq(call('Ẹ', 'abc', 2), 1)
-assert_eq(call('Ẹ', ['abc', 'def', 'ghi'], 2), 1)
-
-assert_eq(call('Ẹ', 'abc', 'abc'), 0)
-assert_eq(call('Ẹ', 'abc', 'def'), 1)
-assert_eq(call('Ẹ', ['abc', 'def', 'ghi'], ['abc', 'xyz', 'ghi']), 1)
-assert_eq(call('Ẹ', ['abc', 'def'], ['abc', 'def']), 0)
+assert_eq(call('Ẹ', 1234), 1, 2, 3, 4)
+assert_eq(call('Ẹ', -789.123), 7, 8, 9, 1, 2, 3)
+
+assert_eq(call('Ẹ', 'abcde'), 'a', 'b', 'c', 'd', 'e')
+assert_eq(call('Ẹ', ''))
+
+assert_eq(call('Ẹ', [1, 2, 3, 4, 5]), 1, 2, 3, 4, 5)
 
 # Ḥ
 
 assert_eq(call('Ḥ', 10), 'a')
 assert_eq(call('Ḥ', [50, 60, 70, 80, 90]), ['32', '3c', '46', '50', '5a'])
 
 assert_eq(call('Ḥ', 'abcde'), ['61', '62', '63', '64', '65'])
```

### Comparing `thunno2-2.1.2/thunno2.egg-info/PKG-INFO` & `thunno2-2.1.3/thunno2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.1.2
+Version: 2.1.3
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.2.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.1.3.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

