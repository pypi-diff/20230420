# Comparing `tmp/CoLT5-attention-0.2.2.tar.gz` & `tmp/CoLT5-attention-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.2.2.tar", last modified: Wed Apr 19 21:53:53 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.3.tar", last modified: Wed Apr 19 22:48:13 2023, max compression
```

## Comparing `CoLT5-attention-0.2.2.tar` & `CoLT5-attention-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.664233 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23750 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 22:48:12.000000 CoLT5-attention-0.2.3/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 22:48:12.999906 CoLT5-attention-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 22:47:56.000000 CoLT5-attention-0.2.3/setup.py
```

### Comparing `CoLT5-attention-0.2.2/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.3/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.2
+Version: 0.2.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.2/LICENSE` & `CoLT5-attention-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.2/PKG-INFO` & `CoLT5-attention-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.2
+Version: 0.2.3
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.2/README.md` & `CoLT5-attention-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 Update: unsure of how the routing normalized scores for the key-values are used. Did some improvising there, <a href="https://github.com/lucidrains/CoLT5-attention/blob/main/colt5_attention/transformer_block.py#L86">scaling the projected values</a>, but if you think you know the answer, please open an issue
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability.ai</a> for the generous sponsorship to work on cutting edge artificial intelligence research
 
+- <a href="https://github.com/arogozhnikov/einops">einops</a> for making my life easy
+
 ## Install
 
 ```bash
 $ pip install colt5-attention
 ```
 
 ## Usage
@@ -117,20 +119,20 @@
 cross_attn_out.shape # (2, 1024, 512) - same as tokens
 ```
 
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
+- [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 - [ ] make flash attention compatible
-- [ ] allow for multi-headed routing (multiple routing tokens), only for key-values
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -2,62 +2,63 @@
 routed efficient attention in the proposed CoLT5 architecture, in Pytorch.
 Besides their use of coordinate descent from this_paper (main algorithm
 originally from Wright_et_al), will also add two other approaches, one based on
 cumulative softmax, the other gumbel sinkhorn (optimal transport). Update:
 unsure of how the routing normalized scores for the key-values are used. Did
 some improvising there, scaling_the_projected_values, but if you think you know
 the answer, please open an issue ## Appreciation - Stability.ai for the
-generous sponsorship to work on cutting edge artificial intelligence research
-## Install ```bash $ pip install colt5-attention ``` ## Usage ```python import
-torch from colt5_attention import ( ConditionalRoutedFeedForward,
-ConditionalRoutedAttention, ConditionalRoutedTransformerBlock ) # mock input,
-say it is 32768 length tokens = torch.randn(2, 32768, 512) mask = torch.ones(2,
-32768).bool() # can handle variable lengthed sequences # feedforward ff =
-ConditionalRoutedFeedForward( dim = 512, light_ff_mult = 0.5, # hidden
-dimension ratio of light branch heavy_ff_mult = 4, # hidden dimension ratio of
-heavy branch num_heavy_tokens = 1024 # heavy branch receives only 1024 routed
-tokens of 32768 ) ff_out = ff(tokens, mask = mask) # (2, 32768, 512) - light
-and heavy branch summed # attention attn = ConditionalRoutedAttention( dim =
-512, light_dim_head = 64, # attention head dimension of light branch
-light_heads = 8, # number of attention heads for light branch light_window_size
-= 128, # local attention receptive field for light heavy_dim_head = 64, #
-attention head dimension of heavy branch heavy_heads = 8, # number of attention
-heads for heavy branch num_heavy_tokens_q = 1024, # heavy branch receives only
-1024 routed tokens of 32768 num_heavy_tokens_kv = 1024 # heavy branch receives
-only 1024 routed tokens of 32768 ) attn_out = attn(tokens, mask = mask) # (2,
-32768, 512) - light and heavy branch summed # both attention and feedforward
-with residual # the complete transformer block # a stack of these would
-constitute the encoder of CoLT5 block = ConditionalRoutedTransformerBlock( dim
-= 512, light_dim_head = 64, light_heads = 8, light_window_size = 128,
-heavy_dim_head = 64, heavy_heads = 8, light_ff_mult = 0.5, heavy_ff_mult = 4,
-num_heavy_ff_tokens = 1024, num_heavy_attn_tokens_q = 1024,
-num_heavy_attn_tokens_kv = 1024, router_type = 'coor_descent' # you have your
-choice of coordinate descent, as in paper - or 'sinkhorn' or 'cum_softmax' )
-block_out = block(tokens, mask = mask) # (2, 32768, 512) ``` Also included a
-variation of the conditionally routed attention for cross attention, to be
-tried with long context memories in a transformer-xl ```python import torch
-from colt5_attention import ConditionalRoutedCrossAttention # mock input, let
-us say it is a transformer of 1024 length attending to 1 million context past
-memories tokens = torch.randn(2, 1024, 512).cuda() tokens_mask = torch.ones(2,
-1024).bool().cuda() memories = torch.randn(2, int(1e6), 512).cuda()
-memories_mask = torch.ones(2, int(1e6)).bool().cuda() # conditionally routed
-cross attention cross_attn = ConditionalRoutedCrossAttention( dim = 512,
-dim_head = 64, heads = 8, num_tokens_q = 512, # only 512 routed from 1024
-num_tokens_kv = 1024, # only 1024 routed from 1 million kv_routing_tokens = 2,
-# say you want 2 routing tokens to route different sets of key / values to the
-queries. 4 attention heads will be allocated to each routed set in this example
-(8 / 2) ).cuda() cross_attn_out = cross_attn( tokens, context = memories, mask
-= tokens_mask, context_mask = memories_mask ) cross_attn_out.shape # (2, 1024,
-512) - same as tokens ``` ## Todo - [x] add the coordinate descent method as
-another router - [x] figure out if it can be done autoregressively and try it
-out - moving to this_repo - [ ] for variable sequence lengths, allow for
-setting k as a function of sequence lengths per sample in batch - [ ] create a
-variant of CoLT5 for high resolution feature maps (image attention) - then try
-out for diffusion - [ ] in the cross attention scenario, support for routing
-token that first queries the source tokens, before retrieving from memories -
-[ ] make flash attention compatible - [ ] allow for multi-headed routing
-(multiple routing tokens), only for key-values ## Citations ```bibtex
-@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
+generous sponsorship to work on cutting edge artificial intelligence research -
+einops for making my life easy ## Install ```bash $ pip install colt5-attention
+``` ## Usage ```python import torch from colt5_attention import
+( ConditionalRoutedFeedForward, ConditionalRoutedAttention,
+ConditionalRoutedTransformerBlock ) # mock input, say it is 32768 length tokens
+= torch.randn(2, 32768, 512) mask = torch.ones(2, 32768).bool() # can handle
+variable lengthed sequences # feedforward ff = ConditionalRoutedFeedForward
+( dim = 512, light_ff_mult = 0.5, # hidden dimension ratio of light branch
+heavy_ff_mult = 4, # hidden dimension ratio of heavy branch num_heavy_tokens =
+1024 # heavy branch receives only 1024 routed tokens of 32768 ) ff_out = ff
+(tokens, mask = mask) # (2, 32768, 512) - light and heavy branch summed #
+attention attn = ConditionalRoutedAttention( dim = 512, light_dim_head = 64, #
+attention head dimension of light branch light_heads = 8, # number of attention
+heads for light branch light_window_size = 128, # local attention receptive
+field for light heavy_dim_head = 64, # attention head dimension of heavy branch
+heavy_heads = 8, # number of attention heads for heavy branch
+num_heavy_tokens_q = 1024, # heavy branch receives only 1024 routed tokens of
+32768 num_heavy_tokens_kv = 1024 # heavy branch receives only 1024 routed
+tokens of 32768 ) attn_out = attn(tokens, mask = mask) # (2, 32768, 512) -
+light and heavy branch summed # both attention and feedforward with residual #
+the complete transformer block # a stack of these would constitute the encoder
+of CoLT5 block = ConditionalRoutedTransformerBlock( dim = 512, light_dim_head =
+64, light_heads = 8, light_window_size = 128, heavy_dim_head = 64, heavy_heads
+= 8, light_ff_mult = 0.5, heavy_ff_mult = 4, num_heavy_ff_tokens = 1024,
+num_heavy_attn_tokens_q = 1024, num_heavy_attn_tokens_kv = 1024, router_type =
+'coor_descent' # you have your choice of coordinate descent, as in paper - or
+'sinkhorn' or 'cum_softmax' ) block_out = block(tokens, mask = mask) # (2,
+32768, 512) ``` Also included a variation of the conditionally routed attention
+for cross attention, to be tried with long context memories in a transformer-xl
+```python import torch from colt5_attention import
+ConditionalRoutedCrossAttention # mock input, let us say it is a transformer of
+1024 length attending to 1 million context past memories tokens = torch.randn
+(2, 1024, 512).cuda() tokens_mask = torch.ones(2, 1024).bool().cuda() memories
+= torch.randn(2, int(1e6), 512).cuda() memories_mask = torch.ones(2, int
+(1e6)).bool().cuda() # conditionally routed cross attention cross_attn =
+ConditionalRoutedCrossAttention( dim = 512, dim_head = 64, heads = 8,
+num_tokens_q = 512, # only 512 routed from 1024 num_tokens_kv = 1024, # only
+1024 routed from 1 million kv_routing_tokens = 2, # say you want 2 routing
+tokens to route different sets of key / values to the queries. 4 attention
+heads will be allocated to each routed set in this example (8 / 2) ).cuda()
+cross_attn_out = cross_attn( tokens, context = memories, mask = tokens_mask,
+context_mask = memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as
+tokens ``` ## Todo - [x] add the coordinate descent method as another router -
+[x] figure out if it can be done autoregressively and try it out - moving to
+this_repo - [x] allow for multi-headed routing (multiple routing tokens), only
+for key-values - [ ] for variable sequence lengths, allow for setting k as a
+function of sequence lengths per sample in batch - [ ] create a variant of
+CoLT5 for high resolution feature maps (image attention) - then try out for
+diffusion - [ ] in the cross attention scenario, support for routing token that
+first queries the source tokens, before retrieving from memories - [ ] make
+flash attention compatible ## Citations ```bibtex @inproceedings
+{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
+Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
+Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
+Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
+Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.2.2/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.3/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.2/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.3/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.2/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.3/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,24 @@
     def forward(
         self,
         x,
         context = None,
         mask = None,
         normalized_scores_kv = None
     ):
+        """
+        einops:
+        b - batch
+        h - heads, or number of heads per route
+        r - routing dimension, for routing different sets of key / values - should be more expressive
+        n - sequence dimension
+        d - head dimension
+        i - input model dimension
+        """
+
         h = self.heads
 
         x = self.norm(x)
 
         if exists(context):
             context = self.norm(context)
 
@@ -472,14 +482,15 @@
 class ConditionalRoutedAttention(nn.Module):
     def __init__(
         self,
         dim,
         *,
         num_heavy_tokens_q,
         num_heavy_tokens_kv,
+        num_routed_kv = 1,
         light_dim_head = 64,
         light_heads = 8,
         light_window_size = 128,        # each token would see ~ 64 tokens either way to left or right
         heavy_dim_head = 64,
         heavy_heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
@@ -511,14 +522,15 @@
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.kv_router = router_klass(
             dim = dim,
+            num_routing_tokens = num_routed_kv,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = heavy_dim_head,
@@ -712,14 +724,15 @@
 class ConditionalRoutedTransformerBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
         num_heavy_attn_tokens_q,
         num_heavy_attn_tokens_kv,
+        num_routed_kv = 1,
         num_heavy_ff_tokens,
         light_dim_head = 64,
         light_heads = 8,
         light_window_size = 128,
         heavy_dim_head = 64,
         heavy_heads = 8,
         light_ff_mult = 0.5,
@@ -744,14 +757,15 @@
             light_dim_head = light_dim_head,
             light_heads = light_heads,
             light_window_size = light_window_size,
             heavy_dim_head = heavy_dim_head,
             heavy_heads = heavy_heads,
             num_heavy_tokens_q = num_heavy_attn_tokens_q,
             num_heavy_tokens_kv = num_heavy_attn_tokens_kv,
+            num_routed_kv = num_routed_kv,
             router_straight_through = router_straight_through,
             router_type = router_type,
             router_kwargs = router_kwargs
         )
 
     def forward(
         self,
```

### Comparing `CoLT5-attention-0.2.2/setup.py` & `CoLT5-attention-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.2.2',
+  version = '0.2.3',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

