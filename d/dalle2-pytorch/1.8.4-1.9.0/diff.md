# Comparing `tmp/dalle2-pytorch-1.8.4.tar.gz` & `tmp/dalle2-pytorch-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalle2-pytorch-1.8.4.tar", last modified: Sat Aug 20 17:56:59 2022, max compression
+gzip compressed data, was "dalle2-pytorch-1.9.0.tar", last modified: Tue Aug 23 15:29:53 2022, max compression
```

## Comparing `dalle2-pytorch-1.8.4.tar` & `dalle2-pytorch-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 17:56:59.677119 dalle2-pytorch-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-20 17:56:59.677119 dalle2-pytorch-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    43961 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 17:56:59.673119 dalle2-pytorch-1.8.4/dalle2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)   120324 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/dalle2_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 17:56:59.673119 dalle2-pytorch-1.8.4/dalle2_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (121)  3194984 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/data/bpe_simple_vocab_16e6.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 17:56:59.677119 dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13714 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/decoder_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/prior_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/simple_image_only_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     6702 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    26497 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/trackers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13228 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/train_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)    26665 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    22061 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/vqgan_vae.py
--rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/dalle2_pytorch/vqgan_vae_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 17:56:59.673119 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-20 17:56:59.000000 dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-20 17:56:59.677119 dalle2-pytorch-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-20 17:56:50.000000 dalle2-pytorch-1.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 15:29:53.710232 dalle2-pytorch-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-23 15:29:53.710232 dalle2-pytorch-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    43961 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 15:29:53.706232 dalle2-pytorch-1.9.0/dalle2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)   121080 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/dalle2_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 15:29:53.706232 dalle2-pytorch-1.9.0/dalle2_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (121)  3194984 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/data/bpe_simple_vocab_16e6.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 15:29:53.710232 dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13714 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/decoder_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/prior_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/simple_image_only_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6702 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26497 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/trackers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13238 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/train_configs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26705 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22061 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/vqgan_vae.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/dalle2_pytorch/vqgan_vae_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 15:29:53.706232 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-23 15:29:53.000000 dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-23 15:29:53.710232 dalle2-pytorch-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-23 15:29:43.000000 dalle2-pytorch-1.9.0/setup.py
```

### Comparing `dalle2-pytorch-1.8.4/LICENSE` & `dalle2-pytorch-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/PKG-INFO` & `dalle2-pytorch-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalle2-pytorch
-Version: 1.8.4
+Version: 1.9.0
 Summary: DALL-E 2
 Home-page: https://github.com/lucidrains/dalle2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dalle2-pytorch-1.8.4/README.md` & `dalle2-pytorch-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/cli.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/cli.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/dalle2_pytorch.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/dalle2_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -974,15 +974,18 @@
 
         self.learned_query = nn.Parameter(torch.randn(dim))
         self.causal_transformer = CausalTransformer(dim = dim, **kwargs)
 
         # dalle1 learned padding strategy
 
         self.max_text_len = max_text_len
-        self.null_text_embed = nn.Parameter(torch.randn(1, max_text_len, dim))
+
+        self.null_text_encodings = nn.Parameter(torch.randn(1, max_text_len, dim))
+        self.null_text_embeds = nn.Parameter(torch.randn(1, num_text_embeds, dim))
+        self.null_image_embed = nn.Parameter(torch.randn(1, dim))
 
         # whether to use self conditioning, Hinton's group's new ddpm technique
 
         self.self_cond = self_cond
 
     def forward_with_cond_scale(
         self,
@@ -991,26 +994,27 @@
         **kwargs
     ):
         logits = self.forward(*args, **kwargs)
 
         if cond_scale == 1:
             return logits
 
-        null_logits = self.forward(*args, cond_drop_prob = 1., **kwargs)
+        null_logits = self.forward(*args, text_cond_drop_prob = 1., image_cond_drop_prob = 1, **kwargs)
         return null_logits + (logits - null_logits) * cond_scale
 
     def forward(
         self,
         image_embed,
         diffusion_timesteps,
         *,
         text_embed,
         text_encodings = None,
         self_cond = None,
-        cond_drop_prob = 0.
+        text_cond_drop_prob = 0.,
+        image_cond_drop_prob = 0.
     ):
         batch, dim, device, dtype = *image_embed.shape, image_embed.device, image_embed.dtype
 
         num_time_embeds, num_image_embeds, num_text_embeds = self.num_time_embeds, self.num_image_embeds, self.num_text_embeds
 
         # setup self conditioning
 
@@ -1020,14 +1024,22 @@
 
         # in section 2.2, last paragraph
         # "... consisting of encoded text, CLIP text embedding, diffusion timestep embedding, noised CLIP image embedding, final embedding for prediction"
 
         text_embed = self.to_text_embeds(text_embed)
         image_embed = self.to_image_embeds(image_embed)
 
+        # classifier free guidance masks
+
+        text_keep_mask = prob_mask_like((batch,), 1 - text_cond_drop_prob, device = device)
+        text_keep_mask = rearrange(text_keep_mask, 'b -> b 1 1')
+
+        image_keep_mask = prob_mask_like((batch,), 1 - image_cond_drop_prob, device = device)
+        image_keep_mask = rearrange(image_keep_mask, 'b -> b 1 1')
+
         # make text encodings optional
         # although the paper seems to suggest it is present <--
 
         if not exists(text_encodings):
             text_encodings = torch.empty((batch, 0, dim), device = device, dtype = dtype)
     
         mask = torch.any(text_encodings != 0., dim = -1)
@@ -1040,40 +1052,47 @@
         text_len = text_encodings.shape[-2]
         remainder = self.max_text_len - text_len
 
         if remainder > 0:
             text_encodings = F.pad(text_encodings, (0, 0, 0, remainder), value = 0.)
             mask = F.pad(mask, (0, remainder), value = False)
 
-        null_text_embeds = self.null_text_embed.to(text_encodings.dtype)
+        # mask out text encodings with null encodings
+
+        null_text_encodings = self.null_text_encodings.to(text_encodings.dtype)
 
         text_encodings = torch.where(
-            rearrange(mask, 'b n -> b n 1').clone(),
+            rearrange(mask, 'b n -> b n 1').clone() & text_keep_mask,
             text_encodings,
-            null_text_embeds
+            null_text_encodings
         )
 
-        # classifier free guidance
+        # mask out text embeddings with null text embeddings
+
+        null_text_embeds = self.null_text_embeds.to(text_embed.dtype)
 
-        keep_mask = prob_mask_like((batch,), 1 - cond_drop_prob, device = device)
-        keep_mask = rearrange(keep_mask, 'b -> b 1')
+        text_embeds = torch.where(
+            text_keep_mask,
+            text_embed,
+            null_text_embeds
+        )
 
-        mask &= keep_mask
+        # mask out image embeddings with null image embeddings
 
-        # whether text embedding is masked or not depends on the classifier free guidance conditional masking
+        null_image_embed = self.null_image_embed.to(image_embed.dtype)
 
-        keep_mask = repeat(keep_mask, 'b 1 -> b n', n = num_text_embeds)
-        mask = torch.cat((mask, keep_mask), dim = 1)
+        image_embed = torch.where(
+            image_keep_mask,
+            image_embed,
+            null_image_embed
+        )
 
         # whether text embedding is used for conditioning depends on whether text encodings are available for attention (for classifier free guidance, even though it seems from the paper it was not used in the prior ddpm, as the objective is different)
         # but let's just do it right
 
-        attend_padding = 1 + num_time_embeds + num_image_embeds + int(self.self_cond) # 1 for learned queries + number of image embeds + time embeds
-        mask = F.pad(mask, (0, attend_padding), value = True) # extend mask for text embedding, noised image embedding, time step embedding, and learned query
-
         time_embed = self.to_time_embeds(diffusion_timesteps)
 
         learned_queries = repeat(self.learned_query, 'd -> b 1 d', b = batch)
 
         if self.self_cond:
             learned_queries = torch.cat((image_embed, self_cond), dim = -2)
 
@@ -1103,14 +1122,16 @@
         clip = None,
         image_embed_dim = None,
         image_size = None,
         image_channels = 3,
         timesteps = 1000,
         sample_timesteps = None,
         cond_drop_prob = 0.,
+        text_cond_drop_prob = None,
+        image_cond_drop_prob = None,
         loss_type = "l2",
         predict_x_start = True,
         beta_schedule = "cosine",
         condition_on_text_encodings = True,  # the paper suggests this is needed, but you can turn it off for your CLIP preprocessed text embed -> image embed training
         sampling_clamp_l2norm = False,       # whether to l2norm clamp the image embed at each denoising iteration (analogous to -1 to 1 clipping for usual DDPMs)
         sampling_final_clamp_l2norm = False, # whether to l2norm the final image embedding output (this is also done for images in ddpm)
         training_clamp_l2norm = False,
@@ -1143,16 +1164,18 @@
             assert exists(image_embed_dim), 'latent dimension must be given, if training prior network without CLIP given'
             self.clip = None
 
         self.net = net
         self.image_embed_dim = default(image_embed_dim, lambda: clip.dim_latent)
         self.channels = default(image_channels, lambda: clip.image_channels)
 
-        self.cond_drop_prob = cond_drop_prob
-        self.can_classifier_guidance = cond_drop_prob > 0.
+        self.text_cond_drop_prob = default(text_cond_drop_prob, cond_drop_prob)
+        self.image_cond_drop_prob = default(image_cond_drop_prob, cond_drop_prob)
+
+        self.can_classifier_guidance = self.text_cond_drop_prob > 0. and self.image_cond_drop_prob > 0.
         self.condition_on_text_encodings = condition_on_text_encodings
 
         # in paper, they do not predict the noise, but predict x0 directly for image embedding, claiming empirically better results. I'll just offer both.
 
         self.predict_x_start = predict_x_start
 
         # @crowsonkb 's suggestion - https://github.com/lucidrains/DALLE2-pytorch/issues/60#issue-1226116132
@@ -1304,15 +1327,16 @@
             with torch.no_grad():
                 self_cond = self.net(image_embed_noisy, times, **text_cond).detach()
 
         pred = self.net(
             image_embed_noisy,
             times,
             self_cond = self_cond,
-            cond_drop_prob = self.cond_drop_prob,
+            text_cond_drop_prob = self.text_cond_drop_prob,
+            image_cond_drop_prob = self.image_cond_drop_prob,
             **text_cond
         )
 
         if self.predict_x_start and self.training_clamp_l2norm:
             pred = self.l2norm_clamp_embed(pred)
 
         target = noise if not self.predict_x_start else image_embed
```

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/data/bpe_simple_vocab_16e6.txt` & `dalle2-pytorch-1.9.0/dalle2_pytorch/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/decoder_loader.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/decoder_loader.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/prior_loader.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/prior_loader.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/dataloaders/simple_image_only_dataloader.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/dataloaders/simple_image_only_dataloader.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/optimizer.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/tokenizer.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/trackers.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/trackers.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/train_configs.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/train_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 class DecoderConfig(BaseModel):
     unets: ListOrTuple[UnetConfig]
     image_size: int = None
     image_sizes: ListOrTuple[int] = None
     clip: Optional[AdapterConfig]   # The clip model to use if embeddings are not provided
     channels: int = 3
     timesteps: int = 1000
-    sample_timesteps: Optional[SingularOrIterable[int]] = None
+    sample_timesteps: Optional[SingularOrIterable[Optional[int]]] = None
     loss_type: str = 'l2'
     beta_schedule: ListOrTuple[str] = None  # None means all cosine
     learned_variance: SingularOrIterable[bool] = True
     image_cond_drop_prob: float = 0.1
     text_cond_drop_prob: float = 0.5
 
     def create(self):
```

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/trainer.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,15 +515,15 @@
                 "no": torch.float
             }
             precision_type = cast_type_map[accelerator.mixed_precision]
             assert precision_type == torch.float, "DeepSpeed currently only supports float32 precision when using on the fly embedding generation from clip"
             clip = decoder.clip
             clip.to(precision_type)
 
-        decoder, *optimizers = list(self.accelerator.prepare(decoder, *optimizers))
+        decoder, train_dataloader, *optimizers = list(self.accelerator.prepare(decoder, dataloaders['train'], *optimizers))
 
         self.decoder = decoder
 
         # prepare dataloaders
 
         train_loader = val_loader = None
         if exists(dataloaders):
```

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/utils.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/vqgan_vae.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/vqgan_vae.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch/vqgan_vae_trainer.py` & `dalle2-pytorch-1.9.0/dalle2_pytorch/vqgan_vae_trainer.py`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/PKG-INFO` & `dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalle2-pytorch
-Version: 1.8.4
+Version: 1.9.0
 Summary: DALL-E 2
 Home-page: https://github.com/lucidrains/dalle2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dalle2-pytorch-1.8.4/dalle2_pytorch.egg-info/SOURCES.txt` & `dalle2-pytorch-1.9.0/dalle2_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dalle2-pytorch-1.8.4/setup.py` & `dalle2-pytorch-1.9.0/setup.py`

 * *Files identical despite different names*

