# Comparing `tmp/pyGPUreg-0.1.2.tar.gz` & `tmp/pyGPUreg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGPUreg-0.1.2.tar", last modified: Wed Apr 19 10:27:33 2023, max compression
+gzip compressed data, was "pyGPUreg-0.1.3.tar", last modified: Thu Apr 20 15:04:29 2023, max compression
```

## Comparing `pyGPUreg-0.1.2.tar` & `pyGPUreg-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/
--rw-rw-rw-   0        0        0    17099 2023-03-23 08:54:10.000000 pyGPUreg-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       73 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4777 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.327499 pyGPUreg-0.1.2/pyGPUreg/
--rw-rw-rw-   0        0        0      114 2023-04-19 10:23:37.000000 pyGPUreg-0.1.2/pyGPUreg/__init__.py
--rw-rw-rw-   0        0        0     5995 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/opengl_classes.py
--rw-rw-rw-   0        0        0    28338 2023-04-19 10:24:44.000000 pyGPUreg-0.1.2/pyGPUreg/pyGPUreg.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/pyGPUreg/shaders/
--rw-rw-rw-   0        0        0     1477 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/butterflytexture.glsl
--rw-rw-rw-   0        0        0      398 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/copy_r_to_rg.glsl
--rw-rw-rw-   0        0        0      392 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/cos_filter.glsl
--rw-rw-rw-   0        0        0      404 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/cos_filter_r.glsl
--rw-rw-rw-   0        0        0     3377 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft.glsl
--rw-rw-rw-   0        0        0      746 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation.glsl
--rw-rw-rw-   0        0        0      458 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
--rw-rw-rw-   0        0        0      532 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation.glsl
--rw-rw-rw-   0        0        0      582 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation_single.glsl
--rw-rw-rw-   0        0        0     2802 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_single.glsl
--rw-rw-rw-   0        0        0      805 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/resample_image.glsl
-drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.335559 pyGPUreg-0.1.2/pyGPUreg.egg-info/
--rw-rw-rw-   0        0        0      274 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-04-19 10:27:30.000000 pyGPUreg-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/
+-rw-rw-rw-   0        0        0    17099 2023-03-23 08:54:10.000000 pyGPUreg-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       73 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4777 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.180385 pyGPUreg-0.1.3/pyGPUreg/
+-rw-rw-rw-   0        0        0      114 2023-04-20 15:04:22.000000 pyGPUreg-0.1.3/pyGPUreg/__init__.py
+-rw-rw-rw-   0        0        0     5995 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/opengl_classes.py
+-rw-rw-rw-   0        0        0    28476 2023-04-20 15:04:19.000000 pyGPUreg-0.1.3/pyGPUreg/pyGPUreg.py
+drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/pyGPUreg/shaders/
+-rw-rw-rw-   0        0        0     1477 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/butterflytexture.glsl
+-rw-rw-rw-   0        0        0      398 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/copy_r_to_rg.glsl
+-rw-rw-rw-   0        0        0      392 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/cos_filter.glsl
+-rw-rw-rw-   0        0        0      404 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/cos_filter_r.glsl
+-rw-rw-rw-   0        0        0     3377 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft.glsl
+-rw-rw-rw-   0        0        0      746 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation.glsl
+-rw-rw-rw-   0        0        0      458 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
+-rw-rw-rw-   0        0        0      532 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation.glsl
+-rw-rw-rw-   0        0        0      582 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation_single.glsl
+-rw-rw-rw-   0        0        0     2802 2023-03-22 07:56:15.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/fft_single.glsl
+-rw-rw-rw-   0        0        0      805 2023-04-19 10:23:36.000000 pyGPUreg-0.1.3/pyGPUreg/shaders/resample_image.glsl
+drwxrwxrwx   0        0        0        0 2023-04-20 15:04:29.196013 pyGPUreg-0.1.3/pyGPUreg.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 15:04:29.000000 pyGPUreg-0.1.3/pyGPUreg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 15:04:29.211521 pyGPUreg-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-04-20 15:04:24.000000 pyGPUreg-0.1.3/setup.py
```

### Comparing `pyGPUreg-0.1.2/LICENSE.txt` & `pyGPUreg-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/README.md` & `pyGPUreg-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/opengl_classes.py` & `pyGPUreg-0.1.3/pyGPUreg/opengl_classes.py`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/pyGPUreg.py` & `pyGPUreg-0.1.3/pyGPUreg/pyGPUreg.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,27 +66,26 @@
     glfw.window_hint(glfw.CONTEXT_VERSION_MINOR, GLFW_CONTEXT_VERSION_MINOR)
     glfw.window_hint(glfw.OPENGL_PROFILE, glfw.OPENGL_CORE_PROFILE)
     glfw.window_hint(glfw.OPENGL_FORWARD_COMPAT, GL_TRUE)
     window = glfw.create_window(2, 2, "pyGPUreg hidden window", None, None)
     glfw.make_context_current(window)
 
     # compile shaders
-    shader_dir = os.path.join(os.path.dirname(__file__))+"\\shaders\\"
-    cs_butterfly = Shader(shader_dir + "butterflytexture.glsl")
-    cs_cosft = Shader(shader_dir + "cos_filter.glsl")
-    cs_fft = Shader(shader_dir + "fft.glsl")
-    cs_fft_pi = Shader(shader_dir + "fft_inversion_permutation.glsl")
-    cs_multiply = Shader(shader_dir + "fft_phase_correlation.glsl")
-    cs_resample = Shader(shader_dir + "resample_image.glsl")
-
-    cs_fft_single = Shader(shader_dir + "fft_single.glsl")
-    cs_fft_pi_single = Shader(shader_dir + "fft_inversion_permutation_single.glsl")
-    cs_multiply_single = Shader(shader_dir + "fft_phase_correlation_single.glsl")
-    cs_copy_r_to_rg = Shader(shader_dir + "copy_r_to_rg.glsl")
-    cs_cosft_single = Shader(shader_dir + "cos_filter_r.glsl")
+    shader_dir = os.path.join(os.path.dirname(__file__), "shaders")
+    cs_butterfly = Shader(os.path.join(shader_dir, "butterflytexture.glsl"))
+    cs_cosft = Shader(os.path.join(shader_dir, "cos_filter.glsl"))
+    cs_fft = Shader(os.path.join(shader_dir, "fft.glsl"))
+    cs_fft_pi = Shader(os.path.join(shader_dir, "fft_inversion_permutation.glsl"))
+    cs_multiply = Shader(os.path.join(shader_dir, "fft_phase_correlation.glsl"))
+    cs_resample = Shader(os.path.join(shader_dir, "resample_image.glsl"))
+    cs_fft_single = Shader(os.path.join(shader_dir, "fft_single.glsl"))
+    cs_fft_pi_single = Shader(os.path.join(shader_dir, "fft_inversion_permutation_single.glsl"))
+    cs_multiply_single = Shader(os.path.join(shader_dir, "fft_phase_correlation_single.glsl"))
+    cs_copy_r_to_rg = Shader(os.path.join(shader_dir, "copy_r_to_rg.glsl"))
+    cs_cosft_single = Shader(os.path.join(shader_dir, "cos_filter_r.glsl"))
 
 
 def set_image_size(size):
     global image_size, log_image_size, compute_space_size, texture_butterfly, texture_cos_mask, texture_data, texture_data_buffer, texture_resample_a, texture_resample_b, texture_r_t, texture_r_i, texture_rg_T, texture_rg_I, texture_rg_buffer
 
     # check size
     N = int(size)
```

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/butterflytexture.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/butterflytexture.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/fft.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/fft.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_inversion_permutation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation_single.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_phase_correlation_single.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_single.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/fft_single.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg/shaders/resample_image.glsl` & `pyGPUreg-0.1.3/pyGPUreg/shaders/resample_image.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/pyGPUreg.egg-info/SOURCES.txt` & `pyGPUreg-0.1.3/pyGPUreg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.2/setup.py` & `pyGPUreg-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyGPUreg',
-    version='0.1.2',
+    version='0.1.3',
     license='GPLv3',
     author="Mart G.F. Last",
     author_email='m.g.f.last@lumc.nl',
     description='GPU-accelerated image registration.\ngithub.com/bionanopatterning/pyGPUreg',
     packages=find_packages(),
     package_data={'pyGPUreg': ['*.glsl', 'shaders/*glsl']},
     include_package_data=True,
```

