# Comparing `tmp/caesar-rock-0.0.8.tar.gz` & `tmp/caesar-rock-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.8.tar", last modified: Thu Apr 20 10:49:43 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.9.tar", last modified: Thu Apr 20 13:35:08 2023, max compression
```

## Comparing `caesar-rock-0.0.8.tar` & `caesar-rock-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.664378 caesar-rock-0.0.8/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     8490 2023-04-20 10:49:43.662435 caesar-rock-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8214 2023-04-20 10:47:01.000000 caesar-rock-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.617355 caesar-rock-0.0.8/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8490 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.657361 caesar-rock-0.0.8/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.8/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.8/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.8/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.8/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 10:49:43.665396 caesar-rock-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-20 10:49:25.000000 caesar-rock-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 13:35:08.395213 caesar-rock-0.0.9/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     8485 2023-04-20 13:35:08.394258 caesar-rock-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8209 2023-04-20 13:33:45.000000 caesar-rock-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 13:35:08.376603 caesar-rock-0.0.9/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8485 2023-04-20 13:35:08.000000 caesar-rock-0.0.9/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 13:35:08.000000 caesar-rock-0.0.9/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 13:35:08.000000 caesar-rock-0.0.9/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 13:35:08.000000 caesar-rock-0.0.9/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 13:35:08.000000 caesar-rock-0.0.9/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 13:35:08.391155 caesar-rock-0.0.9/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.9/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.9/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.9/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.9/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 13:35:08.395213 caesar-rock-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-20 13:34:00.000000 caesar-rock-0.0.9/setup.py
```

### Comparing `caesar-rock-0.0.8/LICENSE` & `caesar-rock-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.8/PKG-INFO` & `caesar-rock-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for estimating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -101,15 +101,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
 df = pd.read_csv('df_p.csv')
 
-ccs = RockStrengthLog(df = df_p,
+ccs = RockStrengthLog(df = df,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
                       limestone_equation = limestone_faquhar_porosity,
                       sandstone_equation = sandstone_edimann_porosity)
@@ -132,15 +132,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
 df = pd.read_csv('df_dt.csv')
 
-ccs = RockStrengthLog(df = df_dt,
+ccs = RockStrengthLog(df = df,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
                       limestone_equation = limestone_golubev_delta_tc,
                       sandstone_equation = sandstone_macnelly_delta_tc)
```

### Comparing `caesar-rock-0.0.8/README.md` & `caesar-rock-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
 df = pd.read_csv('df_p.csv')
 
-ccs = RockStrengthLog(df = df_p,
+ccs = RockStrengthLog(df = df,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
                       limestone_equation = limestone_faquhar_porosity,
                       sandstone_equation = sandstone_edimann_porosity)
@@ -122,15 +122,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
 df = pd.read_csv('df_dt.csv')
 
-ccs = RockStrengthLog(df = df_dt,
+ccs = RockStrengthLog(df = df,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
                       limestone_equation = limestone_golubev_delta_tc,
                       sandstone_equation = sandstone_macnelly_delta_tc)
```

### Comparing `caesar-rock-0.0.8/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.9/caesar_rock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for estimating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -101,15 +101,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
 df = pd.read_csv('df_p.csv')
 
-ccs = RockStrengthLog(df = df_p,
+ccs = RockStrengthLog(df = df,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
                       limestone_equation = limestone_faquhar_porosity,
                       sandstone_equation = sandstone_edimann_porosity)
@@ -132,15 +132,15 @@
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
 df = pd.read_csv('df_dt.csv')
 
-ccs = RockStrengthLog(df = df_dt,
+ccs = RockStrengthLog(df = df,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
                       limestone_equation = limestone_golubev_delta_tc,
                       sandstone_equation = sandstone_macnelly_delta_tc)
```

### Comparing `caesar-rock-0.0.8/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.9/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.8/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.9/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.8/caesarrock/ucs.py` & `caesar-rock-0.0.9/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.8/setup.py` & `caesar-rock-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.8',
+      version='0.0.9',
       license='MIT',
       long_description= long_description,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
       description='Package for estimating the confined compressive strength of rock.',
       packages= ['caesarrock'],
```

