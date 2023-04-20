# Comparing `tmp/phaseaug-0.0.2.tar.gz` & `tmp/phaseaug-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phaseaug-0.0.2.tar", last modified: Mon Nov 21 06:16:32 2022, max compression
+gzip compressed data, was "phaseaug-1.0.0.tar", last modified: Thu Apr 20 04:22:58 2023, max compression
```

## Comparing `phaseaug-0.0.2.tar` & `phaseaug-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-21 06:16:32.590165 phaseaug-0.0.2/
--rw-r--r--   0 jun        (501) staff       (20)     1516 2022-10-07 01:16:31.000000 phaseaug-0.0.2/LICENSE
--rw-r--r--   0 jun        (501) staff       (20)     6640 2022-11-21 06:16:32.590050 phaseaug-0.0.2/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     5269 2022-11-21 05:30:56.000000 phaseaug-0.0.2/README.md
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-21 06:16:32.588609 phaseaug-0.0.2/phaseaug/
--rw-r--r--   0 jun        (501) staff       (20)       23 2022-11-21 06:13:37.000000 phaseaug-0.0.2/phaseaug/__init__.py
--rw-r--r--   0 jun        (501) staff       (20)     4214 2022-11-21 05:16:46.000000 phaseaug-0.0.2/phaseaug/phaseaug.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2022-11-21 06:16:32.589571 phaseaug-0.0.2/phaseaug.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)     6640 2022-11-21 06:16:32.000000 phaseaug-0.0.2/phaseaug.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)      506 2022-11-21 06:16:32.000000 phaseaug-0.0.2/phaseaug.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-21 06:16:32.000000 phaseaug-0.0.2/phaseaug.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-21 06:00:26.000000 phaseaug-0.0.2/phaseaug.egg-info/not-zip-safe
--rw-r--r--   0 jun        (501) staff       (20)       23 2022-11-21 06:16:32.000000 phaseaug-0.0.2/phaseaug.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        9 2022-11-21 06:16:32.000000 phaseaug-0.0.2/phaseaug.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2022-11-21 06:16:32.590203 phaseaug-0.0.2/setup.cfg
--rw-r--r--   0 jun        (501) staff       (20)      857 2022-11-21 06:16:23.000000 phaseaug-0.0.2/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.574484 phaseaug-1.0.0/
+-rw-r--r--   0 jun        (501) staff       (20)     1516 2022-10-07 01:16:31.000000 phaseaug-1.0.0/LICENSE
+-rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-20 04:22:58.574362 phaseaug-1.0.0/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     6196 2023-04-20 04:21:40.000000 phaseaug-1.0.0/README.md
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.572986 phaseaug-1.0.0/phaseaug/
+-rw-r--r--   0 jun        (501) staff       (20)       23 2022-11-21 06:11:54.000000 phaseaug-1.0.0/phaseaug/__init__.py
+-rw-r--r--   0 jun        (501) staff       (20)     4555 2023-04-20 04:16:20.000000 phaseaug-1.0.0/phaseaug/phaseaug.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2023-04-20 04:22:58.573933 phaseaug-1.0.0/phaseaug.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)     6650 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)      506 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2022-11-21 06:00:26.000000 phaseaug-1.0.0/phaseaug.egg-info/not-zip-safe
+-rw-r--r--   0 jun        (501) staff       (20)       23 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        9 2023-04-20 04:22:58.000000 phaseaug-1.0.0/phaseaug.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2023-04-20 04:22:58.574529 phaseaug-1.0.0/setup.cfg
+-rw-r--r--   0 jun        (501) staff       (20)      857 2023-04-20 04:18:16.000000 phaseaug-1.0.0/setup.py
```

### Comparing `phaseaug-0.0.2/LICENSE` & `phaseaug-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phaseaug-0.0.2/PKG-INFO` & `phaseaug-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,136 @@
-Metadata-Version: 2.1
-Name: phaseaug
-Version: 0.0.2
-Summary: PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping
-Home-page: https://github.com/mindslab-ai/phaseaug
-Author: junjun3518
-Author-email: junjun3518@gmail.com
-License: UNKNOWN
-Description: # PhaseAug
-        
-        **PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping**<br>
-        Junhyeok Lee, Seungu Han, Hyunjae Cho, Wonbin Jung @ [MINDsLab Inc.](https://github.com/mindslab-ai), SNU, KAIST
-        
-        [![arXiv](https://img.shields.io/badge/arXiv-2211.04610-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2211.04610) [![GitHub Repo stars](https://img.shields.io/github/stars/mindslab-ai/phaseaug?color=yellow&label=PhaseAug&logo=github&style=flat-square)](https://github.com/mindslab-ai/phaseaug) [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://mindslab-ai.github.io/phaseaug/)
-        
-        
-        **Abstract** : Previous generative adversarial network (GAN)-based neural vocoders are trained to reconstruct the exact ground truth waveform from the paired mel-spectrogram and do not consider the one-to-many relationship of speech synthesis. This conventional training causes overfitting for both the discriminators and the generator, leading to the periodicity artifacts in the generated audio signal. In this work, we present PhaseAug, the first differentiable augmentation for speech synthesis that rotates the phase of each frequency bin to simulate one-to-many mapping. With our proposed method, we outperform baselines without any architecture modification. Code and audio samples will be available at https://github.com/mindslab-ai/phaseaug.
-        
-        Submitted to ICASSP 2023
-        
-        ![phasor](asset/phaseaug_phasor.png) 
-        
-        
-        ## TODO
-        - Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012
-        - Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added.
-        - We will uplade PhaseAug to [pypi](https://pypi.org).
-        
-        ## Use PhaseAug
-        - Install `alias-free-torch==0.0.6` and `phaseaug`
-        ```bash
-        pip install alias-free-torch==0.0.6 phaseaug 
-        ```
-        - Insert PhaseAug in your code, check [train.py](./train.py) as a example.
-        ```python
-        from phaseaug import PhaseAug
-        ...
-        # define phaseaug
-        aug = PhaseAug()
-        ...
-        #discriminator update phase
-        aug_y, aug_y_g = aug.forward_sync(y, y_g_hat.detach())
-        y_df_hat_r, y_df_hat_g, _, _ = mpd(aug_y, aug_y_g)
-        y_ds_hat_r, y_ds_hat_g, _, _ = msd(aug_y, aug_y_g)
-        ...
-        #generator update phase
+# PhaseAug
+
+**PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping**<br>
+Junhyeok Lee, Seungu Han, Hyunjae Cho, Wonbin Jung @ [MINDsLab Inc.](https://github.com/mindslab-ai), SNU, KAIST
+
+[![arXiv](https://img.shields.io/badge/arXiv-2211.04610-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2211.04610) [![GitHub Repo stars](https://img.shields.io/github/stars/mindslab-ai/phaseaug?color=yellow&label=PhaseAug&logo=github&style=flat-square)](https://github.com/mindslab-ai/phaseaug) [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://mindslab-ai.github.io/phaseaug/)
+
+
+**Abstract** : Previous generative adversarial network (GAN)-based neural vocoders are trained to reconstruct the exact ground truth waveform from the paired mel-spectrogram and do not consider the one-to-many relationship of speech synthesis. This conventional training causes overfitting for both the discriminators and the generator, leading to the periodicity artifacts in the generated audio signal. In this work, we present PhaseAug, the first differentiable augmentation for speech synthesis that rotates the phase of each frequency bin to simulate one-to-many mapping. With our proposed method, we outperform baselines without any architecture modification. Code and audio samples will be available at https://github.com/mindslab-ai/phaseaug.
+
+Accepted to ICASSP 2023
+
+![phasor](asset/phaseaug_phasor.png) 
+
+
+## TODO
+- [x] PyTorch 2.0 is released, need to modify STFT and iSTFT for complex support (solved at `1.0.0`)
+- [x] Arxiv updated
+- [x] Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012.
+- [x] Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added. -> transpose m,k to reduce ambiguity
+- [x] Upload PhaseAug to [pypi](https://pypi.org/project/phaseaug/).
+- [x] Upload [VITS](https://arxiv.org/abs/2106.06103)+PhaseAug sampels at demo page.
+- [x] Refactoring codes for packaging.
+
+
+## Use PhaseAug
+- Install `alias-free-torch==0.0.6` and `phaseaug`
+```bash
+pip install alias-free-torch==0.0.6 phaseaug 
+```
+- Insert PhaseAug in your code, check [train.py](./train.py) as a example.
+```python
+from phaseaug.phaseaug import PhaseAug
+...
+# define phaseaug
+aug = PhaseAug()
+...
+# discriminator update phase
+aug_y, aug_y_g = aug.forward_sync(y, y_g_hat.detach())
+y_df_hat_r, y_df_hat_g, _, _ = mpd(aug_y, aug_y_g)
+y_ds_hat_r, y_ds_hat_g, _, _ = msd(aug_y, aug_y_g)
+...
+# generator update phase
+aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
+y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(aug_y, aug_y_g)
+y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(aug_y, aug_y_g)
+```
+
+- If you are applying `torch.cuda.amp.autocast` like [VITS](https://github.com/jaywalnut310/vits), you need to wrap PhaseAug with `autocast(enabled=False)` to prevent [ComplexHalf issue](https://github.com/jaywalnut310/vits/issues/15).
+```python
+from torch.cuda.amp import autocast
+...
+with autocast(enabled=True)
+    # wrapping PhaseAug with autocast(enabled=False)
+    with autocast(enabled=False)
         aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
-        y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(
-                                aug_y, aug_y_g)
-        y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(
-                                aug_y, aug_y_g)
-        ```
-        
-        ## Requirements
-        - [Pytorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
-        - The requirements are highlighted in [requirements.txt](./requirements.txt).
-        - We also provide docker setup [Dockerfile](./Dockerfile).
-        ```
-        docker build -t=phaseaug --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --build-arg USER_NAME=$USER
-        ```
-        - Cloned [official HiFi-GAN repo](https://github.com/jik876/hifi-gan).
-        - Downloaded [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/).
-        - (optional) [MelGAN](https://github.com/descriptinc/melgan-neurips) generator
-        
-        ## Training
-        0. Clone this repository and copy python files to hifi-gan folder
-        ```bash
-        git clone --recursive https://github.com/mindslab-ai/phaseaug
-        cp ./phaseaug/*.py ./phaseaug/hifi-gan/
-        cd ./phaseaug/hifi-gan
-        ```
-        
-          - optional: MelGAN generator
-          ```bash
-          cp ./phaseaug/config_v1_melgan.json ./phaseaug/hifi-gan/
-          ```
-          - Change generator to MelGAN generator at train.py
-          ```python
-          # import MelGanGenerator as Generator at [train.py](./train.py)
-          #from models import Generator # remove original import Generator
-          from models import MelGANGenerator as Generator
-          ```
-        
-        1. Modify dataset path at `train.py`
-        ```python
-             parser.add_argument('--input_wavs_dir',
-                                 default='path/LJSpeech-1.1/wavs_22k')
-             parser.add_argument('--input_mels_dir',
-                                 default='path/LJSpeech-1.1/wavs_22k')
-        ```
-        
-        2. Run train.py
-        ```
-        python train.py --config config_v1.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_hifigan
-        ```
-        ```
-        python train.py --config config_v1_melgan.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_melgan
-        ```
-        
-        
-        ## References
-        This implementation uses code from following repositories:
-        - [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
-        - [Official MelGAN implementation](https://github.com/descriptinc/melgan-neurips)
-        - [Official CARGAN implementation](https://github.com/descriptinc/cargan)
-        - [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
-        
-        This README and the webpage for the audio samples are inspired by:
-        - [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/)
-        - [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
-        
-        ## Citation & Contact
-        
-        If this repostory useful for yout research, please consider citing!
-        ```bib
-        @inproceedings{phaseaug,
-          author={Lee, Junhyeok and Han, Seungu and Cho, Hyunjae and Jung, Wonbin},
-          title={{PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping}},
-          journal = {arXiv preprint arXiv:2211.04610},
-          year=2022,
-        }
-        ```
-        If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@mindslab.ai](mailto:jun3518@mindslab.ai)
-        
-        
-Keywords: torch,pytorch,augmentation,diffaugment,speech synthesis,vocoder
-Platform: UNKNOWN
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+    # usually net_d parts are inside of autocast(enabled=True)
+    y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = net_d(aug_y, aug_y_g)
+
+```
+
+## Requirements
+- [PyTorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+- Support PyTorch>=2.0.0
+- The requirements are highlighted in [requirements.txt](./requirements.txt).
+- We also provide docker setup [Dockerfile](./Dockerfile).
+```
+docker build -t=phaseaug --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --build-arg USER_NAME=$USER
+```
+- Cloned [official HiFi-GAN repo](https://github.com/jik876/hifi-gan).
+- Downloaded [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/).
+- (optional) [MelGAN](https://github.com/descriptinc/melgan-neurips) generator
+
+## Training
+0. Clone this repository and copy python files to hifi-gan folder
+```bash
+git clone --recursive https://github.com/mindslab-ai/phaseaug
+cp ./phaseaug/*.py ./phaseaug/hifi-gan/
+cd ./phaseaug/hifi-gan
+```
+
+  - optional: MelGAN generator
+  ```bash
+  cp ./phaseaug/config_v1_melgan.json ./phaseaug/hifi-gan/
+  ```
+  - Change generator to MelGAN generator at train.py
+  ```python
+  # import MelGanGenerator as Generator at [train.py](./train.py)
+  #from models import Generator # remove original import Generator
+  from models import MelGANGenerator as Generator
+  ```
+
+1. Modify dataset path at `train.py`
+```python
+     parser.add_argument('--input_wavs_dir',
+                         default='path/LJSpeech-1.1/wavs_22k')
+     parser.add_argument('--input_mels_dir',
+                         default='path/LJSpeech-1.1/wavs_22k')
+```
+
+2. Run train.py
+```
+python train.py --config config_v1.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_hifigan
+```
+```
+python train.py --config config_v1_melgan.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_melgan
+```
+
+
+## References
+This implementation uses code from following repositories:
+- [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
+- [Official MelGAN implementation](https://github.com/descriptinc/melgan-neurips)
+- [Official CARGAN implementation](https://github.com/descriptinc/cargan)
+- [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+
+This README and the webpage for the audio samples are inspired by:
+- [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/)
+- [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
+
+## Citation & Contact
+
+If this repostory useful for yout research, please consider citing!
+```bib
+@inproceedings{phaseaug,
+  author={Lee, Junhyeok and Han, Seungu and Cho, Hyunjae and Jung, Wonbin},
+  title={{PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping}},
+  journal = {arXiv preprint arXiv:2211.04610},
+  year=2022,
+}
+```
+
+Bibtex will be updated after ICASSP 2023.
+
+If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@icloud.com](mailto:jun3518@icloud.com)
+
```

### Comparing `phaseaug-0.0.2/README.md` & `phaseaug-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,85 @@
+Metadata-Version: 2.1
+Name: phaseaug
+Version: 1.0.0
+Summary: PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping
+Home-page: https://github.com/mindslab-ai/phaseaug
+Author: junjun3518
+Author-email: junjun3518@gmail.com
+License: UNKNOWN
+Keywords: torch,pytorch,augmentation,diffaugment,speech synthesis,vocoder
+Platform: UNKNOWN
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PhaseAug
 
 **PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping**<br>
 Junhyeok Lee, Seungu Han, Hyunjae Cho, Wonbin Jung @ [MINDsLab Inc.](https://github.com/mindslab-ai), SNU, KAIST
 
 [![arXiv](https://img.shields.io/badge/arXiv-2211.04610-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2211.04610) [![GitHub Repo stars](https://img.shields.io/github/stars/mindslab-ai/phaseaug?color=yellow&label=PhaseAug&logo=github&style=flat-square)](https://github.com/mindslab-ai/phaseaug) [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://mindslab-ai.github.io/phaseaug/)
 
 
 **Abstract** : Previous generative adversarial network (GAN)-based neural vocoders are trained to reconstruct the exact ground truth waveform from the paired mel-spectrogram and do not consider the one-to-many relationship of speech synthesis. This conventional training causes overfitting for both the discriminators and the generator, leading to the periodicity artifacts in the generated audio signal. In this work, we present PhaseAug, the first differentiable augmentation for speech synthesis that rotates the phase of each frequency bin to simulate one-to-many mapping. With our proposed method, we outperform baselines without any architecture modification. Code and audio samples will be available at https://github.com/mindslab-ai/phaseaug.
 
-Submitted to ICASSP 2023
+Accepted to ICASSP 2023
 
 ![phasor](asset/phaseaug_phasor.png) 
 
 
 ## TODO
-- Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012
-- Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added.
-- We will uplade PhaseAug to [pypi](https://pypi.org).
+- [x] PyTorch 2.0 is released, need to modify STFT and iSTFT for complex support (solved at `1.0.0`)
+- [x] Arxiv updated
+- [x] Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012.
+- [x] Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added. -> transpose m,k to reduce ambiguity
+- [x] Upload PhaseAug to [pypi](https://pypi.org/project/phaseaug/).
+- [x] Upload [VITS](https://arxiv.org/abs/2106.06103)+PhaseAug sampels at demo page.
+- [x] Refactoring codes for packaging.
+
 
 ## Use PhaseAug
 - Install `alias-free-torch==0.0.6` and `phaseaug`
 ```bash
 pip install alias-free-torch==0.0.6 phaseaug 
 ```
 - Insert PhaseAug in your code, check [train.py](./train.py) as a example.
 ```python
-from phaseaug import PhaseAug
+from phaseaug.phaseaug import PhaseAug
 ...
 # define phaseaug
 aug = PhaseAug()
 ...
-#discriminator update phase
+# discriminator update phase
 aug_y, aug_y_g = aug.forward_sync(y, y_g_hat.detach())
 y_df_hat_r, y_df_hat_g, _, _ = mpd(aug_y, aug_y_g)
 y_ds_hat_r, y_ds_hat_g, _, _ = msd(aug_y, aug_y_g)
 ...
-#generator update phase
+# generator update phase
 aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
-y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(
-                        aug_y, aug_y_g)
-y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(
-                        aug_y, aug_y_g)
+y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(aug_y, aug_y_g)
+y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(aug_y, aug_y_g)
+```
+
+- If you are applying `torch.cuda.amp.autocast` like [VITS](https://github.com/jaywalnut310/vits), you need to wrap PhaseAug with `autocast(enabled=False)` to prevent [ComplexHalf issue](https://github.com/jaywalnut310/vits/issues/15).
+```python
+from torch.cuda.amp import autocast
+...
+with autocast(enabled=True)
+    # wrapping PhaseAug with autocast(enabled=False)
+    with autocast(enabled=False)
+        aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
+    # usually net_d parts are inside of autocast(enabled=True)
+    y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = net_d(aug_y, aug_y_g)
+
 ```
 
 ## Requirements
-- [Pytorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+- [PyTorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+- Support PyTorch>=2.0.0
 - The requirements are highlighted in [requirements.txt](./requirements.txt).
 - We also provide docker setup [Dockerfile](./Dockerfile).
 ```
 docker build -t=phaseaug --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --build-arg USER_NAME=$USER
 ```
 - Cloned [official HiFi-GAN repo](https://github.com/jik876/hifi-gan).
 - Downloaded [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/).
@@ -108,9 +139,14 @@
 @inproceedings{phaseaug,
   author={Lee, Junhyeok and Han, Seungu and Cho, Hyunjae and Jung, Wonbin},
   title={{PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping}},
   journal = {arXiv preprint arXiv:2211.04610},
   year=2022,
 }
 ```
-If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@mindslab.ai](mailto:jun3518@mindslab.ai)
+
+Bibtex will be updated after ICASSP 2023.
+
+If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@icloud.com](mailto:jun3518@icloud.com)
+
+
```

### Comparing `phaseaug-0.0.2/phaseaug/phaseaug.py` & `phaseaug-1.0.0/phaseaug/phaseaug.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,24 @@
         hop=256, 
         use_filter=True,
         var=6.0,
         delta_max=2.0, 
         cutoff=0.05, 
         half_width=0.012, 
         kernel_size=128, 
-        filter_padding='constant'
+        filter_padding='constant',
+        complex_calc=None
     ):
         super().__init__()
         self.nfft = nfft
         self.hop = hop
         self.var = var
         self.delta_max = delta_max
         self.use_filter = use_filter
+        self.complex_calc = complex_calc
         self.register_buffer('window', torch.hann_window(nfft))
         self.register_buffer('phi_ref', torch.arange(nfft // 2 + 1).unsqueeze(0) * 2 * pi / nfft)
 
         if use_filter:
             self.lpf = LPF(cutoff, half_width, kernel_size=kernel_size, padding_mode=filter_padding)
             def sample_phi(self, batch_size):
                 mu = self.lpf(
@@ -42,74 +44,77 @@
                     torch.randn([batch_size, self.nfft // 2 + 1], device=self.phi_ref.device) +
                     self.delta_max * (2. * torch.rand([batch_size, 1], device=self.phi_ref.device) - 1.)
                 )
                 phi = mu * self.phi_ref
                 return phi   #[B,nfft//2+1]
         self.sample_phi = sample_phi
 
+        if complex_calc or int(torch.__version__[0])>=2:
+            def stft_rot_istft(self, x, phi):
+                X = torch.stft(
+                    x,
+                    self.nfft,
+                    self.hop,
+                    window=self.window,
+                    return_complex=True
+                )  #[B,F,T]
+                
+                rot = torch.exp(torch.tensor([(0.+1.j)], dtype = torch.complex64, device = x.device) * phi) #[B,F,1]
+                X_aug = X * rot
+                x_aug = torch.istft(
+                    X_aug,
+                    self.nfft,
+                    self.hop,
+                    window=self.window,
+                    return_complex=False
+                ).unsqueeze(1)
+                return x_aug
+        else:
+            def stft_rot_istft(self, x, phi):          
+                X = torch.stft(
+                    x,
+                    self.nfft,
+                    self.hop,
+                    window=self.window,
+                    return_complex=False
+                )  #[B,F,T,2]
+
+                phi_cos = phi.cos()
+                phi_sin = phi.sin()
+                rot_mat = torch.cat(
+                    [phi_cos, -phi_sin, phi_sin, phi_cos],  #[B,F,2,2]
+                    dim=-1).view(-1, self.nfft // 2 + 1, 2, 2)
+                # We did not mention that we multiplied rot_mat to "the left side of X"
+                # Paper will be modified at rebuttal phase for clarity.
+                X_aug = torch.einsum('bfij ,bftj->bfti', rot_mat, X)
+                x_aug = torch.istft(
+                    X_aug,
+                    self.nfft,
+                    self.hop,
+                    window=self.window,
+                    return_complex=False
+                ).unsqueeze(1)
+                return x_aug
+        self.stft_rot_istft = stft_rot_istft
+        
     # x: audio [B,1,T] -> [B,1,T]
     # phi: [B,nfft//2+1]
     # also possible for x :[B,C,T] but we did not generalize it.
     def forward(self, x, phi=None):
         x = x.squeeze(1)  #[B,t]
-        X = torch.stft(
-            x,
-            self.nfft,
-            self.hop,
-            window=self.window,
-            return_complex=False
-        )  #[B,F,T,2]
         if phi is None:
             phi = self.sample_phi(self, X.shape[0])
-
         phi[:, 0] = 0. # we are multiplying phi_ref to mu, so it is always zero in our scheme
         phi = phi.unsqueeze(-1)  #[B,F,1]
-        phi_cos = phi.cos()
-        phi_sin = phi.sin()
-        rot_mat = torch.cat(
-            [phi_cos, -phi_sin, phi_sin, phi_cos],  #[B,F,2,2]
-            dim=-1).view(-1, self.nfft // 2 + 1, 2, 2)
-        # We did not mention that we multiplied rot_mat to "the left side of X"
-        # Paper will be modified at rebuttal phase for clarity.
-        X_aug = torch.einsum('bfij ,bftj->bfti', rot_mat, X)
-        x_aug = torch.istft(
-            X_aug,
-            self.nfft,
-            self.hop,
-            window=self.window,
-            return_complex=False
-        )
-        return x_aug.unsqueeze(1)  #[B,1,t]
+        x_aug = self.stft_rot_istft(self, x, phi)
+        return x_aug  #[B,1,t]
 
     # x: audio [B,1,T] -> [B,1,T]
     # phi: [B,nfft//2+1]
     def forward_sync(self, x, x_hat, phi=None):
-        x = torch.cat([x, x_hat], dim=0).squeeze(1) #[2B,t]
-        X = torch.stft(
-            x,
-            self.nfft,
-            self.hop,
-            window=self.window,
-            return_complex=False
-        )  #[2B,F,T,2]
+        B = x.shape[0]
+        x = torch.cat([x, x_hat], dim=0) #[2B,1,t]
         if phi is None:
-            phi = self.sample_phi(self, X.shape[0] // 2)
+            phi = self.sample_phi(self, X.shape[0] // 2) #[2B, nfft//2+1]
         phi = torch.cat([phi, phi], dim=0)
-
-        phi[:, 0] = 0. # we are multiplying phi_ref to mu, so it is always zero in our scheme
-        phi = phi.unsqueeze(-1)  #[2B,F,1]
-        phi_cos = phi.cos()
-        phi_sin = phi.sin()
-        rot_mat = torch.cat(
-            [phi_cos, -phi_sin, phi_sin, phi_cos],  #[2B,F,2,2]
-            dim=-1).view(-1, self.nfft // 2 + 1, 2, 2)
-        # We did not mention that we multiplied rot_mat to "the left side of X"
-        # Paper will be modified at rebuttal phase for clarity.
-        X_aug = torch.einsum('bfij ,bftj->bfti', rot_mat, X)
-        x_aug = torch.istft(
-            X_aug,
-            self.nfft,
-            self.hop,
-            window=self.window,
-            return_complex=False
-        )
-        return x_aug.unsqueeze(1).split(x_aug.shape[0] // 2, dim=0)  #[B,1,t],[B,1,t]
+        x_augs = self.forward(x, phi).split(B, dim=0)
+        return x_augs
```

### Comparing `phaseaug-0.0.2/phaseaug.egg-info/PKG-INFO` & `phaseaug-1.0.0/phaseaug.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,152 @@
 Metadata-Version: 2.1
 Name: phaseaug
-Version: 0.0.2
+Version: 1.0.0
 Summary: PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping
 Home-page: https://github.com/mindslab-ai/phaseaug
 Author: junjun3518
 Author-email: junjun3518@gmail.com
 License: UNKNOWN
-Description: # PhaseAug
-        
-        **PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping**<br>
-        Junhyeok Lee, Seungu Han, Hyunjae Cho, Wonbin Jung @ [MINDsLab Inc.](https://github.com/mindslab-ai), SNU, KAIST
-        
-        [![arXiv](https://img.shields.io/badge/arXiv-2211.04610-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2211.04610) [![GitHub Repo stars](https://img.shields.io/github/stars/mindslab-ai/phaseaug?color=yellow&label=PhaseAug&logo=github&style=flat-square)](https://github.com/mindslab-ai/phaseaug) [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://mindslab-ai.github.io/phaseaug/)
-        
-        
-        **Abstract** : Previous generative adversarial network (GAN)-based neural vocoders are trained to reconstruct the exact ground truth waveform from the paired mel-spectrogram and do not consider the one-to-many relationship of speech synthesis. This conventional training causes overfitting for both the discriminators and the generator, leading to the periodicity artifacts in the generated audio signal. In this work, we present PhaseAug, the first differentiable augmentation for speech synthesis that rotates the phase of each frequency bin to simulate one-to-many mapping. With our proposed method, we outperform baselines without any architecture modification. Code and audio samples will be available at https://github.com/mindslab-ai/phaseaug.
-        
-        Submitted to ICASSP 2023
-        
-        ![phasor](asset/phaseaug_phasor.png) 
-        
-        
-        ## TODO
-        - Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012
-        - Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added.
-        - We will uplade PhaseAug to [pypi](https://pypi.org).
-        
-        ## Use PhaseAug
-        - Install `alias-free-torch==0.0.6` and `phaseaug`
-        ```bash
-        pip install alias-free-torch==0.0.6 phaseaug 
-        ```
-        - Insert PhaseAug in your code, check [train.py](./train.py) as a example.
-        ```python
-        from phaseaug import PhaseAug
-        ...
-        # define phaseaug
-        aug = PhaseAug()
-        ...
-        #discriminator update phase
-        aug_y, aug_y_g = aug.forward_sync(y, y_g_hat.detach())
-        y_df_hat_r, y_df_hat_g, _, _ = mpd(aug_y, aug_y_g)
-        y_ds_hat_r, y_ds_hat_g, _, _ = msd(aug_y, aug_y_g)
-        ...
-        #generator update phase
-        aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
-        y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(
-                                aug_y, aug_y_g)
-        y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(
-                                aug_y, aug_y_g)
-        ```
-        
-        ## Requirements
-        - [Pytorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
-        - The requirements are highlighted in [requirements.txt](./requirements.txt).
-        - We also provide docker setup [Dockerfile](./Dockerfile).
-        ```
-        docker build -t=phaseaug --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --build-arg USER_NAME=$USER
-        ```
-        - Cloned [official HiFi-GAN repo](https://github.com/jik876/hifi-gan).
-        - Downloaded [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/).
-        - (optional) [MelGAN](https://github.com/descriptinc/melgan-neurips) generator
-        
-        ## Training
-        0. Clone this repository and copy python files to hifi-gan folder
-        ```bash
-        git clone --recursive https://github.com/mindslab-ai/phaseaug
-        cp ./phaseaug/*.py ./phaseaug/hifi-gan/
-        cd ./phaseaug/hifi-gan
-        ```
-        
-          - optional: MelGAN generator
-          ```bash
-          cp ./phaseaug/config_v1_melgan.json ./phaseaug/hifi-gan/
-          ```
-          - Change generator to MelGAN generator at train.py
-          ```python
-          # import MelGanGenerator as Generator at [train.py](./train.py)
-          #from models import Generator # remove original import Generator
-          from models import MelGANGenerator as Generator
-          ```
-        
-        1. Modify dataset path at `train.py`
-        ```python
-             parser.add_argument('--input_wavs_dir',
-                                 default='path/LJSpeech-1.1/wavs_22k')
-             parser.add_argument('--input_mels_dir',
-                                 default='path/LJSpeech-1.1/wavs_22k')
-        ```
-        
-        2. Run train.py
-        ```
-        python train.py --config config_v1.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_hifigan
-        ```
-        ```
-        python train.py --config config_v1_melgan.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_melgan
-        ```
-        
-        
-        ## References
-        This implementation uses code from following repositories:
-        - [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
-        - [Official MelGAN implementation](https://github.com/descriptinc/melgan-neurips)
-        - [Official CARGAN implementation](https://github.com/descriptinc/cargan)
-        - [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
-        
-        This README and the webpage for the audio samples are inspired by:
-        - [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/)
-        - [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
-        
-        ## Citation & Contact
-        
-        If this repostory useful for yout research, please consider citing!
-        ```bib
-        @inproceedings{phaseaug,
-          author={Lee, Junhyeok and Han, Seungu and Cho, Hyunjae and Jung, Wonbin},
-          title={{PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping}},
-          journal = {arXiv preprint arXiv:2211.04610},
-          year=2022,
-        }
-        ```
-        If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@mindslab.ai](mailto:jun3518@mindslab.ai)
-        
-        
 Keywords: torch,pytorch,augmentation,diffaugment,speech synthesis,vocoder
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PhaseAug
+
+**PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping**<br>
+Junhyeok Lee, Seungu Han, Hyunjae Cho, Wonbin Jung @ [MINDsLab Inc.](https://github.com/mindslab-ai), SNU, KAIST
+
+[![arXiv](https://img.shields.io/badge/arXiv-2211.04610-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2211.04610) [![GitHub Repo stars](https://img.shields.io/github/stars/mindslab-ai/phaseaug?color=yellow&label=PhaseAug&logo=github&style=flat-square)](https://github.com/mindslab-ai/phaseaug) [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://mindslab-ai.github.io/phaseaug/)
+
+
+**Abstract** : Previous generative adversarial network (GAN)-based neural vocoders are trained to reconstruct the exact ground truth waveform from the paired mel-spectrogram and do not consider the one-to-many relationship of speech synthesis. This conventional training causes overfitting for both the discriminators and the generator, leading to the periodicity artifacts in the generated audio signal. In this work, we present PhaseAug, the first differentiable augmentation for speech synthesis that rotates the phase of each frequency bin to simulate one-to-many mapping. With our proposed method, we outperform baselines without any architecture modification. Code and audio samples will be available at https://github.com/mindslab-ai/phaseaug.
+
+Accepted to ICASSP 2023
+
+![phasor](asset/phaseaug_phasor.png) 
+
+
+## TODO
+- [x] PyTorch 2.0 is released, need to modify STFT and iSTFT for complex support (solved at `1.0.0`)
+- [x] Arxiv updated
+- [x] Errata in paper will be fixed. Section 2.5 in paper, transition band half-width 0.06-> 0.012.
+- [x] Section 2.5, mention about multiplyinng rotation matrix to "the left side of F(x)" will be added. -> transpose m,k to reduce ambiguity
+- [x] Upload PhaseAug to [pypi](https://pypi.org/project/phaseaug/).
+- [x] Upload [VITS](https://arxiv.org/abs/2106.06103)+PhaseAug sampels at demo page.
+- [x] Refactoring codes for packaging.
+
+
+## Use PhaseAug
+- Install `alias-free-torch==0.0.6` and `phaseaug`
+```bash
+pip install alias-free-torch==0.0.6 phaseaug 
+```
+- Insert PhaseAug in your code, check [train.py](./train.py) as a example.
+```python
+from phaseaug.phaseaug import PhaseAug
+...
+# define phaseaug
+aug = PhaseAug()
+...
+# discriminator update phase
+aug_y, aug_y_g = aug.forward_sync(y, y_g_hat.detach())
+y_df_hat_r, y_df_hat_g, _, _ = mpd(aug_y, aug_y_g)
+y_ds_hat_r, y_ds_hat_g, _, _ = msd(aug_y, aug_y_g)
+...
+# generator update phase
+aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
+y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = mpd(aug_y, aug_y_g)
+y_ds_hat_r, y_ds_hat_g, fmap_s_r, fmap_s_g = msd(aug_y, aug_y_g)
+```
+
+- If you are applying `torch.cuda.amp.autocast` like [VITS](https://github.com/jaywalnut310/vits), you need to wrap PhaseAug with `autocast(enabled=False)` to prevent [ComplexHalf issue](https://github.com/jaywalnut310/vits/issues/15).
+```python
+from torch.cuda.amp import autocast
+...
+with autocast(enabled=True)
+    # wrapping PhaseAug with autocast(enabled=False)
+    with autocast(enabled=False)
+        aug_y, aug_y_g = aug.forward_sync(y, y_g_hat)
+    # usually net_d parts are inside of autocast(enabled=True)
+    y_df_hat_r, y_df_hat_g, fmap_f_r, fmap_f_g = net_d(aug_y, aug_y_g)
+
+```
+
+## Requirements
+- [PyTorch>=1.7.0](https://pytorch.org/) for [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+- Support PyTorch>=2.0.0
+- The requirements are highlighted in [requirements.txt](./requirements.txt).
+- We also provide docker setup [Dockerfile](./Dockerfile).
+```
+docker build -t=phaseaug --build-arg USER_ID=$(id -u) --build-arg GROUP_ID=$(id -g) --build-arg USER_NAME=$USER
+```
+- Cloned [official HiFi-GAN repo](https://github.com/jik876/hifi-gan).
+- Downloaded [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/).
+- (optional) [MelGAN](https://github.com/descriptinc/melgan-neurips) generator
+
+## Training
+0. Clone this repository and copy python files to hifi-gan folder
+```bash
+git clone --recursive https://github.com/mindslab-ai/phaseaug
+cp ./phaseaug/*.py ./phaseaug/hifi-gan/
+cd ./phaseaug/hifi-gan
+```
+
+  - optional: MelGAN generator
+  ```bash
+  cp ./phaseaug/config_v1_melgan.json ./phaseaug/hifi-gan/
+  ```
+  - Change generator to MelGAN generator at train.py
+  ```python
+  # import MelGanGenerator as Generator at [train.py](./train.py)
+  #from models import Generator # remove original import Generator
+  from models import MelGANGenerator as Generator
+  ```
+
+1. Modify dataset path at `train.py`
+```python
+     parser.add_argument('--input_wavs_dir',
+                         default='path/LJSpeech-1.1/wavs_22k')
+     parser.add_argument('--input_mels_dir',
+                         default='path/LJSpeech-1.1/wavs_22k')
+```
+
+2. Run train.py
+```
+python train.py --config config_v1.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_hifigan
+```
+```
+python train.py --config config_v1_melgan.json --aug --filter --data_ratio {0.01/0.1/1.} --name phaseaug_melgan
+```
+
+
+## References
+This implementation uses code from following repositories:
+- [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
+- [Official MelGAN implementation](https://github.com/descriptinc/melgan-neurips)
+- [Official CARGAN implementation](https://github.com/descriptinc/cargan)
+- [alias-free-torch](https://github.com/junjun3518/alias-free-torch)
+
+This README and the webpage for the audio samples are inspired by:
+- [LJ Speech Dataset](https://keithito.com/LJ-Speech-Dataset/)
+- [Official HiFi-GAN implementation](https://github.com/jik876/hifi-gan)
+
+## Citation & Contact
+
+If this repostory useful for yout research, please consider citing!
+```bib
+@inproceedings{phaseaug,
+  author={Lee, Junhyeok and Han, Seungu and Cho, Hyunjae and Jung, Wonbin},
+  title={{PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping}},
+  journal = {arXiv preprint arXiv:2211.04610},
+  year=2022,
+}
+```
+
+Bibtex will be updated after ICASSP 2023.
+
+If you have a question or any kind of inquiries, please contact Junhyeok Lee at [jun3518@icloud.com](mailto:jun3518@icloud.com)
+
+
+
```

### Comparing `phaseaug-0.0.2/setup.py` & `phaseaug-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name                = 'phaseaug',
-    version             = '0.0.2',
+    version             = '1.0.0',
     description         = 'PhaseAug: A Differentiable Augmentation for Speech Synthesis to Simulate One-to-Many Mapping',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author              = 'junjun3518',
     author_email        = 'junjun3518@gmail.com',
     url                 = 'https://github.com/mindslab-ai/phaseaug',
     install_requires    = ['torch', 'alias-free-torch'],
```

