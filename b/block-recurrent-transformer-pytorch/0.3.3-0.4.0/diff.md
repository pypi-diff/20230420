# Comparing `tmp/block-recurrent-transformer-pytorch-0.3.3.tar.gz` & `tmp/block-recurrent-transformer-pytorch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "block-recurrent-transformer-pytorch-0.3.3.tar", last modified: Tue Apr 18 18:18:17 2023, max compression
+gzip compressed data, was "block-recurrent-transformer-pytorch-0.4.0.tar", last modified: Thu Apr 20 20:38:08 2023, max compression
```

## Comparing `block-recurrent-transformer-pytorch-0.3.3.tar` & `block-recurrent-transformer-pytorch-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.827175 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 18:18:17.000000 block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:18:17.831175 block-recurrent-transformer-pytorch-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-18 18:17:56.000000 block-recurrent-transformer-pytorch-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.291942 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37124 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:38:08.291942 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 20:38:08.000000 block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 20:38:08.295941 block-recurrent-transformer-pytorch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-20 20:37:56.000000 block-recurrent-transformer-pytorch-0.4.0/setup.py
```

### Comparing `block-recurrent-transformer-pytorch-0.3.3/LICENSE` & `block-recurrent-transformer-pytorch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `block-recurrent-transformer-pytorch-0.3.3/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.3
+Version: 0.4.0
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.3/README.md` & `block-recurrent-transformer-pytorch-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     depth = 6,                      # depth
     dim_head = 64,                  # attention head dimensions
     heads = 8,                      # number of attention heads
     max_seq_len = 1024,             # the total receptive field of the transformer, in the paper this was 2 * block size
     block_width = 512,              # block size - total receptive field is max_seq_len, 2 * block size in paper. the block furthest forwards becomes the new cached xl memories, which is a block size of 1 (please open an issue if i am wrong)
     num_state_vectors = 512,        # number of state vectors, i believe this was a single block size in the paper, but can be any amount
     recurrent_layers = (4,),        # where to place the recurrent layer(s) for states with fixed simple gating
+    use_compressed_mem = False,     # whether to use compressed memories of a single block width, from https://arxiv.org/abs/1911.05507
+    compressed_mem_factor = 4,      # compression factor of compressed memories
     use_flash_attn = True           # use flash attention, if on pytorch 2.0
 )
 
 seq = torch.randint(0, 2000, (1, 1024))
 
 out, mems1, states1 = model(seq)
 out, mems2, states2 = model(seq, xl_memories = mems1, states = states1)
@@ -61,18 +63,18 @@
 - [x] take care of generation with recurrence in `RecurrentTrainWrapper`
 - [x] add ability to dropout to entire memories and states during each segment step during trainng
 - [x] test full system on enwik8 locally and ablate states and memories and see effects first  hand
 - [x] make sure attention allow for single head key / values too
 - [x] run a few experiments of fixed gating in regular transformers - does not work
 - [x] integrate <a href="https://github.com/hazyresearch/flash-attention">flash attention</a>
 - [x] cache attention mask + rotary embeddings
+- [x] add <a href="https://github.com/lucidrains/compressive-transformer-pytorch">compressed memories</a>
 
 - [ ] revisit <a href="https://github.com/lucidrains/memformer">memformer</a>
 - [ ] add ability to gate in memorizing transformers knn attention layers
-- [ ] add <a href="https://github.com/lucidrains/compressive-transformer-pytorch">compressed memories</a>
 
 ## Citations
 
 ```bibtex
 @article{Hutchins2022BlockRecurrentT,
     title   = {Block-Recurrent Transformers},
     author  = {DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam Neyshabur},
```

#### html2text {}

```diff
@@ -12,38 +12,40 @@
 = 8, # number of attention heads max_seq_len = 1024, # the total receptive
 field of the transformer, in the paper this was 2 * block size block_width =
 512, # block size - total receptive field is max_seq_len, 2 * block size in
 paper. the block furthest forwards becomes the new cached xl memories, which is
 a block size of 1 (please open an issue if i am wrong) num_state_vectors = 512,
 # number of state vectors, i believe this was a single block size in the paper,
 but can be any amount recurrent_layers = (4,), # where to place the recurrent
-layer(s) for states with fixed simple gating use_flash_attn = True # use flash
-attention, if on pytorch 2.0 ) seq = torch.randint(0, 2000, (1, 1024)) out,
-mems1, states1 = model(seq) out, mems2, states2 = model(seq, xl_memories =
-mems1, states = states1) out, mems3, states3 = model(seq, xl_memories = mems2,
-states = states2) ``` ## Test on Enwik8 First `pip install -
-r requirements.txt`, then ```bash $ python train.py ``` ## Todo - [x] use
-dynamic positional bias - [x] add enhanced recurrence - [x] setup local
-attention blocks, as in the paper - [x] wrapper transformer class for training
-- [x] take care of generation with recurrence in `RecurrentTrainWrapper` - [x]
-add ability to dropout to entire memories and states during each segment step
-during trainng - [x] test full system on enwik8 locally and ablate states and
-memories and see effects first hand - [x] make sure attention allow for single
-head key / values too - [x] run a few experiments of fixed gating in regular
-transformers - does not work - [x] integrate flash_attention - [x] cache
-attention mask + rotary embeddings - [ ] revisit memformer - [ ] add ability to
-gate in memorizing transformers knn attention layers - [ ] add compressed
-memories ## Citations ```bibtex @article{Hutchins2022BlockRecurrentT, title =
-{Block-Recurrent Transformers}, author = {DeLesley S. Hutchins and Imanol
-Schlag and Yuhuai Wu and Ethan Dyer and Behnam Neyshabur}, journal = {ArXiv},
-year = {2022}, volume = {abs/2203.07852} } ``` ```bibtex @article
-{Shazeer2019FastTD, title = {Fast Transformer Decoding: One Write-Head is All
-You Need}, author = {Noam M. Shazeer}, journal = {ArXiv}, year = {2019}, volume
-= {abs/1911.02150} } ``` ```bibtex @inproceedings{Sun2022ALT, title = {A
-Length-Extrapolatable Transformer}, author = {Yutao Sun and Li Dong and Barun
-Patra and Shuming Ma and Shaohan Huang and Alon Benhaim and Vishrav Chaudhary
-and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex @inproceedings
-{dao2022flashattention, title = {Flash{A}ttention: Fast and Memory-Efficient
-Exact Attention with {IO}-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and
-Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher}, booktitle = {Advances
-in Neural Information Processing Systems}, year = {2022} } ``` *Memory is
-Attention through Time* - Alex Graves
+layer(s) for states with fixed simple gating use_compressed_mem = False, #
+whether to use compressed memories of a single block width, from https://
+arxiv.org/abs/1911.05507 compressed_mem_factor = 4, # compression factor of
+compressed memories use_flash_attn = True # use flash attention, if on pytorch
+2.0 ) seq = torch.randint(0, 2000, (1, 1024)) out, mems1, states1 = model(seq)
+out, mems2, states2 = model(seq, xl_memories = mems1, states = states1) out,
+mems3, states3 = model(seq, xl_memories = mems2, states = states2) ``` ## Test
+on Enwik8 First `pip install -r requirements.txt`, then ```bash $ python
+train.py ``` ## Todo - [x] use dynamic positional bias - [x] add enhanced
+recurrence - [x] setup local attention blocks, as in the paper - [x] wrapper
+transformer class for training - [x] take care of generation with recurrence in
+`RecurrentTrainWrapper` - [x] add ability to dropout to entire memories and
+states during each segment step during trainng - [x] test full system on enwik8
+locally and ablate states and memories and see effects first hand - [x] make
+sure attention allow for single head key / values too - [x] run a few
+experiments of fixed gating in regular transformers - does not work - [x]
+integrate flash_attention - [x] cache attention mask + rotary embeddings - [x]
+add compressed_memories - [ ] revisit memformer - [ ] add ability to gate in
+memorizing transformers knn attention layers ## Citations ```bibtex @article
+{Hutchins2022BlockRecurrentT, title = {Block-Recurrent Transformers}, author =
+{DeLesley S. Hutchins and Imanol Schlag and Yuhuai Wu and Ethan Dyer and Behnam
+Neyshabur}, journal = {ArXiv}, year = {2022}, volume = {abs/2203.07852} } ```
+```bibtex @article{Shazeer2019FastTD, title = {Fast Transformer Decoding: One
+Write-Head is All You Need}, author = {Noam M. Shazeer}, journal = {ArXiv},
+year = {2019}, volume = {abs/1911.02150} } ``` ```bibtex @inproceedings
+{Sun2022ALT, title = {A Length-Extrapolatable Transformer}, author = {Yutao Sun
+and Li Dong and Barun Patra and Shuming Ma and Shaohan Huang and Alon Benhaim
+and Vishrav Chaudhary and Xia Song and Furu Wei}, year = {2022} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ``` *Memory is Attention through Time* - Alex Graves
```

### Comparing `block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py` & `block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch/block_recurrent_transformer_pytorch.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import math
 from random import random
 from functools import wraps, partial
+from itertools import zip_longest
 from collections import namedtuple, defaultdict
 from packaging import version
 
-from einops import rearrange
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, repeat, pack, unpack
+from einops.layers.torch import Rearrange
 
 from beartype import beartype
 from beartype.door import is_bearable
 from beartype.typing import Optional, List, Tuple
 
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
+def is_empty(t: torch.Tensor):
+    return t.numel() == 0
+
+def cast_tuple(t, length = 1):
+    return t if isinstance(t, tuple) else ((t,) * length)
+
 def all_unique(arr):
     return len(arr) == len(set(arr))
 
 def eval_decorator(fn):
     def inner(self, *args, **kwargs):
         was_training = self.training
         self.eval()
@@ -43,26 +50,34 @@
         nonlocal called
         if called:
             return
         called = True
         return fn(x)
     return inner
 
+print_once = once(print)
+
 def compact(arr):
     return [*filter(exists, arr)]
 
 def and_reduce(arr: List[torch.Tensor]):
     if len(arr) == 0:
         return None
     head, *rest = arr
     for t in rest:
         head = head & t
     return head
 
-print_once = once(print)
+def safe_cat(*args, dim = 1):
+    args = compact(args)
+
+    if len(args) == 0:
+        return None
+
+    return torch.cat(args, dim = dim)
 
 def divisible_by(numer, denom):
     return (numer % denom) == 0
 
 def l2norm(t):
     return F.normalize(t, dim = -1)
 
@@ -111,34 +126,37 @@
 # https://arxiv.org/abs/2104.09864
 # https://arxiv.org/abs/2212.10554v1
 
 class RotaryEmbedding(nn.Module):
     def __init__(
         self,
         dim,
+        width,
         scale_base = 512,
         theta = 10000
     ):
         super().__init__()
+        self.width = width
+
         inv_freq = 1.0 / (theta ** (torch.arange(0, dim, 2).float() / dim))
         self.register_buffer("inv_freq", inv_freq, persistent = False)
 
         self.scale_base = scale_base
         scale = (torch.arange(0, dim, 2) + 0.4 * dim) / (1.4 * dim)
         self.register_buffer('scale', scale, persistent = False)
 
         self.register_buffer('cached_freqs', None, persistent = False)
         self.register_buffer('cached_scales', None, persistent = False)
 
     @property
     def device(self):
         return next(self.buffers()).device
 
-    def forward(self, seq_len):
-        device = self.device
+    def forward(self):
+        device, seq_len = self.device, self.width
 
         if exists(self.cached_freqs):
             cached_seq_len = self.cached_freqs.shape[-2]
             if cached_seq_len >= seq_len:
                 return self.cached_freqs[:seq_len], self.cached_scales[:seq_len]
 
         t = torch.arange(seq_len, device = device).type_as(self.inv_freq)
@@ -169,14 +187,115 @@
 
     if isinstance(scale, torch.Tensor):
         assert scale.shape[-2] >= seq_len
         scale = scale[-seq_len:]
 
     return (t * pos.cos() * scale) + (rotate_half(t) * pos.sin() * scale)
 
+# memory management
+
+class MemoryManager(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        layers = 1,
+        mem_lengths = 512,
+        compress_factors = 1
+    ):
+        super().__init__()
+        mem_lengths = cast_tuple(mem_lengths)
+        compress_factors = cast_tuple(compress_factors)
+
+        assert all([mem_length > 0 for mem_length in mem_lengths])
+        assert len(mem_lengths) == len(compress_factors)
+        assert layers >= 1
+
+        self.mem_lengths = mem_lengths
+        self.compress_factors = compress_factors
+
+        self.layers = nn.ModuleList([])
+
+        for _ in range(layers):
+            compress_fns = nn.ModuleList([])
+
+            for compress_factor in compress_factors:
+                compress_fn = nn.Identity()
+                if compress_factor > 1:
+                    compress_fn = nn.Sequential(
+                        Rearrange('b n d -> b d n'),
+                        nn.Conv1d(
+                            dim * 2,
+                            dim * 2,
+                            compress_factor,
+                            stride = compress_factor,
+                            groups = 2
+                        ),
+                        Rearrange('b d n -> b n d'),
+                    )
+
+                compress_fns.append(compress_fn)
+
+            self.layers.append(compress_fns)
+
+    def forward(
+        self,
+        past_memories: List[torch.Tensor],
+        new_memories: List[torch.Tensor]
+    ):
+        next_memories = []
+
+        for past_memory, new_memory, compress_fns in zip_longest(past_memories, new_memories, self.layers):
+
+            # edge case if neither memories exist
+
+            if not (exists(past_memory) or exists(new_memory)):
+                next_memories.append(None)
+                continue
+
+            next_memory = None
+
+            for mem_length, compress_factor, compress_fn in zip(self.mem_lengths, self.compress_factors, compress_fns):
+
+                # first get the memories for the given compression factor "current_memory"
+
+                current_memory = None
+                if exists(past_memory):
+                    past_memory, current_memory = past_memory[..., :-mem_length, :], past_memory[..., -mem_length:, :]
+
+                # compress the new memories coming in, based on the compression factors set at init
+
+                if (not is_empty(new_memory)) and compress_factor > 1:
+                    # make sure memory length is divisible by compression factor
+
+                    new_mem_length = new_memory.shape[-2]
+                    curtailed_length = (new_mem_length // compress_factor) * compress_factor
+                    new_memory = new_memory[..., -curtailed_length:, :]
+
+                    # compress the memory pushed to the next stage
+
+                    new_memory = rearrange(new_memory, 'm b n d -> b n (m d)')
+                    new_memory = compress_fn(new_memory)
+                    new_memory = rearrange(new_memory, 'b n (m d) -> m b n d', m = 2)
+
+                # fifo memory queue
+                # add the new memory on the right
+
+                current_memory = safe_cat(current_memory, new_memory, dim = -2)
+                # "new" memory is new with respect to the next compressed segment
+
+                new_memory, current_memory = current_memory[..., :-mem_length, :], current_memory[..., -mem_length:, :]
+                # concat the new memory to the left into the past
+
+                next_memory = safe_cat(current_memory, next_memory, dim = -2)
+
+            next_memories.append(next_memory)
+
+        return next_memories
+
 # maybe flash attention, if using pytorch 2.0
 
 # constants
 
 Config = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 # state container
@@ -610,15 +729,16 @@
             past_k, past_v = xl_memories
             k = torch.cat((past_k, k), dim = 1)
             v = torch.cat((past_v, v), dim = 1)
 
         # handle cropping of attention mask and positional embeddings
 
         if exists(attn_mask):
-            attn_mask = attn_mask[:seq_len, (width - mem_len):(width + seq_len)]
+            attn_mask = attn_mask[:seq_len, :seq_len]
+            attn_mask = F.pad(attn_mask, (mem_len, 0), value = True)
 
         # attention, but of course
 
         out = self.attn(
             q, k, v,
             rotary_pos_emb = rotary_pos_emb,
             xpos_scale = xpos_scale,
@@ -673,15 +793,17 @@
         ff_mult = 4,
         max_seq_len = 1024,
         block_width = 512,
         recurrent_layers: Optional[Tuple[int, ...]] = None,
         read_recurrent_layers: Optional[Tuple[int, ...]] = None,
         num_state_vectors = None,
         ignore_index = -100,
-        use_flash_attn = False
+        use_flash_attn = False,
+        use_compressed_mem = False,
+        compressed_mem_factor = 4
     ):
         super().__init__()
         num_state_vectors = default(num_state_vectors, block_width)
 
         # set recurrent layers
 
         recurrent_layers = default(recurrent_layers, (depth // 2,)) # default to one recurent layer at middle of the network
@@ -701,15 +823,15 @@
 
         self.read_recurrent_layers = read_recurrent_layers
 
         # token embedding
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
-        self.rotary_pos_emb = RotaryEmbedding(dim = dim_head)
+        self.rotary_pos_emb = RotaryEmbedding(dim = dim_head, width = (2 if not use_compressed_mem else 3) * block_width)
 
         self.layers = nn.ModuleList([])
 
         self.write_to_read_map = {write_layer: read_layer for write_layer, read_layer in zip(recurrent_layers, read_recurrent_layers)}
 
         self.read_state_router = defaultdict(list)
 
@@ -746,14 +868,23 @@
                 self.read_state_router[read_layer].append(attn_block.state_container)
 
             self.layers.append(nn.ModuleList([
                 attn_block,
                 ff_block
             ]))
 
+        # (compressed) memory management
+
+        self.mem_manager = MemoryManager(
+            dim = dim_head,
+            layers = depth,
+            mem_lengths = block_width if not use_compressed_mem else (block_width, block_width // 2),
+            compress_factors = 1 if not use_compressed_mem else (1, compressed_mem_factor)
+        )
+
         # to logits
 
         self.to_logits = nn.Sequential(
             LayerNorm(dim),
             nn.Linear(dim, num_tokens, bias = False)
         )
 
@@ -775,24 +906,16 @@
             cached_mask = self.cached_causal_attn_mask
             cached_width = cached_mask.shape[-2]
             padding = (width - cached_width) // 2
             j_slice = Ellipsis if padding == 0 else slice(padding, -padding)
             return cached_mask[:cached_width, j_slice]
 
         device = self.device
-        causal_mask = torch.ones((width, 2 * width), device = device, dtype = torch.bool).tril(width)
-
-        i_arange = torch.arange(width, device = device)
-        j_arange = torch.arange(width * 2, device = device)
-        rel_pos = ((rearrange(i_arange, 'i -> i 1') + width) - rearrange(j_arange, 'j -> 1 j')).abs()
-        exact_lookback_attn_mask = rel_pos < width  # make sure each token only looks back a block width
-
-        mask = causal_mask & exact_lookback_attn_mask
-        self.register_buffer('cached_causal_attn_mask', mask, persistent = False)
-        return mask
+        causal_mask = torch.ones((width, width), device = device, dtype = torch.bool).triu(1)
+        return ~causal_mask
 
     @torch.no_grad()
     @eval_decorator
     def generate(
         self,
         prime,
         length = None,
@@ -863,15 +986,15 @@
         # token embedding
 
         x = self.token_emb(x)
 
         # dynamic pos bias
 
         attn_mask = self.get_causal_attn_mask(w)
-        rotary_pos_emb, xpos_scale = self.rotary_pos_emb(2 * w)
+        rotary_pos_emb, xpos_scale = self.rotary_pos_emb()
 
         # only return memories and state if at the full block width, but can be overridden
 
         return_memories_and_states = default(return_memories_and_states, self.max_seq_len == x.shape[-2])
 
         # ready output tensor, to be concatted to block by block
 
@@ -882,30 +1005,31 @@
         # split input into blocks of width w
 
         input_blocks = x.split(w, dim = -2)
 
         # process each block at a time
 
         for input_block in input_blocks:
+            input_block_length = input_block.shape[-2]
 
             # ready xl memories and states
 
-            xl_memories = iter(xl_memories)
-            states = iter(states)
+            iter_xl_memories = iter(xl_memories)
+            iter_states = iter(states)
 
             next_xl_memories = []
             next_states = []
 
             # set the states on the appropriate state containers
 
             for attn, _ in self.layers:
                 if not attn.is_recurrent_layer:
                     continue
 
-                attn.state_container.set_next_read_state(next(states, None))
+                attn.state_container.set_next_read_state(next(iter_states, None))
 
             # go through layers
 
             for ind, (attn, ff) in enumerate(self.layers):
 
                 # determine if the layer requires transformer xl memories
 
@@ -913,15 +1037,15 @@
 
                 # whether to pass in xl memories
 
                 attn_kwargs = dict(
                     rotary_pos_emb = rotary_pos_emb,
                     xpos_scale = xpos_scale,
                     attn_mask = attn_mask,
-                    xl_memories = next(xl_memories, None),
+                    xl_memories = next(iter_xl_memories, None),
                     read_from_state_containers = self.read_state_router[layer]
                 )
 
                 # attention layer
 
                 residual = input_block
                 attn_branch_out, layer_xl_memories, layer_next_states = attn(input_block, **attn_kwargs)
@@ -941,15 +1065,18 @@
             # concat to output
 
             out = torch.cat((out, input_block), dim = -2)
 
             # set new xl memories and states
 
             states = next_states
-            xl_memories = next_xl_memories
+
+            if input_block_length == w:
+                xl_memories = self.mem_manager(xl_memories, next_xl_memories)
+
 
         # project to logits
 
         logits = self.to_logits(out)
 
         # detach the states and memories
```

### Comparing `block-recurrent-transformer-pytorch-0.3.3/block_recurrent_transformer_pytorch.egg-info/PKG-INFO` & `block-recurrent-transformer-pytorch-0.4.0/block_recurrent_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: block-recurrent-transformer-pytorch
-Version: 0.3.3
+Version: 0.4.0
 Summary: Block Recurrent Transformer - Pytorch
 Home-page: https://github.com/lucidrains/block-recurrent-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `block-recurrent-transformer-pytorch-0.3.3/setup.py` & `block-recurrent-transformer-pytorch-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'block-recurrent-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.3',
+  version = '0.4.0',
   license='MIT',
   description = 'Block Recurrent Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/block-recurrent-transformer-pytorch',
   keywords = [
```

