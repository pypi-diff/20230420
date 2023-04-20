# Comparing `tmp/conlp-0.0.4.tar.gz` & `tmp/conlp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlp-0.0.4.tar", last modified: Thu Apr 20 19:06:21 2023, max compression
+gzip compressed data, was "conlp-0.0.5.tar", last modified: Thu Apr 20 19:23:23 2023, max compression
```

## Comparing `conlp-0.0.4.tar` & `conlp-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 19:06:21.215140 conlp-0.0.4/
--rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      403 2023-04-20 19:06:21.215140 conlp-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 19:06:21.209139 conlp-0.0.4/conlp/
--rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.4/conlp/__init__.py
--rw-rw-rw-   0        0        0    13709 2023-04-20 19:02:40.000000 conlp-0.0.4/conlp/download.py
--rw-rw-rw-   0        0        0     2553 2023-04-20 19:02:41.000000 conlp-0.0.4/conlp/preprocess.py
--rw-rw-rw-   0        0        0    26151 2023-04-20 19:02:42.000000 conlp-0.0.4/conlp/sentiment.py
-drwxrwxrwx   0        0        0        0 2023-04-20 19:06:21.215140 conlp-0.0.4/conlp.egg-info/
--rw-rw-rw-   0        0        0      403 2023-04-20 19:06:20.000000 conlp-0.0.4/conlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-20 19:06:21.000000 conlp-0.0.4/conlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 19:06:20.000000 conlp-0.0.4/conlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-20 19:06:21.000000 conlp-0.0.4/conlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 19:06:21.000000 conlp-0.0.4/conlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-20 19:06:21.216139 conlp-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      648 2023-04-20 19:02:14.000000 conlp-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.249848 conlp-0.0.5/
+-rw-rw-rw-   0        0        0    11824 2023-04-19 00:13:02.000000 conlp-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      403 2023-04-20 19:23:23.249848 conlp-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:11:59.000000 conlp-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.244849 conlp-0.0.5/conlp/
+-rw-rw-rw-   0        0        0      115 2023-04-18 23:35:11.000000 conlp-0.0.5/conlp/__init__.py
+-rw-rw-rw-   0        0        0    13681 2023-04-20 19:20:32.000000 conlp-0.0.5/conlp/download.py
+-rw-rw-rw-   0        0        0     2553 2023-04-20 19:02:41.000000 conlp-0.0.5/conlp/preprocess.py
+-rw-rw-rw-   0        0        0    26142 2023-04-20 19:21:04.000000 conlp-0.0.5/conlp/sentiment.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:23:23.249848 conlp-0.0.5/conlp.egg-info/
+-rw-rw-rw-   0        0        0      403 2023-04-20 19:23:22.000000 conlp-0.0.5/conlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:23:22.000000 conlp-0.0.5/conlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 19:23:23.000000 conlp-0.0.5/conlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-20 19:23:23.250848 conlp-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      648 2023-04-20 19:23:14.000000 conlp-0.0.5/setup.py
```

### Comparing `conlp-0.0.4/LICENSE.txt` & `conlp-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conlp-0.0.4/conlp/download.py` & `conlp-0.0.5/conlp/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 class download:
     def __init__(self, 
                  models:str or list):
         """
         Downloads Huggingface Natural Language Processing Models in the local environment.  
 
         Args:
-            models (str or list): Target models to download. Available models include ['twitter_roBERTa_v1', 'twitter_roBERTa_v2', 'twitter_XLM_roBERTa', 'finBERT', \
-                'cnn_dailymail_BART', 'xsum_BART', 'cnn_dailymail_distilBART', 'xsum_distilBART','cnn_dailymail_PEGASUS', 'multi_news_PEGASUS', 'bloomberg_PEGASUS', \
-                'keyBERT', 'mnli_distilBART']
+            models (str or list): Target models to download. 
+            Available models include ['twitter_roBERTa_v1', 'twitter_roBERTa_v2', 'twitter_XLM_roBERTa', 'finBERT', 'cnn_dailymail_BART', 'xsum_BART', 'cnn_dailymail_distilBART', 'xsum_distilBART','cnn_dailymail_PEGASUS', 'multi_news_PEGASUS', 'bloomberg_PEGASUS', 'keyBERT', 'mnli_distilBART']
         """
         available_models = [#Sentiment Classification 
                             'twitter_roBERTa_v1', 'twitter_roBERTa_v2', 'twitter_XLM_roBERTa', 'finBERT', 
                             #Text Summarization 
                             'cnn_dailymail_BART', 'xsum_BART', 'cnn_dailymail_distilBART', 'xsum_distilBART',
                             'cnn_dailymail_PEGASUS', 'multi_news_PEGASUS', 'bloomberg_PEGASUS', 
                             #KeyWord Extraction & Zero-Shot Classification 
@@ -29,17 +28,17 @@
         else: 
             raise ValueError("Input models must be either str or list")
         
         for model in models:
             if model in available_models: 
                 pass
             else: 
-                raise ValueError("""'models' includes input '{}', which is not supported. SUPPORTED MODELS: \
-                    (i) Sentiment Classification - 'twitter_roBERTa_v1', 'twitter_roBERTa_v2', 'twitter_XLM_roBERTa', 'FinBERT'; \
-                    (ii) Text Summarization - 'cnn_dailymail_BART', 'xsum_BART', 'cnn_dailymail_distilBART', 'xsum_distilBART', 'cnn_dailymail_PEGASUS', 'multi_news_PEGASUS', 'bloomberg_PEGASUS'; \
+                raise ValueError("""'models' includes input '{}', which is not supported. SUPPORTED MODELS:
+                    (i) Sentiment Classification - 'twitter_roBERTa_v1', 'twitter_roBERTa_v2', 'twitter_XLM_roBERTa', 'FinBERT'; 
+                    (ii) Text Summarization - 'cnn_dailymail_BART', 'xsum_BART', 'cnn_dailymail_distilBART', 'xsum_distilBART', 'cnn_dailymail_PEGASUS', 'multi_news_PEGASUS', 'bloomberg_PEGASUS'; 
                     (iii) Zero-Shot Classification & Keyword Extraction - 'keyBERT', 'mnli_distilBART'""".format(model))
         
         path = Path().resolve()
         
         for model in models: 
             if model == 'alphaVADER': 
                 print("""Installing alphaVADER by [SocialScienceAI] in your local environment...\n(for more details, see https://)""")
```

### Comparing `conlp-0.0.4/conlp/preprocess.py` & `conlp-0.0.5/conlp/preprocess.py`

 * *Files identical despite different names*

### Comparing `conlp-0.0.4/conlp/sentiment.py` & `conlp-0.0.5/conlp/sentiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,1620 +16,1619 @@
 000000f0: 6d70 6f72 7420 7072 6570 726f 6365 7373  mport preprocess
 00000100: 0d0a 0d0a 636c 6173 7320 7365 6e74 696d  ....class sentim
 00000110: 656e 743a 2020 2020 200d 0a20 2020 2064  ent:     ..    d
 00000120: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
 00000130: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
 00000140: 2020 2020 206c 6f61 645f 6d6f 6465 6c73       load_models
 00000150: 3a73 7472 206f 7220 6c69 7374 293a 200d  :str or list): .
-00000160: 0a20 2020 2020 2020 2022 2222 5f73 756d  .        """_sum
-00000170: 6d61 7279 5f0d 0a0d 0a20 2020 2020 2020  mary_....       
-00000180: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00000190: 2020 2020 6c6f 6164 5f6d 6f64 656c 7320      load_models 
-000001a0: 2873 7472 206f 7220 6c69 7374 293a 2041  (str or list): A
-000001b0: 7661 696c 6162 6c65 206d 6f64 656c 7320  vailable models 
-000001c0: 746f 2062 6520 6c6f 6164 6564 2e20 5c6e  to be loaded. \n
-000001d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001e0: 2020 496e 636c 7564 6573 3a20 0d0a 2020    Includes: ..  
-000001f0: 2020 2020 2020 2020 2020 2020 2020 2869                (i
-00000200: 2920 2774 7769 7474 6572 5f72 6f42 4552  ) 'twitter_roBER
-00000210: 5461 5f76 3127 3b0d 0a20 2020 2020 2020  Ta_v1';..       
-00000220: 2020 2020 2020 2020 2028 6969 2927 7477           (ii)'tw
-00000230: 6974 7465 725f 726f 4245 5254 615f 7632  itter_roBERTa_v2
-00000240: 273b 2020 0d0a 2020 2020 2020 2020 2020  ';  ..          
-00000250: 2020 2020 2020 2869 6969 2920 2774 7769        (iii) 'twi
-00000260: 7474 6572 5f58 4c4d 5f72 6f42 4552 5461  tter_XLM_roBERTa
-00000270: 273b 2061 6e64 0d0a 2020 2020 2020 2020  '; and..        
-00000280: 2020 2020 2020 2020 2869 7629 2027 6669          (iv) 'fi
-00000290: 6e42 4552 5427 0d0a 2020 2020 2020 2020  nBERT'..        
-000002a0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-000002b0: 662e 6c6f 6767 6572 203d 206c 6f67 6769  f.logger = loggi
-000002c0: 6e67 2e67 6574 5f6c 6f67 6765 7228 2274  ng.get_logger("t
-000002d0: 7261 6e73 666f 726d 6572 7322 290d 0a20  ransformers").. 
-000002e0: 2020 2020 2020 2061 7661 696c 6162 6c65         available
-000002f0: 5f6d 6f64 656c 7320 3d20 5b23 2761 6c70  _models = [#'alp
-00000300: 6861 5641 4445 5227 0d0a 2020 2020 2020  haVADER'..      
-00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000320: 2020 2020 2020 2774 7769 7474 6572 5f72        'twitter_r
-00000330: 6f42 4552 5461 5f76 3127 2c20 2774 7769  oBERTa_v1', 'twi
-00000340: 7474 6572 5f72 6f42 4552 5461 5f76 3227  tter_roBERTa_v2'
-00000350: 2c20 2774 7769 7474 6572 5f58 4c4d 5f72  , 'twitter_XLM_r
-00000360: 6f42 4552 5461 272c 2027 6669 6e42 4552  oBERTa', 'finBER
-00000370: 5427 5d0d 0a20 2020 2020 2020 200d 0a20  T']..        .. 
-00000380: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00000390: 616e 6365 286c 6f61 645f 6d6f 6465 6c73  ance(load_models
-000003a0: 2c20 7374 7229 3a20 0d0a 2020 2020 2020  , str): ..      
-000003b0: 2020 2020 2020 6966 206c 6f61 645f 6d6f        if load_mo
-000003c0: 6465 6c73 2e6c 6f77 6572 2829 203d 3d20  dels.lower() == 
-000003d0: 2761 6c6c 273a 200d 0a20 2020 2020 2020  'all': ..       
-000003e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-000003f0: 6164 5f6d 6f64 656c 7320 3d20 6176 6169  ad_models = avai
-00000400: 6c61 626c 655f 6d6f 6465 6c73 0d0a 2020  lable_models..  
-00000410: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-00000420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000430: 2020 7365 6c66 2e6c 6f61 645f 6d6f 6465    self.load_mode
-00000440: 6c73 203d 205b 6c6f 6164 5f6d 6f64 656c  ls = [load_model
-00000450: 735d 0d0a 2020 2020 2020 2020 656c 6966  s]..        elif
-00000460: 2069 7369 6e73 7461 6e63 6528 6c6f 6164   isinstance(load
-00000470: 5f6d 6f64 656c 732c 206c 6973 7429 3a20  _models, list): 
-00000480: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000490: 2027 616c 6c27 2069 6e20 6c6f 6164 5f6d   'all' in load_m
-000004a0: 6f64 656c 7320 6f72 2027 416c 6c27 2069  odels or 'All' i
-000004b0: 6e20 6c6f 6164 5f6d 6f64 656c 733a 200d  n load_models: .
-000004c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004d0: 2073 656c 662e 6c6f 6164 5f6d 6f64 656c   self.load_model
-000004e0: 7320 3d20 6176 6169 6c61 626c 655f 6d6f  s = available_mo
-000004f0: 6465 6c73 200d 0a20 2020 2020 2020 2020  dels ..         
-00000500: 2020 2065 6c73 653a 200d 0a20 2020 2020     else: ..     
-00000510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000520: 6c6f 6164 5f6d 6f64 656c 7320 3d20 6c69  load_models = li
-00000530: 7374 2873 6574 286c 6f61 645f 6d6f 6465  st(set(load_mode
-00000540: 6c73 2929 0d0a 2020 2020 2020 2020 656c  ls))..        el
-00000550: 7365 3a20 0d0a 2020 2020 2020 2020 2020  se: ..          
-00000560: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00000570: 6f72 2822 696e 7075 7420 276c 6f61 645f  or("input 'load_
-00000580: 6d6f 6465 6c73 2720 6d75 7374 2062 6520  models' must be 
-00000590: 6569 7468 6572 2073 7472 206f 7220 6c69  either str or li
-000005a0: 7374 2229 0d0a 2020 2020 2020 2020 0d0a  st")..        ..
-000005b0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-000005c0: 6765 722e 7761 726e 696e 6728 2222 2253  ger.warning("""S
-000005d0: 656c 6563 7465 6420 4d6f 6465 6c28 7329  elected Model(s)
-000005e0: 2066 6f72 2053 656e 7469 6d65 6e74 2041   for Sentiment A
-000005f0: 6e61 6c79 7369 733a 207b 7d22 2222 2e66  nalysis: {}""".f
-00000600: 6f72 6d61 7428 7365 6c66 2e6c 6f61 645f  ormat(self.load_
-00000610: 6d6f 6465 6c73 2929 0d0a 2020 2020 2020  models))..      
-00000620: 2020 2343 6865 636b 2077 6865 7468 6572    #Check whether
-00000630: 2073 656c 6563 7465 6420 6d6f 6465 6c73   selected models
-00000640: 2061 7265 2069 6e73 7461 6c6c 6564 2069   are installed i
-00000650: 6e20 7468 6520 6c6f 6361 6c20 656e 7620  n the local env 
-00000660: 0d0a 2020 2020 2020 2020 2343 6865 636b  ..        #Check
-00000670: 2077 6865 7468 6572 2074 6865 2075 7365   whether the use
-00000680: 7220 6173 7369 676e 6564 2061 7661 696c  r assigned avail
-00000690: 6162 6c65 206d 6f64 656c 7320 666f 7220  able models for 
-000006a0: 6c6f 6164 5f6d 6f64 656c 7320 0d0a 2020  load_models ..  
-000006b0: 2020 2020 2020 756e 696e 7374 616c 6c65        uninstalle
-000006c0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
-000006d0: 756e 6176 6169 6c61 626c 6520 3d20 5b5d  unavailable = []
-000006e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000006f0: 2020 2020 666f 7220 6d6f 6465 6c20 696e      for model in
-00000700: 2074 7164 6d28 7365 6c66 2e6c 6f61 645f   tqdm(self.load_
-00000710: 6d6f 6465 6c73 2c20 6465 7363 3d27 4368  models, desc='Ch
-00000720: 6563 6b69 6e67 204d 6f64 656c 2873 2920  ecking Model(s) 
-00000730: 696e 204c 6f63 616c 2064 6972 2729 3a20  in Local dir'): 
-00000740: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000750: 206d 6f64 656c 2069 6e20 6176 6169 6c61   model in availa
-00000760: 626c 655f 6d6f 6465 6c73 3a20 0d0a 2020  ble_models: ..  
-00000770: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00000780: 6966 206d 6f64 656c 203d 3d20 2761 6c70  if model == 'alp
-00000790: 6861 5641 4445 5227 3a20 0d0a 2020 2020  haVADER': ..    
-000007a0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-000007b0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
-000007c0: 2020 2020 2020 2020 2320 656c 7365 3a0d          # else:.
-000007d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007e0: 2023 2020 2020 2069 6620 6f73 2e70 6174   #     if os.pat
-000007f0: 682e 6973 6469 7228 6d6f 6465 6c29 3a20  h.isdir(model): 
-00000800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000810: 2020 2320 2020 2020 2020 2020 7061 7373    #         pass
-00000820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000830: 2020 2320 2020 2020 656c 7365 3a20 0d0a    #     else: ..
-00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000850: 2320 2020 2020 2020 2020 756e 696e 7374  #         uninst
-00000860: 616c 6c65 642e 6170 7065 6e64 286d 6f64  alled.append(mod
-00000870: 656c 290d 0a20 2020 2020 2020 2020 2020  el)..           
-00000880: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00000890: 6973 6469 7228 6d6f 6465 6c29 3a20 0d0a  isdir(model): ..
-000008a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008b0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
-000008c0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-000008d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008e0: 2020 2020 2020 756e 696e 7374 616c 6c65        uninstalle
-000008f0: 642e 6170 7065 6e64 286d 6f64 656c 290d  d.append(model).
-00000900: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00000910: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
-00000920: 2020 2020 2075 6e61 7661 696c 6162 6c65       unavailable
-00000930: 2e61 7070 656e 6428 6d6f 6465 6c29 0d0a  .append(model)..
-00000940: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000950: 2020 6966 206c 656e 2875 6e61 7661 696c    if len(unavail
-00000960: 6162 6c65 2920 3d3d 2030 3a20 0d0a 2020  able) == 0: ..  
-00000970: 2020 2020 2020 2020 2020 7061 7373 0d0a            pass..
-00000980: 2020 2020 2020 2020 656c 7365 3a20 0d0a          else: ..
-00000990: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000009a0: 6520 5661 6c75 6545 7272 6f72 2822 6d6f  e ValueError("mo
-000009b0: 6465 6c28 7329 207b 7d20 6973 2061 7373  del(s) {} is ass
-000009c0: 6967 6e65 6420 696e 2027 6c6f 6164 5f6d  igned in 'load_m
-000009d0: 6f64 656c 7327 2c20 7768 6963 6820 6973  odels', which is
-000009e0: 2075 6e61 7661 6c69 6162 6c65 2e20 4156   unavaliable. AV
-000009f0: 4149 4c41 424c 4520 4d4f 4445 4c53 3a20  AILABLE MODELS: 
-00000a00: 7b7d 222e 666f 726d 6174 2875 6e61 7661  {}".format(unava
-00000a10: 696c 6162 6c65 2c20 6176 6169 6c61 626c  ilable, availabl
-00000a20: 655f 6d6f 6465 6c73 2929 0d0a 2020 2020  e_models))..    
-00000a30: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-00000a40: 206c 656e 2875 6e69 6e73 7461 6c6c 6564   len(uninstalled
-00000a50: 2920 3d3d 2030 3a20 0d0a 2020 2020 2020  ) == 0: ..      
-00000a60: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-00000a70: 2020 2020 656c 7365 3a20 0d0a 2020 2020      else: ..    
-00000a80: 2020 2020 2020 2020 7261 6973 6520 4669          raise Fi
-00000a90: 6c65 4e6f 7446 6f75 6e64 4572 726f 7228  leNotFoundError(
-00000aa0: 2254 6f20 6c6f 6164 2063 6f72 7265 7370  "To load corresp
-00000ab0: 6f6e 6469 6e67 206d 6f64 656c 2873 292c  onding model(s),
-00000ac0: 2070 7265 2d69 6e73 7461 6c6c 207b 7d20   pre-install {} 
-00000ad0: 7669 6120 6e6c 702e 646f 776e 6c6f 6164  via nlp.download
-00000ae0: 286d 6f64 656c 733d 207b 7d29 222e 666f  (models= {})".fo
-00000af0: 726d 6174 2875 6e69 6e73 7461 6c6c 6564  rmat(uninstalled
-00000b00: 2c20 756e 696e 7374 616c 6c65 6429 290d  , uninstalled)).
-00000b10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000b20: 2020 2066 6f72 206d 6f64 656c 2069 6e20     for model in 
-00000b30: 7471 646d 2873 656c 662e 6c6f 6164 5f6d  tqdm(self.load_m
-00000b40: 6f64 656c 732c 2064 6573 633d 274c 6f61  odels, desc='Loa
-00000b50: 6469 6e67 204d 6f64 656c 2873 2927 293a  ding Model(s)'):
-00000b60: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00000b70: 6966 206d 6f64 656c 203d 3d20 2761 6c70  if model == 'alp
-00000b80: 6861 5641 4445 5227 3a20 0d0a 2020 2020  haVADER': ..    
-00000b90: 2020 2020 2020 2020 2320 2020 2020 7365          #     se
-00000ba0: 6c66 2e41 6c70 6861 5641 4445 5220 3d20  lf.AlphaVADER = 
-00000bb0: 616c 7068 6156 4144 4552 2e53 656e 7469  alphaVADER.Senti
-00000bc0: 6d65 6e74 496e 7465 6e73 6974 7941 6e61  mentIntensityAna
-00000bd0: 6c79 7a65 7228 292e 706f 6c61 7269 7479  lyzer().polarity
-00000be0: 5f73 636f 7265 730d 0a20 2020 2020 2020  _scores..       
-00000bf0: 2020 2020 2023 2020 2020 2070 7269 6e74       #     print
-00000c00: 2822 e294 9ce2 9480 e294 8027 616c 7068  (".........'alph
-00000c10: 6156 4144 4552 2720 7375 6363 6573 7366  aVADER' successf
-00000c20: 756c 6c79 206c 6f61 6465 6422 290d 0a20  ully loaded").. 
-00000c30: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00000c40: 2074 696d 652e 736c 6565 7028 3129 0d0a   time.sleep(1)..
-00000c50: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00000c60: 6f64 656c 203d 3d20 2774 7769 7474 6572  odel == 'twitter
-00000c70: 5f72 6f42 4552 5461 5f76 3127 3a20 0d0a  _roBERTa_v1': ..
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 7365 6c66 2e54 7769 7474 6572 5f72 6f42  self.Twitter_roB
-00000ca0: 4552 5461 5f76 315f 746f 6b65 6e69 7a65  ERTa_v1_tokenize
-00000cb0: 7220 3d20 4175 746f 546f 6b65 6e69 7a65  r = AutoTokenize
-00000cc0: 722e 6672 6f6d 5f70 7265 7472 6169 6e65  r.from_pretraine
-00000cd0: 6428 2774 7769 7474 6572 5f72 6f42 4552  d('twitter_roBER
-00000ce0: 5461 5f76 3127 2c20 6c6f 6361 6c5f 6669  Ta_v1', local_fi
-00000cf0: 6c65 735f 6f6e 6c79 3d54 7275 6529 0d0a  les_only=True)..
-00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d10: 7365 6c66 2e54 7769 7474 6572 5f72 6f42  self.Twitter_roB
-00000d20: 4552 5461 5f76 3120 3d20 4175 746f 4d6f  ERTa_v1 = AutoMo
-00000d30: 6465 6c46 6f72 5365 7175 656e 6365 436c  delForSequenceCl
-00000d40: 6173 7369 6669 6361 7469 6f6e 2e66 726f  assification.fro
-00000d50: 6d5f 7072 6574 7261 696e 6564 2827 7477  m_pretrained('tw
-00000d60: 6974 7465 725f 726f 4245 5254 615f 7631  itter_roBERTa_v1
-00000d70: 272c 206c 6f63 616c 5f66 696c 6573 5f6f  ', local_files_o
-00000d80: 6e6c 793d 5472 7565 290d 0a20 2020 2020  nly=True)..     
-00000d90: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00000da0: 2822 e294 9ce2 9480 e294 8027 7477 6974  (".........'twit
-00000db0: 7465 725f 726f 4245 5254 615f 7631 2720  ter_roBERTa_v1' 
-00000dc0: 7375 6363 6573 7366 756c 6c79 206c 6f61  successfully loa
-00000dd0: 6465 6422 290d 0a20 2020 2020 2020 2020  ded")..         
-00000de0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00000df0: 7028 3129 0d0a 2020 2020 2020 2020 2020  p(1)..          
-00000e00: 2020 656c 6966 206d 6f64 656c 203d 3d20    elif model == 
-00000e10: 2774 7769 7474 6572 5f72 6f42 4552 5461  'twitter_roBERTa
-00000e20: 5f76 3227 3a20 0d0a 2020 2020 2020 2020  _v2': ..        
-00000e30: 2020 2020 2020 2020 7365 6c66 2e54 7769          self.Twi
-00000e40: 7474 6572 5f72 6f42 4552 5461 5f76 325f  tter_roBERTa_v2_
-00000e50: 746f 6b65 6e69 7a65 7220 3d20 4175 746f  tokenizer = Auto
-00000e60: 546f 6b65 6e69 7a65 722e 6672 6f6d 5f70  Tokenizer.from_p
-00000e70: 7265 7472 6169 6e65 6428 2774 7769 7474  retrained('twitt
-00000e80: 6572 5f72 6f42 4552 5461 5f76 3227 2c20  er_roBERTa_v2', 
-00000e90: 6c6f 6361 6c5f 6669 6c65 735f 6f6e 6c79  local_files_only
-00000ea0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-00000eb0: 2020 2020 2020 2020 7365 6c66 2e54 7769          self.Twi
-00000ec0: 7474 6572 5f72 6f42 4552 5461 5f76 3220  tter_roBERTa_v2 
-00000ed0: 3d20 4175 746f 4d6f 6465 6c46 6f72 5365  = AutoModelForSe
-00000ee0: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
-00000ef0: 7469 6f6e 2e66 726f 6d5f 7072 6574 7261  tion.from_pretra
-00000f00: 696e 6564 2827 7477 6974 7465 725f 726f  ined('twitter_ro
-00000f10: 4245 5254 615f 7632 272c 206c 6f63 616c  BERTa_v2', local
-00000f20: 5f66 696c 6573 5f6f 6e6c 793d 5472 7565  _files_only=True
-00000f30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00000f40: 2020 2070 7269 6e74 2822 e294 9ce2 9480     print("......
-00000f50: e294 8027 7477 6974 7465 725f 726f 4245  ...'twitter_roBE
-00000f60: 5254 615f 7632 2720 7375 6363 6573 7366  RTa_v2' successf
-00000f70: 756c 6c79 206c 6f61 6465 6422 290d 0a20  ully loaded").. 
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000f90: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
-00000fa0: 2020 2020 2020 2020 2020 656c 6966 206d            elif m
-00000fb0: 6f64 656c 203d 3d20 2774 7769 7474 6572  odel == 'twitter
-00000fc0: 5f58 4c4d 5f72 6f42 4552 5461 273a 0d0a  _XLM_roBERTa':..
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fe0: 7365 6c66 2e54 7769 7474 6572 5f58 4c4d  self.Twitter_XLM
-00000ff0: 5f72 6f42 4552 5461 5f74 6f6b 656e 697a  _roBERTa_tokeniz
-00001000: 6572 203d 2041 7574 6f54 6f6b 656e 697a  er = AutoTokeniz
-00001010: 6572 2e66 726f 6d5f 7072 6574 7261 696e  er.from_pretrain
-00001020: 6564 2827 7477 6974 7465 725f 584c 4d5f  ed('twitter_XLM_
-00001030: 726f 4245 5254 6127 2c20 6c6f 6361 6c5f  roBERTa', local_
-00001040: 6669 6c65 735f 6f6e 6c79 3d54 7275 6529  files_only=True)
-00001050: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001060: 2020 7365 6c66 2e54 7769 7474 6572 5f58    self.Twitter_X
-00001070: 4c4d 5f72 6f42 4552 5461 203d 2041 7574  LM_roBERTa = Aut
-00001080: 6f4d 6f64 656c 466f 7253 6571 7565 6e63  oModelForSequenc
-00001090: 6543 6c61 7373 6966 6963 6174 696f 6e2e  eClassification.
-000010a0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
-000010b0: 2774 7769 7474 6572 5f58 4c4d 5f72 6f42  'twitter_XLM_roB
-000010c0: 4552 5461 272c 206c 6f63 616c 5f66 696c  ERTa', local_fil
-000010d0: 6573 5f6f 6e6c 793d 5472 7565 290d 0a20  es_only=True).. 
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000010f0: 7269 6e74 2822 e294 9ce2 9480 e294 8027  rint(".........'
-00001100: 7477 6974 7465 725f 584c 4d5f 726f 4245  twitter_XLM_roBE
-00001110: 5254 6127 2073 7563 6365 7373 6675 6c6c  RTa' successfull
-00001120: 7920 6c6f 6164 6564 2229 0d0a 2020 2020  y loaded")..    
-00001130: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00001140: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
-00001150: 2020 2020 2020 2065 6c69 6620 6d6f 6465         elif mode
-00001160: 6c20 3d3d 2027 6669 6e42 4552 5427 3a20  l == 'finBERT': 
-00001170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001180: 2020 7365 6c66 2e46 696e 4245 5254 5f74    self.FinBERT_t
-00001190: 6f6b 656e 697a 6572 203d 2041 7574 6f54  okenizer = AutoT
-000011a0: 6f6b 656e 697a 6572 2e66 726f 6d5f 7072  okenizer.from_pr
-000011b0: 6574 7261 696e 6564 2827 6669 6e42 4552  etrained('finBER
-000011c0: 5427 2c20 6c6f 6361 6c5f 6669 6c65 735f  T', local_files_
-000011d0: 6f6e 6c79 3d54 7275 6529 0d0a 2020 2020  only=True)..    
-000011e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000011f0: 2e46 696e 4245 5254 203d 2041 7574 6f4d  .FinBERT = AutoM
-00001200: 6f64 656c 466f 7253 6571 7565 6e63 6543  odelForSequenceC
-00001210: 6c61 7373 6966 6963 6174 696f 6e2e 6672  lassification.fr
-00001220: 6f6d 5f70 7265 7472 6169 6e65 6428 2766  om_pretrained('f
-00001230: 696e 4245 5254 272c 206c 6f63 616c 5f66  inBERT', local_f
-00001240: 696c 6573 5f6f 6e6c 793d 5472 7565 290d  iles_only=True).
-00001250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001260: 2070 7269 6e74 2822 e294 9ce2 9480 e294   print("........
-00001270: 8027 6669 6e42 4552 5427 2073 7563 6365  .'finBERT' succe
-00001280: 7373 6675 6c6c 7920 6c6f 6164 6564 2229  ssfully loaded")
-00001290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000012a0: 2020 7469 6d65 2e73 6c65 6570 2831 290d    time.sleep(1).
-000012b0: 0a0d 0a20 2020 2064 6566 2072 6573 6361  ...    def resca
-000012c0: 6c69 6e67 2873 656c 662c 206f 6c64 5f76  ling(self, old_v
-000012d0: 616c 7565 2c20 6f6c 645f 6d69 6e76 616c  alue, old_minval
-000012e0: 7565 2c20 6f6c 645f 6d61 7876 616c 7565  ue, old_maxvalue
-000012f0: 293a 0d0a 2020 2020 2020 2020 6e65 775f  ):..        new_
-00001300: 6d61 7876 616c 7565 2c20 6e65 775f 6d69  maxvalue, new_mi
-00001310: 6e76 616c 7565 203d 2031 2c20 2d31 0d0a  nvalue = 1, -1..
-00001320: 2020 2020 2020 2020 6e65 775f 7661 6c75          new_valu
-00001330: 6520 3d20 322a 2828 6f6c 645f 7661 6c75  e = 2*((old_valu
-00001340: 6520 2d20 6f6c 645f 6d69 6e76 616c 7565  e - old_minvalue
-00001350: 292f 286f 6c64 5f6d 6178 7661 6c75 6520  )/(old_maxvalue 
-00001360: 2d20 6f6c 645f 6d69 6e76 616c 7565 2929  - old_minvalue))
-00001370: 202d 2031 200d 0a20 2020 2020 2020 2072   - 1 ..        r
-00001380: 6574 7572 6e20 726f 756e 6428 6e65 775f  eturn round(new_
-00001390: 7661 6c75 652c 2035 2920 0d0a 0d0a 2020  value, 5) ....  
-000013a0: 2020 2361 5641 4445 520d 0a20 2020 2023    #aVADER..    #
-000013b0: 2064 6566 2061 6c70 6861 5641 4445 5228   def alphaVADER(
-000013c0: 7365 6c66 2c20 7465 7874 2c20 7465 7874  self, text, text
-000013d0: 5f74 7970 652c 2073 756d 6d61 7269 7a65  _type, summarize
-000013e0: 3d54 7275 6529 3a0d 0a20 2020 2023 2020  =True):..    #  
-000013f0: 2020 2069 6620 7465 7874 5f74 7970 652e     if text_type.
-00001400: 6c6f 7765 7228 2920 3d3d 2027 6e65 7773  lower() == 'news
-00001410: 273a 200d 0a20 2020 2023 2020 2020 2020  ': ..    #      
-00001420: 2020 2074 6578 7420 3d20 7072 6570 726f     text = prepro
-00001430: 6365 7373 2e6e 6577 7328 7465 7874 290d  cess.news(text).
-00001440: 0a20 2020 2023 2020 2020 2065 6c69 6620  .    #     elif 
-00001450: 7465 7874 5f74 7970 652e 6c6f 7765 7228  text_type.lower(
-00001460: 2920 3d3d 2027 7477 6565 7473 273a 200d  ) == 'tweets': .
-00001470: 0a20 2020 2023 2020 2020 2020 2020 2074  .    #         t
-00001480: 6578 7420 3d20 7072 6570 726f 6365 7373  ext = preprocess
-00001490: 2e74 7765 6574 7328 7465 7874 290d 0a20  .tweets(text).. 
-000014a0: 2020 2023 2020 2020 2061 6c70 6861 5641     #     alphaVA
-000014b0: 4445 525f 6469 6374 203d 2073 656c 662e  DER_dict = self.
-000014c0: 416c 7068 6156 4144 4552 2874 6578 7429  AlphaVADER(text)
-000014d0: 0d0a 2020 2020 2320 2020 2020 6966 2073  ..    #     if s
-000014e0: 756d 6d61 7269 7a65 2069 7320 5472 7565  ummarize is True
-000014f0: 3a20 0d0a 2020 2020 2320 2020 2020 2020  : ..    #       
-00001500: 2020 7265 7475 726e 2061 6c70 6861 5641    return alphaVA
-00001510: 4445 525f 6469 6374 5b27 636f 6d70 6f75  DER_dict['compou
-00001520: 6e64 275d 0d0a 2020 2020 2320 2020 2020  nd']..    #     
-00001530: 656c 7365 3a20 0d0a 2020 2020 2320 2020  else: ..    #   
-00001540: 2020 2020 2020 7265 7475 726e 2061 6c70        return alp
-00001550: 6861 5641 4445 525f 6469 6374 0d0a 0d0a  haVADER_dict....
-00001560: 2020 2020 2374 7769 7474 6572 5f72 6f42      #twitter_roB
-00001570: 4552 5461 5f76 310d 0a20 2020 2064 6566  ERTa_v1..    def
-00001580: 2074 7769 7474 6572 5f72 6f42 4552 5461   twitter_roBERTa
-00001590: 5f76 3128 7365 6c66 2c20 0d0a 2020 2020  _v1(self, ..    
-000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2074 6578 743a 7374 722c         text:str,
-000015c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000015d0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-000015e0: 7874 5f74 7970 653a 7374 722c 200d 0a20  xt_type:str, .. 
+00000160: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00000170: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00000180: 2020 2020 2020 2020 206c 6f61 645f 6d6f           load_mo
+00000190: 6465 6c73 2028 7374 7220 6f72 206c 6973  dels (str or lis
+000001a0: 7429 3a20 4176 6169 6c61 626c 6520 6d6f  t): Available mo
+000001b0: 6465 6c73 2074 6f20 6265 206c 6f61 6465  dels to be loade
+000001c0: 642e 205c 6e0d 0a20 2020 2020 2020 2020  d. \n..         
+000001d0: 2020 2020 2020 2049 6e63 6c75 6465 733a         Includes:
+000001e0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000001f0: 2020 2028 6929 2027 7477 6974 7465 725f     (i) 'twitter_
+00000200: 726f 4245 5254 615f 7631 273b 0d0a 2020  roBERTa_v1';..  
+00000210: 2020 2020 2020 2020 2020 2020 2020 2869                (i
+00000220: 6929 2774 7769 7474 6572 5f72 6f42 4552  i)'twitter_roBER
+00000230: 5461 5f76 3227 3b20 200d 0a20 2020 2020  Ta_v2';  ..     
+00000240: 2020 2020 2020 2020 2020 2028 6969 6929             (iii)
+00000250: 2027 7477 6974 7465 725f 584c 4d5f 726f   'twitter_XLM_ro
+00000260: 4245 5254 6127 3b20 616e 640d 0a20 2020  BERTa'; and..   
+00000270: 2020 2020 2020 2020 2020 2020 2028 6976               (iv
+00000280: 2920 2766 696e 4245 5254 270d 0a20 2020  ) 'finBERT'..   
+00000290: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000002a0: 2020 7365 6c66 2e6c 6f67 6765 7220 3d20    self.logger = 
+000002b0: 6c6f 6767 696e 672e 6765 745f 6c6f 6767  logging.get_logg
+000002c0: 6572 2822 7472 616e 7366 6f72 6d65 7273  er("transformers
+000002d0: 2229 0d0a 2020 2020 2020 2020 6176 6169  ")..        avai
+000002e0: 6c61 626c 655f 6d6f 6465 6c73 203d 205b  lable_models = [
+000002f0: 2327 616c 7068 6156 4144 4552 270d 0a20  #'alphaVADER'.. 
+00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000310: 2020 2020 2020 2020 2020 2027 7477 6974             'twit
+00000320: 7465 725f 726f 4245 5254 615f 7631 272c  ter_roBERTa_v1',
+00000330: 2027 7477 6974 7465 725f 726f 4245 5254   'twitter_roBERT
+00000340: 615f 7632 272c 2027 7477 6974 7465 725f  a_v2', 'twitter_
+00000350: 584c 4d5f 726f 4245 5254 6127 2c20 2766  XLM_roBERTa', 'f
+00000360: 696e 4245 5254 275d 0d0a 2020 2020 2020  inBERT']..      
+00000370: 2020 0d0a 2020 2020 2020 2020 6966 2069    ..        if i
+00000380: 7369 6e73 7461 6e63 6528 6c6f 6164 5f6d  sinstance(load_m
+00000390: 6f64 656c 732c 2073 7472 293a 200d 0a20  odels, str): .. 
+000003a0: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+000003b0: 6164 5f6d 6f64 656c 732e 6c6f 7765 7228  ad_models.lower(
+000003c0: 2920 3d3d 2027 616c 6c27 3a20 0d0a 2020  ) == 'all': ..  
+000003d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000003e0: 6c66 2e6c 6f61 645f 6d6f 6465 6c73 203d  lf.load_models =
+000003f0: 2061 7661 696c 6162 6c65 5f6d 6f64 656c   available_model
+00000400: 730d 0a20 2020 2020 2020 2020 2020 2065  s..            e
+00000410: 6c73 653a 200d 0a20 2020 2020 2020 2020  lse: ..         
+00000420: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+00000430: 5f6d 6f64 656c 7320 3d20 5b6c 6f61 645f  _models = [load_
+00000440: 6d6f 6465 6c73 5d0d 0a20 2020 2020 2020  models]..       
+00000450: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000460: 286c 6f61 645f 6d6f 6465 6c73 2c20 6c69  (load_models, li
+00000470: 7374 293a 200d 0a20 2020 2020 2020 2020  st): ..         
+00000480: 2020 2069 6620 2761 6c6c 2720 696e 206c     if 'all' in l
+00000490: 6f61 645f 6d6f 6465 6c73 206f 7220 2741  oad_models or 'A
+000004a0: 6c6c 2720 696e 206c 6f61 645f 6d6f 6465  ll' in load_mode
+000004b0: 6c73 3a20 0d0a 2020 2020 2020 2020 2020  ls: ..          
+000004c0: 2020 2020 2020 7365 6c66 2e6c 6f61 645f        self.load_
+000004d0: 6d6f 6465 6c73 203d 2061 7661 696c 6162  models = availab
+000004e0: 6c65 5f6d 6f64 656c 7320 0d0a 2020 2020  le_models ..    
+000004f0: 2020 2020 2020 2020 656c 7365 3a20 0d0a          else: ..
+00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000510: 7365 6c66 2e6c 6f61 645f 6d6f 6465 6c73  self.load_models
+00000520: 203d 206c 6973 7428 7365 7428 6c6f 6164   = list(set(load
+00000530: 5f6d 6f64 656c 7329 290d 0a20 2020 2020  _models))..     
+00000540: 2020 2065 6c73 653a 200d 0a20 2020 2020     else: ..     
+00000550: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00000560: 7565 4572 726f 7228 2269 6e70 7574 2027  ueError("input '
+00000570: 6c6f 6164 5f6d 6f64 656c 7327 206d 7573  load_models' mus
+00000580: 7420 6265 2065 6974 6865 7220 7374 7220  t be either str 
+00000590: 6f72 206c 6973 7422 290d 0a20 2020 2020  or list")..     
+000005a0: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
+000005b0: 662e 6c6f 6767 6572 2e77 6172 6e69 6e67  f.logger.warning
+000005c0: 2822 2222 5365 6c65 6374 6564 204d 6f64  ("""Selected Mod
+000005d0: 656c 2873 2920 666f 7220 5365 6e74 696d  el(s) for Sentim
+000005e0: 656e 7420 416e 616c 7973 6973 3a20 7b7d  ent Analysis: {}
+000005f0: 2222 222e 666f 726d 6174 2873 656c 662e  """.format(self.
+00000600: 6c6f 6164 5f6d 6f64 656c 7329 290d 0a20  load_models)).. 
+00000610: 2020 2020 2020 2023 4368 6563 6b20 7768         #Check wh
+00000620: 6574 6865 7220 7365 6c65 6374 6564 206d  ether selected m
+00000630: 6f64 656c 7320 6172 6520 696e 7374 616c  odels are instal
+00000640: 6c65 6420 696e 2074 6865 206c 6f63 616c  led in the local
+00000650: 2065 6e76 200d 0a20 2020 2020 2020 2023   env ..        #
+00000660: 4368 6563 6b20 7768 6574 6865 7220 7468  Check whether th
+00000670: 6520 7573 6572 2061 7373 6967 6e65 6420  e user assigned 
+00000680: 6176 6169 6c61 626c 6520 6d6f 6465 6c73  available models
+00000690: 2066 6f72 206c 6f61 645f 6d6f 6465 6c73   for load_models
+000006a0: 200d 0a20 2020 2020 2020 2075 6e69 6e73   ..        unins
+000006b0: 7461 6c6c 6564 203d 205b 5d0d 0a20 2020  talled = []..   
+000006c0: 2020 2020 2075 6e61 7661 696c 6162 6c65       unavailable
+000006d0: 203d 205b 5d0d 0a20 2020 2020 2020 200d   = []..        .
+000006e0: 0a20 2020 2020 2020 2066 6f72 206d 6f64  .        for mod
+000006f0: 656c 2069 6e20 7471 646d 2873 656c 662e  el in tqdm(self.
+00000700: 6c6f 6164 5f6d 6f64 656c 732c 2064 6573  load_models, des
+00000710: 633d 2743 6865 636b 696e 6720 4d6f 6465  c='Checking Mode
+00000720: 6c28 7329 2069 6e20 4c6f 6361 6c20 6469  l(s) in Local di
+00000730: 7227 293a 200d 0a20 2020 2020 2020 2020  r'): ..         
+00000740: 2020 2069 6620 6d6f 6465 6c20 696e 2061     if model in a
+00000750: 7661 696c 6162 6c65 5f6d 6f64 656c 733a  vailable_models:
+00000760: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00000770: 2020 2023 2069 6620 6d6f 6465 6c20 3d3d     # if model ==
+00000780: 2027 616c 7068 6156 4144 4552 273a 200d   'alphaVADER': .
+00000790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007a0: 2023 2020 2020 2070 6173 730d 0a20 2020   #     pass..   
+000007b0: 2020 2020 2020 2020 2020 2020 2023 2065               # e
+000007c0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000007d0: 2020 2020 2020 2320 2020 2020 6966 206f        #     if o
+000007e0: 732e 7061 7468 2e69 7364 6972 286d 6f64  s.path.isdir(mod
+000007f0: 656c 293a 200d 0a20 2020 2020 2020 2020  el): ..         
+00000800: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00000810: 2070 6173 730d 0a20 2020 2020 2020 2020   pass..         
+00000820: 2020 2020 2020 2023 2020 2020 2065 6c73         #     els
+00000830: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
+00000840: 2020 2020 2023 2020 2020 2020 2020 2075       #         u
+00000850: 6e69 6e73 7461 6c6c 6564 2e61 7070 656e  ninstalled.appen
+00000860: 6428 6d6f 6465 6c29 0d0a 2020 2020 2020  d(model)..      
+00000870: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
+00000880: 7061 7468 2e69 7364 6972 286d 6f64 656c  path.isdir(model
+00000890: 293a 200d 0a20 2020 2020 2020 2020 2020  ): ..           
+000008a0: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000008c0: 6c73 653a 200d 0a20 2020 2020 2020 2020  lse: ..         
+000008d0: 2020 2020 2020 2020 2020 2075 6e69 6e73             unins
+000008e0: 7461 6c6c 6564 2e61 7070 656e 6428 6d6f  talled.append(mo
+000008f0: 6465 6c29 0d0a 2020 2020 2020 2020 2020  del)..          
+00000900: 2020 656c 7365 3a20 0d0a 2020 2020 2020    else: ..      
+00000910: 2020 2020 2020 2020 2020 756e 6176 6169            unavai
+00000920: 6c61 626c 652e 6170 7065 6e64 286d 6f64  lable.append(mod
+00000930: 656c 290d 0a20 2020 2020 2020 200d 0a20  el)..        .. 
+00000940: 2020 2020 2020 2069 6620 6c65 6e28 756e         if len(un
+00000950: 6176 6169 6c61 626c 6529 203d 3d20 303a  available) == 0:
+00000960: 200d 0a20 2020 2020 2020 2020 2020 2070   ..            p
+00000970: 6173 730d 0a20 2020 2020 2020 2065 6c73  ass..        els
+00000980: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
+00000990: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000009a0: 7228 226d 6f64 656c 2873 2920 7b7d 2069  r("model(s) {} i
+000009b0: 7320 6173 7369 676e 6564 2069 6e20 276c  s assigned in 'l
+000009c0: 6f61 645f 6d6f 6465 6c73 272c 2077 6869  oad_models', whi
+000009d0: 6368 2069 7320 756e 6176 616c 6961 626c  ch is unavaliabl
+000009e0: 652e 2041 5641 494c 4142 4c45 204d 4f44  e. AVAILABLE MOD
+000009f0: 454c 533a 207b 7d22 2e66 6f72 6d61 7428  ELS: {}".format(
+00000a00: 756e 6176 6169 6c61 626c 652c 2061 7661  unavailable, ava
+00000a10: 696c 6162 6c65 5f6d 6f64 656c 7329 290d  ilable_models)).
+00000a20: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00000a30: 2020 2069 6620 6c65 6e28 756e 696e 7374     if len(uninst
+00000a40: 616c 6c65 6429 203d 3d20 303a 200d 0a20  alled) == 0: .. 
+00000a50: 2020 2020 2020 2020 2020 2070 6173 730d             pass.
+00000a60: 0a20 2020 2020 2020 2065 6c73 653a 200d  .        else: .
+00000a70: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00000a80: 7365 2046 696c 654e 6f74 466f 756e 6445  se FileNotFoundE
+00000a90: 7272 6f72 2822 546f 206c 6f61 6420 636f  rror("To load co
+00000aa0: 7272 6573 706f 6e64 696e 6720 6d6f 6465  rresponding mode
+00000ab0: 6c28 7329 2c20 7072 652d 696e 7374 616c  l(s), pre-instal
+00000ac0: 6c20 7b7d 2076 6961 2063 6f6e 6c70 2e64  l {} via conlp.d
+00000ad0: 6f77 6e6c 6f61 6428 6d6f 6465 6c73 3d20  ownload(models= 
+00000ae0: 7b7d 2922 2e66 6f72 6d61 7428 756e 696e  {})".format(unin
+00000af0: 7374 616c 6c65 642c 2075 6e69 6e73 7461  stalled, uninsta
+00000b00: 6c6c 6564 2929 0d0a 2020 2020 2020 2020  lled))..        
+00000b10: 0d0a 2020 2020 2020 2020 666f 7220 6d6f  ..        for mo
+00000b20: 6465 6c20 696e 2074 7164 6d28 7365 6c66  del in tqdm(self
+00000b30: 2e6c 6f61 645f 6d6f 6465 6c73 2c20 6465  .load_models, de
+00000b40: 7363 3d27 4c6f 6164 696e 6720 4d6f 6465  sc='Loading Mode
+00000b50: 6c28 7329 2729 3a0d 0a20 2020 2020 2020  l(s)'):..       
+00000b60: 2020 2020 2023 2069 6620 6d6f 6465 6c20       # if model 
+00000b70: 3d3d 2027 616c 7068 6156 4144 4552 273a  == 'alphaVADER':
+00000b80: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
+00000b90: 2020 2020 2073 656c 662e 416c 7068 6156       self.AlphaV
+00000ba0: 4144 4552 203d 2061 6c70 6861 5641 4445  ADER = alphaVADE
+00000bb0: 522e 5365 6e74 696d 656e 7449 6e74 656e  R.SentimentInten
+00000bc0: 7369 7479 416e 616c 797a 6572 2829 2e70  sityAnalyzer().p
+00000bd0: 6f6c 6172 6974 795f 7363 6f72 6573 0d0a  olarity_scores..
+00000be0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00000bf0: 2020 7072 696e 7428 22e2 949c e294 80e2    print(".......
+00000c00: 9480 2761 6c70 6861 5641 4445 5227 2073  ..'alphaVADER' s
+00000c10: 7563 6365 7373 6675 6c6c 7920 6c6f 6164  uccessfully load
+00000c20: 6564 2229 0d0a 2020 2020 2020 2020 2020  ed")..          
+00000c30: 2020 2320 2020 2020 7469 6d65 2e73 6c65    #     time.sle
+00000c40: 6570 2831 290d 0a20 2020 2020 2020 2020  ep(1)..         
+00000c50: 2020 2069 6620 6d6f 6465 6c20 3d3d 2027     if model == '
+00000c60: 7477 6974 7465 725f 726f 4245 5254 615f  twitter_roBERTa_
+00000c70: 7631 273a 200d 0a20 2020 2020 2020 2020  v1': ..         
+00000c80: 2020 2020 2020 2073 656c 662e 5477 6974         self.Twit
+00000c90: 7465 725f 726f 4245 5254 615f 7631 5f74  ter_roBERTa_v1_t
+00000ca0: 6f6b 656e 697a 6572 203d 2041 7574 6f54  okenizer = AutoT
+00000cb0: 6f6b 656e 697a 6572 2e66 726f 6d5f 7072  okenizer.from_pr
+00000cc0: 6574 7261 696e 6564 2827 7477 6974 7465  etrained('twitte
+00000cd0: 725f 726f 4245 5254 615f 7631 272c 206c  r_roBERTa_v1', l
+00000ce0: 6f63 616c 5f66 696c 6573 5f6f 6e6c 793d  ocal_files_only=
+00000cf0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+00000d00: 2020 2020 2020 2073 656c 662e 5477 6974         self.Twit
+00000d10: 7465 725f 726f 4245 5254 615f 7631 203d  ter_roBERTa_v1 =
+00000d20: 2041 7574 6f4d 6f64 656c 466f 7253 6571   AutoModelForSeq
+00000d30: 7565 6e63 6543 6c61 7373 6966 6963 6174  uenceClassificat
+00000d40: 696f 6e2e 6672 6f6d 5f70 7265 7472 6169  ion.from_pretrai
+00000d50: 6e65 6428 2774 7769 7474 6572 5f72 6f42  ned('twitter_roB
+00000d60: 4552 5461 5f76 3127 2c20 6c6f 6361 6c5f  ERTa_v1', local_
+00000d70: 6669 6c65 735f 6f6e 6c79 3d54 7275 6529  files_only=True)
+00000d80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000d90: 2020 7072 696e 7428 22e2 949c e294 80e2    print(".......
+00000da0: 9480 2774 7769 7474 6572 5f72 6f42 4552  ..'twitter_roBER
+00000db0: 5461 5f76 3127 2073 7563 6365 7373 6675  Ta_v1' successfu
+00000dc0: 6c6c 7920 6c6f 6164 6564 2229 0d0a 2020  lly loaded")..  
+00000dd0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00000de0: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
+00000df0: 2020 2020 2020 2020 2065 6c69 6620 6d6f           elif mo
+00000e00: 6465 6c20 3d3d 2027 7477 6974 7465 725f  del == 'twitter_
+00000e10: 726f 4245 5254 615f 7632 273a 200d 0a20  roBERTa_v2': .. 
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000e30: 656c 662e 5477 6974 7465 725f 726f 4245  elf.Twitter_roBE
+00000e40: 5254 615f 7632 5f74 6f6b 656e 697a 6572  RTa_v2_tokenizer
+00000e50: 203d 2041 7574 6f54 6f6b 656e 697a 6572   = AutoTokenizer
+00000e60: 2e66 726f 6d5f 7072 6574 7261 696e 6564  .from_pretrained
+00000e70: 2827 7477 6974 7465 725f 726f 4245 5254  ('twitter_roBERT
+00000e80: 615f 7632 272c 206c 6f63 616c 5f66 696c  a_v2', local_fil
+00000e90: 6573 5f6f 6e6c 793d 5472 7565 290d 0a20  es_only=True).. 
+00000ea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000eb0: 656c 662e 5477 6974 7465 725f 726f 4245  elf.Twitter_roBE
+00000ec0: 5254 615f 7632 203d 2041 7574 6f4d 6f64  RTa_v2 = AutoMod
+00000ed0: 656c 466f 7253 6571 7565 6e63 6543 6c61  elForSequenceCla
+00000ee0: 7373 6966 6963 6174 696f 6e2e 6672 6f6d  ssification.from
+00000ef0: 5f70 7265 7472 6169 6e65 6428 2774 7769  _pretrained('twi
+00000f00: 7474 6572 5f72 6f42 4552 5461 5f76 3227  tter_roBERTa_v2'
+00000f10: 2c20 6c6f 6361 6c5f 6669 6c65 735f 6f6e  , local_files_on
+00000f20: 6c79 3d54 7275 6529 0d0a 2020 2020 2020  ly=True)..      
+00000f30: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00000f40: 22e2 949c e294 80e2 9480 2774 7769 7474  ".........'twitt
+00000f50: 6572 5f72 6f42 4552 5461 5f76 3227 2073  er_roBERTa_v2' s
+00000f60: 7563 6365 7373 6675 6c6c 7920 6c6f 6164  uccessfully load
+00000f70: 6564 2229 0d0a 2020 2020 2020 2020 2020  ed")..          
+00000f80: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00000f90: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
+00000fa0: 2065 6c69 6620 6d6f 6465 6c20 3d3d 2027   elif model == '
+00000fb0: 7477 6974 7465 725f 584c 4d5f 726f 4245  twitter_XLM_roBE
+00000fc0: 5254 6127 3a0d 0a20 2020 2020 2020 2020  RTa':..         
+00000fd0: 2020 2020 2020 2073 656c 662e 5477 6974         self.Twit
+00000fe0: 7465 725f 584c 4d5f 726f 4245 5254 615f  ter_XLM_roBERTa_
+00000ff0: 746f 6b65 6e69 7a65 7220 3d20 4175 746f  tokenizer = Auto
+00001000: 546f 6b65 6e69 7a65 722e 6672 6f6d 5f70  Tokenizer.from_p
+00001010: 7265 7472 6169 6e65 6428 2774 7769 7474  retrained('twitt
+00001020: 6572 5f58 4c4d 5f72 6f42 4552 5461 272c  er_XLM_roBERTa',
+00001030: 206c 6f63 616c 5f66 696c 6573 5f6f 6e6c   local_files_onl
+00001040: 793d 5472 7565 290d 0a20 2020 2020 2020  y=True)..       
+00001050: 2020 2020 2020 2020 2073 656c 662e 5477           self.Tw
+00001060: 6974 7465 725f 584c 4d5f 726f 4245 5254  itter_XLM_roBERT
+00001070: 6120 3d20 4175 746f 4d6f 6465 6c46 6f72  a = AutoModelFor
+00001080: 5365 7175 656e 6365 436c 6173 7369 6669  SequenceClassifi
+00001090: 6361 7469 6f6e 2e66 726f 6d5f 7072 6574  cation.from_pret
+000010a0: 7261 696e 6564 2827 7477 6974 7465 725f  rained('twitter_
+000010b0: 584c 4d5f 726f 4245 5254 6127 2c20 6c6f  XLM_roBERTa', lo
+000010c0: 6361 6c5f 6669 6c65 735f 6f6e 6c79 3d54  cal_files_only=T
+000010d0: 7275 6529 0d0a 2020 2020 2020 2020 2020  rue)..          
+000010e0: 2020 2020 2020 7072 696e 7428 22e2 949c        print("...
+000010f0: e294 80e2 9480 2774 7769 7474 6572 5f58  ......'twitter_X
+00001100: 4c4d 5f72 6f42 4552 5461 2720 7375 6363  LM_roBERTa' succ
+00001110: 6573 7366 756c 6c79 206c 6f61 6465 6422  essfully loaded"
+00001120: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00001130: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+00001140: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00001150: 6966 206d 6f64 656c 203d 3d20 2766 696e  if model == 'fin
+00001160: 4245 5254 273a 200d 0a20 2020 2020 2020  BERT': ..       
+00001170: 2020 2020 2020 2020 2073 656c 662e 4669           self.Fi
+00001180: 6e42 4552 545f 746f 6b65 6e69 7a65 7220  nBERT_tokenizer 
+00001190: 3d20 4175 746f 546f 6b65 6e69 7a65 722e  = AutoTokenizer.
+000011a0: 6672 6f6d 5f70 7265 7472 6169 6e65 6428  from_pretrained(
+000011b0: 2766 696e 4245 5254 272c 206c 6f63 616c  'finBERT', local
+000011c0: 5f66 696c 6573 5f6f 6e6c 793d 5472 7565  _files_only=True
+000011d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000011e0: 2020 2073 656c 662e 4669 6e42 4552 5420     self.FinBERT 
+000011f0: 3d20 4175 746f 4d6f 6465 6c46 6f72 5365  = AutoModelForSe
+00001200: 7175 656e 6365 436c 6173 7369 6669 6361  quenceClassifica
+00001210: 7469 6f6e 2e66 726f 6d5f 7072 6574 7261  tion.from_pretra
+00001220: 696e 6564 2827 6669 6e42 4552 5427 2c20  ined('finBERT', 
+00001230: 6c6f 6361 6c5f 6669 6c65 735f 6f6e 6c79  local_files_only
+00001240: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00001250: 2020 2020 2020 2020 7072 696e 7428 22e2          print(".
+00001260: 949c e294 80e2 9480 2766 696e 4245 5254  ........'finBERT
+00001270: 2720 7375 6363 6573 7366 756c 6c79 206c  ' successfully l
+00001280: 6f61 6465 6422 290d 0a20 2020 2020 2020  oaded")..       
+00001290: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+000012a0: 6565 7028 3129 0d0a 0d0a 2020 2020 6465  eep(1)....    de
+000012b0: 6620 7265 7363 616c 696e 6728 7365 6c66  f rescaling(self
+000012c0: 2c20 6f6c 645f 7661 6c75 652c 206f 6c64  , old_value, old
+000012d0: 5f6d 696e 7661 6c75 652c 206f 6c64 5f6d  _minvalue, old_m
+000012e0: 6178 7661 6c75 6529 3a0d 0a20 2020 2020  axvalue):..     
+000012f0: 2020 206e 6577 5f6d 6178 7661 6c75 652c     new_maxvalue,
+00001300: 206e 6577 5f6d 696e 7661 6c75 6520 3d20   new_minvalue = 
+00001310: 312c 202d 310d 0a20 2020 2020 2020 206e  1, -1..        n
+00001320: 6577 5f76 616c 7565 203d 2032 2a28 286f  ew_value = 2*((o
+00001330: 6c64 5f76 616c 7565 202d 206f 6c64 5f6d  ld_value - old_m
+00001340: 696e 7661 6c75 6529 2f28 6f6c 645f 6d61  invalue)/(old_ma
+00001350: 7876 616c 7565 202d 206f 6c64 5f6d 696e  xvalue - old_min
+00001360: 7661 6c75 6529 2920 2d20 3120 0d0a 2020  value)) - 1 ..  
+00001370: 2020 2020 2020 7265 7475 726e 2072 6f75        return rou
+00001380: 6e64 286e 6577 5f76 616c 7565 2c20 3529  nd(new_value, 5)
+00001390: 200d 0a0d 0a20 2020 2023 6156 4144 4552   ....    #aVADER
+000013a0: 0d0a 2020 2020 2320 6465 6620 616c 7068  ..    # def alph
+000013b0: 6156 4144 4552 2873 656c 662c 2074 6578  aVADER(self, tex
+000013c0: 742c 2074 6578 745f 7479 7065 2c20 7375  t, text_type, su
+000013d0: 6d6d 6172 697a 653d 5472 7565 293a 0d0a  mmarize=True):..
+000013e0: 2020 2020 2320 2020 2020 6966 2074 6578      #     if tex
+000013f0: 745f 7479 7065 2e6c 6f77 6572 2829 203d  t_type.lower() =
+00001400: 3d20 276e 6577 7327 3a20 0d0a 2020 2020  = 'news': ..    
+00001410: 2320 2020 2020 2020 2020 7465 7874 203d  #         text =
+00001420: 2070 7265 7072 6f63 6573 732e 6e65 7773   preprocess.news
+00001430: 2874 6578 7429 0d0a 2020 2020 2320 2020  (text)..    #   
+00001440: 2020 656c 6966 2074 6578 745f 7479 7065    elif text_type
+00001450: 2e6c 6f77 6572 2829 203d 3d20 2774 7765  .lower() == 'twe
+00001460: 6574 7327 3a20 0d0a 2020 2020 2320 2020  ets': ..    #   
+00001470: 2020 2020 2020 7465 7874 203d 2070 7265        text = pre
+00001480: 7072 6f63 6573 732e 7477 6565 7473 2874  process.tweets(t
+00001490: 6578 7429 0d0a 2020 2020 2320 2020 2020  ext)..    #     
+000014a0: 616c 7068 6156 4144 4552 5f64 6963 7420  alphaVADER_dict 
+000014b0: 3d20 7365 6c66 2e41 6c70 6861 5641 4445  = self.AlphaVADE
+000014c0: 5228 7465 7874 290d 0a20 2020 2023 2020  R(text)..    #  
+000014d0: 2020 2069 6620 7375 6d6d 6172 697a 6520     if summarize 
+000014e0: 6973 2054 7275 653a 200d 0a20 2020 2023  is True: ..    #
+000014f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001500: 616c 7068 6156 4144 4552 5f64 6963 745b  alphaVADER_dict[
+00001510: 2763 6f6d 706f 756e 6427 5d0d 0a20 2020  'compound']..   
+00001520: 2023 2020 2020 2065 6c73 653a 200d 0a20   #     else: .. 
+00001530: 2020 2023 2020 2020 2020 2020 2072 6574     #         ret
+00001540: 7572 6e20 616c 7068 6156 4144 4552 5f64  urn alphaVADER_d
+00001550: 6963 740d 0a0d 0a20 2020 2023 7477 6974  ict....    #twit
+00001560: 7465 725f 726f 4245 5254 615f 7631 0d0a  ter_roBERTa_v1..
+00001570: 2020 2020 6465 6620 7477 6974 7465 725f      def twitter_
+00001580: 726f 4245 5254 615f 7631 2873 656c 662c  roBERTa_v1(self,
+00001590: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000015a0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+000015b0: 7874 3a73 7472 2c20 0d0a 2020 2020 2020  xt:str, ..      
+000015c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015d0: 2020 2020 2074 6578 745f 7479 7065 3a73       text_type:s
+000015e0: 7472 2c20 0d0a 2020 2020 2020 2020 2020  tr, ..          
 000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 2020 2020 2020 7375 6d6d 6172            summar
-00001610: 697a 653a 626f 6f6c 3d54 7275 6529 202d  ize:bool=True) -
-00001620: 3e20 666c 6f61 7420 6f72 2064 6963 743a  > float or dict:
-00001630: 0d0a 2020 2020 2020 2020 2222 2261 2072  ..        """a r
-00001640: 6f42 4552 5461 206d 6f64 656c 2074 7261  oBERTa model tra
-00001650: 696e 6564 206f 6e20 3538 4d20 7477 6565  ined on 58M twee
-00001660: 7473 2061 6e64 2066 696e 6574 756e 6564  ts and finetuned
-00001670: 2066 6f72 2073 656e 7469 6d65 6e74 2061   for sentiment a
-00001680: 6e61 6c79 7369 7320 7769 7468 2074 6865  nalysis with the
-00001690: 2054 7765 6574 4576 616c 2062 656e 6368   TweetEval bench
-000016a0: 6d61 726b 2222 220d 0a20 2020 2020 2020  mark"""..       
-000016b0: 2074 7279 3a20 0d0a 2020 2020 2020 2020   try: ..        
-000016c0: 2020 2020 6966 2074 6578 745f 7479 7065      if text_type
-000016d0: 2e6c 6f77 6572 2829 203d 3d20 276e 6577  .lower() == 'new
-000016e0: 7327 3a20 0d0a 2020 2020 2020 2020 2020  s': ..          
-000016f0: 2020 2020 2020 6f72 6967 696e 616c 5f64        original_d
-00001700: 6f63 203d 2070 7265 7072 6f63 6573 732e  oc = preprocess.
-00001710: 6e65 7773 2874 6578 7429 0d0a 2020 2020  news(text)..    
-00001720: 2020 2020 2020 2020 656c 6966 2074 6578          elif tex
-00001730: 745f 7479 7065 2e6c 6f77 6572 2829 203d  t_type.lower() =
-00001740: 3d20 2774 7765 6574 7327 3a20 0d0a 2020  = 'tweets': ..  
-00001750: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-00001760: 6967 696e 616c 5f64 6f63 203d 2070 7265  iginal_doc = pre
-00001770: 7072 6f63 6573 732e 7477 6565 7473 2874  process.tweets(t
-00001780: 6578 7429 0d0a 2020 2020 2020 2020 2020  ext)..          
-00001790: 2020 6c61 6265 6c73 203d 205b 276e 6567    labels = ['neg
-000017a0: 6174 6976 6527 2c20 276e 6575 7472 616c  ative', 'neutral
-000017b0: 272c 2027 706f 7369 7469 7665 275d 0d0a  ', 'positive']..
-000017c0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-000017d0: 696e 616c 5f74 6f6b 656e 7320 3d20 7365  inal_tokens = se
-000017e0: 6c66 2e54 7769 7474 6572 5f72 6f42 4552  lf.Twitter_roBER
-000017f0: 5461 5f76 315f 746f 6b65 6e69 7a65 7228  Ta_v1_tokenizer(
-00001800: 6f72 6967 696e 616c 5f64 6f63 2c20 7265  original_doc, re
-00001810: 7475 726e 5f74 656e 736f 7273 3d27 7074  turn_tensors='pt
-00001820: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
-00001830: 6c65 6e5f 6f72 6967 696e 616c 5f74 6f6b  len_original_tok
-00001840: 656e 7320 3d20 6c65 6e28 6f72 6967 696e  ens = len(origin
-00001850: 616c 5f74 6f6b 656e 735b 2769 6e70 7574  al_tokens['input
-00001860: 5f69 6473 275d 5b30 5d29 0d0a 2020 2020  _ids'][0])..    
-00001870: 2020 2020 2020 2020 6966 206c 656e 5f6f          if len_o
-00001880: 7269 6769 6e61 6c5f 746f 6b65 6e73 203c  riginal_tokens <
-00001890: 3d20 3531 343a 200d 0a20 2020 2020 2020  = 514: ..       
-000018a0: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
-000018b0: 203d 2073 656c 662e 5477 6974 7465 725f   = self.Twitter_
-000018c0: 726f 4245 5254 615f 7631 282a 2a6f 7269  roBERTa_v1(**ori
-000018d0: 6769 6e61 6c5f 746f 6b65 6e73 290d 0a20  ginal_tokens).. 
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000018f0: 636f 7269 6e67 203d 2073 636f 7269 6e67  coring = scoring
-00001900: 5b30 5d5b 305d 2e64 6574 6163 6828 292e  [0][0].detach().
-00001910: 6e75 6d70 7928 290d 0a20 2020 2020 2020  numpy()..       
-00001920: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
-00001930: 203d 2073 6f66 746d 6178 2873 636f 7269   = softmax(scori
-00001940: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
-00001950: 2020 2020 2072 616e 6b69 6e67 203d 206e       ranking = n
-00001960: 702e 6172 6773 6f72 7428 7363 6f72 696e  p.argsort(scorin
-00001970: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-00001980: 2020 2020 7365 6e74 5f64 6963 742c 2063      sent_dict, c
-00001990: 6f6d 706f 756e 6420 3d20 7b27 6e65 6727  ompound = {'neg'
-000019a0: 3a20 302c 2027 6e65 7527 3a20 302c 2027  : 0, 'neu': 0, '
-000019b0: 706f 7327 3a20 302c 2027 636f 6d70 6f75  pos': 0, 'compou
-000019c0: 6e64 273a 2030 7d2c 2030 200d 0a20 2020  nd': 0}, 0 ..   
-000019d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-000019e0: 2069 2069 6e20 7261 6e67 6528 7363 6f72   i in range(scor
-000019f0: 696e 672e 7368 6170 655b 305d 293a 0d0a  ing.shape[0]):..
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a10: 2020 2020 6c20 3d20 6c61 6265 6c73 5b72      l = labels[r
-00001a20: 616e 6b69 6e67 5b69 5d5d 0d0a 2020 2020  anking[i]]..    
-00001a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a40: 7320 3d20 7363 6f72 696e 675b 7261 6e6b  s = scoring[rank
-00001a50: 696e 675b 695d 5d0d 0a20 2020 2020 2020  ing[i]]..       
-00001a60: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001a70: 6c20 3d3d 2027 706f 7369 7469 7665 273a  l == 'positive':
-00001a80: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00001a90: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
-00001aa0: 756e 6420 2b3d 2073 2a31 300d 0a20 2020  und += s*10..   
-00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ac0: 2020 2020 2073 656e 745f 6469 6374 2e75       sent_dict.u
-00001ad0: 7064 6174 6528 7b27 706f 7327 3a20 726f  pdate({'pos': ro
-00001ae0: 756e 6428 666c 6f61 7428 7329 2c20 3529  und(float(s), 5)
-00001af0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00001b00: 2020 2020 2020 2020 656c 6966 206c 203d          elif l =
-00001b10: 3d20 276e 6567 6174 6976 6527 3a20 0d0a  = 'negative': ..
-00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2020 2020 2020 2020 636f 6d70 6f75 6e64          compound
-00001b40: 202d 3d20 732a 3130 0d0a 2020 2020 2020   -= s*10..      
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 7365 6e74 5f64 6963 742e 7570 6461    sent_dict.upda
-00001b70: 7465 287b 276e 6567 273a 2072 6f75 6e64  te({'neg': round
-00001b80: 2866 6c6f 6174 2873 292c 2035 297d 290d  (float(s), 5)}).
-00001b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ba0: 2020 2020 2065 6c73 653a 200d 0a20 2020       else: ..   
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 2020 2020 2063 6f6d 706f 756e 6420 2b3d       compound +=
-00001bd0: 2073 2a31 0d0a 2020 2020 2020 2020 2020   s*1..          
-00001be0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001bf0: 6e74 5f64 6963 742e 7570 6461 7465 287b  nt_dict.update({
-00001c00: 276e 6575 273a 2072 6f75 6e64 2866 6c6f  'neu': round(flo
-00001c10: 6174 2873 292c 2035 297d 290d 0a20 2020  at(s), 5)})..   
-00001c20: 2020 2020 2020 2020 2020 2020 2073 656e               sen
-00001c30: 745f 6469 6374 2e75 7064 6174 6528 7b27  t_dict.update({'
-00001c40: 636f 6d70 6f75 6e64 273a 2073 656c 662e  compound': self.
-00001c50: 7265 7363 616c 696e 6728 666c 6f61 7428  rescaling(float(
-00001c60: 636f 6d70 6f75 6e64 292c 202d 3130 2c20  compound), -10, 
-00001c70: 3130 297d 290d 0a20 2020 2020 2020 2020  10)})..         
-00001c80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001c90: 2020 2020 2020 2020 2069 6620 7375 6d6d           if summ
-00001ca0: 6172 697a 6520 6973 2054 7275 653a 200d  arize is True: .
-00001cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001cc0: 2020 2020 2072 6574 7572 6e20 7365 6e74       return sent
-00001cd0: 5f64 6963 745b 2763 6f6d 706f 756e 6427  _dict['compound'
-00001ce0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00001cf0: 2020 2065 6c73 653a 200d 0a20 2020 2020     else: ..     
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001d10: 6574 7572 6e20 7365 6e74 5f64 6963 740d  eturn sent_dict.
-00001d20: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00001d30: 6620 6c65 6e5f 6f72 6967 696e 616c 5f74  f len_original_t
-00001d40: 6f6b 656e 7320 3e20 3531 343a 200d 0a20  okens > 514: .. 
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00001d60: 7365 6c66 2e6c 6f67 6765 722e 7761 726e  self.logger.warn
-00001d70: 696e 6728 22e2 949c e294 80e2 9480 2041  ing("......... A
-00001d80: 6e79 2077 6172 6e69 6e67 7320 7265 6c61  ny warnings rela
-00001d90: 7465 6420 746f 2054 6f6b 656e 5365 7175  ted to TokenSequ
-00001da0: 656e 6365 4c65 6e67 7468 2063 616e 2062  enceLength can b
-00001db0: 6520 6967 6e6f 7265 6420 6173 2069 6e70  e ignored as inp
-00001dc0: 7574 2027 7465 7874 2720 6861 7320 6265  ut 'text' has be
-00001dd0: 656e 2073 706c 6974 6564 2c20 7375 6368  en splited, such
-00001de0: 2074 6861 7420 7468 6520 7365 7175 656e   that the sequen
-00001df0: 6365 206c 656e 6774 6820 6f66 2065 6163  ce length of eac
-00001e00: 6820 7370 6c69 7420 6973 2061 6c77 6179  h split is alway
-00001e10: 7320 6c65 7373 2074 6861 6e20 7468 6520  s less than the 
-00001e20: 7370 6563 6966 6965 6420 6d61 7869 6d75  specified maximu
-00001e30: 6d20 7365 7175 656e 6365 206c 656e 6774  m sequence lengt
-00001e40: 6822 290d 0a20 2020 2020 2020 2020 2020  h")..           
-00001e50: 2020 2020 2074 6f74 616c 5f6e 6567 2c20       total_neg, 
-00001e60: 746f 7461 6c5f 6e65 752c 2074 6f74 616c  total_neu, total
-00001e70: 5f70 6f73 2c20 746f 7461 6c5f 636f 6d70  _pos, total_comp
-00001e80: 6f75 6e64 203d 2030 2c20 302c 2030 2c20  ound = 0, 0, 0, 
-00001e90: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
-00001ea0: 2020 2020 6f72 6967 696e 616c 5f64 6f63      original_doc
-00001eb0: 203d 206e 702e 6172 7261 7928 5b6f 7269   = np.array([ori
-00001ec0: 6769 6e61 6c5f 646f 632e 7370 6c69 7428  ginal_doc.split(
-00001ed0: 295d 290d 0a20 2020 2020 2020 2020 2020  )])..           
-00001ee0: 2020 2020 206e 756d 5f73 706c 6974 203d       num_split =
-00001ef0: 2069 6e74 2872 6f75 6e64 2828 6c65 6e5f   int(round((len_
-00001f00: 6f72 6967 696e 616c 5f74 6f6b 656e 732f  original_tokens/
-00001f10: 3531 3429 2b31 2c20 3029 290d 0a20 2020  514)+1, 0))..   
-00001f20: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00001f30: 6167 7261 7068 7320 3d20 6e70 2e61 7272  agraphs = np.arr
-00001f40: 6179 5f73 706c 6974 286f 7269 6769 6e61  ay_split(origina
-00001f50: 6c5f 646f 632c 206e 756d 5f73 706c 6974  l_doc, num_split
-00001f60: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
-00001f70: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00001f80: 2069 6e20 7261 6e67 6528 6e75 6d5f 7370   in range(num_sp
-00001f90: 6c69 7429 3a20 0d0a 2020 2020 2020 2020  lit): ..        
-00001fa0: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00001fb0: 6772 6170 6820 3d20 7061 7261 6772 6170  graph = paragrap
-00001fc0: 6873 5b69 5d0d 0a20 2020 2020 2020 2020  hs[i]..         
-00001fd0: 2020 2020 2020 2020 2020 2070 6172 6167             parag
-00001fe0: 7261 7068 203d 2022 2022 2e6a 6f69 6e28  raph = " ".join(
-00001ff0: 7374 7228 776f 7264 292e 7265 706c 6163  str(word).replac
-00002000: 6528 2227 222c 2022 2229 2066 6f72 2077  e("'", "") for w
-00002010: 6f72 6420 696e 206c 6973 7428 7061 7261  ord in list(para
-00002020: 6772 6170 6829 290d 0a20 2020 2020 2020  graph))..       
-00002030: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00002040: 6167 7261 7068 203d 2070 6172 6167 7261  agraph = paragra
-00002050: 7068 2e72 6570 6c61 6365 2822 5c6e 222c  ph.replace("\n",
-00002060: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
-00002070: 2020 2020 2020 2020 2020 7061 7261 6772            paragr
-00002080: 6170 6820 3d20 7061 7261 6772 6170 682e  aph = paragraph.
-00002090: 7265 706c 6163 6528 225b 222c 2022 2229  replace("[", "")
-000020a0: 2e72 6570 6c61 6365 2822 5d22 2c20 2222  .replace("]", ""
-000020b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000020c0: 2020 2020 2020 2074 6f6b 656e 7320 3d20         tokens = 
-000020d0: 7365 6c66 2e54 7769 7474 6572 5f72 6f42  self.Twitter_roB
-000020e0: 4552 5461 5f76 315f 746f 6b65 6e69 7a65  ERTa_v1_tokenize
-000020f0: 7228 7061 7261 6772 6170 682c 2072 6574  r(paragraph, ret
-00002100: 7572 6e5f 7465 6e73 6f72 733d 2770 7427  urn_tensors='pt'
-00002110: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002120: 2020 2020 2020 2073 636f 7269 6e67 203d         scoring =
-00002130: 2073 656c 662e 5477 6974 7465 725f 726f   self.Twitter_ro
-00002140: 4245 5254 615f 7631 282a 2a74 6f6b 656e  BERTa_v1(**token
-00002150: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
-00002160: 2020 2020 2020 2020 7363 6f72 696e 6720          scoring 
-00002170: 3d20 7363 6f72 696e 675b 305d 5b30 5d2e  = scoring[0][0].
-00002180: 6465 7461 6368 2829 2e6e 756d 7079 2829  detach().numpy()
-00002190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000021a0: 2020 2020 2020 7363 6f72 696e 6720 3d20        scoring = 
-000021b0: 736f 6674 6d61 7828 7363 6f72 696e 6729  softmax(scoring)
-000021c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000021d0: 2020 2020 2020 7261 6e6b 696e 6720 3d20        ranking = 
-000021e0: 6e70 2e61 7267 736f 7274 2873 636f 7269  np.argsort(scori
-000021f0: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
-00002200: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-00002210: 6e20 7261 6e67 6528 7363 6f72 696e 672e  n range(scoring.
-00002220: 7368 6170 655b 305d 293a 0d0a 2020 2020  shape[0]):..    
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 6c20 3d20 6c61 6265 6c73 5b72      l = labels[r
-00002250: 616e 6b69 6e67 5b69 5d5d 0d0a 2020 2020  anking[i]]..    
-00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002270: 2020 2020 7320 3d20 7363 6f72 696e 675b      s = scoring[
-00002280: 7261 6e6b 696e 675b 695d 5d0d 0a20 2020  ranking[i]]..   
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2069 6620 6c20 3d3d 2027 706f       if l == 'po
-000022b0: 7369 7469 7665 273a 200d 0a20 2020 2020  sitive': ..     
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2020 2020 2074 6f74 616c 5f70 6f73         total_pos
-000022e0: 202b 3d20 7320 0d0a 2020 2020 2020 2020   += s ..        
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 746f 7461 6c5f 636f 6d70 6f75      total_compou
-00002310: 6e64 202b 3d20 732a 3130 0d0a 2020 2020  nd += s*10..    
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2020 656c 6966 206c 203d 3d20 276e      elif l == 'n
-00002340: 6567 6174 6976 6527 3a20 0d0a 2020 2020  egative': ..    
-00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002360: 2020 2020 2020 2020 746f 7461 6c5f 6e65          total_ne
-00002370: 6720 2b3d 2073 0d0a 2020 2020 2020 2020  g += s..        
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 2020 746f 7461 6c5f 636f 6d70 6f75      total_compou
-000023a0: 6e64 202d 3d20 732a 3130 0d0a 2020 2020  nd -= s*10..    
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2020 2020 656c 7365 3a20 0d0a 2020 2020      else: ..    
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 2020 2020 746f 7461 6c5f 6e65          total_ne
-000023f0: 7520 2b3d 2073 0d0a 2020 2020 2020 2020  u += s..        
-00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002410: 2020 2020 746f 7461 6c5f 636f 6d70 6f75      total_compou
-00002420: 6e64 202b 3d20 732a 310d 0a20 2020 2020  nd += s*1..     
-00002430: 2020 2020 2020 2020 2020 2073 656e 745f             sent_
-00002440: 6469 6374 203d 207b 276e 6567 273a 2072  dict = {'neg': r
-00002450: 6f75 6e64 2874 6f74 616c 5f6e 6567 2f6e  ound(total_neg/n
-00002460: 756d 5f73 706c 6974 2c20 3529 2c20 0d0a  um_split, 5), ..
+00001600: 2073 756d 6d61 7269 7a65 3a62 6f6f 6c3d   summarize:bool=
+00001610: 5472 7565 2920 2d3e 2066 6c6f 6174 206f  True) -> float o
+00001620: 7220 6469 6374 3a0d 0a20 2020 2020 2020  r dict:..       
+00001630: 2022 2222 6120 726f 4245 5254 6120 6d6f   """a roBERTa mo
+00001640: 6465 6c20 7472 6169 6e65 6420 6f6e 2035  del trained on 5
+00001650: 384d 2074 7765 6574 7320 616e 6420 6669  8M tweets and fi
+00001660: 6e65 7475 6e65 6420 666f 7220 7365 6e74  netuned for sent
+00001670: 696d 656e 7420 616e 616c 7973 6973 2077  iment analysis w
+00001680: 6974 6820 7468 6520 5477 6565 7445 7661  ith the TweetEva
+00001690: 6c20 6265 6e63 686d 6172 6b22 2222 0d0a  l benchmark"""..
+000016a0: 2020 2020 2020 2020 7472 793a 200d 0a20          try: .. 
+000016b0: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+000016c0: 7874 5f74 7970 652e 6c6f 7765 7228 2920  xt_type.lower() 
+000016d0: 3d3d 2027 6e65 7773 273a 200d 0a20 2020  == 'news': ..   
+000016e0: 2020 2020 2020 2020 2020 2020 206f 7269               ori
+000016f0: 6769 6e61 6c5f 646f 6320 3d20 7072 6570  ginal_doc = prep
+00001700: 726f 6365 7373 2e6e 6577 7328 7465 7874  rocess.news(text
+00001710: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00001720: 6c69 6620 7465 7874 5f74 7970 652e 6c6f  lif text_type.lo
+00001730: 7765 7228 2920 3d3d 2027 7477 6565 7473  wer() == 'tweets
+00001740: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
+00001750: 2020 2020 206f 7269 6769 6e61 6c5f 646f       original_do
+00001760: 6320 3d20 7072 6570 726f 6365 7373 2e74  c = preprocess.t
+00001770: 7765 6574 7328 7465 7874 290d 0a20 2020  weets(text)..   
+00001780: 2020 2020 2020 2020 206c 6162 656c 7320           labels 
+00001790: 3d20 5b27 6e65 6761 7469 7665 272c 2027  = ['negative', '
+000017a0: 6e65 7574 7261 6c27 2c20 2770 6f73 6974  neutral', 'posit
+000017b0: 6976 6527 5d0d 0a20 2020 2020 2020 2020  ive']..         
+000017c0: 2020 206f 7269 6769 6e61 6c5f 746f 6b65     original_toke
+000017d0: 6e73 203d 2073 656c 662e 5477 6974 7465  ns = self.Twitte
+000017e0: 725f 726f 4245 5254 615f 7631 5f74 6f6b  r_roBERTa_v1_tok
+000017f0: 656e 697a 6572 286f 7269 6769 6e61 6c5f  enizer(original_
+00001800: 646f 632c 2072 6574 7572 6e5f 7465 6e73  doc, return_tens
+00001810: 6f72 733d 2770 7427 290d 0a20 2020 2020  ors='pt')..     
+00001820: 2020 2020 2020 206c 656e 5f6f 7269 6769         len_origi
+00001830: 6e61 6c5f 746f 6b65 6e73 203d 206c 656e  nal_tokens = len
+00001840: 286f 7269 6769 6e61 6c5f 746f 6b65 6e73  (original_tokens
+00001850: 5b27 696e 7075 745f 6964 7327 5d5b 305d  ['input_ids'][0]
+00001860: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00001870: 6620 6c65 6e5f 6f72 6967 696e 616c 5f74  f len_original_t
+00001880: 6f6b 656e 7320 3c3d 2035 3134 3a20 0d0a  okens <= 514: ..
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 7363 6f72 696e 6720 3d20 7365 6c66 2e54  scoring = self.T
+000018b0: 7769 7474 6572 5f72 6f42 4552 5461 5f76  witter_roBERTa_v
+000018c0: 3128 2a2a 6f72 6967 696e 616c 5f74 6f6b  1(**original_tok
+000018d0: 656e 7329 0d0a 2020 2020 2020 2020 2020  ens)..          
+000018e0: 2020 2020 2020 7363 6f72 696e 6720 3d20        scoring = 
+000018f0: 7363 6f72 696e 675b 305d 5b30 5d2e 6465  scoring[0][0].de
+00001900: 7461 6368 2829 2e6e 756d 7079 2829 0d0a  tach().numpy()..
+00001910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001920: 7363 6f72 696e 6720 3d20 736f 6674 6d61  scoring = softma
+00001930: 7828 7363 6f72 696e 6729 0d0a 2020 2020  x(scoring)..    
+00001940: 2020 2020 2020 2020 2020 2020 7261 6e6b              rank
+00001950: 696e 6720 3d20 6e70 2e61 7267 736f 7274  ing = np.argsort
+00001960: 2873 636f 7269 6e67 290d 0a20 2020 2020  (scoring)..     
+00001970: 2020 2020 2020 2020 2020 2073 656e 745f             sent_
+00001980: 6469 6374 2c20 636f 6d70 6f75 6e64 203d  dict, compound =
+00001990: 207b 276e 6567 273a 2030 2c20 276e 6575   {'neg': 0, 'neu
+000019a0: 273a 2030 2c20 2770 6f73 273a 2030 2c20  ': 0, 'pos': 0, 
+000019b0: 2763 6f6d 706f 756e 6427 3a20 307d 2c20  'compound': 0}, 
+000019c0: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
+000019d0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+000019e0: 6765 2873 636f 7269 6e67 2e73 6861 7065  ge(scoring.shape
+000019f0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+00001a00: 2020 2020 2020 2020 2020 206c 203d 206c             l = l
+00001a10: 6162 656c 735b 7261 6e6b 696e 675b 695d  abels[ranking[i]
+00001a20: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00001a30: 2020 2020 2020 2073 203d 2073 636f 7269         s = scori
+00001a40: 6e67 5b72 616e 6b69 6e67 5b69 5d5d 0d0a  ng[ranking[i]]..
+00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a60: 2020 2020 6966 206c 203d 3d20 2770 6f73      if l == 'pos
+00001a70: 6974 6976 6527 3a20 0d0a 2020 2020 2020  itive': ..      
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 636f 6d70 6f75 6e64 202b 3d20 732a    compound += s*
+00001aa0: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
+00001ab0: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
+00001ac0: 5f64 6963 742e 7570 6461 7465 287b 2770  _dict.update({'p
+00001ad0: 6f73 273a 2072 6f75 6e64 2866 6c6f 6174  os': round(float
+00001ae0: 2873 292c 2035 297d 290d 0a20 2020 2020  (s), 5)})..     
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00001b00: 6c69 6620 6c20 3d3d 2027 6e65 6761 7469  lif l == 'negati
+00001b10: 7665 273a 200d 0a20 2020 2020 2020 2020  ve': ..         
+00001b20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001b30: 6f6d 706f 756e 6420 2d3d 2073 2a31 300d  ompound -= s*10.
+00001b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b50: 2020 2020 2020 2020 2073 656e 745f 6469           sent_di
+00001b60: 6374 2e75 7064 6174 6528 7b27 6e65 6727  ct.update({'neg'
+00001b70: 3a20 726f 756e 6428 666c 6f61 7428 7329  : round(float(s)
+00001b80: 2c20 3529 7d29 0d0a 2020 2020 2020 2020  , 5)})..        
+00001b90: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00001ba0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+00001bb0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00001bc0: 6f75 6e64 202b 3d20 732a 310d 0a20 2020  ound += s*1..   
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2073 656e 745f 6469 6374 2e75       sent_dict.u
+00001bf0: 7064 6174 6528 7b27 6e65 7527 3a20 726f  pdate({'neu': ro
+00001c00: 756e 6428 666c 6f61 7428 7329 2c20 3529  und(float(s), 5)
+00001c10: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00001c20: 2020 2020 7365 6e74 5f64 6963 742e 7570      sent_dict.up
+00001c30: 6461 7465 287b 2763 6f6d 706f 756e 6427  date({'compound'
+00001c40: 3a20 7365 6c66 2e72 6573 6361 6c69 6e67  : self.rescaling
+00001c50: 2866 6c6f 6174 2863 6f6d 706f 756e 6429  (float(compound)
+00001c60: 2c20 2d31 302c 2031 3029 7d29 0d0a 2020  , -10, 10)})..  
+00001c70: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 6966 2073 756d 6d61 7269 7a65 2069 7320  if summarize is 
+00001ca0: 5472 7565 3a20 0d0a 2020 2020 2020 2020  True: ..        
+00001cb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00001cc0: 726e 2073 656e 745f 6469 6374 5b27 636f  rn sent_dict['co
+00001cd0: 6d70 6f75 6e64 275d 0d0a 2020 2020 2020  mpound']..      
+00001ce0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+00001cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001d00: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
+00001d10: 745f 6469 6374 0d0a 2020 2020 2020 2020  t_dict..        
+00001d20: 2020 2020 656c 6966 206c 656e 5f6f 7269      elif len_ori
+00001d30: 6769 6e61 6c5f 746f 6b65 6e73 203e 2035  ginal_tokens > 5
+00001d40: 3134 3a20 0d0a 2020 2020 2020 2020 2020  14: ..          
+00001d50: 2020 2020 2020 2373 656c 662e 6c6f 6767        #self.logg
+00001d60: 6572 2e77 6172 6e69 6e67 2822 e294 9ce2  er.warning("....
+00001d70: 9480 e294 8020 416e 7920 7761 726e 696e  ..... Any warnin
+00001d80: 6773 2072 656c 6174 6564 2074 6f20 546f  gs related to To
+00001d90: 6b65 6e53 6571 7565 6e63 654c 656e 6774  kenSequenceLengt
+00001da0: 6820 6361 6e20 6265 2069 676e 6f72 6564  h can be ignored
+00001db0: 2061 7320 696e 7075 7420 2774 6578 7427   as input 'text'
+00001dc0: 2068 6173 2062 6565 6e20 7370 6c69 7465   has been splite
+00001dd0: 642c 2073 7563 6820 7468 6174 2074 6865  d, such that the
+00001de0: 2073 6571 7565 6e63 6520 6c65 6e67 7468   sequence length
+00001df0: 206f 6620 6561 6368 2073 706c 6974 2069   of each split i
+00001e00: 7320 616c 7761 7973 206c 6573 7320 7468  s always less th
+00001e10: 616e 2074 6865 2073 7065 6369 6669 6564  an the specified
+00001e20: 206d 6178 696d 756d 2073 6571 7565 6e63   maximum sequenc
+00001e30: 6520 6c65 6e67 7468 2229 0d0a 2020 2020  e length")..    
+00001e40: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00001e50: 6c5f 6e65 672c 2074 6f74 616c 5f6e 6575  l_neg, total_neu
+00001e60: 2c20 746f 7461 6c5f 706f 732c 2074 6f74  , total_pos, tot
+00001e70: 616c 5f63 6f6d 706f 756e 6420 3d20 302c  al_compound = 0,
+00001e80: 2030 2c20 302c 2030 200d 0a20 2020 2020   0, 0, 0 ..     
+00001e90: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+00001ea0: 6e61 6c5f 646f 6320 3d20 6e70 2e61 7272  nal_doc = np.arr
+00001eb0: 6179 285b 6f72 6967 696e 616c 5f64 6f63  ay([original_doc
+00001ec0: 2e73 706c 6974 2829 5d29 0d0a 2020 2020  .split()])..    
+00001ed0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00001ee0: 7370 6c69 7420 3d20 696e 7428 726f 756e  split = int(roun
+00001ef0: 6428 286c 656e 5f6f 7269 6769 6e61 6c5f  d((len_original_
+00001f00: 746f 6b65 6e73 2f35 3134 292b 312c 2030  tokens/514)+1, 0
+00001f10: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00001f20: 2020 2020 7061 7261 6772 6170 6873 203d      paragraphs =
+00001f30: 206e 702e 6172 7261 795f 7370 6c69 7428   np.array_split(
+00001f40: 6f72 6967 696e 616c 5f64 6f63 2c20 6e75  original_doc, nu
+00001f50: 6d5f 7370 6c69 742c 2061 7869 733d 3129  m_split, axis=1)
+00001f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001f70: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00001f80: 286e 756d 5f73 706c 6974 293a 200d 0a20  (num_split): .. 
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2070 6172 6167 7261 7068 203d 2070     paragraph = p
+00001fb0: 6172 6167 7261 7068 735b 695d 0d0a 2020  aragraphs[i]..  
+00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fd0: 2020 7061 7261 6772 6170 6820 3d20 2220    paragraph = " 
+00001fe0: 222e 6a6f 696e 2873 7472 2877 6f72 6429  ".join(str(word)
+00001ff0: 2e72 6570 6c61 6365 2822 2722 2c20 2222  .replace("'", ""
+00002000: 2920 666f 7220 776f 7264 2069 6e20 6c69  ) for word in li
+00002010: 7374 2870 6172 6167 7261 7068 2929 0d0a  st(paragraph))..
+00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002030: 2020 2020 7061 7261 6772 6170 6820 3d20      paragraph = 
+00002040: 7061 7261 6772 6170 682e 7265 706c 6163  paragraph.replac
+00002050: 6528 225c 6e22 2c20 2222 290d 0a20 2020  e("\n", "")..   
+00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002070: 2070 6172 6167 7261 7068 203d 2070 6172   paragraph = par
+00002080: 6167 7261 7068 2e72 6570 6c61 6365 2822  agraph.replace("
+00002090: 5b22 2c20 2222 292e 7265 706c 6163 6528  [", "").replace(
+000020a0: 225d 222c 2022 2229 0d0a 2020 2020 2020  "]", "")..      
+000020b0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+000020c0: 6b65 6e73 203d 2073 656c 662e 5477 6974  kens = self.Twit
+000020d0: 7465 725f 726f 4245 5254 615f 7631 5f74  ter_roBERTa_v1_t
+000020e0: 6f6b 656e 697a 6572 2870 6172 6167 7261  okenizer(paragra
+000020f0: 7068 2c20 7265 7475 726e 5f74 656e 736f  ph, return_tenso
+00002100: 7273 3d27 7074 2729 0d0a 2020 2020 2020  rs='pt')..      
+00002110: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00002120: 6f72 696e 6720 3d20 7365 6c66 2e54 7769  oring = self.Twi
+00002130: 7474 6572 5f72 6f42 4552 5461 5f76 3128  tter_roBERTa_v1(
+00002140: 2a2a 746f 6b65 6e73 290d 0a20 2020 2020  **tokens)..     
+00002150: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002160: 636f 7269 6e67 203d 2073 636f 7269 6e67  coring = scoring
+00002170: 5b30 5d5b 305d 2e64 6574 6163 6828 292e  [0][0].detach().
+00002180: 6e75 6d70 7928 290d 0a20 2020 2020 2020  numpy()..       
+00002190: 2020 2020 2020 2020 2020 2020 2073 636f               sco
+000021a0: 7269 6e67 203d 2073 6f66 746d 6178 2873  ring = softmax(s
+000021b0: 636f 7269 6e67 290d 0a20 2020 2020 2020  coring)..       
+000021c0: 2020 2020 2020 2020 2020 2020 2072 616e               ran
+000021d0: 6b69 6e67 203d 206e 702e 6172 6773 6f72  king = np.argsor
+000021e0: 7428 7363 6f72 696e 6729 0d0a 2020 2020  t(scoring)..    
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 666f 7220 6920 696e 2072 616e 6765 2873  for i in range(s
+00002210: 636f 7269 6e67 2e73 6861 7065 5b30 5d29  coring.shape[0])
+00002220: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002230: 2020 2020 2020 2020 2020 206c 203d 206c             l = l
+00002240: 6162 656c 735b 7261 6e6b 696e 675b 695d  abels[ranking[i]
+00002250: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00002260: 2020 2020 2020 2020 2020 2073 203d 2073             s = s
+00002270: 636f 7269 6e67 5b72 616e 6b69 6e67 5b69  coring[ranking[i
+00002280: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
+00002290: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+000022a0: 203d 3d20 2770 6f73 6974 6976 6527 3a20   == 'positive': 
+000022b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000022c0: 2020 2020 2020 2020 2020 2020 2020 746f                to
+000022d0: 7461 6c5f 706f 7320 2b3d 2073 200d 0a20  tal_pos += s .. 
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00002300: 5f63 6f6d 706f 756e 6420 2b3d 2073 2a31  _compound += s*1
+00002310: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00002320: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00002330: 6c20 3d3d 2027 6e65 6761 7469 7665 273a  l == 'negative':
+00002340: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00002350: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00002360: 6f74 616c 5f6e 6567 202b 3d20 730d 0a20  otal_neg += s.. 
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00002390: 5f63 6f6d 706f 756e 6420 2d3d 2073 2a31  _compound -= s*1
+000023a0: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+000023b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000023c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000023d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000023e0: 6f74 616c 5f6e 6575 202b 3d20 730d 0a20  otal_neu += s.. 
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00002410: 5f63 6f6d 706f 756e 6420 2b3d 2073 2a31  _compound += s*1
+00002420: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002430: 2020 7365 6e74 5f64 6963 7420 3d20 7b27    sent_dict = {'
+00002440: 6e65 6727 3a20 726f 756e 6428 746f 7461  neg': round(tota
+00002450: 6c5f 6e65 672f 6e75 6d5f 7370 6c69 742c  l_neg/num_split,
+00002460: 2035 292c 200d 0a20 2020 2020 2020 2020   5), ..         
 00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 2020 2020 2020 2020 2027 6e65               'ne
-00002490: 7527 3a20 726f 756e 6428 746f 7461 6c5f  u': round(total_
-000024a0: 6e65 752f 6e75 6d5f 7370 6c69 742c 2035  neu/num_split, 5
-000024b0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024d0: 2020 2770 6f73 273a 2072 6f75 6e64 2874    'pos': round(t
-000024e0: 6f74 616c 5f70 6f73 2f6e 756d 5f73 706c  otal_pos/num_spl
-000024f0: 6974 2c20 3529 2c20 0d0a 2020 2020 2020  it, 5), ..      
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2020 2020 2020 2027 636f 6d70 6f75 6e64         'compound
-00002520: 273a 2073 656c 662e 7265 7363 616c 696e  ': self.rescalin
-00002530: 6728 746f 7461 6c5f 636f 6d70 6f75 6e64  g(total_compound
-00002540: 2c20 2d31 302a 6e75 6d5f 7370 6c69 742c  , -10*num_split,
-00002550: 2031 302a 6e75 6d5f 7370 6c69 7429 7d0d   10*num_split)}.
-00002560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002570: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002580: 2020 2069 6620 7375 6d6d 6172 697a 6520     if summarize 
-00002590: 6973 2054 7275 653a 200d 0a20 2020 2020  is True: ..     
-000025a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000025b0: 6574 7572 6e20 7365 6e74 5f64 6963 745b  eturn sent_dict[
-000025c0: 2763 6f6d 706f 756e 6427 5d0d 0a20 2020  'compound']..   
-000025d0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000025e0: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
-000025f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002600: 7365 6e74 5f64 6963 7420 0d0a 2020 2020  sent_dict ..    
-00002610: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
-00002620: 6275 7465 4572 726f 723a 200d 0a20 2020  buteError: ..   
-00002630: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-00002640: 7973 7465 6d45 7272 6f72 2822 7477 6974  ystemError("twit
-00002650: 7465 725f 726f 4245 5254 615f 7631 206d  ter_roBERTa_v1 m
-00002660: 7573 7420 6265 206c 6f61 6465 6420 696e  ust be loaded in
-00002670: 2070 7269 6f72 2e20 4c6f 6164 2074 6865   prior. Load the
-00002680: 206d 6f64 656c 2076 6961 206e 6c70 2e73   model via nlp.s
-00002690: 656e 7469 6d65 6e74 286c 6f61 645f 6d6f  entiment(load_mo
-000026a0: 6465 6c73 3d27 7477 6974 7465 725f 726f  dels='twitter_ro
-000026b0: 4245 5254 615f 7631 2729 2229 0d0a 0d0a  BERTa_v1')")....
-000026c0: 2020 2020 2374 7769 7474 6572 5f72 6f42      #twitter_roB
-000026d0: 4552 5461 5f76 320d 0a20 2020 2064 6566  ERTa_v2..    def
-000026e0: 2074 7769 7474 6572 5f72 6f42 4552 5461   twitter_roBERTa
-000026f0: 5f76 3228 7365 6c66 2c20 0d0a 2020 2020  _v2(self, ..    
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2020 2020 2020 2074 6578 743a 7374 722c         text:str,
-00002720: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002730: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00002740: 7874 5f74 7970 653a 7374 722c 200d 0a20  xt_type:str, .. 
+00002480: 2020 2020 276e 6575 273a 2072 6f75 6e64      'neu': round
+00002490: 2874 6f74 616c 5f6e 6575 2f6e 756d 5f73  (total_neu/num_s
+000024a0: 706c 6974 2c20 3529 2c20 0d0a 2020 2020  plit, 5), ..    
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2027 706f 7327 3a20           'pos': 
+000024d0: 726f 756e 6428 746f 7461 6c5f 706f 732f  round(total_pos/
+000024e0: 6e75 6d5f 7370 6c69 742c 2035 292c 200d  num_split, 5), .
+000024f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002500: 2020 2020 2020 2020 2020 2020 2020 2763                'c
+00002510: 6f6d 706f 756e 6427 3a20 7365 6c66 2e72  ompound': self.r
+00002520: 6573 6361 6c69 6e67 2874 6f74 616c 5f63  escaling(total_c
+00002530: 6f6d 706f 756e 642c 202d 3130 2a6e 756d  ompound, -10*num
+00002540: 5f73 706c 6974 2c20 3130 2a6e 756d 5f73  _split, 10*num_s
+00002550: 706c 6974 297d 0d0a 2020 2020 2020 2020  plit)}..        
+00002560: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00002570: 2020 2020 2020 2020 2020 6966 2073 756d            if sum
+00002580: 6d61 7269 7a65 2069 7320 5472 7565 3a20  marize is True: 
+00002590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000025a0: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
+000025b0: 745f 6469 6374 5b27 636f 6d70 6f75 6e64  t_dict['compound
+000025c0: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
+000025d0: 2020 2020 656c 7365 3a20 0d0a 2020 2020      else: ..    
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025f0: 7265 7475 726e 2073 656e 745f 6469 6374  return sent_dict
+00002600: 200d 0a20 2020 2020 2020 2065 7863 6570   ..        excep
+00002610: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
+00002620: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+00002630: 7261 6973 6520 5379 7374 656d 4572 726f  raise SystemErro
+00002640: 7228 2274 7769 7474 6572 5f72 6f42 4552  r("twitter_roBER
+00002650: 5461 5f76 3120 6d75 7374 2062 6520 6c6f  Ta_v1 must be lo
+00002660: 6164 6564 2069 6e20 7072 696f 722e 204c  aded in prior. L
+00002670: 6f61 6420 7468 6520 6d6f 6465 6c20 7669  oad the model vi
+00002680: 6120 6e6c 702e 7365 6e74 696d 656e 7428  a nlp.sentiment(
+00002690: 6c6f 6164 5f6d 6f64 656c 733d 2774 7769  load_models='twi
+000026a0: 7474 6572 5f72 6f42 4552 5461 5f76 3127  tter_roBERTa_v1'
+000026b0: 2922 290d 0a0d 0a20 2020 2023 7477 6974  )")....    #twit
+000026c0: 7465 725f 726f 4245 5254 615f 7632 0d0a  ter_roBERTa_v2..
+000026d0: 2020 2020 6465 6620 7477 6974 7465 725f      def twitter_
+000026e0: 726f 4245 5254 615f 7632 2873 656c 662c  roBERTa_v2(self,
+000026f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00002700: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00002710: 7874 3a73 7472 2c20 0d0a 2020 2020 2020  xt:str, ..      
+00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002730: 2020 2020 2074 6578 745f 7479 7065 3a73       text_type:s
+00002740: 7472 2c20 0d0a 2020 2020 2020 2020 2020  tr, ..          
 00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002760: 2020 2020 2020 2020 2020 7375 6d6d 6172            summar
-00002770: 697a 653a 626f 6f6c 3d54 7275 6529 202d  ize:bool=True) -
-00002780: 3e20 666c 6f61 7420 6f72 2064 6963 743a  > float or dict:
-00002790: 0d0a 2020 2020 2020 2020 7472 793a 200d  ..        try: .
-000027a0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-000027b0: 6120 726f 4245 5254 6120 6d6f 6465 6c20  a roBERTa model 
-000027c0: 7472 6169 6e65 6420 6f6e 2031 3234 4d20  trained on 124M 
-000027d0: 7477 6565 7473 2061 6e64 2066 696e 6574  tweets and finet
-000027e0: 756e 6564 2066 6f72 2073 656e 7469 6d65  uned for sentime
-000027f0: 6e74 2061 6e61 6c79 7369 7320 7769 7468  nt analysis with
-00002800: 2074 6865 2054 7765 6574 4576 616c 2062   the TweetEval b
-00002810: 656e 6368 6d61 726b 2222 220d 0a20 2020  enchmark"""..   
-00002820: 2020 2020 2020 2020 2069 6620 7465 7874           if text
-00002830: 5f74 7970 652e 6c6f 7765 7228 2920 3d3d  _type.lower() ==
-00002840: 2027 6e65 7773 273a 200d 0a20 2020 2020   'news': ..     
-00002850: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-00002860: 6e61 6c5f 646f 6320 3d20 7072 6570 726f  nal_doc = prepro
-00002870: 6365 7373 2e6e 6577 7328 7465 7874 290d  cess.news(text).
-00002880: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00002890: 6620 7465 7874 5f74 7970 652e 6c6f 7765  f text_type.lowe
-000028a0: 7228 2920 3d3d 2027 7477 6565 7473 273a  r() == 'tweets':
-000028b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000028c0: 2020 206f 7269 6769 6e61 6c5f 646f 6320     original_doc 
-000028d0: 3d20 7072 6570 726f 6365 7373 2e74 7765  = preprocess.twe
-000028e0: 6574 7328 7465 7874 290d 0a20 2020 2020  ets(text)..     
-000028f0: 2020 2020 2020 206c 6162 656c 7320 3d20         labels = 
-00002900: 5b27 6e65 6761 7469 7665 272c 2027 6e65  ['negative', 'ne
-00002910: 7574 7261 6c27 2c20 2770 6f73 6974 6976  utral', 'positiv
-00002920: 6527 5d0d 0a20 2020 2020 2020 2020 2020  e']..           
-00002930: 206f 7269 6769 6e61 6c5f 746f 6b65 6e73   original_tokens
-00002940: 203d 2073 656c 662e 5477 6974 7465 725f   = self.Twitter_
-00002950: 726f 4245 5254 615f 7632 5f74 6f6b 656e  roBERTa_v2_token
-00002960: 697a 6572 286f 7269 6769 6e61 6c5f 646f  izer(original_do
-00002970: 632c 2072 6574 7572 6e5f 7465 6e73 6f72  c, return_tensor
-00002980: 733d 2770 7427 290d 0a20 2020 2020 2020  s='pt')..       
-00002990: 2020 2020 206c 656e 5f6f 7269 6769 6e61       len_origina
-000029a0: 6c5f 746f 6b65 6e73 203d 206c 656e 286f  l_tokens = len(o
-000029b0: 7269 6769 6e61 6c5f 746f 6b65 6e73 5b27  riginal_tokens['
-000029c0: 696e 7075 745f 6964 7327 5d5b 305d 290d  input_ids'][0]).
-000029d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000029e0: 6c65 6e5f 6f72 6967 696e 616c 5f74 6f6b  len_original_tok
-000029f0: 656e 7320 3c3d 2035 3134 3a0d 0a20 2020  ens <= 514:..   
-00002a00: 2020 2020 2020 2020 2020 2020 2073 636f               sco
-00002a10: 7269 6e67 203d 2073 656c 662e 5477 6974  ring = self.Twit
-00002a20: 7465 725f 726f 4245 5254 615f 7632 282a  ter_roBERTa_v2(*
-00002a30: 2a6f 7269 6769 6e61 6c5f 746f 6b65 6e73  *original_tokens
-00002a40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002a50: 2020 2073 636f 7269 6e67 203d 2073 636f     scoring = sco
-00002a60: 7269 6e67 5b30 5d5b 305d 2e64 6574 6163  ring[0][0].detac
-00002a70: 6828 292e 6e75 6d70 7928 290d 0a20 2020  h().numpy()..   
-00002a80: 2020 2020 2020 2020 2020 2020 2073 636f               sco
-00002a90: 7269 6e67 203d 2073 6f66 746d 6178 2873  ring = softmax(s
-00002aa0: 636f 7269 6e67 290d 0a20 2020 2020 2020  coring)..       
-00002ab0: 2020 2020 2020 2020 2072 616e 6b69 6e67           ranking
-00002ac0: 203d 206e 702e 6172 6773 6f72 7428 7363   = np.argsort(sc
-00002ad0: 6f72 696e 6729 0d0a 2020 2020 2020 2020  oring)..        
-00002ae0: 2020 2020 2020 2020 7365 6e74 5f64 6963          sent_dic
-00002af0: 742c 2063 6f6d 706f 756e 6420 3d20 7b27  t, compound = {'
-00002b00: 6e65 6727 3a20 302c 2027 6e65 7527 3a20  neg': 0, 'neu': 
-00002b10: 302c 2027 706f 7327 3a20 302c 2027 636f  0, 'pos': 0, 'co
-00002b20: 6d70 6f75 6e64 273a 2030 7d2c 2030 200d  mpound': 0}, 0 .
-00002b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b40: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00002b50: 7363 6f72 696e 672e 7368 6170 655b 305d  scoring.shape[0]
-00002b60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00002b70: 2020 2020 2020 2020 6c20 3d20 6c61 6265          l = labe
-00002b80: 6c73 5b72 616e 6b69 6e67 5b69 5d5d 0d0a  ls[ranking[i]]..
-00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ba0: 2020 2020 7320 3d20 7363 6f72 696e 675b      s = scoring[
-00002bb0: 7261 6e6b 696e 675b 695d 5d0d 0a20 2020  ranking[i]]..   
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bd0: 2069 6620 6c20 3d3d 2027 706f 7369 7469   if l == 'positi
-00002be0: 7665 273a 200d 0a20 2020 2020 2020 2020  ve': ..         
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002c00: 6f6d 706f 756e 6420 2b3d 2073 2a31 300d  ompound += s*10.
-00002c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c20: 2020 2020 2020 2020 2073 656e 745f 6469           sent_di
-00002c30: 6374 2e75 7064 6174 6528 7b27 706f 7327  ct.update({'pos'
-00002c40: 3a20 726f 756e 6428 666c 6f61 7428 7329  : round(float(s)
-00002c50: 2c20 3529 7d29 0d0a 2020 2020 2020 2020  , 5)})..        
-00002c60: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00002c70: 206c 203d 3d20 276e 6567 6174 6976 6527   l == 'negative'
-00002c80: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
-00002c90: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
-00002ca0: 6f75 6e64 202d 3d20 732a 3130 0d0a 2020  ound -= s*10..  
-00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 7365 6e74 5f64 6963 742e        sent_dict.
-00002cd0: 7570 6461 7465 287b 276e 6567 273a 2072  update({'neg': r
-00002ce0: 6f75 6e64 2866 6c6f 6174 2873 292c 2035  ound(float(s), 5
-00002cf0: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
-00002d00: 2020 2020 2020 2020 2065 6c73 653a 200d           else: .
-00002d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d20: 2020 2020 2020 2020 2063 6f6d 706f 756e           compoun
-00002d30: 6420 2b3d 2073 2a31 0d0a 2020 2020 2020  d += s*1..      
-00002d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d50: 2020 7365 6e74 5f64 6963 742e 7570 6461    sent_dict.upda
-00002d60: 7465 287b 276e 6575 273a 2072 6f75 6e64  te({'neu': round
-00002d70: 2866 6c6f 6174 2873 292c 2035 297d 290d  (float(s), 5)}).
-00002d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d90: 2073 656e 745f 6469 6374 2e75 7064 6174   sent_dict.updat
-00002da0: 6528 7b27 636f 6d70 6f75 6e64 273a 2073  e({'compound': s
-00002db0: 656c 662e 7265 7363 616c 696e 6728 666c  elf.rescaling(fl
-00002dc0: 6f61 7428 636f 6d70 6f75 6e64 292c 202d  oat(compound), -
-00002dd0: 3130 2c20 3130 297d 290d 0a20 2020 2020  10, 10)})..     
-00002de0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00002df0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002e00: 7375 6d6d 6172 697a 6520 6973 2054 7275  summarize is Tru
-00002e10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002e20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002e30: 656e 745f 6469 6374 5b27 636f 6d70 6f75  ent_dict['compou
-00002e40: 6e64 275d 0d0a 2020 2020 2020 2020 2020  nd']..          
-00002e50: 2020 2020 2020 656c 7365 3a20 0d0a 2020        else: ..  
-00002e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e70: 2020 7265 7475 726e 2073 656e 745f 6469    return sent_di
-00002e80: 6374 200d 0a20 2020 2020 2020 2020 2020  ct ..           
-00002e90: 2065 6c69 6620 6c65 6e5f 6f72 6967 696e   elif len_origin
-00002ea0: 616c 5f74 6f6b 656e 7320 3e20 3531 343a  al_tokens > 514:
-00002eb0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00002ec0: 2020 2023 7365 6c66 2e6c 6f67 6765 722e     #self.logger.
-00002ed0: 7761 726e 696e 6728 22e2 949c e294 80e2  warning(".......
-00002ee0: 9480 2041 6e79 2077 6172 6e69 6e67 7320  .. Any warnings 
-00002ef0: 7265 6c61 7465 6420 746f 2054 6f6b 656e  related to Token
-00002f00: 5365 7175 656e 6365 4c65 6e67 7468 2063  SequenceLength c
-00002f10: 616e 2062 6520 6967 6e6f 7265 6420 6173  an be ignored as
-00002f20: 2069 6e70 7574 2027 7465 7874 2720 6861   input 'text' ha
-00002f30: 7320 6265 656e 2073 706c 6974 6564 2c20  s been splited, 
-00002f40: 7375 6368 2074 6861 7420 7468 6520 7365  such that the se
-00002f50: 7175 656e 6365 206c 656e 6774 6820 6f66  quence length of
-00002f60: 2065 6163 6820 7370 6c69 7420 6973 2061   each split is a
-00002f70: 6c77 6179 7320 6c65 7373 2074 6861 6e20  lways less than 
-00002f80: 7468 6520 7370 6563 6966 6965 6420 6d61  the specified ma
-00002f90: 7869 6d75 6d20 7365 7175 656e 6365 206c  ximum sequence l
-00002fa0: 656e 6774 6822 290d 0a20 2020 2020 2020  ength")..       
-00002fb0: 2020 2020 2020 2020 2074 6f74 616c 5f6e           total_n
-00002fc0: 6567 2c20 746f 7461 6c5f 6e65 752c 2074  eg, total_neu, t
-00002fd0: 6f74 616c 5f70 6f73 2c20 746f 7461 6c5f  otal_pos, total_
-00002fe0: 636f 6d70 6f75 6e64 203d 2030 2c20 302c  compound = 0, 0,
-00002ff0: 2030 2c20 3020 0d0a 2020 2020 2020 2020   0, 0 ..        
-00003000: 2020 2020 2020 2020 6f72 6967 696e 616c          original
-00003010: 5f64 6f63 203d 206e 702e 6172 7261 7928  _doc = np.array(
-00003020: 5b6f 7269 6769 6e61 6c5f 646f 632e 7370  [original_doc.sp
-00003030: 6c69 7428 295d 290d 0a20 2020 2020 2020  lit()])..       
-00003040: 2020 2020 2020 2020 206e 756d 5f73 706c           num_spl
-00003050: 6974 203d 2069 6e74 2872 6f75 6e64 2828  it = int(round((
-00003060: 6c65 6e5f 6f72 6967 696e 616c 5f74 6f6b  len_original_tok
-00003070: 656e 732f 3531 3429 2b31 2c20 3029 290d  ens/514)+1, 0)).
-00003080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003090: 2070 6172 6167 7261 7068 7320 3d20 6e70   paragraphs = np
-000030a0: 2e61 7272 6179 5f73 706c 6974 286f 7269  .array_split(ori
-000030b0: 6769 6e61 6c5f 646f 632c 206e 756d 5f73  ginal_doc, num_s
-000030c0: 706c 6974 2c20 6178 6973 3d31 290d 0a20  plit, axis=1).. 
-000030d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000030e0: 6f72 2069 2069 6e20 7261 6e67 6528 6e75  or i in range(nu
-000030f0: 6d5f 7370 6c69 7429 3a20 0d0a 2020 2020  m_split): ..    
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 7061 7261 6772 6170 6820 3d20 7061 7261  paragraph = para
-00003120: 6772 6170 6873 5b69 5d0d 0a20 2020 2020  graphs[i]..     
-00003130: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003140: 6172 6167 7261 7068 203d 2022 2022 2e6a  aragraph = " ".j
-00003150: 6f69 6e28 7374 7228 776f 7264 292e 7265  oin(str(word).re
-00003160: 706c 6163 6528 2227 222c 2022 2229 2066  place("'", "") f
-00003170: 6f72 2077 6f72 6420 696e 206c 6973 7428  or word in list(
-00003180: 7061 7261 6772 6170 6829 290d 0a20 2020  paragraph))..   
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2070 6172 6167 7261 7068 203d 2070 6172   paragraph = par
-000031b0: 6167 7261 7068 2e72 6570 6c61 6365 2822  agraph.replace("
-000031c0: 5c6e 222c 2022 2229 0d0a 2020 2020 2020  \n", "")..      
-000031d0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-000031e0: 7261 6772 6170 6820 3d20 7061 7261 6772  ragraph = paragr
-000031f0: 6170 682e 7265 706c 6163 6528 225b 222c  aph.replace("[",
-00003200: 2022 2229 2e72 6570 6c61 6365 2822 5d22   "").replace("]"
-00003210: 2c20 2222 290d 0a20 2020 2020 2020 2020  , "")..         
-00003220: 2020 2020 2020 2020 2020 2074 6f6b 656e             token
-00003230: 7320 3d20 7365 6c66 2e54 7769 7474 6572  s = self.Twitter
-00003240: 5f72 6f42 4552 5461 5f76 325f 746f 6b65  _roBERTa_v2_toke
-00003250: 6e69 7a65 7228 7061 7261 6772 6170 682c  nizer(paragraph,
-00003260: 2072 6574 7572 6e5f 7465 6e73 6f72 733d   return_tensors=
-00003270: 2770 7427 290d 0a20 2020 2020 2020 2020  'pt')..         
-00003280: 2020 2020 2020 2020 2020 2073 636f 7269             scori
-00003290: 6e67 203d 2073 656c 662e 5477 6974 7465  ng = self.Twitte
-000032a0: 725f 726f 4245 5254 615f 7632 282a 2a74  r_roBERTa_v2(**t
-000032b0: 6f6b 656e 7329 0d0a 2020 2020 2020 2020  okens)..        
-000032c0: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
-000032d0: 696e 6720 3d20 7363 6f72 696e 675b 305d  ing = scoring[0]
-000032e0: 5b30 5d2e 6465 7461 6368 2829 2e6e 756d  [0].detach().num
-000032f0: 7079 2829 0d0a 2020 2020 2020 2020 2020  py()..          
-00003300: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
-00003310: 6720 3d20 736f 6674 6d61 7828 7363 6f72  g = softmax(scor
-00003320: 696e 6729 0d0a 2020 2020 2020 2020 2020  ing)..          
-00003330: 2020 2020 2020 2020 2020 7261 6e6b 696e            rankin
-00003340: 6720 3d20 6e70 2e61 7267 736f 7274 2873  g = np.argsort(s
-00003350: 636f 7269 6e67 290d 0a20 2020 2020 2020  coring)..       
-00003360: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00003370: 2069 2069 6e20 7261 6e67 6528 7363 6f72   i in range(scor
-00003380: 696e 672e 7368 6170 655b 305d 293a 0d0a  ing.shape[0]):..
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2020 2020 6c20 3d20 6c61 6265          l = labe
-000033b0: 6c73 5b72 616e 6b69 6e67 5b69 5d5d 0d0a  ls[ranking[i]]..
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2020 2020 2020 2020 7320 3d20 7363 6f72          s = scor
-000033e0: 696e 675b 7261 6e6b 696e 675b 695d 5d0d  ing[ranking[i]].
-000033f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003400: 2020 2020 2020 2020 2069 6620 6c20 3d3d           if l ==
-00003410: 2027 706f 7369 7469 7665 273a 200d 0a20   'positive': .. 
+00002760: 2073 756d 6d61 7269 7a65 3a62 6f6f 6c3d   summarize:bool=
+00002770: 5472 7565 2920 2d3e 2066 6c6f 6174 206f  True) -> float o
+00002780: 7220 6469 6374 3a0d 0a20 2020 2020 2020  r dict:..       
+00002790: 2074 7279 3a20 0d0a 2020 2020 2020 2020   try: ..        
+000027a0: 2020 2020 2222 2261 2072 6f42 4552 5461      """a roBERTa
+000027b0: 206d 6f64 656c 2074 7261 696e 6564 206f   model trained o
+000027c0: 6e20 3132 344d 2074 7765 6574 7320 616e  n 124M tweets an
+000027d0: 6420 6669 6e65 7475 6e65 6420 666f 7220  d finetuned for 
+000027e0: 7365 6e74 696d 656e 7420 616e 616c 7973  sentiment analys
+000027f0: 6973 2077 6974 6820 7468 6520 5477 6565  is with the Twee
+00002800: 7445 7661 6c20 6265 6e63 686d 6172 6b22  tEval benchmark"
+00002810: 2222 0d0a 2020 2020 2020 2020 2020 2020  ""..            
+00002820: 6966 2074 6578 745f 7479 7065 2e6c 6f77  if text_type.low
+00002830: 6572 2829 203d 3d20 276e 6577 7327 3a20  er() == 'news': 
+00002840: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002850: 2020 6f72 6967 696e 616c 5f64 6f63 203d    original_doc =
+00002860: 2070 7265 7072 6f63 6573 732e 6e65 7773   preprocess.news
+00002870: 2874 6578 7429 0d0a 2020 2020 2020 2020  (text)..        
+00002880: 2020 2020 656c 6966 2074 6578 745f 7479      elif text_ty
+00002890: 7065 2e6c 6f77 6572 2829 203d 3d20 2774  pe.lower() == 't
+000028a0: 7765 6574 7327 3a20 0d0a 2020 2020 2020  weets': ..      
+000028b0: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
+000028c0: 616c 5f64 6f63 203d 2070 7265 7072 6f63  al_doc = preproc
+000028d0: 6573 732e 7477 6565 7473 2874 6578 7429  ess.tweets(text)
+000028e0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
+000028f0: 6265 6c73 203d 205b 276e 6567 6174 6976  bels = ['negativ
+00002900: 6527 2c20 276e 6575 7472 616c 272c 2027  e', 'neutral', '
+00002910: 706f 7369 7469 7665 275d 0d0a 2020 2020  positive']..    
+00002920: 2020 2020 2020 2020 6f72 6967 696e 616c          original
+00002930: 5f74 6f6b 656e 7320 3d20 7365 6c66 2e54  _tokens = self.T
+00002940: 7769 7474 6572 5f72 6f42 4552 5461 5f76  witter_roBERTa_v
+00002950: 325f 746f 6b65 6e69 7a65 7228 6f72 6967  2_tokenizer(orig
+00002960: 696e 616c 5f64 6f63 2c20 7265 7475 726e  inal_doc, return
+00002970: 5f74 656e 736f 7273 3d27 7074 2729 0d0a  _tensors='pt')..
+00002980: 2020 2020 2020 2020 2020 2020 6c65 6e5f              len_
+00002990: 6f72 6967 696e 616c 5f74 6f6b 656e 7320  original_tokens 
+000029a0: 3d20 6c65 6e28 6f72 6967 696e 616c 5f74  = len(original_t
+000029b0: 6f6b 656e 735b 2769 6e70 7574 5f69 6473  okens['input_ids
+000029c0: 275d 5b30 5d29 0d0a 2020 2020 2020 2020  '][0])..        
+000029d0: 2020 2020 6966 206c 656e 5f6f 7269 6769      if len_origi
+000029e0: 6e61 6c5f 746f 6b65 6e73 203c 3d20 3531  nal_tokens <= 51
+000029f0: 343a 0d0a 2020 2020 2020 2020 2020 2020  4:..            
+00002a00: 2020 2020 7363 6f72 696e 6720 3d20 7365      scoring = se
+00002a10: 6c66 2e54 7769 7474 6572 5f72 6f42 4552  lf.Twitter_roBER
+00002a20: 5461 5f76 3228 2a2a 6f72 6967 696e 616c  Ta_v2(**original
+00002a30: 5f74 6f6b 656e 7329 0d0a 2020 2020 2020  _tokens)..      
+00002a40: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
+00002a50: 6720 3d20 7363 6f72 696e 675b 305d 5b30  g = scoring[0][0
+00002a60: 5d2e 6465 7461 6368 2829 2e6e 756d 7079  ].detach().numpy
+00002a70: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00002a80: 2020 2020 7363 6f72 696e 6720 3d20 736f      scoring = so
+00002a90: 6674 6d61 7828 7363 6f72 696e 6729 0d0a  ftmax(scoring)..
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 7261 6e6b 696e 6720 3d20 6e70 2e61 7267  ranking = np.arg
+00002ac0: 736f 7274 2873 636f 7269 6e67 290d 0a20  sort(scoring).. 
+00002ad0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002ae0: 656e 745f 6469 6374 2c20 636f 6d70 6f75  ent_dict, compou
+00002af0: 6e64 203d 207b 276e 6567 273a 2030 2c20  nd = {'neg': 0, 
+00002b00: 276e 6575 273a 2030 2c20 2770 6f73 273a  'neu': 0, 'pos':
+00002b10: 2030 2c20 2763 6f6d 706f 756e 6427 3a20   0, 'compound': 
+00002b20: 307d 2c20 3020 0d0a 2020 2020 2020 2020  0}, 0 ..        
+00002b30: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00002b40: 2072 616e 6765 2873 636f 7269 6e67 2e73   range(scoring.s
+00002b50: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
+00002b60: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002b70: 203d 206c 6162 656c 735b 7261 6e6b 696e   = labels[rankin
+00002b80: 675b 695d 5d0d 0a20 2020 2020 2020 2020  g[i]]..         
+00002b90: 2020 2020 2020 2020 2020 2073 203d 2073             s = s
+00002ba0: 636f 7269 6e67 5b72 616e 6b69 6e67 5b69  coring[ranking[i
+00002bb0: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
+00002bc0: 2020 2020 2020 2020 6966 206c 203d 3d20          if l == 
+00002bd0: 2770 6f73 6974 6976 6527 3a20 0d0a 2020  'positive': ..  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 636f 6d70 6f75 6e64 202b        compound +
+00002c00: 3d20 732a 3130 0d0a 2020 2020 2020 2020  = s*10..        
+00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c20: 7365 6e74 5f64 6963 742e 7570 6461 7465  sent_dict.update
+00002c30: 287b 2770 6f73 273a 2072 6f75 6e64 2866  ({'pos': round(f
+00002c40: 6c6f 6174 2873 292c 2035 297d 290d 0a20  loat(s), 5)}).. 
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2065 6c69 6620 6c20 3d3d 2027 6e65     elif l == 'ne
+00002c70: 6761 7469 7665 273a 200d 0a20 2020 2020  gative': ..     
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2020 2063 6f6d 706f 756e 6420 2d3d 2073     compound -= s
+00002ca0: 2a31 300d 0a20 2020 2020 2020 2020 2020  *10..           
+00002cb0: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00002cc0: 745f 6469 6374 2e75 7064 6174 6528 7b27  t_dict.update({'
+00002cd0: 6e65 6727 3a20 726f 756e 6428 666c 6f61  neg': round(floa
+00002ce0: 7428 7329 2c20 3529 7d29 0d0a 2020 2020  t(s), 5)})..    
+00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d00: 656c 7365 3a20 0d0a 2020 2020 2020 2020  else: ..        
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d20: 636f 6d70 6f75 6e64 202b 3d20 732a 310d  compound += s*1.
+00002d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d40: 2020 2020 2020 2020 2073 656e 745f 6469           sent_di
+00002d50: 6374 2e75 7064 6174 6528 7b27 6e65 7527  ct.update({'neu'
+00002d60: 3a20 726f 756e 6428 666c 6f61 7428 7329  : round(float(s)
+00002d70: 2c20 3529 7d29 0d0a 2020 2020 2020 2020  , 5)})..        
+00002d80: 2020 2020 2020 2020 7365 6e74 5f64 6963          sent_dic
+00002d90: 742e 7570 6461 7465 287b 2763 6f6d 706f  t.update({'compo
+00002da0: 756e 6427 3a20 7365 6c66 2e72 6573 6361  und': self.resca
+00002db0: 6c69 6e67 2866 6c6f 6174 2863 6f6d 706f  ling(float(compo
+00002dc0: 756e 6429 2c20 2d31 302c 2031 3029 7d29  und), -10, 10)})
+00002dd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002de0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00002df0: 2020 2020 6966 2073 756d 6d61 7269 7a65      if summarize
+00002e00: 2069 7320 5472 7565 3a0d 0a20 2020 2020   is True:..     
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002e20: 6574 7572 6e20 7365 6e74 5f64 6963 745b  eturn sent_dict[
+00002e30: 2763 6f6d 706f 756e 6427 5d0d 0a20 2020  'compound']..   
+00002e40: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00002e50: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
+00002e60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002e70: 7365 6e74 5f64 6963 7420 0d0a 2020 2020  sent_dict ..    
+00002e80: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
+00002e90: 5f6f 7269 6769 6e61 6c5f 746f 6b65 6e73  _original_tokens
+00002ea0: 203e 2035 3134 3a20 0d0a 2020 2020 2020   > 514: ..      
+00002eb0: 2020 2020 2020 2020 2020 2373 656c 662e            #self.
+00002ec0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00002ed0: e294 9ce2 9480 e294 8020 416e 7920 7761  ......... Any wa
+00002ee0: 726e 696e 6773 2072 656c 6174 6564 2074  rnings related t
+00002ef0: 6f20 546f 6b65 6e53 6571 7565 6e63 654c  o TokenSequenceL
+00002f00: 656e 6774 6820 6361 6e20 6265 2069 676e  ength can be ign
+00002f10: 6f72 6564 2061 7320 696e 7075 7420 2774  ored as input 't
+00002f20: 6578 7427 2068 6173 2062 6565 6e20 7370  ext' has been sp
+00002f30: 6c69 7465 642c 2073 7563 6820 7468 6174  lited, such that
+00002f40: 2074 6865 2073 6571 7565 6e63 6520 6c65   the sequence le
+00002f50: 6e67 7468 206f 6620 6561 6368 2073 706c  ngth of each spl
+00002f60: 6974 2069 7320 616c 7761 7973 206c 6573  it is always les
+00002f70: 7320 7468 616e 2074 6865 2073 7065 6369  s than the speci
+00002f80: 6669 6564 206d 6178 696d 756d 2073 6571  fied maximum seq
+00002f90: 7565 6e63 6520 6c65 6e67 7468 2229 0d0a  uence length")..
+00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fb0: 746f 7461 6c5f 6e65 672c 2074 6f74 616c  total_neg, total
+00002fc0: 5f6e 6575 2c20 746f 7461 6c5f 706f 732c  _neu, total_pos,
+00002fd0: 2074 6f74 616c 5f63 6f6d 706f 756e 6420   total_compound 
+00002fe0: 3d20 302c 2030 2c20 302c 2030 200d 0a20  = 0, 0, 0, 0 .. 
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00003000: 7269 6769 6e61 6c5f 646f 6320 3d20 6e70  riginal_doc = np
+00003010: 2e61 7272 6179 285b 6f72 6967 696e 616c  .array([original
+00003020: 5f64 6f63 2e73 706c 6974 2829 5d29 0d0a  _doc.split()])..
+00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003040: 6e75 6d5f 7370 6c69 7420 3d20 696e 7428  num_split = int(
+00003050: 726f 756e 6428 286c 656e 5f6f 7269 6769  round((len_origi
+00003060: 6e61 6c5f 746f 6b65 6e73 2f35 3134 292b  nal_tokens/514)+
+00003070: 312c 2030 2929 0d0a 2020 2020 2020 2020  1, 0))..        
+00003080: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
+00003090: 6873 203d 206e 702e 6172 7261 795f 7370  hs = np.array_sp
+000030a0: 6c69 7428 6f72 6967 696e 616c 5f64 6f63  lit(original_doc
+000030b0: 2c20 6e75 6d5f 7370 6c69 742c 2061 7869  , num_split, axi
+000030c0: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
+000030d0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+000030e0: 616e 6765 286e 756d 5f73 706c 6974 293a  ange(num_split):
+000030f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003100: 2020 2020 2020 2070 6172 6167 7261 7068         paragraph
+00003110: 203d 2070 6172 6167 7261 7068 735b 695d   = paragraphs[i]
+00003120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003130: 2020 2020 2020 7061 7261 6772 6170 6820        paragraph 
+00003140: 3d20 2220 222e 6a6f 696e 2873 7472 2877  = " ".join(str(w
+00003150: 6f72 6429 2e72 6570 6c61 6365 2822 2722  ord).replace("'"
+00003160: 2c20 2222 2920 666f 7220 776f 7264 2069  , "") for word i
+00003170: 6e20 6c69 7374 2870 6172 6167 7261 7068  n list(paragraph
+00003180: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00003190: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
+000031a0: 6820 3d20 7061 7261 6772 6170 682e 7265  h = paragraph.re
+000031b0: 706c 6163 6528 225c 6e22 2c20 2222 290d  place("\n", "").
+000031c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000031d0: 2020 2020 2070 6172 6167 7261 7068 203d       paragraph =
+000031e0: 2070 6172 6167 7261 7068 2e72 6570 6c61   paragraph.repla
+000031f0: 6365 2822 5b22 2c20 2222 292e 7265 706c  ce("[", "").repl
+00003200: 6163 6528 225d 222c 2022 2229 0d0a 2020  ace("]", "")..  
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 2020 746f 6b65 6e73 203d 2073 656c 662e    tokens = self.
+00003230: 5477 6974 7465 725f 726f 4245 5254 615f  Twitter_roBERTa_
+00003240: 7632 5f74 6f6b 656e 697a 6572 2870 6172  v2_tokenizer(par
+00003250: 6167 7261 7068 2c20 7265 7475 726e 5f74  agraph, return_t
+00003260: 656e 736f 7273 3d27 7074 2729 0d0a 2020  ensors='pt')..  
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2020 7363 6f72 696e 6720 3d20 7365 6c66    scoring = self
+00003290: 2e54 7769 7474 6572 5f72 6f42 4552 5461  .Twitter_roBERTa
+000032a0: 5f76 3228 2a2a 746f 6b65 6e73 290d 0a20  _v2(**tokens).. 
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032c0: 2020 2073 636f 7269 6e67 203d 2073 636f     scoring = sco
+000032d0: 7269 6e67 5b30 5d5b 305d 2e64 6574 6163  ring[0][0].detac
+000032e0: 6828 292e 6e75 6d70 7928 290d 0a20 2020  h().numpy()..   
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2073 636f 7269 6e67 203d 2073 6f66 746d   scoring = softm
+00003310: 6178 2873 636f 7269 6e67 290d 0a20 2020  ax(scoring)..   
+00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003330: 2072 616e 6b69 6e67 203d 206e 702e 6172   ranking = np.ar
+00003340: 6773 6f72 7428 7363 6f72 696e 6729 0d0a  gsort(scoring)..
+00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003360: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00003370: 6765 2873 636f 7269 6e67 2e73 6861 7065  ge(scoring.shape
+00003380: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+00003390: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000033a0: 203d 206c 6162 656c 735b 7261 6e6b 696e   = labels[rankin
+000033b0: 675b 695d 5d0d 0a20 2020 2020 2020 2020  g[i]]..         
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000033d0: 203d 2073 636f 7269 6e67 5b72 616e 6b69   = scoring[ranki
+000033e0: 6e67 5b69 5d5d 0d0a 2020 2020 2020 2020  ng[i]]..        
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 6966 206c 203d 3d20 2770 6f73 6974 6976  if l == 'positiv
+00003410: 6527 3a20 0d0a 2020 2020 2020 2020 2020  e': ..          
 00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003430: 2020 2020 2020 2020 2020 2074 6f74 616c             total
-00003440: 5f70 6f73 202b 3d20 7320 0d0a 2020 2020  _pos += s ..    
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
-00003470: 6d70 6f75 6e64 202b 3d20 732a 3130 0d0a  mpound += s*10..
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2020 2020 2020 2020 656c 6966 206c 203d          elif l =
-000034a0: 3d20 276e 6567 6174 6976 6527 3a20 0d0a  = 'negative': ..
+00003430: 2020 746f 7461 6c5f 706f 7320 2b3d 2073    total_pos += s
+00003440: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003450: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003460: 6f74 616c 5f63 6f6d 706f 756e 6420 2b3d  otal_compound +=
+00003470: 2073 2a31 300d 0a20 2020 2020 2020 2020   s*10..         
+00003480: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003490: 6c69 6620 6c20 3d3d 2027 6e65 6761 7469  lif l == 'negati
+000034a0: 7665 273a 200d 0a20 2020 2020 2020 2020  ve': ..         
 000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-000034d0: 6c5f 6e65 6720 2b3d 2073 0d0a 2020 2020  l_neg += s..    
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
-00003500: 6d70 6f75 6e64 202d 3d20 732a 3130 0d0a  mpound -= s*10..
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 656c 7365 3a20 0d0a          else: ..
+000034c0: 2020 2074 6f74 616c 5f6e 6567 202b 3d20     total_neg += 
+000034d0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000034f0: 6f74 616c 5f63 6f6d 706f 756e 6420 2d3d  otal_compound -=
+00003500: 2073 2a31 300d 0a20 2020 2020 2020 2020   s*10..         
+00003510: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003520: 6c73 653a 200d 0a20 2020 2020 2020 2020  lse: ..         
 00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-00003550: 6c5f 6e65 7520 2b3d 2073 0d0a 2020 2020  l_neu += s..    
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
-00003580: 6d70 6f75 6e64 202b 3d20 732a 310d 0a20  mpound += s*1.. 
-00003590: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000035a0: 656e 745f 6469 6374 203d 207b 276e 6567  ent_dict = {'neg
-000035b0: 273a 2072 6f75 6e64 2874 6f74 616c 5f6e  ': round(total_n
-000035c0: 6567 2f6e 756d 5f73 706c 6974 2c20 3529  eg/num_split, 5)
-000035d0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000035e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035f0: 2027 6e65 7527 3a20 726f 756e 6428 746f   'neu': round(to
-00003600: 7461 6c5f 6e65 752f 6e75 6d5f 7370 6c69  tal_neu/num_spli
-00003610: 742c 2035 292c 200d 0a20 2020 2020 2020  t, 5), ..       
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2770 6f73 273a 2072 6f75        'pos': rou
-00003640: 6e64 2874 6f74 616c 5f70 6f73 2f6e 756d  nd(total_pos/num
-00003650: 5f73 706c 6974 2c20 3529 2c20 0d0a 2020  _split, 5), ..  
+00003540: 2020 2074 6f74 616c 5f6e 6575 202b 3d20     total_neu += 
+00003550: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00003560: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00003570: 6f74 616c 5f63 6f6d 706f 756e 6420 2b3d  otal_compound +=
+00003580: 2073 2a31 0d0a 2020 2020 2020 2020 2020   s*1..          
+00003590: 2020 2020 2020 7365 6e74 5f64 6963 7420        sent_dict 
+000035a0: 3d20 7b27 6e65 6727 3a20 726f 756e 6428  = {'neg': round(
+000035b0: 746f 7461 6c5f 6e65 672f 6e75 6d5f 7370  total_neg/num_sp
+000035c0: 6c69 742c 2035 292c 200d 0a20 2020 2020  lit, 5), ..     
+000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035e0: 2020 2020 2020 2020 276e 6575 273a 2072          'neu': r
+000035f0: 6f75 6e64 2874 6f74 616c 5f6e 6575 2f6e  ound(total_neu/n
+00003600: 756d 5f73 706c 6974 2c20 3529 2c20 0d0a  um_split, 5), ..
+00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003620: 2020 2020 2020 2020 2020 2020 2027 706f               'po
+00003630: 7327 3a20 726f 756e 6428 746f 7461 6c5f  s': round(total_
+00003640: 706f 732f 6e75 6d5f 7370 6c69 742c 2035  pos/num_split, 5
+00003650: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
 00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2020 2020 2020 2020 2020 2027 636f 6d70             'comp
-00003680: 6f75 6e64 273a 2073 656c 662e 7265 7363  ound': self.resc
-00003690: 616c 696e 6728 746f 7461 6c5f 636f 6d70  aling(total_comp
-000036a0: 6f75 6e64 2c20 2d31 302a 6e75 6d5f 7370  ound, -10*num_sp
-000036b0: 6c69 742c 2031 302a 6e75 6d5f 7370 6c69  lit, 10*num_spli
-000036c0: 7429 7d0d 0a20 2020 2020 2020 2020 2020  t)}..           
-000036d0: 2020 2020 2069 6620 7375 6d6d 6172 697a       if summariz
-000036e0: 6520 6973 2054 7275 653a 200d 0a20 2020  e is True: ..   
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 2072 6574 7572 6e20 7365 6e74 5f64 6963   return sent_dic
-00003710: 745b 2763 6f6d 706f 756e 6427 5d0d 0a20  t['compound'].. 
-00003720: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003730: 6c73 653a 200d 0a20 2020 2020 2020 2020  lse: ..         
-00003740: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003750: 6e20 7365 6e74 5f64 6963 7420 0d0a 2020  n sent_dict ..  
-00003760: 2020 2020 2020 6578 6365 7074 2041 7474        except Att
-00003770: 7269 6275 7465 4572 726f 723a 200d 0a20  ributeError: .. 
-00003780: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003790: 2053 7973 7465 6d45 7272 6f72 2822 7477   SystemError("tw
-000037a0: 6974 7465 725f 726f 4245 5254 615f 7632  itter_roBERTa_v2
-000037b0: 206d 7573 7420 6265 206c 6f61 6465 6420   must be loaded 
-000037c0: 696e 2070 7269 6f72 2e20 4c6f 6164 2074  in prior. Load t
-000037d0: 6865 206d 6f64 656c 2076 6961 206e 6c70  he model via nlp
-000037e0: 2e73 656e 7469 6d65 6e74 286c 6f61 645f  .sentiment(load_
-000037f0: 6d6f 6465 6c73 3d27 7477 6974 7465 725f  models='twitter_
-00003800: 726f 4245 5254 615f 7632 2729 2229 0d0a  roBERTa_v2')")..
-00003810: 0d0a 2020 2020 2374 7769 7474 6572 5f58  ..    #twitter_X
-00003820: 4c4d 5f72 6f42 4552 5461 0d0a 2020 2020  LM_roBERTa..    
-00003830: 6465 6620 7477 6974 7465 725f 584c 4d5f  def twitter_XLM_
-00003840: 726f 4245 5254 6128 7365 6c66 2c20 0d0a  roBERTa(self, ..
+00003670: 2020 2763 6f6d 706f 756e 6427 3a20 7365    'compound': se
+00003680: 6c66 2e72 6573 6361 6c69 6e67 2874 6f74  lf.rescaling(tot
+00003690: 616c 5f63 6f6d 706f 756e 642c 202d 3130  al_compound, -10
+000036a0: 2a6e 756d 5f73 706c 6974 2c20 3130 2a6e  *num_split, 10*n
+000036b0: 756d 5f73 706c 6974 297d 0d0a 2020 2020  um_split)}..    
+000036c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000036d0: 756d 6d61 7269 7a65 2069 7320 5472 7565  ummarize is True
+000036e0: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+000036f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003700: 656e 745f 6469 6374 5b27 636f 6d70 6f75  ent_dict['compou
+00003710: 6e64 275d 0d0a 2020 2020 2020 2020 2020  nd']..          
+00003720: 2020 2020 2020 656c 7365 3a20 0d0a 2020        else: ..  
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 2020 7265 7475 726e 2073 656e 745f 6469    return sent_di
+00003750: 6374 200d 0a20 2020 2020 2020 2065 7863  ct ..        exc
+00003760: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
+00003770: 6f72 3a20 0d0a 2020 2020 2020 2020 2020  or: ..          
+00003780: 2020 7261 6973 6520 5379 7374 656d 4572    raise SystemEr
+00003790: 726f 7228 2274 7769 7474 6572 5f72 6f42  ror("twitter_roB
+000037a0: 4552 5461 5f76 3220 6d75 7374 2062 6520  ERTa_v2 must be 
+000037b0: 6c6f 6164 6564 2069 6e20 7072 696f 722e  loaded in prior.
+000037c0: 204c 6f61 6420 7468 6520 6d6f 6465 6c20   Load the model 
+000037d0: 7669 6120 6e6c 702e 7365 6e74 696d 656e  via nlp.sentimen
+000037e0: 7428 6c6f 6164 5f6d 6f64 656c 733d 2774  t(load_models='t
+000037f0: 7769 7474 6572 5f72 6f42 4552 5461 5f76  witter_roBERTa_v
+00003800: 3227 2922 290d 0a0d 0a20 2020 2023 7477  2')")....    #tw
+00003810: 6974 7465 725f 584c 4d5f 726f 4245 5254  itter_XLM_roBERT
+00003820: 610d 0a20 2020 2064 6566 2074 7769 7474  a..    def twitt
+00003830: 6572 5f58 4c4d 5f72 6f42 4552 5461 2873  er_XLM_roBERTa(s
+00003840: 656c 662c 200d 0a20 2020 2020 2020 2020  elf, ..         
 00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00003870: 3a73 7472 2c20 0d0a 2020 2020 2020 2020  :str, ..        
-00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003890: 2020 2020 7465 7874 5f74 7970 653a 7374      text_type:st
-000038a0: 722c 200d 0a20 2020 2020 2020 2020 2020  r, ..           
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2073 756d 6d61 7269 7a65 3a62 6f6f 6c3d   summarize:bool=
-000038d0: 5472 7565 2920 2d3e 2066 6c6f 6174 206f  True) -> float o
-000038e0: 7220 6469 6374 3a0d 0a20 2020 2020 2020  r dict:..       
-000038f0: 2074 7279 3a20 0d0a 2020 2020 2020 2020   try: ..        
-00003900: 2020 2020 2222 2261 2058 4c4d 2d72 6f42      """a XLM-roB
-00003910: 4552 5461 206d 6f64 656c 2074 7261 696e  ERTa model train
-00003920: 6564 206f 6e20 3139 384d 2074 7765 6574  ed on 198M tweet
-00003930: 7320 616e 6420 6669 6e65 7475 6e65 6420  s and finetuned 
-00003940: 666f 7220 7365 6e74 696d 656e 7420 616e  for sentiment an
-00003950: 616c 7973 6973 2077 6974 6822 2222 0d0a  alysis with"""..
-00003960: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-00003970: 6578 745f 7479 7065 2e6c 6f77 6572 2829  ext_type.lower()
-00003980: 203d 3d20 276e 6577 7327 3a20 0d0a 2020   == 'news': ..  
-00003990: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-000039a0: 6967 696e 616c 5f64 6f63 203d 2070 7265  iginal_doc = pre
-000039b0: 7072 6f63 6573 732e 6e65 7773 2874 6578  process.news(tex
-000039c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000039d0: 656c 6966 2074 6578 745f 7479 7065 2e6c  elif text_type.l
-000039e0: 6f77 6572 2829 203d 3d20 2774 7765 6574  ower() == 'tweet
-000039f0: 7327 3a20 0d0a 2020 2020 2020 2020 2020  s': ..          
-00003a00: 2020 2020 2020 6f72 6967 696e 616c 5f64        original_d
-00003a10: 6f63 203d 2070 7265 7072 6f63 6573 732e  oc = preprocess.
-00003a20: 7477 6565 7473 2874 6578 7429 0d0a 2020  tweets(text)..  
-00003a30: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
-00003a40: 203d 205b 276e 6567 6174 6976 6527 2c20   = ['negative', 
-00003a50: 276e 6575 7472 616c 272c 2027 706f 7369  'neutral', 'posi
-00003a60: 7469 7665 275d 0d0a 2020 2020 2020 2020  tive']..        
-00003a70: 2020 2020 6f72 6967 696e 616c 5f74 6f6b      original_tok
-00003a80: 656e 7320 3d20 7365 6c66 2e54 7769 7474  ens = self.Twitt
-00003a90: 6572 5f58 4c4d 5f72 6f42 4552 5461 5f74  er_XLM_roBERTa_t
-00003aa0: 6f6b 656e 697a 6572 286f 7269 6769 6e61  okenizer(origina
-00003ab0: 6c5f 646f 632c 2072 6574 7572 6e5f 7465  l_doc, return_te
-00003ac0: 6e73 6f72 733d 2770 7427 290d 0a20 2020  nsors='pt')..   
-00003ad0: 2020 2020 2020 2020 206c 656e 5f6f 7269           len_ori
-00003ae0: 6769 6e61 6c5f 746f 6b65 6e73 203d 206c  ginal_tokens = l
-00003af0: 656e 286f 7269 6769 6e61 6c5f 746f 6b65  en(original_toke
-00003b00: 6e73 5b27 696e 7075 745f 6964 7327 5d5b  ns['input_ids'][
-00003b10: 305d 290d 0a20 2020 2020 2020 2020 2020  0])..           
-00003b20: 2069 6620 6c65 6e5f 6f72 6967 696e 616c   if len_original
-00003b30: 5f74 6f6b 656e 7320 3c3d 2035 3134 3a20  _tokens <= 514: 
-00003b40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003b50: 2020 7363 6f72 696e 6720 3d20 7365 6c66    scoring = self
-00003b60: 2e54 7769 7474 6572 5f58 4c4d 5f72 6f42  .Twitter_XLM_roB
-00003b70: 4552 5461 282a 2a6f 7269 6769 6e61 6c5f  ERTa(**original_
-00003b80: 746f 6b65 6e73 290d 0a20 2020 2020 2020  tokens)..       
-00003b90: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
-00003ba0: 203d 2073 636f 7269 6e67 5b30 5d5b 305d   = scoring[0][0]
-00003bb0: 2e64 6574 6163 6828 292e 6e75 6d70 7928  .detach().numpy(
-00003bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00003bd0: 2020 2073 636f 7269 6e67 203d 2073 6f66     scoring = sof
-00003be0: 746d 6178 2873 636f 7269 6e67 290d 0a20  tmax(scoring).. 
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003c00: 616e 6b69 6e67 203d 206e 702e 6172 6773  anking = np.args
-00003c10: 6f72 7428 7363 6f72 696e 6729 0d0a 2020  ort(scoring)..  
-00003c20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003c30: 6e74 5f64 6963 742c 2063 6f6d 706f 756e  nt_dict, compoun
-00003c40: 6420 3d20 7b27 6e65 6727 3a20 302c 2027  d = {'neg': 0, '
-00003c50: 6e65 7527 3a20 302c 2027 706f 7327 3a20  neu': 0, 'pos': 
-00003c60: 302c 2027 636f 6d70 6f75 6e64 273a 2030  0, 'compound': 0
-00003c70: 7d2c 2030 200d 0a20 2020 2020 2020 2020  }, 0 ..         
-00003c80: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00003c90: 7261 6e67 6528 7363 6f72 696e 672e 7368  range(scoring.sh
-00003ca0: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
-00003cb0: 2020 2020 2020 2020 2020 2020 2020 6c20                l 
-00003cc0: 3d20 6c61 6265 6c73 5b72 616e 6b69 6e67  = labels[ranking
-00003cd0: 5b69 5d5d 0d0a 2020 2020 2020 2020 2020  [i]]..          
-00003ce0: 2020 2020 2020 2020 2020 7320 3d20 7363            s = sc
-00003cf0: 6f72 696e 675b 7261 6e6b 696e 675b 695d  oring[ranking[i]
-00003d00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00003d10: 2020 2020 2020 2069 6620 6c20 3d3d 2027         if l == '
-00003d20: 706f 7369 7469 7665 273a 200d 0a20 2020  positive': ..   
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2063 6f6d 706f 756e 6420 2b3d       compound +=
-00003d50: 2073 2a31 300d 0a20 2020 2020 2020 2020   s*10..         
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003d70: 656e 745f 6469 6374 2e75 7064 6174 6528  ent_dict.update(
-00003d80: 7b27 706f 7327 3a20 726f 756e 6428 666c  {'pos': round(fl
-00003d90: 6f61 7428 7329 2c20 3529 7d29 0d0a 2020  oat(s), 5)})..  
-00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 656c 6966 206c 203d 3d20 276e 6567    elif l == 'neg
-00003dc0: 6174 6976 6527 3a20 0d0a 2020 2020 2020  ative': ..      
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 636f 6d70 6f75 6e64 202d 3d20 732a    compound -= s*
-00003df0: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
-00003e00: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
-00003e10: 5f64 6963 742e 7570 6461 7465 287b 276e  _dict.update({'n
-00003e20: 6567 273a 2072 6f75 6e64 2866 6c6f 6174  eg': round(float
-00003e30: 2873 292c 2035 297d 290d 0a20 2020 2020  (s), 5)})..     
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00003e50: 6c73 653a 200d 0a20 2020 2020 2020 2020  lse: ..         
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003e70: 6f6d 706f 756e 6420 2b3d 2073 2a31 0d0a  ompound += s*1..
-00003e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e90: 2020 2020 2020 2020 7365 6e74 5f64 6963          sent_dic
-00003ea0: 742e 7570 6461 7465 287b 276e 6575 273a  t.update({'neu':
-00003eb0: 2072 6f75 6e64 2866 6c6f 6174 2873 292c   round(float(s),
-00003ec0: 2035 297d 290d 0a20 2020 2020 2020 2020   5)})..         
-00003ed0: 2020 2020 2020 2073 656e 745f 6469 6374         sent_dict
-00003ee0: 2e75 7064 6174 6528 7b27 636f 6d70 6f75  .update({'compou
-00003ef0: 6e64 273a 2073 656c 662e 7265 7363 616c  nd': self.rescal
-00003f00: 696e 6728 666c 6f61 7428 636f 6d70 6f75  ing(float(compou
-00003f10: 6e64 292c 202d 3130 2c20 3130 297d 290d  nd), -10, 10)}).
-00003f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003f30: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00003f40: 2020 2069 6620 7375 6d6d 6172 697a 6520     if summarize 
-00003f50: 6973 2054 7275 653a 200d 0a20 2020 2020  is True: ..     
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003f70: 6574 7572 6e20 7365 6e74 5f64 6963 745b  eturn sent_dict[
-00003f80: 2763 6f6d 706f 756e 6427 5d0d 0a20 2020  'compound']..   
-00003f90: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00003fa0: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
-00003fb0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003fc0: 7365 6e74 5f64 6963 7420 0d0a 2020 2020  sent_dict ..    
-00003fd0: 2020 2020 2020 2020 656c 6966 206c 656e          elif len
-00003fe0: 5f6f 7269 6769 6e61 6c5f 746f 6b65 6e73  _original_tokens
-00003ff0: 203e 2035 3134 3a20 0d0a 2020 2020 2020   > 514: ..      
-00004000: 2020 2020 2020 2020 2020 2373 656c 662e            #self.
-00004010: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-00004020: e294 9ce2 9480 e294 8020 416e 7920 7761  ......... Any wa
-00004030: 726e 696e 6773 2072 656c 6174 6564 2074  rnings related t
-00004040: 6f20 546f 6b65 6e53 6571 7565 6e63 654c  o TokenSequenceL
-00004050: 656e 6774 6820 6361 6e20 6265 2069 676e  ength can be ign
-00004060: 6f72 6564 2061 7320 696e 7075 7420 2774  ored as input 't
-00004070: 6578 7427 2068 6173 2062 6565 6e20 7370  ext' has been sp
-00004080: 6c69 7465 642c 2073 7563 6820 7468 6174  lited, such that
-00004090: 2074 6865 2073 6571 7565 6e63 6520 6c65   the sequence le
-000040a0: 6e67 7468 206f 6620 6561 6368 2073 706c  ngth of each spl
-000040b0: 6974 2069 7320 616c 7761 7973 206c 6573  it is always les
-000040c0: 7320 7468 616e 2074 6865 2073 7065 6369  s than the speci
-000040d0: 6669 6564 206d 6178 696d 756d 2073 6571  fied maximum seq
-000040e0: 7565 6e63 6520 6c65 6e67 7468 2229 0d0a  uence length")..
-000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 746f 7461 6c5f 6e65 672c 2074 6f74 616c  total_neg, total
-00004110: 5f6e 6575 2c20 746f 7461 6c5f 706f 732c  _neu, total_pos,
-00004120: 2074 6f74 616c 5f63 6f6d 706f 756e 6420   total_compound 
-00004130: 3d20 302c 2030 2c20 302c 2030 200d 0a20  = 0, 0, 0, 0 .. 
-00004140: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00004150: 7269 6769 6e61 6c5f 646f 6320 3d20 6e70  riginal_doc = np
-00004160: 2e61 7272 6179 285b 6f72 6967 696e 616c  .array([original
-00004170: 5f64 6f63 2e73 706c 6974 2829 5d29 0d0a  _doc.split()])..
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 6e75 6d5f 7370 6c69 7420 3d20 696e 7428  num_split = int(
-000041a0: 726f 756e 6428 286c 656e 5f6f 7269 6769  round((len_origi
-000041b0: 6e61 6c5f 746f 6b65 6e73 2f35 3134 292b  nal_tokens/514)+
-000041c0: 312c 2030 2929 0d0a 2020 2020 2020 2020  1, 0))..        
-000041d0: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
-000041e0: 6873 203d 206e 702e 6172 7261 795f 7370  hs = np.array_sp
-000041f0: 6c69 7428 6f72 6967 696e 616c 5f64 6f63  lit(original_doc
-00004200: 2c20 6e75 6d5f 7370 6c69 742c 2061 7869  , num_split, axi
-00004210: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
-00004220: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00004230: 616e 6765 286e 756d 5f73 706c 6974 293a  ange(num_split):
-00004240: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004250: 2020 2020 2020 2070 6172 6167 7261 7068         paragraph
-00004260: 203d 2070 6172 6167 7261 7068 735b 695d   = paragraphs[i]
-00004270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004280: 2020 2020 2020 7061 7261 6772 6170 6820        paragraph 
-00004290: 3d20 2220 222e 6a6f 696e 2873 7472 2877  = " ".join(str(w
-000042a0: 6f72 6429 2e72 6570 6c61 6365 2822 2722  ord).replace("'"
-000042b0: 2c20 2222 2920 666f 7220 776f 7264 2069  , "") for word i
-000042c0: 6e20 6c69 7374 2870 6172 6167 7261 7068  n list(paragraph
-000042d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000042e0: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
-000042f0: 6820 3d20 7061 7261 6772 6170 682e 7265  h = paragraph.re
-00004300: 706c 6163 6528 225c 6e22 2c20 2222 290d  place("\n", "").
-00004310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004320: 2020 2020 2070 6172 6167 7261 7068 203d       paragraph =
-00004330: 2070 6172 6167 7261 7068 2e72 6570 6c61   paragraph.repla
-00004340: 6365 2822 5b22 2c20 2222 292e 7265 706c  ce("[", "").repl
-00004350: 6163 6528 225d 222c 2022 2229 0d0a 2020  ace("]", "")..  
-00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 2020 746f 6b65 6e73 203d 2073 656c 662e    tokens = self.
-00004380: 5477 6974 7465 725f 584c 4d5f 726f 4245  Twitter_XLM_roBE
-00004390: 5254 615f 746f 6b65 6e69 7a65 7228 7061  RTa_tokenizer(pa
-000043a0: 7261 6772 6170 682c 2072 6574 7572 6e5f  ragraph, return_
-000043b0: 7465 6e73 6f72 733d 2770 7427 290d 0a20  tensors='pt').. 
-000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043d0: 2020 2073 636f 7269 6e67 203d 2073 656c     scoring = sel
-000043e0: 662e 5477 6974 7465 725f 584c 4d5f 726f  f.Twitter_XLM_ro
-000043f0: 4245 5254 6128 2a2a 746f 6b65 6e73 290d  BERTa(**tokens).
-00004400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004410: 2020 2020 2073 636f 7269 6e67 203d 2073       scoring = s
-00004420: 636f 7269 6e67 5b30 5d5b 305d 2e64 6574  coring[0][0].det
-00004430: 6163 6828 292e 6e75 6d70 7928 290d 0a20  ach().numpy().. 
-00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004450: 2020 2073 636f 7269 6e67 203d 2073 6f66     scoring = sof
-00004460: 746d 6178 2873 636f 7269 6e67 290d 0a20  tmax(scoring).. 
-00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004480: 2020 2072 616e 6b69 6e67 203d 206e 702e     ranking = np.
-00004490: 6172 6773 6f72 7428 7363 6f72 696e 6729  argsort(scoring)
-000044a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000044b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-000044c0: 616e 6765 2873 636f 7269 6e67 2e73 6861  ange(scoring.sha
-000044d0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 206c 203d 206c 6162 656c 735b 7261 6e6b   l = labels[rank
-00004500: 696e 675b 695d 5d0d 0a20 2020 2020 2020  ing[i]]..       
-00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 2073 203d 2073 636f 7269 6e67 5b72 616e   s = scoring[ran
-00004530: 6b69 6e67 5b69 5d5d 0d0a 2020 2020 2020  king[i]]..      
-00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004550: 2020 6966 206c 203d 3d20 2770 6f73 6974    if l == 'posit
-00004560: 6976 6527 3a20 0d0a 2020 2020 2020 2020  ive': ..        
-00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004580: 2020 2020 746f 7461 6c5f 706f 7320 2b3d      total_pos +=
-00004590: 2073 200d 0a20 2020 2020 2020 2020 2020   s ..           
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2074 6f74 616c 5f63 6f6d 706f 756e 6420   total_compound 
-000045c0: 2b3d 2073 2a31 300d 0a20 2020 2020 2020  += s*10..       
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2065 6c69 6620 6c20 3d3d 2027 6e65 6761   elif l == 'nega
-000045f0: 7469 7665 273a 200d 0a20 2020 2020 2020  tive': ..       
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 2074 6f74 616c 5f6e 6567 202b       total_neg +
-00004620: 3d20 730d 0a20 2020 2020 2020 2020 2020  = s..           
-00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004640: 2074 6f74 616c 5f63 6f6d 706f 756e 6420   total_compound 
-00004650: 2d3d 2073 2a31 300d 0a20 2020 2020 2020  -= s*10..       
-00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2065 6c73 653a 200d 0a20 2020 2020 2020   else: ..       
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2074 6f74 616c 5f6e 6575 202b       total_neu +
-000046a0: 3d20 730d 0a20 2020 2020 2020 2020 2020  = s..           
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2074 6f74 616c 5f63 6f6d 706f 756e 6420   total_compound 
-000046d0: 2b3d 2073 2a31 0d0a 2020 2020 2020 2020  += s*1..        
-000046e0: 2020 2020 2020 2020 7365 6e74 5f64 6963          sent_dic
-000046f0: 7420 3d20 7b27 6e65 6727 3a20 726f 756e  t = {'neg': roun
-00004700: 6428 746f 7461 6c5f 6e65 672f 6e75 6d5f  d(total_neg/num_
-00004710: 7370 6c69 742c 2035 292c 200d 0a20 2020  split, 5), ..   
+00003860: 2020 2074 6578 743a 7374 722c 200d 0a20     text:str, .. 
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2020 2020 2074 6578 745f             text_
+00003890: 7479 7065 3a73 7472 2c20 0d0a 2020 2020  type:str, ..    
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038b0: 2020 2020 2020 2020 7375 6d6d 6172 697a          summariz
+000038c0: 653a 626f 6f6c 3d54 7275 6529 202d 3e20  e:bool=True) -> 
+000038d0: 666c 6f61 7420 6f72 2064 6963 743a 0d0a  float or dict:..
+000038e0: 2020 2020 2020 2020 7472 793a 200d 0a20          try: .. 
+000038f0: 2020 2020 2020 2020 2020 2022 2222 6120             """a 
+00003900: 584c 4d2d 726f 4245 5254 6120 6d6f 6465  XLM-roBERTa mode
+00003910: 6c20 7472 6169 6e65 6420 6f6e 2031 3938  l trained on 198
+00003920: 4d20 7477 6565 7473 2061 6e64 2066 696e  M tweets and fin
+00003930: 6574 756e 6564 2066 6f72 2073 656e 7469  etuned for senti
+00003940: 6d65 6e74 2061 6e61 6c79 7369 7320 7769  ment analysis wi
+00003950: 7468 2222 220d 0a20 2020 2020 2020 2020  th"""..         
+00003960: 2020 2069 6620 7465 7874 5f74 7970 652e     if text_type.
+00003970: 6c6f 7765 7228 2920 3d3d 2027 6e65 7773  lower() == 'news
+00003980: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
+00003990: 2020 2020 206f 7269 6769 6e61 6c5f 646f       original_do
+000039a0: 6320 3d20 7072 6570 726f 6365 7373 2e6e  c = preprocess.n
+000039b0: 6577 7328 7465 7874 290d 0a20 2020 2020  ews(text)..     
+000039c0: 2020 2020 2020 2065 6c69 6620 7465 7874         elif text
+000039d0: 5f74 7970 652e 6c6f 7765 7228 2920 3d3d  _type.lower() ==
+000039e0: 2027 7477 6565 7473 273a 200d 0a20 2020   'tweets': ..   
+000039f0: 2020 2020 2020 2020 2020 2020 206f 7269               ori
+00003a00: 6769 6e61 6c5f 646f 6320 3d20 7072 6570  ginal_doc = prep
+00003a10: 726f 6365 7373 2e74 7765 6574 7328 7465  rocess.tweets(te
+00003a20: 7874 290d 0a20 2020 2020 2020 2020 2020  xt)..           
+00003a30: 206c 6162 656c 7320 3d20 5b27 6e65 6761   labels = ['nega
+00003a40: 7469 7665 272c 2027 6e65 7574 7261 6c27  tive', 'neutral'
+00003a50: 2c20 2770 6f73 6974 6976 6527 5d0d 0a20  , 'positive'].. 
+00003a60: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+00003a70: 6e61 6c5f 746f 6b65 6e73 203d 2073 656c  nal_tokens = sel
+00003a80: 662e 5477 6974 7465 725f 584c 4d5f 726f  f.Twitter_XLM_ro
+00003a90: 4245 5254 615f 746f 6b65 6e69 7a65 7228  BERTa_tokenizer(
+00003aa0: 6f72 6967 696e 616c 5f64 6f63 2c20 7265  original_doc, re
+00003ab0: 7475 726e 5f74 656e 736f 7273 3d27 7074  turn_tensors='pt
+00003ac0: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00003ad0: 6c65 6e5f 6f72 6967 696e 616c 5f74 6f6b  len_original_tok
+00003ae0: 656e 7320 3d20 6c65 6e28 6f72 6967 696e  ens = len(origin
+00003af0: 616c 5f74 6f6b 656e 735b 2769 6e70 7574  al_tokens['input
+00003b00: 5f69 6473 275d 5b30 5d29 0d0a 2020 2020  _ids'][0])..    
+00003b10: 2020 2020 2020 2020 6966 206c 656e 5f6f          if len_o
+00003b20: 7269 6769 6e61 6c5f 746f 6b65 6e73 203c  riginal_tokens <
+00003b30: 3d20 3531 343a 200d 0a20 2020 2020 2020  = 514: ..       
+00003b40: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
+00003b50: 203d 2073 656c 662e 5477 6974 7465 725f   = self.Twitter_
+00003b60: 584c 4d5f 726f 4245 5254 6128 2a2a 6f72  XLM_roBERTa(**or
+00003b70: 6967 696e 616c 5f74 6f6b 656e 7329 0d0a  iginal_tokens)..
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 7363 6f72 696e 6720 3d20 7363 6f72 696e  scoring = scorin
+00003ba0: 675b 305d 5b30 5d2e 6465 7461 6368 2829  g[0][0].detach()
+00003bb0: 2e6e 756d 7079 2829 0d0a 2020 2020 2020  .numpy()..      
+00003bc0: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
+00003bd0: 6720 3d20 736f 6674 6d61 7828 7363 6f72  g = softmax(scor
+00003be0: 696e 6729 0d0a 2020 2020 2020 2020 2020  ing)..          
+00003bf0: 2020 2020 2020 7261 6e6b 696e 6720 3d20        ranking = 
+00003c00: 6e70 2e61 7267 736f 7274 2873 636f 7269  np.argsort(scori
+00003c10: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
+00003c20: 2020 2020 2073 656e 745f 6469 6374 2c20       sent_dict, 
+00003c30: 636f 6d70 6f75 6e64 203d 207b 276e 6567  compound = {'neg
+00003c40: 273a 2030 2c20 276e 6575 273a 2030 2c20  ': 0, 'neu': 0, 
+00003c50: 2770 6f73 273a 2030 2c20 2763 6f6d 706f  'pos': 0, 'compo
+00003c60: 756e 6427 3a20 307d 2c20 3020 0d0a 2020  und': 0}, 0 ..  
+00003c70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00003c80: 7220 6920 696e 2072 616e 6765 2873 636f  r i in range(sco
+00003c90: 7269 6e67 2e73 6861 7065 5b30 5d29 3a0d  ring.shape[0]):.
+00003ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cb0: 2020 2020 206c 203d 206c 6162 656c 735b       l = labels[
+00003cc0: 7261 6e6b 696e 675b 695d 5d0d 0a20 2020  ranking[i]]..   
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ce0: 2073 203d 2073 636f 7269 6e67 5b72 616e   s = scoring[ran
+00003cf0: 6b69 6e67 5b69 5d5d 0d0a 2020 2020 2020  king[i]]..      
+00003d00: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00003d10: 206c 203d 3d20 2770 6f73 6974 6976 6527   l == 'positive'
+00003d20: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+00003d30: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00003d40: 6f75 6e64 202b 3d20 732a 3130 0d0a 2020  ound += s*10..  
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 2020 2020 2020 7365 6e74 5f64 6963 742e        sent_dict.
+00003d70: 7570 6461 7465 287b 2770 6f73 273a 2072  update({'pos': r
+00003d80: 6f75 6e64 2866 6c6f 6174 2873 292c 2035  ound(float(s), 5
+00003d90: 297d 290d 0a20 2020 2020 2020 2020 2020  )})..           
+00003da0: 2020 2020 2020 2020 2065 6c69 6620 6c20           elif l 
+00003db0: 3d3d 2027 6e65 6761 7469 7665 273a 200d  == 'negative': .
+00003dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003dd0: 2020 2020 2020 2020 2063 6f6d 706f 756e           compoun
+00003de0: 6420 2d3d 2073 2a31 300d 0a20 2020 2020  d -= s*10..     
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2020 2073 656e 745f 6469 6374 2e75 7064     sent_dict.upd
+00003e10: 6174 6528 7b27 6e65 6727 3a20 726f 756e  ate({'neg': roun
+00003e20: 6428 666c 6f61 7428 7329 2c20 3529 7d29  d(float(s), 5)})
+00003e30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003e40: 2020 2020 2020 656c 7365 3a20 0d0a 2020        else: ..  
+00003e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e60: 2020 2020 2020 636f 6d70 6f75 6e64 202b        compound +
+00003e70: 3d20 732a 310d 0a20 2020 2020 2020 2020  = s*1..         
+00003e80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003e90: 656e 745f 6469 6374 2e75 7064 6174 6528  ent_dict.update(
+00003ea0: 7b27 6e65 7527 3a20 726f 756e 6428 666c  {'neu': round(fl
+00003eb0: 6f61 7428 7329 2c20 3529 7d29 0d0a 2020  oat(s), 5)})..  
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003ed0: 6e74 5f64 6963 742e 7570 6461 7465 287b  nt_dict.update({
+00003ee0: 2763 6f6d 706f 756e 6427 3a20 7365 6c66  'compound': self
+00003ef0: 2e72 6573 6361 6c69 6e67 2866 6c6f 6174  .rescaling(float
+00003f00: 2863 6f6d 706f 756e 6429 2c20 2d31 302c  (compound), -10,
+00003f10: 2031 3029 7d29 0d0a 2020 2020 2020 2020   10)})..        
+00003f20: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003f30: 2020 2020 2020 2020 2020 6966 2073 756d            if sum
+00003f40: 6d61 7269 7a65 2069 7320 5472 7565 3a20  marize is True: 
+00003f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003f60: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
+00003f70: 745f 6469 6374 5b27 636f 6d70 6f75 6e64  t_dict['compound
+00003f80: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
+00003f90: 2020 2020 656c 7365 3a20 0d0a 2020 2020      else: ..    
+00003fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fb0: 7265 7475 726e 2073 656e 745f 6469 6374  return sent_dict
+00003fc0: 200d 0a20 2020 2020 2020 2020 2020 2065   ..            e
+00003fd0: 6c69 6620 6c65 6e5f 6f72 6967 696e 616c  lif len_original
+00003fe0: 5f74 6f6b 656e 7320 3e20 3531 343a 200d  _tokens > 514: .
+00003ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004000: 2023 7365 6c66 2e6c 6f67 6765 722e 7761   #self.logger.wa
+00004010: 726e 696e 6728 22e2 949c e294 80e2 9480  rning(".........
+00004020: 2041 6e79 2077 6172 6e69 6e67 7320 7265   Any warnings re
+00004030: 6c61 7465 6420 746f 2054 6f6b 656e 5365  lated to TokenSe
+00004040: 7175 656e 6365 4c65 6e67 7468 2063 616e  quenceLength can
+00004050: 2062 6520 6967 6e6f 7265 6420 6173 2069   be ignored as i
+00004060: 6e70 7574 2027 7465 7874 2720 6861 7320  nput 'text' has 
+00004070: 6265 656e 2073 706c 6974 6564 2c20 7375  been splited, su
+00004080: 6368 2074 6861 7420 7468 6520 7365 7175  ch that the sequ
+00004090: 656e 6365 206c 656e 6774 6820 6f66 2065  ence length of e
+000040a0: 6163 6820 7370 6c69 7420 6973 2061 6c77  ach split is alw
+000040b0: 6179 7320 6c65 7373 2074 6861 6e20 7468  ays less than th
+000040c0: 6520 7370 6563 6966 6965 6420 6d61 7869  e specified maxi
+000040d0: 6d75 6d20 7365 7175 656e 6365 206c 656e  mum sequence len
+000040e0: 6774 6822 290d 0a20 2020 2020 2020 2020  gth")..         
+000040f0: 2020 2020 2020 2074 6f74 616c 5f6e 6567         total_neg
+00004100: 2c20 746f 7461 6c5f 6e65 752c 2074 6f74  , total_neu, tot
+00004110: 616c 5f70 6f73 2c20 746f 7461 6c5f 636f  al_pos, total_co
+00004120: 6d70 6f75 6e64 203d 2030 2c20 302c 2030  mpound = 0, 0, 0
+00004130: 2c20 3020 0d0a 2020 2020 2020 2020 2020  , 0 ..          
+00004140: 2020 2020 2020 6f72 6967 696e 616c 5f64        original_d
+00004150: 6f63 203d 206e 702e 6172 7261 7928 5b6f  oc = np.array([o
+00004160: 7269 6769 6e61 6c5f 646f 632e 7370 6c69  riginal_doc.spli
+00004170: 7428 295d 290d 0a20 2020 2020 2020 2020  t()])..         
+00004180: 2020 2020 2020 206e 756d 5f73 706c 6974         num_split
+00004190: 203d 2069 6e74 2872 6f75 6e64 2828 6c65   = int(round((le
+000041a0: 6e5f 6f72 6967 696e 616c 5f74 6f6b 656e  n_original_token
+000041b0: 732f 3531 3429 2b31 2c20 3029 290d 0a20  s/514)+1, 0)).. 
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000041d0: 6172 6167 7261 7068 7320 3d20 6e70 2e61  aragraphs = np.a
+000041e0: 7272 6179 5f73 706c 6974 286f 7269 6769  rray_split(origi
+000041f0: 6e61 6c5f 646f 632c 206e 756d 5f73 706c  nal_doc, num_spl
+00004200: 6974 2c20 6178 6973 3d31 290d 0a20 2020  it, axis=1)..   
+00004210: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00004220: 2069 2069 6e20 7261 6e67 6528 6e75 6d5f   i in range(num_
+00004230: 7370 6c69 7429 3a20 0d0a 2020 2020 2020  split): ..      
+00004240: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00004250: 7261 6772 6170 6820 3d20 7061 7261 6772  ragraph = paragr
+00004260: 6170 6873 5b69 5d0d 0a20 2020 2020 2020  aphs[i]..       
+00004270: 2020 2020 2020 2020 2020 2020 2070 6172               par
+00004280: 6167 7261 7068 203d 2022 2022 2e6a 6f69  agraph = " ".joi
+00004290: 6e28 7374 7228 776f 7264 292e 7265 706c  n(str(word).repl
+000042a0: 6163 6528 2227 222c 2022 2229 2066 6f72  ace("'", "") for
+000042b0: 2077 6f72 6420 696e 206c 6973 7428 7061   word in list(pa
+000042c0: 7261 6772 6170 6829 290d 0a20 2020 2020  ragraph))..     
+000042d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000042e0: 6172 6167 7261 7068 203d 2070 6172 6167  aragraph = parag
+000042f0: 7261 7068 2e72 6570 6c61 6365 2822 5c6e  raph.replace("\n
+00004300: 222c 2022 2229 0d0a 2020 2020 2020 2020  ", "")..        
+00004310: 2020 2020 2020 2020 2020 2020 7061 7261              para
+00004320: 6772 6170 6820 3d20 7061 7261 6772 6170  graph = paragrap
+00004330: 682e 7265 706c 6163 6528 225b 222c 2022  h.replace("[", "
+00004340: 2229 2e72 6570 6c61 6365 2822 5d22 2c20  ").replace("]", 
+00004350: 2222 290d 0a20 2020 2020 2020 2020 2020  "")..           
+00004360: 2020 2020 2020 2020 2074 6f6b 656e 7320           tokens 
+00004370: 3d20 7365 6c66 2e54 7769 7474 6572 5f58  = self.Twitter_X
+00004380: 4c4d 5f72 6f42 4552 5461 5f74 6f6b 656e  LM_roBERTa_token
+00004390: 697a 6572 2870 6172 6167 7261 7068 2c20  izer(paragraph, 
+000043a0: 7265 7475 726e 5f74 656e 736f 7273 3d27  return_tensors='
+000043b0: 7074 2729 0d0a 2020 2020 2020 2020 2020  pt')..          
+000043c0: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
+000043d0: 6720 3d20 7365 6c66 2e54 7769 7474 6572  g = self.Twitter
+000043e0: 5f58 4c4d 5f72 6f42 4552 5461 282a 2a74  _XLM_roBERTa(**t
+000043f0: 6f6b 656e 7329 0d0a 2020 2020 2020 2020  okens)..        
+00004400: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
+00004410: 696e 6720 3d20 7363 6f72 696e 675b 305d  ing = scoring[0]
+00004420: 5b30 5d2e 6465 7461 6368 2829 2e6e 756d  [0].detach().num
+00004430: 7079 2829 0d0a 2020 2020 2020 2020 2020  py()..          
+00004440: 2020 2020 2020 2020 2020 7363 6f72 696e            scorin
+00004450: 6720 3d20 736f 6674 6d61 7828 7363 6f72  g = softmax(scor
+00004460: 696e 6729 0d0a 2020 2020 2020 2020 2020  ing)..          
+00004470: 2020 2020 2020 2020 2020 7261 6e6b 696e            rankin
+00004480: 6720 3d20 6e70 2e61 7267 736f 7274 2873  g = np.argsort(s
+00004490: 636f 7269 6e67 290d 0a20 2020 2020 2020  coring)..       
+000044a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000044b0: 2069 2069 6e20 7261 6e67 6528 7363 6f72   i in range(scor
+000044c0: 696e 672e 7368 6170 655b 305d 293a 0d0a  ing.shape[0]):..
+000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044e0: 2020 2020 2020 2020 6c20 3d20 6c61 6265          l = labe
+000044f0: 6c73 5b72 616e 6b69 6e67 5b69 5d5d 0d0a  ls[ranking[i]]..
+00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004510: 2020 2020 2020 2020 7320 3d20 7363 6f72          s = scor
+00004520: 696e 675b 7261 6e6b 696e 675b 695d 5d0d  ing[ranking[i]].
+00004530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004540: 2020 2020 2020 2020 2069 6620 6c20 3d3d           if l ==
+00004550: 2027 706f 7369 7469 7665 273a 200d 0a20   'positive': .. 
+00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004570: 2020 2020 2020 2020 2020 2074 6f74 616c             total
+00004580: 5f70 6f73 202b 3d20 7320 0d0a 2020 2020  _pos += s ..    
+00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045a0: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
+000045b0: 6d70 6f75 6e64 202b 3d20 732a 3130 0d0a  mpound += s*10..
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 2020 2020 2020 2020 656c 6966 206c 203d          elif l =
+000045e0: 3d20 276e 6567 6174 6976 6527 3a20 0d0a  = 'negative': ..
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00004610: 6c5f 6e65 6720 2b3d 2073 0d0a 2020 2020  l_neg += s..    
+00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004630: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
+00004640: 6d70 6f75 6e64 202d 3d20 732a 3130 0d0a  mpound -= s*10..
+00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004660: 2020 2020 2020 2020 656c 7365 3a20 0d0a          else: ..
+00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004680: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00004690: 6c5f 6e65 7520 2b3d 2073 0d0a 2020 2020  l_neu += s..    
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 2020 2020 2020 2020 746f 7461 6c5f 636f          total_co
+000046c0: 6d70 6f75 6e64 202b 3d20 732a 310d 0a20  mpound += s*1.. 
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000046e0: 656e 745f 6469 6374 203d 207b 276e 6567  ent_dict = {'neg
+000046f0: 273a 2072 6f75 6e64 2874 6f74 616c 5f6e  ': round(total_n
+00004700: 6567 2f6e 756d 5f73 706c 6974 2c20 3529  eg/num_split, 5)
+00004710: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
 00004720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004730: 2020 2020 2020 2020 2020 276e 6575 273a            'neu':
-00004740: 2072 6f75 6e64 2874 6f74 616c 5f6e 6575   round(total_neu
-00004750: 2f6e 756d 5f73 706c 6974 2c20 3529 2c20  /num_split, 5), 
-00004760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004770: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00004780: 706f 7327 3a20 726f 756e 6428 746f 7461  pos': round(tota
-00004790: 6c5f 706f 732f 6e75 6d5f 7370 6c69 742c  l_pos/num_split,
-000047a0: 2035 292c 200d 0a20 2020 2020 2020 2020   5), ..         
-000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 2020 2763 6f6d 706f 756e 6427 3a20      'compound': 
-000047d0: 7365 6c66 2e72 6573 6361 6c69 6e67 2874  self.rescaling(t
-000047e0: 6f74 616c 5f63 6f6d 706f 756e 642c 202d  otal_compound, -
-000047f0: 3130 2a6e 756d 5f73 706c 6974 2c20 3130  10*num_split, 10
-00004800: 2a6e 756d 5f73 706c 6974 297d 0d0a 2020  *num_split)}..  
-00004810: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004830: 6966 2073 756d 6d61 7269 7a65 2069 7320  if summarize is 
-00004840: 5472 7565 3a20 0d0a 2020 2020 2020 2020  True: ..        
-00004850: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004860: 726e 2073 656e 745f 6469 6374 5b27 636f  rn sent_dict['co
-00004870: 6d70 6f75 6e64 275d 0d0a 2020 2020 2020  mpound']..      
-00004880: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-00004890: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000048a0: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
-000048b0: 745f 6469 6374 200d 0a20 2020 2020 2020  t_dict ..       
-000048c0: 2065 7863 6570 7420 4174 7472 6962 7574   except Attribut
-000048d0: 6545 7272 6f72 3a20 0d0a 2020 2020 2020  eError: ..      
-000048e0: 2020 2020 2020 7261 6973 6520 5379 7374        raise Syst
-000048f0: 656d 4572 726f 7228 2258 4c4d 5f72 6f42  emError("XLM_roB
-00004900: 4552 5461 206d 7573 7420 6265 206c 6f61  ERTa must be loa
-00004910: 6465 6420 696e 2070 7269 6f72 2e20 4c6f  ded in prior. Lo
-00004920: 6164 2074 6865 206d 6f64 656c 2076 6961  ad the model via
-00004930: 206e 6c70 2e73 656e 7469 6d65 6e74 286c   nlp.sentiment(l
-00004940: 6f61 645f 6d6f 6465 6c73 3d27 584c 4d5f  oad_models='XLM_
-00004950: 726f 4245 5254 6127 2922 290d 0a0d 0a20  roBERTa')").... 
-00004960: 2020 2023 6669 6e42 4552 540d 0a20 2020     #finBERT..   
-00004970: 2064 6566 2066 696e 4245 5254 2873 656c   def finBERT(sel
-00004980: 662c 200d 0a20 2020 2020 2020 2020 2020  f, ..           
-00004990: 2020 2020 2074 6578 743a 7374 722c 200d       text:str, .
-000049a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049b0: 2074 6578 745f 7479 7065 3a73 7472 2c20   text_type:str, 
-000049c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000049d0: 2020 7375 6d6d 6172 697a 653a 626f 6f6c    summarize:bool
-000049e0: 3d54 7275 6529 202d 3e20 666c 6f61 7420  =True) -> float 
-000049f0: 6f72 2064 6963 743a 200d 0a20 2020 2020  or dict: ..     
-00004a00: 2020 2074 7279 3a20 0d0a 2020 2020 2020     try: ..      
-00004a10: 2020 2020 2020 2222 2261 2042 4552 5420        """a BERT 
-00004a20: 6d6f 6465 6c20 7472 6169 6e65 6420 6f6e  model trained on
-00004a30: 2034 3030 6b20 6669 6e61 6e63 6961 6c20   400k financial 
-00004a40: 7465 7874 732c 2069 6e63 6c75 6469 6e67  texts, including
-00004a50: 2054 5243 322d 6669 6e61 6e63 6961 6c20   TRC2-financial 
-00004a60: 6461 7461 7365 742c 2046 696e 616e 6369  dataset, Financi
-00004a70: 616c 2050 6872 6173 6542 616e 6b2c 2061  al PhraseBank, a
-00004a80: 6e64 2046 6951 4120 5365 6e74 696d 656e  nd FiQA Sentimen
-00004a90: 7420 6461 7461 7365 7422 2222 0d0a 2020  t dataset"""..  
-00004aa0: 2020 2020 2020 2020 2020 6966 2074 6578            if tex
-00004ab0: 745f 7479 7065 2e6c 6f77 6572 2829 203d  t_type.lower() =
-00004ac0: 3d20 276e 6577 7327 3a20 0d0a 2020 2020  = 'news': ..    
-00004ad0: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
-00004ae0: 696e 616c 5f64 6f63 203d 2070 7265 7072  inal_doc = prepr
-00004af0: 6f63 6573 732e 6e65 7773 2874 6578 7429  ocess.news(text)
-00004b00: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00004b10: 6966 2074 6578 745f 7479 7065 2e6c 6f77  if text_type.low
-00004b20: 6572 2829 203d 3d20 2774 7765 6574 7327  er() == 'tweets'
-00004b30: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
-00004b40: 2020 2020 6f72 6967 696e 616c 5f64 6f63      original_doc
-00004b50: 203d 2070 7265 7072 6f63 6573 732e 7477   = preprocess.tw
-00004b60: 6565 7473 2874 6578 7429 0d0a 2020 2020  eets(text)..    
-00004b70: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
-00004b80: 205b 276e 6575 7472 616c 272c 2027 706f   ['neutral', 'po
-00004b90: 7369 7469 7665 272c 2027 6e65 6761 7469  sitive', 'negati
-00004ba0: 7665 275d 0d0a 2020 2020 2020 2020 2020  ve']..          
-00004bb0: 2020 6f72 6967 696e 616c 5f74 6f6b 656e    original_token
-00004bc0: 7320 3d20 7365 6c66 2e46 696e 4245 5254  s = self.FinBERT
-00004bd0: 5f74 6f6b 656e 697a 6572 286f 7269 6769  _tokenizer(origi
-00004be0: 6e61 6c5f 646f 632c 2072 6574 7572 6e5f  nal_doc, return_
-00004bf0: 7465 6e73 6f72 733d 2770 7427 290d 0a20  tensors='pt').. 
-00004c00: 2020 2020 2020 2020 2020 206c 656e 5f6f             len_o
-00004c10: 7269 6769 6e61 6c5f 746f 6b65 6e73 203d  riginal_tokens =
-00004c20: 206c 656e 286f 7269 6769 6e61 6c5f 746f   len(original_to
-00004c30: 6b65 6e73 5b27 696e 7075 745f 6964 7327  kens['input_ids'
-00004c40: 5d5b 305d 290d 0a20 2020 2020 2020 2020  ][0])..         
-00004c50: 2020 2069 6620 6c65 6e5f 6f72 6967 696e     if len_origin
-00004c60: 616c 5f74 6f6b 656e 7320 3c3d 2035 3132  al_tokens <= 512
-00004c70: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
-00004c80: 2020 2020 7363 6f72 696e 6720 3d20 7365      scoring = se
-00004c90: 6c66 2e46 696e 4245 5254 282a 2a6f 7269  lf.FinBERT(**ori
-00004ca0: 6769 6e61 6c5f 746f 6b65 6e73 290d 0a20  ginal_tokens).. 
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004cc0: 636f 7269 6e67 203d 2073 636f 7269 6e67  coring = scoring
-00004cd0: 5b30 5d5b 305d 2e64 6574 6163 6828 292e  [0][0].detach().
-00004ce0: 6e75 6d70 7928 290d 0a20 2020 2020 2020  numpy()..       
-00004cf0: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
-00004d00: 203d 2073 6f66 746d 6178 2873 636f 7269   = softmax(scori
-00004d10: 6e67 290d 0a20 2020 2020 2020 2020 2020  ng)..           
-00004d20: 2020 2020 2072 616e 6b69 6e67 203d 206e       ranking = n
-00004d30: 702e 6172 6773 6f72 7428 7363 6f72 696e  p.argsort(scorin
-00004d40: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-00004d50: 2020 2020 7365 6e74 5f64 6963 742c 2063      sent_dict, c
-00004d60: 6f6d 706f 756e 6420 3d20 7b27 6e65 6727  ompound = {'neg'
-00004d70: 3a20 302c 2027 6e65 7527 3a20 302c 2027  : 0, 'neu': 0, '
-00004d80: 706f 7327 3a20 302c 2027 636f 6d70 6f75  pos': 0, 'compou
-00004d90: 6e64 273a 2030 7d2c 2030 200d 0a20 2020  nd': 0}, 0 ..   
-00004da0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00004db0: 2069 2069 6e20 7261 6e67 6528 7363 6f72   i in range(scor
-00004dc0: 696e 672e 7368 6170 655b 305d 293a 0d0a  ing.shape[0]):..
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 6c20 3d20 6c61 6265 6c73 5b72      l = labels[r
-00004df0: 616e 6b69 6e67 5b69 5d5d 0d0a 2020 2020  anking[i]]..    
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 7320 3d20 7363 6f72 696e 675b 7261 6e6b  s = scoring[rank
-00004e20: 696e 675b 695d 5d0d 0a20 2020 2020 2020  ing[i]]..       
-00004e30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004e40: 6c20 3d3d 2027 706f 7369 7469 7665 273a  l == 'positive':
-00004e50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00004e60: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
-00004e70: 756e 6420 2b3d 2073 2a31 300d 0a20 2020  und += s*10..   
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e90: 2020 2020 2073 656e 745f 6469 6374 2e75       sent_dict.u
-00004ea0: 7064 6174 6528 7b27 706f 7327 3a20 726f  pdate({'pos': ro
-00004eb0: 756e 6428 666c 6f61 7428 7329 2c20 3529  und(float(s), 5)
-00004ec0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
-00004ed0: 2020 2020 2020 2020 656c 6966 206c 203d          elif l =
-00004ee0: 3d20 276e 6567 6174 6976 6527 3a20 0d0a  = 'negative': ..
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 2020 2020 2020 636f 6d70 6f75 6e64          compound
-00004f10: 202d 3d20 732a 3130 0d0a 2020 2020 2020   -= s*10..      
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f30: 2020 7365 6e74 5f64 6963 742e 7570 6461    sent_dict.upda
-00004f40: 7465 287b 276e 6567 273a 2072 6f75 6e64  te({'neg': round
-00004f50: 2866 6c6f 6174 2873 292c 2035 297d 290d  (float(s), 5)}).
-00004f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004f70: 2020 2020 2065 6c73 653a 200d 0a20 2020       else: ..   
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 2020 2020 2063 6f6d 706f 756e 6420 2b3d       compound +=
-00004fa0: 2073 2a31 0d0a 2020 2020 2020 2020 2020   s*1..          
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004fc0: 6e74 5f64 6963 742e 7570 6461 7465 287b  nt_dict.update({
-00004fd0: 276e 6575 273a 2072 6f75 6e64 2866 6c6f  'neu': round(flo
-00004fe0: 6174 2873 292c 2035 297d 290d 0a20 2020  at(s), 5)})..   
-00004ff0: 2020 2020 2020 2020 2020 2020 2073 656e               sen
-00005000: 745f 6469 6374 2e75 7064 6174 6528 7b27  t_dict.update({'
-00005010: 636f 6d70 6f75 6e64 273a 2073 656c 662e  compound': self.
-00005020: 7265 7363 616c 696e 6728 666c 6f61 7428  rescaling(float(
-00005030: 636f 6d70 6f75 6e64 292c 202d 3130 2c20  compound), -10, 
-00005040: 3130 297d 290d 0a20 2020 2020 2020 2020  10)})..         
-00005050: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00005060: 2020 2020 2020 2020 2069 6620 7375 6d6d           if summ
-00005070: 6172 697a 6520 6973 2054 7275 653a 200d  arize is True: .
-00005080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005090: 2020 2020 2072 6574 7572 6e20 7365 6e74       return sent
-000050a0: 5f64 6963 745b 2763 6f6d 706f 756e 6427  _dict['compound'
-000050b0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-000050c0: 2020 2065 6c73 653a 200d 0a20 2020 2020     else: ..     
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000050e0: 6574 7572 6e20 7365 6e74 5f64 6963 7420  eturn sent_dict 
-000050f0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00005100: 6966 206c 656e 5f6f 7269 6769 6e61 6c5f  if len_original_
-00005110: 746f 6b65 6e73 203e 2035 3132 3a20 0d0a  tokens > 512: ..
-00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 7365 6c66 2e6c 6f67 6765 722e 7761 726e  self.logger.warn
-00005140: 696e 6728 22e2 949c e294 80e2 9480 2041  ing("......... A
-00005150: 6e79 2077 6172 6e69 6e67 7320 7265 6c61  ny warnings rela
-00005160: 7465 6420 746f 2054 6f6b 656e 5365 7175  ted to TokenSequ
-00005170: 656e 6365 4c65 6e67 7468 2063 616e 2062  enceLength can b
-00005180: 6520 6967 6e6f 7265 6420 6173 2069 6e70  e ignored as inp
-00005190: 7574 2027 7465 7874 2720 6861 7320 6265  ut 'text' has be
-000051a0: 656e 2073 706c 6974 6564 2c20 7375 6368  en splited, such
-000051b0: 2074 6861 7420 7468 6520 7365 7175 656e   that the sequen
-000051c0: 6365 206c 656e 6774 6820 6f66 2065 6163  ce length of eac
-000051d0: 6820 7370 6c69 7420 6973 2061 6c77 6179  h split is alway
-000051e0: 7320 6c65 7373 2074 6861 6e20 7468 6520  s less than the 
-000051f0: 7370 6563 6966 6965 6420 6d61 7869 6d75  specified maximu
-00005200: 6d20 7365 7175 656e 6365 206c 656e 6774  m sequence lengt
-00005210: 6822 290d 0a20 2020 2020 2020 2020 2020  h")..           
-00005220: 2020 2020 2074 6f74 616c 5f6e 6567 2c20       total_neg, 
-00005230: 746f 7461 6c5f 6e65 752c 2074 6f74 616c  total_neu, total
-00005240: 5f70 6f73 2c20 746f 7461 6c5f 636f 6d70  _pos, total_comp
-00005250: 6f75 6e64 203d 2030 2c20 302c 2030 2c20  ound = 0, 0, 0, 
-00005260: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
-00005270: 2020 2020 6f72 6967 696e 616c 5f64 6f63      original_doc
-00005280: 203d 206e 702e 6172 7261 7928 5b6f 7269   = np.array([ori
-00005290: 6769 6e61 6c5f 646f 632e 7370 6c69 7428  ginal_doc.split(
-000052a0: 295d 290d 0a20 2020 2020 2020 2020 2020  )])..           
-000052b0: 2020 2020 206e 756d 5f73 706c 6974 203d       num_split =
-000052c0: 2069 6e74 2872 6f75 6e64 2828 6c65 6e5f   int(round((len_
-000052d0: 6f72 6967 696e 616c 5f74 6f6b 656e 732f  original_tokens/
-000052e0: 3531 3229 2b31 2c20 3029 290d 0a20 2020  512)+1, 0))..   
-000052f0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00005300: 6167 7261 7068 7320 3d20 6e70 2e61 7272  agraphs = np.arr
-00005310: 6179 5f73 706c 6974 286f 7269 6769 6e61  ay_split(origina
-00005320: 6c5f 646f 632c 206e 756d 5f73 706c 6974  l_doc, num_split
-00005330: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
-00005340: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00005350: 2069 6e20 7261 6e67 6528 6e75 6d5f 7370   in range(num_sp
-00005360: 6c69 7429 3a20 0d0a 2020 2020 2020 2020  lit): ..        
-00005370: 2020 2020 2020 2020 2020 2020 7061 7261              para
-00005380: 6772 6170 6820 3d20 7061 7261 6772 6170  graph = paragrap
-00005390: 6873 5b69 5d0d 0a20 2020 2020 2020 2020  hs[i]..         
-000053a0: 2020 2020 2020 2020 2020 2070 6172 6167             parag
-000053b0: 7261 7068 203d 2022 2022 2e6a 6f69 6e28  raph = " ".join(
-000053c0: 7374 7228 776f 7264 292e 7265 706c 6163  str(word).replac
-000053d0: 6528 2227 222c 2022 2229 2066 6f72 2077  e("'", "") for w
-000053e0: 6f72 6420 696e 206c 6973 7428 7061 7261  ord in list(para
-000053f0: 6772 6170 6829 290d 0a20 2020 2020 2020  graph))..       
-00005400: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00005410: 6167 7261 7068 203d 2070 6172 6167 7261  agraph = paragra
-00005420: 7068 2e72 6570 6c61 6365 2822 5c6e 222c  ph.replace("\n",
-00005430: 2022 2229 0d0a 2020 2020 2020 2020 2020   "")..          
-00005440: 2020 2020 2020 2020 2020 7061 7261 6772            paragr
-00005450: 6170 6820 3d20 7061 7261 6772 6170 682e  aph = paragraph.
-00005460: 7265 706c 6163 6528 225b 222c 2022 2229  replace("[", "")
-00005470: 2e72 6570 6c61 6365 2822 5d22 2c20 2222  .replace("]", ""
-00005480: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005490: 2020 2020 2020 2074 6f6b 656e 7320 3d20         tokens = 
-000054a0: 7365 6c66 2e46 696e 4245 5254 5f74 6f6b  self.FinBERT_tok
-000054b0: 656e 697a 6572 2870 6172 6167 7261 7068  enizer(paragraph
-000054c0: 2c20 7265 7475 726e 5f74 656e 736f 7273  , return_tensors
-000054d0: 3d27 7074 2729 0d0a 2020 2020 2020 2020  ='pt')..        
-000054e0: 2020 2020 2020 2020 2020 2020 7363 6f72              scor
-000054f0: 696e 6720 3d20 7365 6c66 2e46 696e 4245  ing = self.FinBE
-00005500: 5254 282a 2a74 6f6b 656e 7329 0d0a 2020  RT(**tokens)..  
-00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005520: 2020 7363 6f72 696e 6720 3d20 7363 6f72    scoring = scor
-00005530: 696e 675b 305d 5b30 5d2e 6465 7461 6368  ing[0][0].detach
-00005540: 2829 2e6e 756d 7079 2829 0d0a 2020 2020  ().numpy()..    
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 7363 6f72 696e 6720 3d20 736f 6674 6d61  scoring = softma
-00005570: 7828 7363 6f72 696e 6729 0d0a 2020 2020  x(scoring)..    
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 7261 6e6b 696e 6720 3d20 6e70 2e61 7267  ranking = np.arg
-000055a0: 736f 7274 2873 636f 7269 6e67 290d 0a20  sort(scoring).. 
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-000055d0: 6528 7363 6f72 696e 672e 7368 6170 655b  e(scoring.shape[
-000055e0: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
-000055f0: 2020 2020 2020 2020 2020 2020 2020 6c20                l 
-00005600: 3d20 6c61 6265 6c73 5b72 616e 6b69 6e67  = labels[ranking
-00005610: 5b69 5d5d 0d0a 2020 2020 2020 2020 2020  [i]]..          
-00005620: 2020 2020 2020 2020 2020 2020 2020 7320                s 
-00005630: 3d20 7363 6f72 696e 675b 7261 6e6b 696e  = scoring[rankin
-00005640: 675b 695d 5d0d 0a20 2020 2020 2020 2020  g[i]]..         
-00005650: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00005660: 6620 6c20 3d3d 2027 706f 7369 7469 7665  f l == 'positive
-00005670: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2074 6f74 616c 5f70 6f73 202b 3d20 7320   total_pos += s 
-000056a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000056b0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-000056c0: 7461 6c5f 636f 6d70 6f75 6e64 202b 3d20  tal_compound += 
-000056d0: 732a 3130 0d0a 2020 2020 2020 2020 2020  s*10..          
-000056e0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000056f0: 6966 206c 203d 3d20 276e 6567 6174 6976  if l == 'negativ
-00005700: 6527 3a20 0d0a 2020 2020 2020 2020 2020  e': ..          
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2020 746f 7461 6c5f 6e65 6720 2b3d 2073    total_neg += s
-00005730: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005740: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00005750: 7461 6c5f 636f 6d70 6f75 6e64 202d 3d20  tal_compound -= 
-00005760: 732a 3130 0d0a 2020 2020 2020 2020 2020  s*10..          
-00005770: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005780: 7365 3a20 0d0a 2020 2020 2020 2020 2020  se: ..          
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 746f 7461 6c5f 6e65 7520 2b3d 2073    total_neu += s
-000057b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000057c0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-000057d0: 7461 6c5f 636f 6d70 6f75 6e64 202b 3d20  tal_compound += 
-000057e0: 732a 310d 0a20 2020 2020 2020 2020 2020  s*1..           
-000057f0: 2020 2020 2073 656e 745f 6469 6374 203d       sent_dict =
-00005800: 207b 276e 6567 273a 2072 6f75 6e64 2874   {'neg': round(t
-00005810: 6f74 616c 5f6e 6567 2f6e 756d 5f73 706c  otal_neg/num_spl
-00005820: 6974 2c20 3529 2c20 0d0a 2020 2020 2020  it, 5), ..      
-00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005840: 2020 2020 2020 2027 6e65 7527 3a20 726f         'neu': ro
-00005850: 756e 6428 746f 7461 6c5f 6e65 752f 6e75  und(total_neu/nu
-00005860: 6d5f 7370 6c69 742c 2035 292c 200d 0a20  m_split, 5), .. 
+00004730: 2027 6e65 7527 3a20 726f 756e 6428 746f   'neu': round(to
+00004740: 7461 6c5f 6e65 752f 6e75 6d5f 7370 6c69  tal_neu/num_spli
+00004750: 742c 2035 292c 200d 0a20 2020 2020 2020  t, 5), ..       
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 2020 2020 2770 6f73 273a 2072 6f75        'pos': rou
+00004780: 6e64 2874 6f74 616c 5f70 6f73 2f6e 756d  nd(total_pos/num
+00004790: 5f73 706c 6974 2c20 3529 2c20 0d0a 2020  _split, 5), ..  
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 2020 2020 2020 2027 636f 6d70             'comp
+000047c0: 6f75 6e64 273a 2073 656c 662e 7265 7363  ound': self.resc
+000047d0: 616c 696e 6728 746f 7461 6c5f 636f 6d70  aling(total_comp
+000047e0: 6f75 6e64 2c20 2d31 302a 6e75 6d5f 7370  ound, -10*num_sp
+000047f0: 6c69 742c 2031 302a 6e75 6d5f 7370 6c69  lit, 10*num_spli
+00004800: 7429 7d0d 0a20 2020 2020 2020 2020 2020  t)}..           
+00004810: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00004820: 2020 2020 2020 2069 6620 7375 6d6d 6172         if summar
+00004830: 697a 6520 6973 2054 7275 653a 200d 0a20  ize is True: .. 
+00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004850: 2020 2072 6574 7572 6e20 7365 6e74 5f64     return sent_d
+00004860: 6963 745b 2763 6f6d 706f 756e 6427 5d0d  ict['compound'].
+00004870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004880: 2065 6c73 653a 200d 0a20 2020 2020 2020   else: ..       
+00004890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000048a0: 7572 6e20 7365 6e74 5f64 6963 7420 0d0a  urn sent_dict ..
+000048b0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+000048c0: 7474 7269 6275 7465 4572 726f 723a 200d  ttributeError: .
+000048d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000048e0: 7365 2053 7973 7465 6d45 7272 6f72 2822  se SystemError("
+000048f0: 584c 4d5f 726f 4245 5254 6120 6d75 7374  XLM_roBERTa must
+00004900: 2062 6520 6c6f 6164 6564 2069 6e20 7072   be loaded in pr
+00004910: 696f 722e 204c 6f61 6420 7468 6520 6d6f  ior. Load the mo
+00004920: 6465 6c20 7669 6120 6e6c 702e 7365 6e74  del via nlp.sent
+00004930: 696d 656e 7428 6c6f 6164 5f6d 6f64 656c  iment(load_model
+00004940: 733d 2758 4c4d 5f72 6f42 4552 5461 2729  s='XLM_roBERTa')
+00004950: 2229 0d0a 0d0a 2020 2020 2366 696e 4245  ")....    #finBE
+00004960: 5254 0d0a 2020 2020 6465 6620 6669 6e42  RT..    def finB
+00004970: 4552 5428 7365 6c66 2c20 0d0a 2020 2020  ERT(self, ..    
+00004980: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00004990: 3a73 7472 2c20 0d0a 2020 2020 2020 2020  :str, ..        
+000049a0: 2020 2020 2020 2020 7465 7874 5f74 7970          text_typ
+000049b0: 653a 7374 722c 200d 0a20 2020 2020 2020  e:str, ..       
+000049c0: 2020 2020 2020 2020 2073 756d 6d61 7269           summari
+000049d0: 7a65 3a62 6f6f 6c3d 5472 7565 2920 2d3e  ze:bool=True) ->
+000049e0: 2066 6c6f 6174 206f 7220 6469 6374 3a20   float or dict: 
+000049f0: 0d0a 2020 2020 2020 2020 7472 793a 200d  ..        try: .
+00004a00: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+00004a10: 6120 4245 5254 206d 6f64 656c 2074 7261  a BERT model tra
+00004a20: 696e 6564 206f 6e20 3430 306b 2066 696e  ined on 400k fin
+00004a30: 616e 6369 616c 2074 6578 7473 2c20 696e  ancial texts, in
+00004a40: 636c 7564 696e 6720 5452 4332 2d66 696e  cluding TRC2-fin
+00004a50: 616e 6369 616c 2064 6174 6173 6574 2c20  ancial dataset, 
+00004a60: 4669 6e61 6e63 6961 6c20 5068 7261 7365  Financial Phrase
+00004a70: 4261 6e6b 2c20 616e 6420 4669 5141 2053  Bank, and FiQA S
+00004a80: 656e 7469 6d65 6e74 2064 6174 6173 6574  entiment dataset
+00004a90: 2222 220d 0a20 2020 2020 2020 2020 2020  """..           
+00004aa0: 2069 6620 7465 7874 5f74 7970 652e 6c6f   if text_type.lo
+00004ab0: 7765 7228 2920 3d3d 2027 6e65 7773 273a  wer() == 'news':
+00004ac0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00004ad0: 2020 206f 7269 6769 6e61 6c5f 646f 6320     original_doc 
+00004ae0: 3d20 7072 6570 726f 6365 7373 2e6e 6577  = preprocess.new
+00004af0: 7328 7465 7874 290d 0a20 2020 2020 2020  s(text)..       
+00004b00: 2020 2020 2065 6c69 6620 7465 7874 5f74       elif text_t
+00004b10: 7970 652e 6c6f 7765 7228 2920 3d3d 2027  ype.lower() == '
+00004b20: 7477 6565 7473 273a 200d 0a20 2020 2020  tweets': ..     
+00004b30: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+00004b40: 6e61 6c5f 646f 6320 3d20 7072 6570 726f  nal_doc = prepro
+00004b50: 6365 7373 2e74 7765 6574 7328 7465 7874  cess.tweets(text
+00004b60: 290d 0a20 2020 2020 2020 2020 2020 206c  )..            l
+00004b70: 6162 656c 7320 3d20 5b27 6e65 7574 7261  abels = ['neutra
+00004b80: 6c27 2c20 2770 6f73 6974 6976 6527 2c20  l', 'positive', 
+00004b90: 276e 6567 6174 6976 6527 5d0d 0a20 2020  'negative']..   
+00004ba0: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
+00004bb0: 6c5f 746f 6b65 6e73 203d 2073 656c 662e  l_tokens = self.
+00004bc0: 4669 6e42 4552 545f 746f 6b65 6e69 7a65  FinBERT_tokenize
+00004bd0: 7228 6f72 6967 696e 616c 5f64 6f63 2c20  r(original_doc, 
+00004be0: 7265 7475 726e 5f74 656e 736f 7273 3d27  return_tensors='
+00004bf0: 7074 2729 0d0a 2020 2020 2020 2020 2020  pt')..          
+00004c00: 2020 6c65 6e5f 6f72 6967 696e 616c 5f74    len_original_t
+00004c10: 6f6b 656e 7320 3d20 6c65 6e28 6f72 6967  okens = len(orig
+00004c20: 696e 616c 5f74 6f6b 656e 735b 2769 6e70  inal_tokens['inp
+00004c30: 7574 5f69 6473 275d 5b30 5d29 0d0a 2020  ut_ids'][0])..  
+00004c40: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00004c50: 5f6f 7269 6769 6e61 6c5f 746f 6b65 6e73  _original_tokens
+00004c60: 203c 3d20 3531 323a 200d 0a20 2020 2020   <= 512: ..     
+00004c70: 2020 2020 2020 2020 2020 2073 636f 7269             scori
+00004c80: 6e67 203d 2073 656c 662e 4669 6e42 4552  ng = self.FinBER
+00004c90: 5428 2a2a 6f72 6967 696e 616c 5f74 6f6b  T(**original_tok
+00004ca0: 656e 7329 0d0a 2020 2020 2020 2020 2020  ens)..          
+00004cb0: 2020 2020 2020 7363 6f72 696e 6720 3d20        scoring = 
+00004cc0: 7363 6f72 696e 675b 305d 5b30 5d2e 6465  scoring[0][0].de
+00004cd0: 7461 6368 2829 2e6e 756d 7079 2829 0d0a  tach().numpy()..
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 7363 6f72 696e 6720 3d20 736f 6674 6d61  scoring = softma
+00004d00: 7828 7363 6f72 696e 6729 0d0a 2020 2020  x(scoring)..    
+00004d10: 2020 2020 2020 2020 2020 2020 7261 6e6b              rank
+00004d20: 696e 6720 3d20 6e70 2e61 7267 736f 7274  ing = np.argsort
+00004d30: 2873 636f 7269 6e67 290d 0a20 2020 2020  (scoring)..     
+00004d40: 2020 2020 2020 2020 2020 2073 656e 745f             sent_
+00004d50: 6469 6374 2c20 636f 6d70 6f75 6e64 203d  dict, compound =
+00004d60: 207b 276e 6567 273a 2030 2c20 276e 6575   {'neg': 0, 'neu
+00004d70: 273a 2030 2c20 2770 6f73 273a 2030 2c20  ': 0, 'pos': 0, 
+00004d80: 2763 6f6d 706f 756e 6427 3a20 307d 2c20  'compound': 0}, 
+00004d90: 3020 0d0a 2020 2020 2020 2020 2020 2020  0 ..            
+00004da0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00004db0: 6765 2873 636f 7269 6e67 2e73 6861 7065  ge(scoring.shape
+00004dc0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+00004dd0: 2020 2020 2020 2020 2020 206c 203d 206c             l = l
+00004de0: 6162 656c 735b 7261 6e6b 696e 675b 695d  abels[ranking[i]
+00004df0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00004e00: 2020 2020 2020 2073 203d 2073 636f 7269         s = scori
+00004e10: 6e67 5b72 616e 6b69 6e67 5b69 5d5d 0d0a  ng[ranking[i]]..
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e30: 2020 2020 6966 206c 203d 3d20 2770 6f73      if l == 'pos
+00004e40: 6974 6976 6527 3a20 0d0a 2020 2020 2020  itive': ..      
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 636f 6d70 6f75 6e64 202b 3d20 732a    compound += s*
+00004e70: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
+00004e80: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
+00004e90: 5f64 6963 742e 7570 6461 7465 287b 2770  _dict.update({'p
+00004ea0: 6f73 273a 2072 6f75 6e64 2866 6c6f 6174  os': round(float
+00004eb0: 2873 292c 2035 297d 290d 0a20 2020 2020  (s), 5)})..     
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004ed0: 6c69 6620 6c20 3d3d 2027 6e65 6761 7469  lif l == 'negati
+00004ee0: 7665 273a 200d 0a20 2020 2020 2020 2020  ve': ..         
+00004ef0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00004f00: 6f6d 706f 756e 6420 2d3d 2073 2a31 300d  ompound -= s*10.
+00004f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f20: 2020 2020 2020 2020 2073 656e 745f 6469           sent_di
+00004f30: 6374 2e75 7064 6174 6528 7b27 6e65 6727  ct.update({'neg'
+00004f40: 3a20 726f 756e 6428 666c 6f61 7428 7329  : round(float(s)
+00004f50: 2c20 3529 7d29 0d0a 2020 2020 2020 2020  , 5)})..        
+00004f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00004f70: 3a20 0d0a 2020 2020 2020 2020 2020 2020  : ..            
+00004f80: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00004f90: 6f75 6e64 202b 3d20 732a 310d 0a20 2020  ound += s*1..   
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fb0: 2020 2020 2073 656e 745f 6469 6374 2e75       sent_dict.u
+00004fc0: 7064 6174 6528 7b27 6e65 7527 3a20 726f  pdate({'neu': ro
+00004fd0: 756e 6428 666c 6f61 7428 7329 2c20 3529  und(float(s), 5)
+00004fe0: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00004ff0: 2020 2020 7365 6e74 5f64 6963 742e 7570      sent_dict.up
+00005000: 6461 7465 287b 2763 6f6d 706f 756e 6427  date({'compound'
+00005010: 3a20 7365 6c66 2e72 6573 6361 6c69 6e67  : self.rescaling
+00005020: 2866 6c6f 6174 2863 6f6d 706f 756e 6429  (float(compound)
+00005030: 2c20 2d31 302c 2031 3029 7d29 0d0a 2020  , -10, 10)})..  
+00005040: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005060: 6966 2073 756d 6d61 7269 7a65 2069 7320  if summarize is 
+00005070: 5472 7565 3a20 0d0a 2020 2020 2020 2020  True: ..        
+00005080: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00005090: 726e 2073 656e 745f 6469 6374 5b27 636f  rn sent_dict['co
+000050a0: 6d70 6f75 6e64 275d 0d0a 2020 2020 2020  mpound']..      
+000050b0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
+000050c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000050d0: 2020 2020 2020 7265 7475 726e 2073 656e        return sen
+000050e0: 745f 6469 6374 200d 0a20 2020 2020 2020  t_dict ..       
+000050f0: 2020 2020 2065 6c69 6620 6c65 6e5f 6f72       elif len_or
+00005100: 6967 696e 616c 5f74 6f6b 656e 7320 3e20  iginal_tokens > 
+00005110: 3531 323a 200d 0a20 2020 2020 2020 2020  512: ..         
+00005120: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+00005130: 6572 2e77 6172 6e69 6e67 2822 e294 9ce2  er.warning("....
+00005140: 9480 e294 8020 416e 7920 7761 726e 696e  ..... Any warnin
+00005150: 6773 2072 656c 6174 6564 2074 6f20 546f  gs related to To
+00005160: 6b65 6e53 6571 7565 6e63 654c 656e 6774  kenSequenceLengt
+00005170: 6820 6361 6e20 6265 2069 676e 6f72 6564  h can be ignored
+00005180: 2061 7320 696e 7075 7420 2774 6578 7427   as input 'text'
+00005190: 2068 6173 2062 6565 6e20 7370 6c69 7465   has been splite
+000051a0: 642c 2073 7563 6820 7468 6174 2074 6865  d, such that the
+000051b0: 2073 6571 7565 6e63 6520 6c65 6e67 7468   sequence length
+000051c0: 206f 6620 6561 6368 2073 706c 6974 2069   of each split i
+000051d0: 7320 616c 7761 7973 206c 6573 7320 7468  s always less th
+000051e0: 616e 2074 6865 2073 7065 6369 6669 6564  an the specified
+000051f0: 206d 6178 696d 756d 2073 6571 7565 6e63   maximum sequenc
+00005200: 6520 6c65 6e67 7468 2229 0d0a 2020 2020  e length")..    
+00005210: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00005220: 6c5f 6e65 672c 2074 6f74 616c 5f6e 6575  l_neg, total_neu
+00005230: 2c20 746f 7461 6c5f 706f 732c 2074 6f74  , total_pos, tot
+00005240: 616c 5f63 6f6d 706f 756e 6420 3d20 302c  al_compound = 0,
+00005250: 2030 2c20 302c 2030 200d 0a20 2020 2020   0, 0, 0 ..     
+00005260: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+00005270: 6e61 6c5f 646f 6320 3d20 6e70 2e61 7272  nal_doc = np.arr
+00005280: 6179 285b 6f72 6967 696e 616c 5f64 6f63  ay([original_doc
+00005290: 2e73 706c 6974 2829 5d29 0d0a 2020 2020  .split()])..    
+000052a0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+000052b0: 7370 6c69 7420 3d20 696e 7428 726f 756e  split = int(roun
+000052c0: 6428 286c 656e 5f6f 7269 6769 6e61 6c5f  d((len_original_
+000052d0: 746f 6b65 6e73 2f35 3132 292b 312c 2030  tokens/512)+1, 0
+000052e0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000052f0: 2020 2020 7061 7261 6772 6170 6873 203d      paragraphs =
+00005300: 206e 702e 6172 7261 795f 7370 6c69 7428   np.array_split(
+00005310: 6f72 6967 696e 616c 5f64 6f63 2c20 6e75  original_doc, nu
+00005320: 6d5f 7370 6c69 742c 2061 7869 733d 3129  m_split, axis=1)
+00005330: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005340: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00005350: 286e 756d 5f73 706c 6974 293a 200d 0a20  (num_split): .. 
+00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005370: 2020 2070 6172 6167 7261 7068 203d 2070     paragraph = p
+00005380: 6172 6167 7261 7068 735b 695d 0d0a 2020  aragraphs[i]..  
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 2020 7061 7261 6772 6170 6820 3d20 2220    paragraph = " 
+000053b0: 222e 6a6f 696e 2873 7472 2877 6f72 6429  ".join(str(word)
+000053c0: 2e72 6570 6c61 6365 2822 2722 2c20 2222  .replace("'", ""
+000053d0: 2920 666f 7220 776f 7264 2069 6e20 6c69  ) for word in li
+000053e0: 7374 2870 6172 6167 7261 7068 2929 0d0a  st(paragraph))..
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 2020 7061 7261 6772 6170 6820 3d20      paragraph = 
+00005410: 7061 7261 6772 6170 682e 7265 706c 6163  paragraph.replac
+00005420: 6528 225c 6e22 2c20 2222 290d 0a20 2020  e("\n", "")..   
+00005430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005440: 2070 6172 6167 7261 7068 203d 2070 6172   paragraph = par
+00005450: 6167 7261 7068 2e72 6570 6c61 6365 2822  agraph.replace("
+00005460: 5b22 2c20 2222 292e 7265 706c 6163 6528  [", "").replace(
+00005470: 225d 222c 2022 2229 0d0a 2020 2020 2020  "]", "")..      
+00005480: 2020 2020 2020 2020 2020 2020 2020 746f                to
+00005490: 6b65 6e73 203d 2073 656c 662e 4669 6e42  kens = self.FinB
+000054a0: 4552 545f 746f 6b65 6e69 7a65 7228 7061  ERT_tokenizer(pa
+000054b0: 7261 6772 6170 682c 2072 6574 7572 6e5f  ragraph, return_
+000054c0: 7465 6e73 6f72 733d 2770 7427 290d 0a20  tensors='pt').. 
+000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054e0: 2020 2073 636f 7269 6e67 203d 2073 656c     scoring = sel
+000054f0: 662e 4669 6e42 4552 5428 2a2a 746f 6b65  f.FinBERT(**toke
+00005500: 6e73 290d 0a20 2020 2020 2020 2020 2020  ns)..           
+00005510: 2020 2020 2020 2020 2073 636f 7269 6e67           scoring
+00005520: 203d 2073 636f 7269 6e67 5b30 5d5b 305d   = scoring[0][0]
+00005530: 2e64 6574 6163 6828 292e 6e75 6d70 7928  .detach().numpy(
+00005540: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005550: 2020 2020 2020 2073 636f 7269 6e67 203d         scoring =
+00005560: 2073 6f66 746d 6178 2873 636f 7269 6e67   softmax(scoring
+00005570: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005580: 2020 2020 2020 2072 616e 6b69 6e67 203d         ranking =
+00005590: 206e 702e 6172 6773 6f72 7428 7363 6f72   np.argsort(scor
+000055a0: 696e 6729 0d0a 2020 2020 2020 2020 2020  ing)..          
+000055b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+000055c0: 696e 2072 616e 6765 2873 636f 7269 6e67  in range(scoring
+000055d0: 2e73 6861 7065 5b30 5d29 3a0d 0a20 2020  .shape[0]):..   
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 206c 203d 206c 6162 656c 735b       l = labels[
+00005600: 7261 6e6b 696e 675b 695d 5d0d 0a20 2020  ranking[i]]..   
+00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005620: 2020 2020 2073 203d 2073 636f 7269 6e67       s = scoring
+00005630: 5b72 616e 6b69 6e67 5b69 5d5d 0d0a 2020  [ranking[i]]..  
+00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005650: 2020 2020 2020 6966 206c 203d 3d20 2770        if l == 'p
+00005660: 6f73 6974 6976 6527 3a20 0d0a 2020 2020  ositive': ..    
+00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005680: 2020 2020 2020 2020 746f 7461 6c5f 706f          total_po
+00005690: 7320 2b3d 2073 200d 0a20 2020 2020 2020  s += s ..       
+000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056b0: 2020 2020 2074 6f74 616c 5f63 6f6d 706f       total_compo
+000056c0: 756e 6420 2b3d 2073 2a31 300d 0a20 2020  und += s*10..   
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056e0: 2020 2020 2065 6c69 6620 6c20 3d3d 2027       elif l == '
+000056f0: 6e65 6761 7469 7665 273a 200d 0a20 2020  negative': ..   
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2020 2020 2020 2074 6f74 616c 5f6e           total_n
+00005720: 6567 202b 3d20 730d 0a20 2020 2020 2020  eg += s..       
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2020 2020 2074 6f74 616c 5f63 6f6d 706f       total_compo
+00005750: 756e 6420 2d3d 2073 2a31 300d 0a20 2020  und -= s*10..   
+00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005770: 2020 2020 2065 6c73 653a 200d 0a20 2020       else: ..   
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2020 2020 2074 6f74 616c 5f6e           total_n
+000057a0: 6575 202b 3d20 730d 0a20 2020 2020 2020  eu += s..       
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2020 2020 2074 6f74 616c 5f63 6f6d 706f       total_compo
+000057d0: 756e 6420 2b3d 2073 2a31 0d0a 2020 2020  und += s*1..    
+000057e0: 2020 2020 2020 2020 2020 2020 7365 6e74              sent
+000057f0: 5f64 6963 7420 3d20 7b27 6e65 6727 3a20  _dict = {'neg': 
+00005800: 726f 756e 6428 746f 7461 6c5f 6e65 672f  round(total_neg/
+00005810: 6e75 6d5f 7370 6c69 742c 2035 292c 200d  num_split, 5), .
+00005820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005830: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+00005840: 6575 273a 2072 6f75 6e64 2874 6f74 616c  eu': round(total
+00005850: 5f6e 6575 2f6e 756d 5f73 706c 6974 2c20  _neu/num_split, 
+00005860: 3529 2c20 0d0a 2020 2020 2020 2020 2020  5), ..          
 00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 2020 2020 2020 2020 2020 2020 2770 6f73              'pos
-00005890: 273a 2072 6f75 6e64 2874 6f74 616c 5f70  ': round(total_p
-000058a0: 6f73 2f6e 756d 5f73 706c 6974 2c20 3529  os/num_split, 5)
-000058b0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2027 636f 6d70 6f75 6e64 273a 2073 656c   'compound': sel
-000058e0: 662e 7265 7363 616c 696e 6728 746f 7461  f.rescaling(tota
-000058f0: 6c5f 636f 6d70 6f75 6e64 2c20 2d31 302a  l_compound, -10*
-00005900: 6e75 6d5f 7370 6c69 742c 2031 302a 6e75  num_split, 10*nu
-00005910: 6d5f 7370 6c69 7429 7d0d 0a20 2020 2020  m_split)}..     
-00005920: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00005930: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005940: 7375 6d6d 6172 697a 6520 6973 2054 7275  summarize is Tru
-00005950: 653a 200d 0a20 2020 2020 2020 2020 2020  e: ..           
-00005960: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005970: 7365 6e74 5f64 6963 745b 2763 6f6d 706f  sent_dict['compo
-00005980: 756e 6427 5d0d 0a20 2020 2020 2020 2020  und']..         
-00005990: 2020 2020 2020 2065 6c73 653a 200d 0a20         else: .. 
-000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059b0: 2020 2072 6574 7572 6e20 7365 6e74 5f64     return sent_d
-000059c0: 6963 7420 0d0a 2020 2020 2020 2020 6578  ict ..        ex
-000059d0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-000059e0: 726f 723a 200d 0a20 2020 2020 2020 2020  ror: ..         
-000059f0: 2020 2072 6169 7365 2053 7973 7465 6d45     raise SystemE
-00005a00: 7272 6f72 2822 6669 6e42 4552 5420 6d75  rror("finBERT mu
-00005a10: 7374 2062 6520 6c6f 6164 6564 2069 6e20  st be loaded in 
-00005a20: 7072 696f 722e 204c 6f61 6420 7468 6520  prior. Load the 
-00005a30: 6d6f 6465 6c20 7669 6120 6e6c 702e 7365  model via nlp.se
-00005a40: 6e74 696d 656e 7428 6c6f 6164 5f6d 6f64  ntiment(load_mod
-00005a50: 656c 733d 2766 696e 4245 5254 2729 2229  els='finBERT')")
-00005a60: 0d0a 0d0a 2020 2020 2341 6c6c 206d 6f64  ....    #All mod
-00005a70: 656c 7320 200d 0a20 2020 2064 6566 2061  els  ..    def a
-00005a80: 6767 7265 6761 7465 2873 656c 662c 200d  ggregate(self, .
-00005a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005aa0: 2020 2074 6578 743a 7374 722c 200d 0a20     text:str, .. 
-00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ac0: 2074 6578 745f 7479 7065 3a73 7472 2c20   text_type:str, 
-00005ad0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005ae0: 2020 2020 7375 6d6d 6172 697a 653a 626f      summarize:bo
-00005af0: 6f6c 3d54 7275 6529 202d 3e20 666c 6f61  ol=True) -> floa
-00005b00: 7420 6f72 2064 6963 743a 200d 0a20 2020  t or dict: ..   
-00005b10: 2020 2020 2074 7279 3a20 0d0a 2020 2020       try: ..    
-00005b20: 2020 2020 2020 2020 6966 2073 756d 6d61          if summa
-00005b30: 7269 7a65 2069 7320 5472 7565 3a20 0d0a  rize is True: ..
-00005b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b50: 2320 616c 7068 6156 4144 4552 5f63 203d  # alphaVADER_c =
-00005b60: 2073 656c 662e 616c 7068 6156 4144 4552   self.alphaVADER
-00005b70: 2874 6578 742c 2074 6578 745f 7479 7065  (text, text_type
-00005b80: 3d74 6578 745f 7479 7065 290d 0a20 2020  =text_type)..   
-00005b90: 2020 2020 2020 2020 2020 2020 2072 6f42               roB
-00005ba0: 4552 5461 5f76 315f 6320 3d20 7365 6c66  ERTa_v1_c = self
-00005bb0: 2e74 7769 7474 6572 5f72 6f42 4552 5461  .twitter_roBERTa
-00005bc0: 5f76 3128 7465 7874 2c20 7465 7874 5f74  _v1(text, text_t
-00005bd0: 7970 653d 7465 7874 5f74 7970 6529 0d0a  ype=text_type)..
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bf0: 726f 4245 5254 615f 7632 5f63 203d 2073  roBERTa_v2_c = s
-00005c00: 656c 662e 7477 6974 7465 725f 726f 4245  elf.twitter_roBE
-00005c10: 5254 615f 7632 2874 6578 742c 2074 6578  RTa_v2(text, tex
-00005c20: 745f 7479 7065 3d74 6578 745f 7479 7065  t_type=text_type
-00005c30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00005c40: 2020 2058 4c4d 5f72 6f42 4552 5461 5f63     XLM_roBERTa_c
-00005c50: 203d 2073 656c 662e 7477 6974 7465 725f   = self.twitter_
-00005c60: 584c 4d5f 726f 4245 5254 6128 7465 7874  XLM_roBERTa(text
-00005c70: 2c20 7465 7874 5f74 7970 653d 7465 7874  , text_type=text
-00005c80: 5f74 7970 6529 0d0a 2020 2020 2020 2020  _type)..        
-00005c90: 2020 2020 2020 2020 6669 6e42 4552 545f          finBERT_
-00005ca0: 6320 3d20 7365 6c66 2e66 696e 4245 5254  c = self.finBERT
-00005cb0: 2874 6578 742c 2074 6578 745f 7479 7065  (text, text_type
-00005cc0: 3d74 6578 745f 7479 7065 290d 0a20 2020  =text_type)..   
-00005cd0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00005ce0: 7572 6e20 7b23 2761 6c70 6861 5641 4445  urn {#'alphaVADE
-00005cf0: 5227 3a20 616c 7068 6156 4144 4552 5f63  R': alphaVADER_c
-00005d00: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00005d10: 2020 2020 2020 2020 2020 2027 726f 4245             'roBE
-00005d20: 5254 615f 7631 273a 2072 6f42 4552 5461  RTa_v1': roBERTa
-00005d30: 5f76 315f 632c 0d0a 2020 2020 2020 2020  _v1_c,..        
-00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d50: 2772 6f42 4552 5461 5f76 3227 3a20 726f  'roBERTa_v2': ro
-00005d60: 4245 5254 615f 7632 5f63 2c0d 0a20 2020  BERTa_v2_c,..   
-00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d80: 2020 2020 2027 584c 4d5f 726f 4245 5254       'XLM_roBERT
-00005d90: 6127 3a20 584c 4d5f 726f 4245 5254 615f  a': XLM_roBERTa_
-00005da0: 632c 0d0a 2020 2020 2020 2020 2020 2020  c,..            
-00005db0: 2020 2020 2020 2020 2020 2020 2766 696e              'fin
-00005dc0: 4245 5254 273a 2066 696e 4245 5254 5f63  BERT': finBERT_c
-00005dd0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-00005de0: 2020 2020 2020 2020 2020 2020 2774 6f74              'tot
-00005df0: 616c 273a 2072 6f75 6e64 286e 702e 6d65  al': round(np.me
-00005e00: 616e 285b 2361 6c70 6861 5641 4445 525f  an([#alphaVADER_
-00005e10: 632c 200d 0a20 2020 2020 2020 2020 2020  c, ..           
+00005880: 2020 2027 706f 7327 3a20 726f 756e 6428     'pos': round(
+00005890: 746f 7461 6c5f 706f 732f 6e75 6d5f 7370  total_pos/num_sp
+000058a0: 6c69 742c 2035 292c 200d 0a20 2020 2020  lit, 5), ..     
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 2020 2020 2763 6f6d 706f 756e          'compoun
+000058d0: 6427 3a20 7365 6c66 2e72 6573 6361 6c69  d': self.rescali
+000058e0: 6e67 2874 6f74 616c 5f63 6f6d 706f 756e  ng(total_compoun
+000058f0: 642c 202d 3130 2a6e 756d 5f73 706c 6974  d, -10*num_split
+00005900: 2c20 3130 2a6e 756d 5f73 706c 6974 297d  , 10*num_split)}
+00005910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005920: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00005930: 2020 2020 6966 2073 756d 6d61 7269 7a65      if summarize
+00005940: 2069 7320 5472 7565 3a20 0d0a 2020 2020   is True: ..    
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 7265 7475 726e 2073 656e 745f 6469 6374  return sent_dict
+00005970: 5b27 636f 6d70 6f75 6e64 275d 0d0a 2020  ['compound']..  
+00005980: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005990: 7365 3a20 0d0a 2020 2020 2020 2020 2020  se: ..          
+000059a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000059b0: 2073 656e 745f 6469 6374 200d 0a20 2020   sent_dict ..   
+000059c0: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
+000059d0: 6962 7574 6545 7272 6f72 3a20 0d0a 2020  ibuteError: ..  
+000059e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000059f0: 5379 7374 656d 4572 726f 7228 2266 696e  SystemError("fin
+00005a00: 4245 5254 206d 7573 7420 6265 206c 6f61  BERT must be loa
+00005a10: 6465 6420 696e 2070 7269 6f72 2e20 4c6f  ded in prior. Lo
+00005a20: 6164 2074 6865 206d 6f64 656c 2076 6961  ad the model via
+00005a30: 206e 6c70 2e73 656e 7469 6d65 6e74 286c   nlp.sentiment(l
+00005a40: 6f61 645f 6d6f 6465 6c73 3d27 6669 6e42  oad_models='finB
+00005a50: 4552 5427 2922 290d 0a0d 0a20 2020 2023  ERT')")....    #
+00005a60: 416c 6c20 6d6f 6465 6c73 2020 0d0a 2020  All models  ..  
+00005a70: 2020 6465 6620 6167 6772 6567 6174 6528    def aggregate(
+00005a80: 7365 6c66 2c20 0d0a 2020 2020 2020 2020  self, ..        
+00005a90: 2020 2020 2020 2020 2020 7465 7874 3a73            text:s
+00005aa0: 7472 2c20 0d0a 2020 2020 2020 2020 2020  tr, ..          
+00005ab0: 2020 2020 2020 2020 7465 7874 5f74 7970          text_typ
+00005ac0: 653a 7374 722c 200d 0a20 2020 2020 2020  e:str, ..       
+00005ad0: 2020 2020 2020 2020 2020 2073 756d 6d61             summa
+00005ae0: 7269 7a65 3a62 6f6f 6c3d 5472 7565 2920  rize:bool=True) 
+00005af0: 2d3e 2066 6c6f 6174 206f 7220 6469 6374  -> float or dict
+00005b00: 3a20 0d0a 2020 2020 2020 2020 7472 793a  : ..        try:
+00005b10: 200d 0a20 2020 2020 2020 2020 2020 2069   ..            i
+00005b20: 6620 7375 6d6d 6172 697a 6520 6973 2054  f summarize is T
+00005b30: 7275 653a 200d 0a20 2020 2020 2020 2020  rue: ..         
+00005b40: 2020 2020 2020 2023 2061 6c70 6861 5641         # alphaVA
+00005b50: 4445 525f 6320 3d20 7365 6c66 2e61 6c70  DER_c = self.alp
+00005b60: 6861 5641 4445 5228 7465 7874 2c20 7465  haVADER(text, te
+00005b70: 7874 5f74 7970 653d 7465 7874 5f74 7970  xt_type=text_typ
+00005b80: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00005b90: 2020 2020 726f 4245 5254 615f 7631 5f63      roBERTa_v1_c
+00005ba0: 203d 2073 656c 662e 7477 6974 7465 725f   = self.twitter_
+00005bb0: 726f 4245 5254 615f 7631 2874 6578 742c  roBERTa_v1(text,
+00005bc0: 2074 6578 745f 7479 7065 3d74 6578 745f   text_type=text_
+00005bd0: 7479 7065 290d 0a20 2020 2020 2020 2020  type)..         
+00005be0: 2020 2020 2020 2072 6f42 4552 5461 5f76         roBERTa_v
+00005bf0: 325f 6320 3d20 7365 6c66 2e74 7769 7474  2_c = self.twitt
+00005c00: 6572 5f72 6f42 4552 5461 5f76 3228 7465  er_roBERTa_v2(te
+00005c10: 7874 2c20 7465 7874 5f74 7970 653d 7465  xt, text_type=te
+00005c20: 7874 5f74 7970 6529 0d0a 2020 2020 2020  xt_type)..      
+00005c30: 2020 2020 2020 2020 2020 584c 4d5f 726f            XLM_ro
+00005c40: 4245 5254 615f 6320 3d20 7365 6c66 2e74  BERTa_c = self.t
+00005c50: 7769 7474 6572 5f58 4c4d 5f72 6f42 4552  witter_XLM_roBER
+00005c60: 5461 2874 6578 742c 2074 6578 745f 7479  Ta(text, text_ty
+00005c70: 7065 3d74 6578 745f 7479 7065 290d 0a20  pe=text_type).. 
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00005c90: 696e 4245 5254 5f63 203d 2073 656c 662e  inBERT_c = self.
+00005ca0: 6669 6e42 4552 5428 7465 7874 2c20 7465  finBERT(text, te
+00005cb0: 7874 5f74 7970 653d 7465 7874 5f74 7970  xt_type=text_typ
+00005cc0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00005cd0: 2020 2020 7265 7475 726e 207b 2327 616c      return {#'al
+00005ce0: 7068 6156 4144 4552 273a 2061 6c70 6861  phaVADER': alpha
+00005cf0: 5641 4445 525f 632c 0d0a 2020 2020 2020  VADER_c,..      
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 2020 2772 6f42 4552 5461 5f76 3127 3a20    'roBERTa_v1': 
+00005d20: 726f 4245 5254 615f 7631 5f63 2c0d 0a20  roBERTa_v1_c,.. 
+00005d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d40: 2020 2020 2020 2027 726f 4245 5254 615f         'roBERTa_
+00005d50: 7632 273a 2072 6f42 4552 5461 5f76 325f  v2': roBERTa_v2_
+00005d60: 632c 0d0a 2020 2020 2020 2020 2020 2020  c,..            
+00005d70: 2020 2020 2020 2020 2020 2020 2758 4c4d              'XLM
+00005d80: 5f72 6f42 4552 5461 273a 2058 4c4d 5f72  _roBERTa': XLM_r
+00005d90: 6f42 4552 5461 5f63 2c0d 0a20 2020 2020  oBERTa_c,..     
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2027 6669 6e42 4552 5427 3a20 6669     'finBERT': fi
+00005dc0: 6e42 4552 545f 632c 200d 0a20 2020 2020  nBERT_c, ..     
+00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005de0: 2020 2027 746f 7461 6c27 3a20 726f 756e     'total': roun
+00005df0: 6428 6e70 2e6d 6561 6e28 5b23 616c 7068  d(np.mean([#alph
+00005e00: 6156 4144 4552 5f63 2c20 0d0a 2020 2020  aVADER_c, ..    
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e40: 2020 2020 2072 6f42 4552 5461 5f76 315f       roBERTa_v1_
-00005e50: 632c 2072 6f42 4552 5461 5f76 325f 632c  c, roBERTa_v2_c,
-00005e60: 2058 4c4d 5f72 6f42 4552 5461 5f63 2c20   XLM_roBERTa_c, 
-00005e70: 6669 6e42 4552 545f 635d 292c 2035 297d  finBERT_c]), 5)}
-00005e80: 200d 0a20 2020 2020 2020 2020 2020 2065   ..            e
-00005e90: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00005ea0: 2020 2020 2020 2320 616c 7068 6156 4144        # alphaVAD
-00005eb0: 4552 5f64 6963 7420 3d20 7365 6c66 2e61  ER_dict = self.a
-00005ec0: 6c70 6861 5641 4445 5228 7465 7874 2c20  lphaVADER(text, 
-00005ed0: 7465 7874 5f74 7970 653d 7465 7874 5f74  text_type=text_t
-00005ee0: 7970 652c 2073 756d 6d61 7269 7a65 3d73  ype, summarize=s
-00005ef0: 756d 6d61 7269 7a65 290d 0a20 2020 2020  ummarize)..     
-00005f00: 2020 2020 2020 2020 2020 2072 6f42 4552             roBER
-00005f10: 5461 5f76 315f 6469 6374 203d 2073 656c  Ta_v1_dict = sel
-00005f20: 662e 7477 6974 7465 725f 726f 4245 5254  f.twitter_roBERT
-00005f30: 615f 7631 2874 6578 742c 2074 6578 745f  a_v1(text, text_
-00005f40: 7479 7065 3d74 6578 745f 7479 7065 2c20  type=text_type, 
-00005f50: 7375 6d6d 6172 697a 653d 7375 6d6d 6172  summarize=summar
-00005f60: 697a 6529 0d0a 2020 2020 2020 2020 2020  ize)..          
-00005f70: 2020 2020 2020 726f 4245 5254 615f 7632        roBERTa_v2
-00005f80: 5f64 6963 7420 3d20 7365 6c66 2e74 7769  _dict = self.twi
-00005f90: 7474 6572 5f72 6f42 4552 5461 5f76 3228  tter_roBERTa_v2(
-00005fa0: 7465 7874 2c20 7465 7874 5f74 7970 653d  text, text_type=
-00005fb0: 7465 7874 5f74 7970 652c 2073 756d 6d61  text_type, summa
-00005fc0: 7269 7a65 3d73 756d 6d61 7269 7a65 290d  rize=summarize).
-00005fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005fe0: 2058 4c4d 5f72 6f42 4552 5461 5f64 6963   XLM_roBERTa_dic
-00005ff0: 7420 3d20 7365 6c66 2e74 7769 7474 6572  t = self.twitter
-00006000: 5f58 4c4d 5f72 6f42 4552 5461 2874 6578  _XLM_roBERTa(tex
-00006010: 742c 2074 6578 745f 7479 7065 3d74 6578  t, text_type=tex
-00006020: 745f 7479 7065 2c20 7375 6d6d 6172 697a  t_type, summariz
-00006030: 653d 7375 6d6d 6172 697a 6529 0d0a 2020  e=summarize)..  
-00006040: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00006050: 6e42 4552 545f 6469 6374 203d 2073 656c  nBERT_dict = sel
-00006060: 662e 6669 6e42 4552 5428 7465 7874 2c20  f.finBERT(text, 
-00006070: 7465 7874 5f74 7970 653d 7465 7874 5f74  text_type=text_t
-00006080: 7970 652c 2073 756d 6d61 7269 7a65 3d73  ype, summarize=s
-00006090: 756d 6d61 7269 7a65 290d 0a0d 0a20 2020  ummarize)....   
-000060a0: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-000060b0: 203d 205b 2361 6c70 6861 5641 4445 525f   = [#alphaVADER_
-000060c0: 6469 6374 5b27 706f 7327 5d2c 200d 0a20  dict['pos'], .. 
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 726f 4245 5254 615f 7631        roBERTa_v1
-000060f0: 5f64 6963 745b 2770 6f73 275d 2c20 726f  _dict['pos'], ro
-00006100: 4245 5254 615f 7632 5f64 6963 745b 2770  BERTa_v2_dict['p
-00006110: 6f73 275d 2c20 584c 4d5f 726f 4245 5254  os'], XLM_roBERT
-00006120: 615f 6469 6374 5b27 706f 7327 5d2c 2066  a_dict['pos'], f
-00006130: 696e 4245 5254 5f64 6963 745b 2770 6f73  inBERT_dict['pos
-00006140: 275d 5d0d 0a20 2020 2020 2020 2020 2020  ']]..           
-00006150: 2020 2020 206e 6567 203d 205b 2361 6c70       neg = [#alp
-00006160: 6861 5641 4445 525f 6469 6374 5b27 6e65  haVADER_dict['ne
-00006170: 6727 5d2c 200d 0a20 2020 2020 2020 2020  g'], ..         
-00006180: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00006190: 4245 5254 615f 7631 5f64 6963 745b 276e  BERTa_v1_dict['n
-000061a0: 6567 275d 2c20 726f 4245 5254 615f 7632  eg'], roBERTa_v2
-000061b0: 5f64 6963 745b 276e 6567 275d 2c20 584c  _dict['neg'], XL
-000061c0: 4d5f 726f 4245 5254 615f 6469 6374 5b27  M_roBERTa_dict['
-000061d0: 6e65 6727 5d2c 2066 696e 4245 5254 5f64  neg'], finBERT_d
-000061e0: 6963 745b 276e 6567 275d 5d0d 0a20 2020  ict['neg']]..   
-000061f0: 2020 2020 2020 2020 2020 2020 206e 6575               neu
-00006200: 203d 205b 2361 6c70 6861 5641 4445 525f   = [#alphaVADER_
-00006210: 6469 6374 5b27 6e65 7527 5d2c 200d 0a20  dict['neu'], .. 
-00006220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006230: 2020 2020 2020 726f 4245 5254 615f 7631        roBERTa_v1
-00006240: 5f64 6963 745b 276e 6575 275d 2c20 726f  _dict['neu'], ro
-00006250: 4245 5254 615f 7632 5f64 6963 745b 276e  BERTa_v2_dict['n
-00006260: 6575 275d 2c20 584c 4d5f 726f 4245 5254  eu'], XLM_roBERT
-00006270: 615f 6469 6374 5b27 6e65 7527 5d2c 2066  a_dict['neu'], f
-00006280: 696e 4245 5254 5f64 6963 745b 276e 6575  inBERT_dict['neu
-00006290: 275d 5d0d 0a20 2020 2020 2020 2020 2020  ']]..           
-000062a0: 2020 2020 2063 6f6d 706f 756e 6420 3d20       compound = 
-000062b0: 5b23 616c 7068 6156 4144 4552 5f64 6963  [#alphaVADER_dic
-000062c0: 745b 2763 6f6d 706f 756e 6427 5d2c 200d  t['compound'], .
-000062d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062e0: 2020 2020 2020 2020 2020 2020 2072 6f42               roB
-000062f0: 4552 5461 5f76 315f 6469 6374 5b27 636f  ERTa_v1_dict['co
-00006300: 6d70 6f75 6e64 275d 2c20 726f 4245 5254  mpound'], roBERT
-00006310: 615f 7632 5f64 6963 745b 2763 6f6d 706f  a_v2_dict['compo
-00006320: 756e 6427 5d2c 2058 4c4d 5f72 6f42 4552  und'], XLM_roBER
-00006330: 5461 5f64 6963 745b 2763 6f6d 706f 756e  Ta_dict['compoun
-00006340: 6427 5d2c 2066 696e 4245 5254 5f64 6963  d'], finBERT_dic
-00006350: 745b 2763 6f6d 706f 756e 6427 5d5d 0d0a  t['compound']]..
-00006360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006370: 2020 7265 7475 726e 207b 2327 616c 7068    return {#'alph
-00006380: 6156 4144 4552 273a 2061 6c70 6861 5641  aVADER': alphaVA
-00006390: 4445 525f 6469 6374 2c0d 0a20 2020 2020  DER_dict,..     
-000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2027 726f 4245 5254 615f 7631 273a     'roBERTa_v1':
-000063c0: 2072 6f42 4552 5461 5f76 315f 6469 6374   roBERTa_v1_dict
-000063d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000063e0: 2020 2020 2020 2020 2020 2027 726f 4245             'roBE
-000063f0: 5254 615f 7632 273a 2072 6f42 4552 5461  RTa_v2': roBERTa
-00006400: 5f76 325f 6469 6374 2c0d 0a20 2020 2020  _v2_dict,..     
-00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006420: 2020 2027 584c 4d5f 726f 4245 5254 6127     'XLM_roBERTa'
-00006430: 3a20 584c 4d5f 726f 4245 5254 615f 6469  : XLM_roBERTa_di
-00006440: 6374 2c0d 0a20 2020 2020 2020 2020 2020  ct,..           
-00006450: 2020 2020 2020 2020 2020 2020 2027 6669               'fi
-00006460: 6e42 4552 5427 3a20 6669 6e42 4552 545f  nBERT': finBERT_
-00006470: 6469 6374 2c20 0d0a 2020 2020 2020 2020  dict, ..        
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2774 6f74 616c 273a 207b 276e 6567 273a  'total': {'neg':
-000064a0: 2072 6f75 6e64 286e 702e 6d65 616e 286e   round(np.mean(n
-000064b0: 6567 292c 3529 2c20 0d0a 2020 2020 2020  eg),5), ..      
+00005e30: 2020 2020 2020 2020 2020 2020 726f 4245              roBE
+00005e40: 5254 615f 7631 5f63 2c20 726f 4245 5254  RTa_v1_c, roBERT
+00005e50: 615f 7632 5f63 2c20 584c 4d5f 726f 4245  a_v2_c, XLM_roBE
+00005e60: 5254 615f 632c 2066 696e 4245 5254 5f63  RTa_c, finBERT_c
+00005e70: 5d29 2c20 3529 7d20 0d0a 2020 2020 2020  ]), 5)} ..      
+00005e80: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00005e90: 2020 2020 2020 2020 2020 2020 2023 2061               # a
+00005ea0: 6c70 6861 5641 4445 525f 6469 6374 203d  lphaVADER_dict =
+00005eb0: 2073 656c 662e 616c 7068 6156 4144 4552   self.alphaVADER
+00005ec0: 2874 6578 742c 2074 6578 745f 7479 7065  (text, text_type
+00005ed0: 3d74 6578 745f 7479 7065 2c20 7375 6d6d  =text_type, summ
+00005ee0: 6172 697a 653d 7375 6d6d 6172 697a 6529  arize=summarize)
+00005ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005f00: 2020 726f 4245 5254 615f 7631 5f64 6963    roBERTa_v1_dic
+00005f10: 7420 3d20 7365 6c66 2e74 7769 7474 6572  t = self.twitter
+00005f20: 5f72 6f42 4552 5461 5f76 3128 7465 7874  _roBERTa_v1(text
+00005f30: 2c20 7465 7874 5f74 7970 653d 7465 7874  , text_type=text
+00005f40: 5f74 7970 652c 2073 756d 6d61 7269 7a65  _type, summarize
+00005f50: 3d73 756d 6d61 7269 7a65 290d 0a20 2020  =summarize)..   
+00005f60: 2020 2020 2020 2020 2020 2020 2072 6f42               roB
+00005f70: 4552 5461 5f76 325f 6469 6374 203d 2073  ERTa_v2_dict = s
+00005f80: 656c 662e 7477 6974 7465 725f 726f 4245  elf.twitter_roBE
+00005f90: 5254 615f 7632 2874 6578 742c 2074 6578  RTa_v2(text, tex
+00005fa0: 745f 7479 7065 3d74 6578 745f 7479 7065  t_type=text_type
+00005fb0: 2c20 7375 6d6d 6172 697a 653d 7375 6d6d  , summarize=summ
+00005fc0: 6172 697a 6529 0d0a 2020 2020 2020 2020  arize)..        
+00005fd0: 2020 2020 2020 2020 584c 4d5f 726f 4245          XLM_roBE
+00005fe0: 5254 615f 6469 6374 203d 2073 656c 662e  RTa_dict = self.
+00005ff0: 7477 6974 7465 725f 584c 4d5f 726f 4245  twitter_XLM_roBE
+00006000: 5254 6128 7465 7874 2c20 7465 7874 5f74  RTa(text, text_t
+00006010: 7970 653d 7465 7874 5f74 7970 652c 2073  ype=text_type, s
+00006020: 756d 6d61 7269 7a65 3d73 756d 6d61 7269  ummarize=summari
+00006030: 7a65 290d 0a20 2020 2020 2020 2020 2020  ze)..           
+00006040: 2020 2020 2066 696e 4245 5254 5f64 6963       finBERT_dic
+00006050: 7420 3d20 7365 6c66 2e66 696e 4245 5254  t = self.finBERT
+00006060: 2874 6578 742c 2074 6578 745f 7479 7065  (text, text_type
+00006070: 3d74 6578 745f 7479 7065 2c20 7375 6d6d  =text_type, summ
+00006080: 6172 697a 653d 7375 6d6d 6172 697a 6529  arize=summarize)
+00006090: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000060a0: 2020 2020 706f 7320 3d20 5b23 616c 7068      pos = [#alph
+000060b0: 6156 4144 4552 5f64 6963 745b 2770 6f73  aVADER_dict['pos
+000060c0: 275d 2c20 0d0a 2020 2020 2020 2020 2020  '], ..          
+000060d0: 2020 2020 2020 2020 2020 2020 2072 6f42               roB
+000060e0: 4552 5461 5f76 315f 6469 6374 5b27 706f  ERTa_v1_dict['po
+000060f0: 7327 5d2c 2072 6f42 4552 5461 5f76 325f  s'], roBERTa_v2_
+00006100: 6469 6374 5b27 706f 7327 5d2c 2058 4c4d  dict['pos'], XLM
+00006110: 5f72 6f42 4552 5461 5f64 6963 745b 2770  _roBERTa_dict['p
+00006120: 6f73 275d 2c20 6669 6e42 4552 545f 6469  os'], finBERT_di
+00006130: 6374 5b27 706f 7327 5d5d 0d0a 2020 2020  ct['pos']]..    
+00006140: 2020 2020 2020 2020 2020 2020 6e65 6720              neg 
+00006150: 3d20 5b23 616c 7068 6156 4144 4552 5f64  = [#alphaVADER_d
+00006160: 6963 745b 276e 6567 275d 2c20 0d0a 2020  ict['neg'], ..  
+00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006180: 2020 2020 2072 6f42 4552 5461 5f76 315f       roBERTa_v1_
+00006190: 6469 6374 5b27 6e65 6727 5d2c 2072 6f42  dict['neg'], roB
+000061a0: 4552 5461 5f76 325f 6469 6374 5b27 6e65  ERTa_v2_dict['ne
+000061b0: 6727 5d2c 2058 4c4d 5f72 6f42 4552 5461  g'], XLM_roBERTa
+000061c0: 5f64 6963 745b 276e 6567 275d 2c20 6669  _dict['neg'], fi
+000061d0: 6e42 4552 545f 6469 6374 5b27 6e65 6727  nBERT_dict['neg'
+000061e0: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
+000061f0: 2020 2020 6e65 7520 3d20 5b23 616c 7068      neu = [#alph
+00006200: 6156 4144 4552 5f64 6963 745b 276e 6575  aVADER_dict['neu
+00006210: 275d 2c20 0d0a 2020 2020 2020 2020 2020  '], ..          
+00006220: 2020 2020 2020 2020 2020 2020 2072 6f42               roB
+00006230: 4552 5461 5f76 315f 6469 6374 5b27 6e65  ERTa_v1_dict['ne
+00006240: 7527 5d2c 2072 6f42 4552 5461 5f76 325f  u'], roBERTa_v2_
+00006250: 6469 6374 5b27 6e65 7527 5d2c 2058 4c4d  dict['neu'], XLM
+00006260: 5f72 6f42 4552 5461 5f64 6963 745b 276e  _roBERTa_dict['n
+00006270: 6575 275d 2c20 6669 6e42 4552 545f 6469  eu'], finBERT_di
+00006280: 6374 5b27 6e65 7527 5d5d 0d0a 2020 2020  ct['neu']]..    
+00006290: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+000062a0: 6f75 6e64 203d 205b 2361 6c70 6861 5641  ound = [#alphaVA
+000062b0: 4445 525f 6469 6374 5b27 636f 6d70 6f75  DER_dict['compou
+000062c0: 6e64 275d 2c20 0d0a 2020 2020 2020 2020  nd'], ..        
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2020 726f 4245 5254 615f 7631 5f64      roBERTa_v1_d
+000062f0: 6963 745b 2763 6f6d 706f 756e 6427 5d2c  ict['compound'],
+00006300: 2072 6f42 4552 5461 5f76 325f 6469 6374   roBERTa_v2_dict
+00006310: 5b27 636f 6d70 6f75 6e64 275d 2c20 584c  ['compound'], XL
+00006320: 4d5f 726f 4245 5254 615f 6469 6374 5b27  M_roBERTa_dict['
+00006330: 636f 6d70 6f75 6e64 275d 2c20 6669 6e42  compound'], finB
+00006340: 4552 545f 6469 6374 5b27 636f 6d70 6f75  ERT_dict['compou
+00006350: 6e64 275d 5d0d 0a0d 0a20 2020 2020 2020  nd']]....       
+00006360: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006370: 7b23 2761 6c70 6861 5641 4445 5227 3a20  {#'alphaVADER': 
+00006380: 616c 7068 6156 4144 4552 5f64 6963 742c  alphaVADER_dict,
+00006390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000063a0: 2020 2020 2020 2020 2020 2772 6f42 4552            'roBER
+000063b0: 5461 5f76 3127 3a20 726f 4245 5254 615f  Ta_v1': roBERTa_
+000063c0: 7631 5f64 6963 742c 0d0a 2020 2020 2020  v1_dict,..      
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2772 6f42 4552 5461 5f76 3227 3a20    'roBERTa_v2': 
+000063f0: 726f 4245 5254 615f 7632 5f64 6963 742c  roBERTa_v2_dict,
+00006400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006410: 2020 2020 2020 2020 2020 2758 4c4d 5f72            'XLM_r
+00006420: 6f42 4552 5461 273a 2058 4c4d 5f72 6f42  oBERTa': XLM_roB
+00006430: 4552 5461 5f64 6963 742c 0d0a 2020 2020  ERTa_dict,..    
+00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006450: 2020 2020 2766 696e 4245 5254 273a 2066      'finBERT': f
+00006460: 696e 4245 5254 5f64 6963 742c 200d 0a20  inBERT_dict, .. 
+00006470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006480: 2020 2020 2020 2027 746f 7461 6c27 3a20         'total': 
+00006490: 7b27 6e65 6727 3a20 726f 756e 6428 6e70  {'neg': round(np
+000064a0: 2e6d 6561 6e28 6e65 6729 2c35 292c 200d  .mean(neg),5), .
+000064b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 2020 2020 2020 2020 2020 276e 6575              'neu
-000064e0: 273a 2072 6f75 6e64 286e 702e 6d65 616e  ': round(np.mean
-000064f0: 286e 6575 292c 3529 2c20 0d0a 2020 2020  (neu),5), ..    
+000064d0: 2020 2027 6e65 7527 3a20 726f 756e 6428     'neu': round(
+000064e0: 6e70 2e6d 6561 6e28 6e65 7529 2c35 292c  np.mean(neu),5),
+000064f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
 00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-00006520: 6f73 273a 2072 6f75 6e64 286e 702e 6d65  os': round(np.me
-00006530: 616e 2870 6f73 292c 3529 2c20 0d0a 2020  an(pos),5), ..  
+00006510: 2020 2020 2027 706f 7327 3a20 726f 756e       'pos': roun
+00006520: 6428 6e70 2e6d 6561 6e28 706f 7329 2c35  d(np.mean(pos),5
+00006530: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
 00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006560: 2763 6f6d 706f 756e 6427 3a20 726f 756e  'compound': roun
-00006570: 6428 6e70 2e6d 6561 6e28 636f 6d70 6f75  d(np.mean(compou
-00006580: 6e64 292c 3529 7d7d 200d 0a20 2020 2020  nd),5)}} ..     
-00006590: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
-000065a0: 7574 6545 7272 6f72 3a20 0d0a 2020 2020  uteError: ..    
-000065b0: 2020 2020 2020 2020 7261 6973 6520 5379          raise Sy
-000065c0: 7374 656d 4572 726f 7228 2241 6c6c 206d  stemError("All m
-000065d0: 6f64 656c 7320 6d75 7374 2062 6520 6c6f  odels must be lo
-000065e0: 6164 6564 2069 6e20 7072 696f 722e 204c  aded in prior. L
-000065f0: 6f61 6420 7468 6520 6d6f 6465 6c73 2076  oad the models v
-00006600: 6961 206e 6c70 2e73 656e 7469 6d65 6e74  ia nlp.sentiment
-00006610: 286c 6f61 645f 6d6f 6465 6c73 3d27 616c  (load_models='al
-00006620: 6c27 2922 290d 0a                        l')")..
+00006550: 2020 2020 2020 2027 636f 6d70 6f75 6e64         'compound
+00006560: 273a 2072 6f75 6e64 286e 702e 6d65 616e  ': round(np.mean
+00006570: 2863 6f6d 706f 756e 6429 2c35 297d 7d20  (compound),5)}} 
+00006580: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00006590: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
+000065a0: 200d 0a20 2020 2020 2020 2020 2020 2072   ..            r
+000065b0: 6169 7365 2053 7973 7465 6d45 7272 6f72  aise SystemError
+000065c0: 2822 416c 6c20 6d6f 6465 6c73 206d 7573  ("All models mus
+000065d0: 7420 6265 206c 6f61 6465 6420 696e 2070  t be loaded in p
+000065e0: 7269 6f72 2e20 4c6f 6164 2074 6865 206d  rior. Load the m
+000065f0: 6f64 656c 7320 7669 6120 6e6c 702e 7365  odels via nlp.se
+00006600: 6e74 696d 656e 7428 6c6f 6164 5f6d 6f64  ntiment(load_mod
+00006610: 656c 733d 2761 6c6c 2729 2229 0d0a       els='all')")..
```

### Comparing `conlp-0.0.4/setup.py` & `conlp-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup 
 
 setup(
   name = 'conlp',
   packages = ['conlp'],
-  version = '0.0.4',
+  version = '0.0.5',
   license='Apache-2.0',
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',
   author_email = 'nick.sh.oh@socialscience.ai',    
   url = 'https://github.com/SOCIALSCIENCEai/coNLP',  
-  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.4.tar.gz',
+  download_url = 'https://github.com/SOCIALSCIENCEai/coNLP/archive/refs/tags/0.0.5.tar.gz',
   keywords = ['NLP', 'SOCIAL SCIENCE'],   
   install_requires=[           
           'torch',
           'transformers',
           'transformers[sentencepiece]',
           'scipy',
           'numpy',
```

