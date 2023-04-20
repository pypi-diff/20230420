# Comparing `tmp/dadaptation-1.5.tar.gz` & `tmp/dadaptation-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadaptation-1.5.tar", last modified: Thu Jan 26 16:16:59 2023, max compression
+gzip compressed data, was "/private/home/adefazio/dadaptation/dist/.tmp-ylrxb0c3/dadaptation-2.0.tar", last modified: Thu Apr 20 15:42:27 2023, max compression
```

## Comparing `dadaptation-1.5.tar` & `dadaptation-2.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-01-26 16:16:59.000000 dadaptation-1.5/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-1.5/LICENSE
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2492 2023-01-26 16:16:59.000000 dadaptation-1.5/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1994 2023-01-25 15:53:57.000000 dadaptation-1.5/README.md
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-01-26 16:16:59.000000 dadaptation-1.5/dadaptation/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      111 2023-01-26 16:15:03.000000 dadaptation-1.5/dadaptation/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8812 2023-01-25 15:53:57.000000 dadaptation-1.5/dadaptation/dadapt_adagrad.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6787 2023-01-25 15:53:57.000000 dadaptation-1.5/dadaptation/dadapt_adam.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     4944 2023-01-25 15:53:57.000000 dadaptation-1.5/dadaptation/dadapt_sgd.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-01-26 16:16:59.000000 dadaptation-1.5/dadaptation/experimental/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       79 2023-01-26 16:15:12.000000 dadaptation-1.5/dadaptation/experimental/__init__.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     6926 2023-01-25 15:53:57.000000 dadaptation-1.5/dadaptation/experimental/dadapt_adam_ip.py
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     5583 2023-01-25 15:53:57.000000 dadaptation-1.5/dadaptation/experimental/dadapt_sgd_ip.py
-drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-01-26 16:16:59.000000 dadaptation-1.5/dadaptation.egg-info/
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2492 2023-01-26 16:16:58.000000 dadaptation-1.5/dadaptation.egg-info/PKG-INFO
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      410 2023-01-26 16:16:58.000000 dadaptation-1.5/dadaptation.egg-info/SOURCES.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-01-26 16:16:58.000000 dadaptation-1.5/dadaptation.egg-info/dependency_links.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-01-26 16:16:58.000000 dadaptation-1.5/dadaptation.egg-info/top_level.txt
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-1.5/pyproject.toml
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-01-26 16:16:59.000000 dadaptation-1.5/setup.cfg
--rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-01-26 16:15:36.000000 dadaptation-1.5/setup.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     1091 2023-01-09 18:27:36.000000 dadaptation-2.0/LICENSE
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2747 2023-04-20 15:42:27.000000 dadaptation-2.0/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2286 2023-04-20 15:38:30.000000 dadaptation-2.0/README.md
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      148 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9168 2023-02-09 18:31:57.000000 dadaptation-2.0/dadaptation/dadapt_adagrad.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9012 2023-04-18 15:13:04.000000 dadaptation-2.0/dadaptation/dadapt_adam.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9593 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/dadapt_adan.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7131 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/dadapt_sgd.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation/experimental/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      121 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/__init__.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     8230 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_adam_ip.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     9737 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_adan_ip.py
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     7213 2023-04-17 18:47:49.000000 dadaptation-2.0/dadaptation/experimental/dadapt_sgd_ip.py
+drwxrwxr-x   0 adefazio (1185200101) adefazio (1185200101)        0 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)     2747 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/PKG-INFO
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      480 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/SOURCES.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)        1 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/dependency_links.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       12 2023-04-20 15:42:27.000000 dadaptation-2.0/dadaptation.egg-info/top_level.txt
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      304 2023-01-20 15:51:35.000000 dadaptation-2.0/pyproject.toml
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)       38 2023-04-20 15:42:27.000000 dadaptation-2.0/setup.cfg
+-rw-rw-r--   0 adefazio (1185200101) adefazio (1185200101)      895 2023-04-20 15:33:41.000000 dadaptation-2.0/setup.py
```

### Comparing `dadaptation-1.5/LICENSE` & `dadaptation-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dadaptation-1.5/PKG-INFO` & `dadaptation-2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 1.5
+Version: 2.0
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,25 +18,33 @@
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
 ## Details
 
-The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
+The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
  - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
  - Only the AdaGrad version supports sparse gradients.
  - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
- - If you encounter divergence early on, and are not already using learning rate warmup, try change growth_rate to match a reasonable warmup schedule rate for your problem. 
+ - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
+## Change Log
+
+### Version 2.0
+ - Added DAdaptAdan - should still be considered experimental.
+ - Added support for PyTorch's Fully Sharded Data Parallel. 
+ - Improved support of edge cases such as learning rate zero.
+ - Improved logging - uses Python logging rather than print statements
+
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
 ![vision](figures/dadapt_cifar100.png)
 ![vision](figures/dadapt_imagenet.png)
 ![vision](figures/dadapt_vit.png)
 ![vision](figures/dadapt_lstm.png)
@@ -46,9 +52,7 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
-
-
```

### Comparing `dadaptation-1.5/README.md` & `dadaptation-2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
 ## Details
 
-The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
+The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
  - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
  - Only the AdaGrad version supports sparse gradients.
  - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
- - If you encounter divergence early on, and are not already using learning rate warmup, try change growth_rate to match a reasonable warmup schedule rate for your problem. 
+ - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
+## Change Log
+
+### Version 2.0
+ - Added DAdaptAdan - should still be considered experimental.
+ - Added support for PyTorch's Fully Sharded Data Parallel. 
+ - Improved support of edge cases such as learning rate zero.
+ - Improved logging - uses Python logging rather than print statements
+
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
 ![vision](figures/dadapt_cifar100.png)
 ![vision](figures/dadapt_imagenet.png)
 ![vision](figures/dadapt_vit.png)
 ![vision](figures/dadapt_lstm.png)
```

### Comparing `dadaptation-1.5/dadaptation/dadapt_adagrad.py` & `dadaptation-2.0/dadaptation/dadapt_adagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         eps (float): 
-            Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
+            Term added to the denominator outside of the root operation to improve numerical stability. (default: 1e-6).
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
             prevent the D estimate from growing faster than this multiplicative rate. 
             Default is inf, for unrestricted.
     """
 
@@ -43,19 +43,22 @@
         lr: float = 1.0,
         momentum: float = 0, 
         log_every: int = 0,
         weight_decay: float = 0.0,
         eps: float = 0.0,
         d0 = 1e-6, growth_rate=float('inf')
     ):
+        if d0 <= 0:
+            raise ValueError("Invalid d0 value: {}".format(d0))
         if lr <= 0:
             raise ValueError(f"Learning rate {lr} must be positive")
         if momentum < 0:
             raise ValueError(f"Momentum {momentum} must be non-negative")
-
+        if eps <= 0:
+            raise ValueError("Invalid epsilon value: {}".format(eps))
 
         defaults = dict(lr=lr, 
             momentum=momentum,
             eps=eps, 
             weight_decay=weight_decay,
             gsq_weighted=0.0, 
             log_every=log_every,
@@ -185,14 +188,19 @@
                     sksq_weighted_change += sksq_weighted_param - old_sksq_weighted_param
                     skl1_change += skl1_param - old_skl1_param
             ######
             
         sksq_weighted = sksq_weighted + sksq_weighted_change
         skl1 = skl1 + skl1_change
 
+        # if we have not done any progres, return
+        # if we have any gradients available, will have skl1 > 0 (unless \|g\|=0)
+        if skl1 == 0:
+            return loss
+
         gsq_weighted = gsq_weighted + dlr*dlr*g_sq
         d_hat = d
         
         if lr > 0.0:
             d_hat = (sksq_weighted - gsq_weighted)/skl1
             d = group['d'] = max(d, min(d_hat, d*growth_rate))
```

### Comparing `dadaptation-1.5/dadaptation/dadapt_adam.py` & `dadaptation-2.0/dadaptation/dadapt_adam.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,73 +8,90 @@
 from typing import TYPE_CHECKING, Any, Callable, Optional
 
 import torch
 import torch.optim
 import pdb
 import logging
 import os
+import torch.distributed as dist
 
 if TYPE_CHECKING:
     from torch.optim.optimizer import _params_t
 else:
     _params_t = Any
 
+def to_real(x):
+    if torch.is_complex(x):
+        return x.real
+    else:
+        return x
+
 class DAdaptAdam(torch.optim.Optimizer):
     r"""
     Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
         momentum (float): 
             Momentum value in  the range [0,1) (default: 0.9).
         eps (float): 
-            Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
+            Term added to the denominator outside of the root operation to improve numerical stability. (default: 1e-8).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
         decouple (boolean): 
             Use AdamW style decoupled weight decay
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
             prevent the D estimate from growing faster than this multiplicative rate. 
             Default is inf, for unrestricted. Values like 1.02 give a kind of learning
             rate warmup effect.
+        fsdp_in_use (bool):
+            If you're using sharded parameters, this should be set to True. The optimizer
+            will attempt to auto-detect this, but if you're using an implementation other
+            than PyTorch's builtin version, the auto-detection won't work.
     """
     def __init__(self, params, lr=1.0, 
-                 betas=(0.9, 0.999), eps=1e-8,
-                 weight_decay=0, log_every=0,
+                 betas=(0.9, 0.999), 
+                 eps=1e-8,
+                 weight_decay=0, 
+                 log_every=0,
                  decouple=False,
-                 d0=1e-6, growth_rate=float('inf')):
-        if not 0.0 <= lr:
+                 d0=1e-6, 
+                 growth_rate=float('inf'),
+                 fsdp_in_use=False):
+        if not 0.0 < d0:
+            raise ValueError("Invalid d0 value: {}".format(d0))
+        if not 0.0 < lr:
             raise ValueError("Invalid learning rate: {}".format(lr))
-        if not 0.0 <= eps:
+        if not 0.0 < eps:
             raise ValueError("Invalid epsilon value: {}".format(eps))
         if not 0.0 <= betas[0] < 1.0:
             raise ValueError("Invalid beta parameter at index 0: {}".format(betas[0]))
         if not 0.0 <= betas[1] < 1.0:
             raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
 
         if decouple:
             print(f"Using decoupled weight decay")
 
-        
         defaults = dict(lr=lr, betas=betas, eps=eps,
                         weight_decay=weight_decay,
                         d = d0, 
                         k=0, 
                         gsq_weighted=0.0,
                         log_every=log_every,
+                        decouple=decouple,
                         growth_rate=growth_rate,
-                        decouple=decouple)
+                        fsdp_in_use=fsdp_in_use)
         
         super().__init__(params, defaults)
 
     @property
     def supports_memory_efficient_fp16(self):
         return False
 
@@ -94,85 +111,116 @@
             loss = closure()
 
 
         g_sq = 0.0
         sksq_weighted = 0.0
         sk_l1 = 0.0
 
-        ngroups = len(self.param_groups)
+        lr = max(group['lr'] for group in self.param_groups)
 
         group = self.param_groups[0]
         gsq_weighted = group['gsq_weighted']
         d = group['d']
-        lr = group['lr']
         dlr = d*lr
         
         growth_rate = group['growth_rate']
         decouple = group['decouple']
+        fsdp_in_use = group['fsdp_in_use']
         log_every = group['log_every']
 
         beta1, beta2 = group['betas']
 
         for group in self.param_groups:
+            group_lr = group['lr']
             decay = group['weight_decay']
             k = group['k']
             eps = group['eps']
 
+            if group_lr not in [lr, 0.0]:
+                raise RuntimeError(f"Setting different lr values in different parameter groups is only supported for values of 0")
+
             for p in group['params']:
                 if p.grad is None:
                     continue
+                if hasattr(p, "_fsdp_flattened"):
+                    fsdp_in_use = True
                 grad = p.grad.data
                 
                 # Apply weight decay (coupled variant)
                 if decay != 0 and not decouple:
                     grad.add_(p.data, alpha=decay)
 
                 state = self.state[p]
 
                 # State initialization
                 if 'step' not in state:
                     state['step'] = 0
-                    state['s'] = torch.zeros_like(p.data).detach()
+                    state['s'] = torch.zeros_like(p.data, memory_format=torch.preserve_format).detach()
                     # Exponential moving average of gradient values
-                    state['exp_avg'] = torch.zeros_like(p.data).detach()
+                    state['exp_avg'] = torch.zeros_like(p.data, memory_format=torch.preserve_format).detach()
                     # Exponential moving average of squared gradient values
-                    state['exp_avg_sq'] = torch.zeros_like(p.data).detach()
+                    state['exp_avg_sq'] = torch.zeros_like(to_real(p.data), memory_format=torch.preserve_format).detach()
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
                 
+                grad_grad = to_real(grad * grad.conj())
 
                 # Adam EMA updates
-                exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1-beta1))
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1-beta2)
-                
-                denom = exp_avg_sq.sqrt().add_(eps)
-
-                g_sq += (grad * grad).div_(denom).sum().item()
-
-                s = state['s']
-                s.mul_(beta2).add_(grad, alpha=dlr*(1-beta2))
-                sksq_weighted += (s * s).div_(denom).sum().item()
-                sk_l1 += s.abs().sum().item()
+                if group_lr > 0:
+                    exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1-beta1))
+                    exp_avg_sq.mul_(beta2).add_(grad_grad, alpha=1-beta2)
+                    
+                    denom = exp_avg_sq.sqrt().add_(eps)
+
+                    g_sq += grad_grad.div_(denom).sum().item()
+
+                    s = state['s']
+                    s.mul_(beta2).add_(grad, alpha=dlr*(1-beta2))
+                    sksq_weighted += to_real(s * s.conj()).div_(denom).sum().item()
+                    sk_l1 += s.abs().sum().item()
 
             ######
 
         gsq_weighted = beta2*gsq_weighted + g_sq*(dlr**2)*(1-beta2)
         d_hat = d
 
+        # if we have not done any progres, return
+        # if we have any gradients available, will have sk_l1 > 0 (unless \|g\|=0)
+        if sk_l1 == 0:
+            return loss
+
         if lr > 0.0:
-            d_hat = (sksq_weighted/(1-beta2) - gsq_weighted)/sk_l1
+            if fsdp_in_use:
+                dist_tensor = torch.zeros(3).cuda()
+                dist_tensor[0] = sksq_weighted
+                dist_tensor[1] = gsq_weighted
+                dist_tensor[2] = sk_l1
+                dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
+                global_sksq_weighted = dist_tensor[0]
+                global_gsq_weighted = dist_tensor[1]
+                global_sk_l1 = dist_tensor[2]
+            else:
+                global_sksq_weighted = sksq_weighted
+                global_gsq_weighted = gsq_weighted
+                global_sk_l1 = sk_l1
+
+            d_hat = (global_sksq_weighted/(1-beta2) - global_gsq_weighted)/global_sk_l1
             d = max(d, min(d_hat, d*growth_rate))
 
         if log_every > 0 and k % log_every == 0:
-            print(f"ng: {ngroups} lr: {lr} dlr: {dlr} d_hat: {d_hat}, d: {d}. sksq_weighted={sksq_weighted:1.1e} sk_l1={sk_l1:1.1e} gsq_weighted={gsq_weighted:1.1e}")
+            logging.info(
+                f"(k={k}) dlr: {dlr:1.1e} d_hat: {d_hat:1.1e}, d: {d:1.8}. "
+                f"sksq_weighted={global_sksq_weighted:1.1e} gsq_weighted={global_gsq_weighted:1.1e} "
+                f"sk_l1={global_sk_l1:1.1e}{' (FSDP)' if fsdp_in_use else ''}")
 
         for group in self.param_groups:
             group['gsq_weighted'] = gsq_weighted
             group['d'] = d
 
+            group_lr = group['lr']
             decay = group['weight_decay']
             k = group['k']
             eps = group['eps']
 
             for p in group['params']:
                 if p.grad is None:
                     continue
@@ -181,17 +229,18 @@
                 state = self.state[p]
 
                 exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
 
                 state['step'] += 1
 
                 denom = exp_avg_sq.sqrt().add_(eps)
+                denom = denom.type(p.type())
 
                 # Apply weight decay (decoupled variant)
-                if decay != 0 and decouple:
+                if decay != 0 and decouple and group_lr > 0:
                     p.data.add_(p.data, alpha=-decay * dlr)
 
 
                 ### Take step
                 p.data.addcdiv_(exp_avg, denom, value=-1)
 
             group['k'] = k + 1
```

### Comparing `dadaptation-1.5/dadaptation/dadapt_sgd.py` & `dadaptation-2.0/dadaptation/experimental/dadapt_sgd_ip.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 import torch.optim
 import pdb
 import math
+import logging
+import torch.distributed as dist
 
-class DAdaptSGD(torch.optim.Optimizer):
+class DAdaptSGDIP(torch.optim.Optimizer):
     r"""
-    Implements SGD with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    Implements Adam with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
+    
+    Unlike the AdamIP variant, this IP variant is computing almost exactly the same bound, and should perform 
+    similarly to the non-IP version.
+
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
@@ -27,26 +33,40 @@
             Log using print every k steps, default 0 (no logging).
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
             prevent the D estimate from growing faster than this multiplicative rate. 
             Default is inf, for unrestricted. More conservative values like 1.02 may
             help if training is unstable.
+        fsdp_in_use (bool):
+            If you're using sharded parameters, this should be set to True. The optimizer
+            will attempt to auto-detect this, but if you're using an implementation other
+            than PyTorch's builtin version, the auto-detection won't work.
     """
     def __init__(self, params, 
-        lr=1e-2, 
+        lr=1.0, 
         momentum=0, 
         weight_decay=0, 
         log_every=0,
-        d0=1e-6, growth_rate=float('inf')):
+        d0=1e-6, growth_rate=float('inf'),
+        fsdp_in_use=False):
+
+        if not 0.0 < d0:
+            raise ValueError("Invalid d0 value: {}".format(d0))
+        if not 0.0 < lr:
+            raise ValueError("Invalid learning rate: {}".format(lr))
+
         defaults = dict(lr=lr,
             momentum=momentum, 
             weight_decay=weight_decay, k=0,
             log_every=log_every,
-            gsq_weighted=0.0, d=d0, growth_rate=growth_rate)
+            numerator_weighted=0.0, 
+            d=d0, 
+            growth_rate=growth_rate,
+            fsdp_in_use=fsdp_in_use)
         self.loggables = {}
 
         try:
             self.rank = torch.distributed.get_rank()
         except:
             self.rank = 0
 
@@ -54,83 +74,118 @@
 
     def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
 
         group = self.param_groups[0]
-        lr = group['lr']
+        lr = max(group['lr'] for group in self.param_groups)
+
         decay = group['weight_decay']
         momentum = group['momentum']
         log_every = group['log_every']
         ck = 1 - momentum
         k = group['k']
 
-        gsq_weighted = group['gsq_weighted']
+        numerator_weighted = group['numerator_weighted']
         growth_rate = group['growth_rate']
         d = group['d']
+        fsdp_in_use = group['fsdp_in_use']
+        
+        group = self.param_groups[0]
         
-
-        g_sq = 0.0
         sk_sq = 0.0
 
-        for group in self.param_groups:
-            for p in group['params']:
-                if p.grad is None:
-                    continue
-                grad = p.grad.data
-                
-                # Apply weight decay
-                if decay != 0:
-                    if grad.is_sparse:
-                        raise RuntimeError("weight_decay option is not compatible with sparse gradients")
-
-                    grad.add_(p.data, alpha=decay)
-
-                state = self.state[p]
-
-                g_sq += (grad * grad).sum().item()
-
-
-        group = self.param_groups[0]
         if k == 0: 
-            group['g0_norm'] = g0_norm = math.sqrt(g_sq)
+            g_sq = 0.0
+            for group in self.param_groups:
+                for p in group['params']:
+                    if p.grad is None:
+                        continue
+                    if hasattr(p, "_fsdp_flattened"):
+                        fsdp_in_use = True
+                    grad = p.grad.data
+                    
+                    # Apply weight decay
+                    if decay != 0:
+                        if grad.is_sparse:
+                            raise RuntimeError("weight_decay option is not compatible with sparse gradients")
+
+                        grad.add(p.data, alpha=decay)
+
+                    state = self.state[p]
+
+                    g_sq += (grad * grad).sum().item()
+
+            if fsdp_in_use:
+                dist_tensor = torch.zeros(1).cuda()
+                dist_tensor[0] = g_sq
+                dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
+                global_gsq = dist_tensor[0]
+            else:
+                global_gsq = g_sq
+            g0_norm = math.sqrt(global_gsq)
 
-        g0_norm = group['g0_norm']
         dlr = d*lr/g0_norm
 
         for group in self.param_groups:
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
                 state = self.state[p]
 
                 if 'z' not in state:
                     z = state['z'] = torch.clone(p.data).detach()
                     s = state['s'] = torch.zeros_like(p.data).detach()
                     x0 = state['x0'] = torch.clone(p.data).detach()
 
+                    # Apply weight decay
+                    if decay != 0:
+                        if grad.is_sparse:
+                            raise RuntimeError("weight_decay option is not compatible with sparse gradients")
+
+                        grad.add_(p.data, alpha=decay)
+
                 s = state['s']
+
+                numerator_weighted += dlr * torch.dot(grad.flatten(), s.flatten()).item()
+                
                 s.data.add_(grad, alpha=dlr)
                 sk_sq += (s * s).sum().item()
             ######
 
-        gsq_weighted = group['gsq_weighted'] = gsq_weighted + dlr*dlr*g_sq
         d_hat = d
 
         if lr > 0.0:
-            d_hat = (sk_sq - gsq_weighted)/(math.sqrt(sk_sq))
-            d = group['d'] = max(d, min(d_hat, d*growth_rate))
+            if fsdp_in_use:
+                dist_tensor = torch.zeros(2).cuda()
+                dist_tensor[0] = sk_sq
+                dist_tensor[1] = numerator_weighted
+                dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
+                global_sk_sq = dist_tensor[0]
+                global_numerator_weighted = dist_tensor[1]
+            else:
+                global_sk_sq = sk_sq
+                global_numerator_weighted = numerator_weighted
+
+            d_hat = 2*global_numerator_weighted/math.sqrt(global_sk_sq)
+            d = max(d, min(d_hat, d*growth_rate))
+
+
+        # if we have not done any updates
+        # if we have any gradients available, will have sk_sq > 0 (unless \|g\|=0)
+        if global_sk_sq == 0:
+            return loss
 
         if log_every > 0 and k % log_every == 0:
-            print(f"(r={self.rank},k={k}) dlr: {dlr} d_hat: {d_hat}, d: {d}. sk_sq={sk_sq} gsq_weighted={gsq_weighted} g0_norm={g0_norm}", flush=True)
+            logging.info(f"(r={self.rank},k={k}) dlr: {dlr} d_hat: {d_hat}, d: {d}. sk_norm={math.sqrt(global_sk_sq)} numerator_weighted={global_numerator_weighted} g0_norm={g0_norm}", flush=True)
 
         for group in self.param_groups:
-            group['gsq_weighted'] = gsq_weighted
+            group['numerator_weighted'] = numerator_weighted
             group['d'] = d
             group['g0_norm'] = g0_norm
             ######################################
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
```

### Comparing `dadaptation-1.5/dadaptation/experimental/dadapt_adam_ip.py` & `dadaptation-2.0/dadaptation/dadapt_sgd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,207 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 # 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-import math
-from typing import TYPE_CHECKING, Any, Callable, Optional
-
 import torch
 import torch.optim
 import pdb
+import math
 import logging
-import os
+import torch.distributed as dist
 
-if TYPE_CHECKING:
-    from torch.optim.optimizer import _params_t
-else:
-    _params_t = Any
-
-class DAdaptAdamIP(torch.optim.Optimizer):
+class DAdaptSGD(torch.optim.Optimizer):
     r"""
-    Implements Adam with D-Adaptation automatic step-sizes. 
-    Leave LR set to 1 unless you encounter instability.
-
-    This IP variant uses a tighter bound than the non-IP version,
-    and so will typically choose larger step sizes. It has not 
-    been as extensively tested.
-    
+    Implements SGD with D-Adaptation automatic step-sizes. Leave LR set to 1 unless you encounter instability.
     Arguments:
         params (iterable): 
             Iterable of parameters to optimize or dicts defining parameter groups.
         lr (float): 
             Learning rate adjustment parameter. Increases or decreases the D-adapted learning rate.
         betas (Tuple[float, float], optional): coefficients used for computing
             running averages of gradient and its square (default: (0.9, 0.999))
         momentum (float): 
             Momentum value in  the range [0,1) (default: 0.9).
-        eps (float): 
-            Term added to the denominator outside of the root operation to improve numerical stability. (default: 0).
         weight_decay (float): 
             Weight decay, i.e. a L2 penalty (default: 0).
         log_every (int): 
             Log using print every k steps, default 0 (no logging).
-        decouple (boolean): 
-            Use AdamW style decoupled weight decay
         d0 (float):
             Initial D estimate for D-adaptation (default 1e-6). Rarely needs changing.
         growth_rate (float):
             prevent the D estimate from growing faster than this multiplicative rate. 
-            Default is inf, for unrestricted. Values like 1.02 give a kind of learning
-            rate warmup effect.
+            Default is inf, for unrestricted. More conservative values like 1.02 may
+            help if training is unstable.
+        fsdp_in_use (bool):
+            If you're using sharded parameters, this should be set to True. The optimizer
+            will attempt to auto-detect this, but if you're using an implementation other
+            than PyTorch's builtin version, the auto-detection won't work.
     """
-    def __init__(self, params, lr=1.0, 
-                 betas=(0.9, 0.999), eps=1e-8,
-                 weight_decay=0, log_every=0,
-                 decouple=False,
-                 d0=1e-6, growth_rate=float('inf')):
-        if not 0.0 <= lr:
+    def __init__(self, params, 
+        lr=1.0, 
+        momentum=0, 
+        weight_decay=0, 
+        log_every=0,
+        d0=1e-6, growth_rate=float('inf'),
+        fsdp_in_use=False):
+
+        if d0 <= 0:
+            raise ValueError("Invalid d0 value: {}".format(d0))
+        if lr <= 0:
             raise ValueError("Invalid learning rate: {}".format(lr))
-        if not 0.0 <= eps:
-            raise ValueError("Invalid epsilon value: {}".format(eps))
-        if not 0.0 <= betas[0] < 1.0:
-            raise ValueError("Invalid beta parameter at index 0: {}".format(betas[0]))
-        if not 0.0 <= betas[1] < 1.0:
-            raise ValueError("Invalid beta parameter at index 1: {}".format(betas[1]))
-
-        if decouple:
-            print(f"Using decoupled weight decay")
-
-        
-        defaults = dict(lr=lr, betas=betas, eps=eps,
-                        weight_decay=weight_decay,
-                        d = d0, 
-                        k=0, 
-                        numerator_weighted=0.0,
-                        log_every=log_every,
-                        growth_rate=growth_rate,
-                        decouple=decouple)
-        self.d0 = d0
-        super().__init__(params, defaults)
 
-    @property
-    def supports_memory_efficient_fp16(self):
-        return False
-
-    @property
-    def supports_flat_params(self):
-        return True
+        defaults = dict(lr=lr,
+            momentum=momentum, 
+            weight_decay=weight_decay, 
+            k=0,
+            log_every=log_every,
+            gsq_weighted=0.0, 
+            g0_norm=0.0,
+            d=d0, 
+            growth_rate=growth_rate,
+            fsdp_in_use=fsdp_in_use)
+        self.loggables = {}
+
+        try:
+            self.rank = torch.distributed.get_rank()
+        except:
+            self.rank = 0
 
-    def step(self, closure=None):
-        """Performs a single optimization step.
+        #self.group = dist.new_group(range(dist.get_world_size()))
 
-        Arguments:
-            closure (callable, optional): A closure that reevaluates the model
-                and returns the loss.
-        """
+        super().__init__(params, defaults)
+
+    def step(self, closure=None):
         loss = None
         if closure is not None:
             loss = closure()
 
-        sk_l1 = 0.0
-
-        ngroups = len(self.param_groups)
+        lr = max(group['lr'] for group in self.param_groups)
 
+        # Stored at the group level to ensure resuming from checkpoints works
         group = self.param_groups[0]
-        numerator_weighted = group['numerator_weighted']
-        d = group['d']
-        lr = group['lr']
-        dlr = d*lr
-        
-        growth_rate = group['growth_rate']
-        decouple = group['decouple']
+        decay = group['weight_decay']
+        momentum = group['momentum']
         log_every = group['log_every']
+        ck = 1 - momentum
+        k = group['k']
 
-        beta1, beta2 = group['betas']
+        gsq_weighted = group['gsq_weighted']
+        g0_norm = group['g0_norm']
+        growth_rate = group['growth_rate']
+        fsdp_in_use = group['fsdp_in_use']
+        d = group['d']
 
-        numerator_acum = 0.0
+        g_sq = 0.0
+        sk_sq = 0.0
 
         for group in self.param_groups:
-            decay = group['weight_decay']
-            k = group['k']
-            eps = group['eps']
-
+            group_lr = group['lr']
+            if group_lr not in [lr, 0.0]:
+                raise RuntimeError(f"Setting different lr values in different parameter groups is only supported for values of 0")
             for p in group['params']:
                 if p.grad is None:
                     continue
+                if hasattr(p, "_fsdp_flattened"):
+                    fsdp_in_use = True
                 grad = p.grad.data
                 
-                # Apply weight decay (coupled variant)
-                if decay != 0 and not decouple:
+                # Apply weight decay
+                if decay != 0:
+                    if grad.is_sparse:
+                        raise RuntimeError("weight_decay option is not compatible with sparse gradients")
+
                     grad.add_(p.data, alpha=decay)
 
                 state = self.state[p]
 
-                # State initialization
-                if 'step' not in state:
-                    state['step'] = 0
-                    state['s'] = torch.zeros_like(p.data).detach()
-                    # Exponential moving average of gradient values
-                    state['exp_avg'] = torch.zeros_like(p.data).detach()
-                    # Exponential moving average of squared gradient values
-                    state['exp_avg_sq'] = torch.zeros_like(p.data).detach()
+                if group_lr > 0.0:
+                    g_sq += (grad * grad).sum().item()
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-                
-                s = state['s']
+        # if we have any gradients available, will have g_sq > 0 (unless \|g\|=0)
+        if g_sq == 0:
+            return loss
+
+        if k == 0: 
+            if fsdp_in_use:
+                dist_tensor = torch.zeros(1).cuda()
+                dist_tensor[0] = g_sq
+                dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
+                global_gsq = dist_tensor[0]
+            else:
+                global_gsq = g_sq
+            g0_norm = math.sqrt(global_gsq)
 
-                denom = exp_avg_sq.sqrt().add_(eps)
-                numerator_acum += dlr * torch.dot(grad.flatten(), s.div(denom).flatten())
+        dlr = d*lr/g0_norm
 
-                # Adam EMA updates
-                exp_avg.mul_(beta1).add_(grad, alpha=dlr*(1-beta1))
-                exp_avg_sq.mul_(beta2).addcmul_(grad, grad, value=1-beta2)
+        for group in self.param_groups:
+            group_lr = group['lr']
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+                grad = p.grad.data
+                state = self.state[p]
+
+                if 'z' not in state:
+                    z = state['z'] = torch.clone(p.data).detach()
+                    s = state['s'] = torch.zeros_like(p.data).detach()
+                    x0 = state['x0'] = torch.clone(p.data).detach()
 
-                s.mul_(beta2).add_(grad, alpha=dlr*(1-beta2))
-                sk_l1 += s.abs().sum().item()
+                s = state['s']
 
+                if group_lr > 0.0:
+                    s.data.add_(grad, alpha=dlr)
+                
+                sk_sq += (s * s).sum().item()
             ######
 
-        numerator_weighted = beta2*numerator_weighted + (1-beta2)*numerator_acum
+        gsq_weighted = gsq_weighted + dlr*dlr*g_sq
         d_hat = d
-        
+
         if lr > 0.0:
-            d_hat = 2*(beta2/(1-beta2))*numerator_weighted/sk_l1
-            d = max(d, min(d_hat, d*growth_rate))
+            if fsdp_in_use:
+                dist_tensor = torch.zeros(2).cuda()
+                dist_tensor[0] = sk_sq
+                dist_tensor[1] = gsq_weighted
+                dist.all_reduce(dist_tensor, op=dist.ReduceOp.SUM)
+                global_sk_sq = dist_tensor[0]
+                global_gsq_weighted = dist_tensor[1]
+            else:
+                global_sk_sq = sk_sq
+                global_gsq_weighted = gsq_weighted
+
+            d_hat = (global_sk_sq - global_gsq_weighted)/(math.sqrt(global_sk_sq))
+            d = group['d'] = max(d, min(d_hat, d*growth_rate))
 
         if log_every > 0 and k % log_every == 0:
-            print(f"ng: {ngroups} lr: {lr} dlr: {dlr} d_hat: {d_hat}, d: {d}. sk_l1={sk_l1:1.1e} numerator_weighted={numerator_weighted:1.1e}")
+            logging.info(
+                f"(k={k}) dlr: {dlr:1.1e} d_hat: {d_hat:1.1e}, d: {d:1.8}. "
+                f"sk_sq={global_sk_sq:1.1e} gsq_weighted={global_gsq_weighted:1.1e} "
+                f"g0_norm={g0_norm:1.1e}{' (FSDP)' if fsdp_in_use else ''}")
 
         for group in self.param_groups:
-            group['numerator_weighted'] = numerator_weighted
+            group['gsq_weighted'] = gsq_weighted
             group['d'] = d
-
-            decay = group['weight_decay']
-            k = group['k']
-            eps = group['eps']
-
+            group['g0_norm'] = g0_norm
+            ######################################
             for p in group['params']:
                 if p.grad is None:
                     continue
                 grad = p.grad.data
-
                 state = self.state[p]
 
-                exp_avg, exp_avg_sq = state['exp_avg'], state['exp_avg_sq']
-
-                state['step'] += 1
-
-                denom = exp_avg_sq.sqrt().add_(eps)
-
-                # Apply weight decay (decoupled variant)
-                if decay != 0 and decouple:
-                    p.data.add_(p.data, alpha=-decay * dlr)
+                s = state['s']
+                x0 = state['x0']
+                z = state['z']
 
+                # z step
+                z.data.copy_(x0 - s)
 
-                ### Take step
-                p.data.addcdiv_(exp_avg, denom, value=-1)
+                # x step
+                p.data.mul_(1-ck).add_(z, alpha=ck)
 
             group['k'] = k + 1
 
         return loss
+
```

### Comparing `dadaptation-1.5/dadaptation.egg-info/PKG-INFO` & `dadaptation-2.0/dadaptation.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: dadaptation
-Version: 1.5
+Version: 2.0
 Summary: Learning Rate Free Learning for Adam, SGD and AdaGrad
 Home-page: https://github.com/facebookresearch/dadaptation
 Author: Aaron Defazio
 Author-email: adefazio@meta.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,25 +18,33 @@
 
 *by Aaron Defazio and Konstantin Mishchenko [(Arxiv)](https://arxiv.org/abs/2301.07733)*
 
 ``` pip install dadaptation ```
 
 ## Details
 
-The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
+The provided Pytorch Optimizer classes are drop-in replacements, either copy into your project or use via pip with dadaptation.DAdaptSGD,  dadaptation.DAdaptAdam or dadaptation.DAdaptAdaGrad.
 
  - **Set the LR parameter to 1.0**. This parameter is not ignored, rather, setting it larger to smaller will directly scale up or down the D-Adapted learning rate. 
  - **Use the same learning rate scheduler you would normally use on the problem.**
  - The Adam variant supports AdamW style weight decay, just set decouple=True. It is not turned on by default, so if you are replacing your adam implementation, make sure you use decoupled if necessary.
  - It may be necessary to use larger weight decay than you would normally use, try a factor of 2 or 4 bigger if you see overfitting. D-Adaptation uses larger learning rates than people typically hand-choose, in some cases that requires more decay.
  - Use the log_every setting to see the learning rate being used (d*lr) and the current D bound.
  - Only the AdaGrad version supports sparse gradients.
  - The Adam IP variant implements a tighter D bound, which may help on some problems. The IP variants should be considered experimental.
- - If you encounter divergence early on, and are not already using learning rate warmup, try change growth_rate to match a reasonable warmup schedule rate for your problem. 
+ - Parameter-group level LR values are not fully supported. The optimizer only supports setting zero LR for some groups in order to do fine-tuning on parts of a model.
  
+## Change Log
+
+### Version 2.0
+ - Added DAdaptAdan - should still be considered experimental.
+ - Added support for PyTorch's Fully Sharded Data Parallel. 
+ - Improved support of edge cases such as learning rate zero.
+ - Improved logging - uses Python logging rather than print statements
+
  # Experimental results
 
 ![vision](figures/dadapt_cifar.png)
 ![vision](figures/dadapt_cifar100.png)
 ![vision](figures/dadapt_imagenet.png)
 ![vision](figures/dadapt_vit.png)
 ![vision](figures/dadapt_lstm.png)
@@ -46,9 +52,7 @@
 ![vision](figures/dadapt_gpt.png)
 ![vision](figures/dadapt_fastmri.png)
 ![vision](figures/dadapt_detectron.png)
 ![vision](figures/dadapt_dlrm.png)
 
 # License
 See the [License file](/LICENSE).
-
-
```

### Comparing `dadaptation-1.5/setup.py` & `dadaptation-2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dadaptation",
-    version="1.5",
+    version="2.0",
     author="Aaron Defazio",
     author_email="adefazio@meta.com",
     description="Learning Rate Free Learning for Adam, SGD and AdaGrad",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/facebookresearch/dadaptation",
     packages=setuptools.find_packages(),
```

