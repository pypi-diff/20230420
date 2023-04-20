# Comparing `tmp/gpt2ppl-zh-0.2.0.tar.gz` & `tmp/gpt2ppl-zh-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt2ppl-zh-0.2.0.tar", last modified: Mon Mar 27 08:58:18 2023, max compression
+gzip compressed data, was "gpt2ppl-zh-0.3.0.tar", last modified: Thu Apr 20 02:10:54 2023, max compression
```

## Comparing `gpt2ppl-zh-0.2.0.tar` & `gpt2ppl-zh-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-03-27 08:58:18.251854 gpt2ppl-zh-0.2.0/
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4584 2023-03-27 08:58:18.250854 gpt2ppl-zh-0.2.0/PKG-INFO
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4321 2023-03-27 08:28:11.000000 gpt2ppl-zh-0.2.0/README.rst
-drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-03-27 08:58:18.250854 gpt2ppl-zh-0.2.0/gpt2ppl/
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       51 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.2.0/gpt2ppl/__init__.py
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     3385 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.2.0/gpt2ppl/demo_doc.py
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      607 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.2.0/gpt2ppl/demo_sent.py
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4852 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.2.0/gpt2ppl/gpt2ppl.py
-drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-03-27 08:58:18.250854 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4584 2023-03-27 08:58:18.000000 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/PKG-INFO
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      268 2023-03-27 08:58:18.000000 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/SOURCES.txt
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)        1 2023-03-27 08:58:18.000000 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/dependency_links.txt
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       19 2023-03-27 08:58:18.000000 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/requires.txt
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)        8 2023-03-27 08:58:18.000000 gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/top_level.txt
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       38 2023-03-27 08:58:18.251854 gpt2ppl-zh-0.2.0/setup.cfg
--rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      730 2023-03-27 08:28:56.000000 gpt2ppl-zh-0.2.0/setup.py
+drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-04-20 02:10:54.900133 gpt2ppl-zh-0.3.0/
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4584 2023-04-20 02:10:54.899133 gpt2ppl-zh-0.3.0/PKG-INFO
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4321 2023-03-27 08:28:11.000000 gpt2ppl-zh-0.3.0/README.rst
+drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-04-20 02:10:54.898133 gpt2ppl-zh-0.3.0/gpt2ppl/
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       51 2023-04-20 02:02:32.000000 gpt2ppl-zh-0.3.0/gpt2ppl/__init__.py
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     3385 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.3.0/gpt2ppl/demo_doc.py
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      607 2023-03-27 08:25:44.000000 gpt2ppl-zh-0.3.0/gpt2ppl/demo_sent.py
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     5096 2023-04-20 01:55:58.000000 gpt2ppl-zh-0.3.0/gpt2ppl/gpt2ppl.py
+drwxrwxr-x   0 wangzejun  (1008) wangzejun  (1009)        0 2023-04-20 02:10:54.899133 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)     4584 2023-04-20 02:10:54.000000 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/PKG-INFO
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      268 2023-04-20 02:10:54.000000 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)        1 2023-04-20 02:10:54.000000 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       19 2023-04-20 02:10:54.000000 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/requires.txt
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)        8 2023-04-20 02:10:54.000000 gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/top_level.txt
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)       38 2023-04-20 02:10:54.900133 gpt2ppl-zh-0.3.0/setup.cfg
+-rw-rw-r--   0 wangzejun  (1008) wangzejun  (1009)      730 2023-04-20 02:02:18.000000 gpt2ppl-zh-0.3.0/setup.py
```

### Comparing `gpt2ppl-zh-0.2.0/PKG-INFO` & `gpt2ppl-zh-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt2ppl-zh
-Version: 0.2.0
+Version: 0.3.0
 Summary: Chinese sentence perplexity calculation based on GPT2 pre-trained model
 Home-page: https://github.com/zejunwang1/gpt2ppl-zh
 Author: wangzejun
 Author-email: wangzejunscut@126.com
 License: MIT License
 
 gpt2ppl-zh: 基于中文 GPT2 预训练模型的语句困惑度计算
```

### Comparing `gpt2ppl-zh-0.2.0/README.rst` & `gpt2ppl-zh-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gpt2ppl-zh-0.2.0/gpt2ppl/demo_doc.py` & `gpt2ppl-zh-0.3.0/gpt2ppl/demo_doc.py`

 * *Files identical despite different names*

### Comparing `gpt2ppl-zh-0.2.0/gpt2ppl/demo_sent.py` & `gpt2ppl-zh-0.3.0/gpt2ppl/demo_sent.py`

 * *Files identical despite different names*

### Comparing `gpt2ppl-zh-0.2.0/gpt2ppl/gpt2ppl.py` & `gpt2ppl-zh-0.3.0/gpt2ppl/gpt2ppl.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 def Chinese_chars_num(text):
     count = 0
     for c in text:
         if is_Chinese(c):
             count += 1
     return count
 
-def split_sentence(text, min_length=8, max_length=510, return_loc=False):
+def split_sentence(text, min_length=8, max_length=512, return_loc=False):
     pos_list = []
     sentence_list = []
     lines = text.split("\n")
     pos = 0
     for line in lines:
         if not line.rstrip():
             pos += len(line)
             pos += 1
             continue
-        line = re.sub("([。！？!?…])(.)", r"\1\n\2", line)
+
+        line = re.sub("([。！？；!?;])([^”’])", r"\1\n\2", line)
+        line = re.sub("([。！？；!?;][”’])(.)", r"\1\n\2", line)
         line = line.split("\n")
+
         begin = 0
         end = len(line)
         while begin < end:
             sentence = line[begin]
             if len(sentence) < min_length:
                 while len(sentence) < min_length and begin < end - 1:
                     begin += 1
@@ -49,15 +52,15 @@
                     sentence = sentence[max_length:]
                     pos += max_length
                 if len(sentence) < min_length:
                     sentence_list[len(sentence_list) - 1] += sentence
                 else:
                     pos_list.append(pos)
                     sentence_list.append(sentence)
-                    pos += len(sentence)
+                pos += len(sentence)
             else:
                 pos_list.append(pos)
                 sentence_list.append(sentence)
                 pos += len(sentence)
             begin += 1
         pos += 1
 
@@ -71,56 +74,62 @@
         tokenizer_mode="bert",
         device="cuda",
         stride=512
     ):
         assert device in ["cuda", "cpu"]
         self.model = GPT2LMHeadModel.from_pretrained(model_name_or_path).to(device)
         
+        assert tokenizer_mode in ["bert", "gpt2"]
         if tokenizer_mode == "bert":
             self.tokenizer = BertTokenizerFast.from_pretrained(model_name_or_path)
         else:
             self.tokenizer = GPT2TokenizerFast.from_pretrained(model_name_or_path)
         
         self.device = device
         self.stride = stride
         self.max_positions = self.model.config.n_positions
     
     def get_ppl(self, text):
-        encodings = self.tokenizer(text.strip(), add_special_tokens=False, return_tensors="pt")
+        encodings = self.tokenizer(
+            text, 
+            add_special_tokens=False, 
+            return_token_type_ids=False,
+            return_attention_mask=False,
+            return_tensors="pt"
+        )
         seq_len = encodings.input_ids.size(1)
         
         nlls = []
         prev_end_loc = 0
         for begin_loc in range(0, seq_len, self.stride):
             end_loc = min(begin_loc + self.max_positions, seq_len)
             trg_len = end_loc - prev_end_loc  # may be different from stride on last loop
             input_ids = encodings.input_ids[:, begin_loc:end_loc].to(self.device)
             target_ids = input_ids.clone()
             target_ids[:, :-trg_len] = -100
             
             with torch.no_grad():
                 outputs = self.model(input_ids, labels=target_ids)
-
+                
                 # loss is calculated using CrossEntropyLoss which averages over input tokens.
                 # Multiply it with trg_len to get the summation instead of average.
                 # We will take average over all the tokens to get the true average
                 # in the last step of this example.
                 neg_log_likelihood = outputs.loss * trg_len
             
             nlls.append(neg_log_likelihood)
 
             prev_end_loc = end_loc
             if end_loc == seq_len:
                 break
 
-        ppl = torch.exp(torch.stack(nlls).sum() / end_loc)
-        ppl = ppl.cpu().tolist()
+        ppl = torch.exp(torch.stack(nlls).sum() / end_loc).tolist()
         return ppl
         
-    def get_ppl_per_sentence(self, text, ratio=0.4, min_length=8, max_length=510, return_loc=False):
+    def get_ppl_per_sentence(self, text, ratio=0.4, min_length=8, max_length=512, return_loc=False):
         outputs = split_sentence(text, min_length, max_length, return_loc)
         sentence_list = outputs
         if return_loc:
             pos_list, sentence_list = outputs
         
         ppl_list = []
         for i in range(len(sentence_list)):
```

### Comparing `gpt2ppl-zh-0.2.0/gpt2ppl_zh.egg-info/PKG-INFO` & `gpt2ppl-zh-0.3.0/gpt2ppl_zh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt2ppl-zh
-Version: 0.2.0
+Version: 0.3.0
 Summary: Chinese sentence perplexity calculation based on GPT2 pre-trained model
 Home-page: https://github.com/zejunwang1/gpt2ppl-zh
 Author: wangzejun
 Author-email: wangzejunscut@126.com
 License: MIT License
 
 gpt2ppl-zh: 基于中文 GPT2 预训练模型的语句困惑度计算
```

### Comparing `gpt2ppl-zh-0.2.0/setup.py` & `gpt2ppl-zh-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     with io.open("README.rst", encoding='utf-8') as fid:
         return fid.read()
 
 
 setup(
     name='gpt2ppl-zh',
-    version='0.2.0',
+    version='0.3.0',
     author='wangzejun',
     author_email='wangzejunscut@126.com',
     description='Chinese sentence perplexity calculation based on GPT2 pre-trained model',
     long_description=_get_readme(),
     license='MIT License',
     url='https://github.com/zejunwang1/gpt2ppl-zh',
     install_requires=['transformers', 'torch'],
```

