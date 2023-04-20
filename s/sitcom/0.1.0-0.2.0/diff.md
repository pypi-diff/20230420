# Comparing `tmp/sitcom-0.1.0.tar.gz` & `tmp/sitcom-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitcom-0.1.0.tar", max compression
+gzip compressed data, was "sitcom-0.2.0.tar", max compression
```

## Comparing `sitcom-0.1.0.tar` & `sitcom-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-04-20 09:49:15.900364 sitcom-0.1.0/LICENSE
--rw-r--r--   0        0        0      488 2023-04-20 10:21:06.940230 sitcom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0   669228 2022-11-06 01:18:32.000000 sitcom-0.1.0/src/sitcom/Lato-Semibold.ttf
--rw-r--r--   0        0        0      168 2023-01-18 17:37:14.000000 sitcom-0.1.0/src/sitcom/Pipfile
--rw-r--r--   0        0        0      497 2023-01-18 17:37:14.000000 sitcom-0.1.0/src/sitcom/Pipfile.lock
--rw-r--r--   0        0        0    84116 2023-04-07 11:04:38.000000 sitcom-0.1.0/src/sitcom/Sine_curve.png
--rw-r--r--   0        0        0      313 2023-04-19 08:07:39.639901 sitcom-0.1.0/src/sitcom/__init.py__
--rw-r--r--   0        0        0    47356 2023-04-20 10:13:25.505365 sitcom-0.1.0/src/sitcom/__main__.py
--rw-r--r--   0        0        0   539595 2023-04-07 03:05:36.000000 sitcom-0.1.0/src/sitcom/black.png
--rw-r--r--   0        0        0       60 2023-04-19 08:06:00.824504 sitcom-0.1.0/src/sitcom/config.toml
--rw-r--r--   0        0        0     1611 2023-04-18 06:48:20.931330 sitcom-0.1.0/src/sitcom/sfit.py
--rw-r--r--   0        0        0     6427 2023-04-20 10:08:30.303532 sitcom-0.1.0/src/sitcom/sirgraf.py
--rw-r--r--   0        0        0     1693 2023-04-19 12:35:24.173813 sitcom-0.1.0/src/sitcom/sitcom.egg-info/PKG-INFO
--rw-r--r--   0        0        0      325 2023-04-19 12:35:24.189813 sitcom-0.1.0/src/sitcom/sitcom.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-04-19 12:35:24.173813 sitcom-0.1.0/src/sitcom/sitcom.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       48 2023-04-19 12:35:24.173813 sitcom-0.1.0/src/sitcom/sitcom.egg-info/requires.txt
--rw-r--r--   0        0        0        7 2023-04-19 12:35:24.173813 sitcom-0.1.0/src/sitcom/sitcom.egg-info/top_level.txt
--rw-r--r--   0        0        0    37378 2023-04-20 10:07:37.111202 sitcom-0.1.0/src/sitcom/st1.py
--rw-r--r--   0        0        0     4577 2023-04-20 09:42:27.505828 sitcom-0.1.0/src/sitcom/st2.py
--rw-r--r--   0        0        0   599404 2023-04-07 03:03:58.000000 sitcom-0.1.0/src/sitcom/white.png
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 sitcom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-20 09:49:15.900364 sitcom-0.2.0/LICENSE
+-rw-r--r--   0        0        0      519 2023-04-20 11:11:42.935081 sitcom-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0   669228 2022-11-06 01:18:32.000000 sitcom-0.2.0/src/sitcom/Lato-Semibold.ttf
+-rw-r--r--   0        0        0      168 2023-01-18 17:37:14.000000 sitcom-0.2.0/src/sitcom/Pipfile
+-rw-r--r--   0        0        0      497 2023-01-18 17:37:14.000000 sitcom-0.2.0/src/sitcom/Pipfile.lock
+-rw-r--r--   0        0        0    84116 2023-04-07 11:04:38.000000 sitcom-0.2.0/src/sitcom/Sine_curve.png
+-rw-r--r--   0        0        0      313 2023-04-19 08:07:39.639901 sitcom-0.2.0/src/sitcom/__init.py__
+-rw-r--r--   0        0        0      697 2023-04-20 06:24:29.200074 sitcom-0.2.0/src/sitcom/__main__.py
+-rw-r--r--   0        0        0   539595 2023-04-07 03:05:36.000000 sitcom-0.2.0/src/sitcom/black.png
+-rw-r--r--   0        0        0       60 2023-04-19 08:06:00.824504 sitcom-0.2.0/src/sitcom/config.toml
+-rw-r--r--   0        0        0     1611 2023-04-18 06:48:20.931330 sitcom-0.2.0/src/sitcom/sfit.py
+-rw-r--r--   0        0        0     6413 2023-04-20 11:02:55.695807 sitcom-0.2.0/src/sitcom/sirgraf.py
+-rw-r--r--   0        0        0     1693 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-04-19 12:35:24.189813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       48 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/requires.txt
+-rw-r--r--   0        0        0        7 2023-04-19 12:35:24.173813 sitcom-0.2.0/src/sitcom/sitcom.egg-info/top_level.txt
+-rw-r--r--   0        0        0    47356 2023-04-20 11:01:59.431458 sitcom-0.2.0/src/sitcom/st.py
+-rw-r--r--   0        0        0    37378 2023-04-20 10:07:37.111202 sitcom-0.2.0/src/sitcom/st1.py
+-rw-r--r--   0        0        0     4577 2023-04-20 09:42:27.505828 sitcom-0.2.0/src/sitcom/st2.py
+-rw-r--r--   0        0        0   599404 2023-04-07 03:03:58.000000 sitcom-0.2.0/src/sitcom/white.png
+-rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 sitcom-0.2.0/PKG-INFO
```

### Comparing `sitcom-0.1.0/LICENSE` & `sitcom-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/Lato-Semibold.ttf` & `sitcom-0.2.0/src/sitcom/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/Sine_curve.png` & `sitcom-0.2.0/src/sitcom/Sine_curve.png`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/__main__.py` & `sitcom-0.2.0/src/sitcom/st.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/black.png` & `sitcom-0.2.0/src/sitcom/black.png`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/sfit.py` & `sitcom-0.2.0/src/sitcom/sfit.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/sirgraf.py` & `sitcom-0.2.0/src/sitcom/sirgraf.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 	ima,time=[],[]
 	#pool = multiprocessing.Pool(processes=multiprocessing.cpu_count())
 	for i in range(len(filenames)):
 		f1=fits.open(filenames[i],memmap=False)
 		time.append(f1[0].header['DATE-OBS'].split('T')[1].split('.')[0])
 		ima.append(np.flipud(f1[0].data))
 		f1.close()
-	gc.collect()
 	stack_image=np.array(ima)
 	min_image=np.copy(stack_image[0])
 	#Find minimum intensity images
 	for i in range(len(ima)):
 		for j in range(len(ima[0])):
 			b=stack_image[i,j,j]
 			if b>0:
```

### Comparing `sitcom-0.1.0/src/sitcom/sitcom.egg-info/PKG-INFO` & `sitcom-0.2.0/src/sitcom/sitcom.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/st1.py` & `sitcom-0.2.0/src/sitcom/st1.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/st2.py` & `sitcom-0.2.0/src/sitcom/st2.py`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/src/sitcom/white.png` & `sitcom-0.2.0/src/sitcom/white.png`

 * *Files identical despite different names*

### Comparing `sitcom-0.1.0/PKG-INFO` & `sitcom-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitcom
-Version: 0.1.0
+Version: 0.2.0
 Summary: SITCoM: SiRGraF Integrated Tool for Coronal dynaMics
 Author: Purvi Udhwani
 Author-email: purviaries@aries.res.in
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

