# Comparing `tmp/caesar-rock-0.0.7.tar.gz` & `tmp/caesar-rock-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.7.tar", last modified: Thu Apr 20 04:58:42 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.8.tar", last modified: Thu Apr 20 10:49:43 2023, max compression
```

## Comparing `caesar-rock-0.0.7.tar` & `caesar-rock-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.240451 caesar-rock-0.0.7/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     8483 2023-04-20 04:58:42.239447 caesar-rock-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8206 2023-04-20 04:56:33.000000 caesar-rock-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.220490 caesar-rock-0.0.7/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8483 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 04:58:42.000000 caesar-rock-0.0.7/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.235459 caesar-rock-0.0.7/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.7/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.7/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.7/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.7/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 04:58:42.241463 caesar-rock-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      618 2023-04-20 04:57:53.000000 caesar-rock-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.664378 caesar-rock-0.0.8/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     8490 2023-04-20 10:49:43.662435 caesar-rock-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8214 2023-04-20 10:47:01.000000 caesar-rock-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.617355 caesar-rock-0.0.8/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8490 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 10:49:43.000000 caesar-rock-0.0.8/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 10:49:43.657361 caesar-rock-0.0.8/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.8/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.8/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.8/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.8/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 10:49:43.665396 caesar-rock-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-20 10:49:25.000000 caesar-rock-0.0.8/setup.py
```

### Comparing `caesar-rock-0.0.7/LICENSE` & `caesar-rock-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.7/PKG-INFO` & `caesar-rock-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.7
-Summary: Package for calculating the confined compressive strength of rock.
+Version: 0.0.8
+Summary: Package for estimating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
@@ -99,15 +99,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
-df = pd.read_csv('df_p')
+df = pd.read_csv('df_p.csv')
 
 ccs = RockStrengthLog(df = df_p,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
@@ -130,15 +130,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
-df = pd.read_csv('df_dt')
+df = pd.read_csv('df_dt.csv')
 
 ccs = RockStrengthLog(df = df_dt,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
```

### Comparing `caesar-rock-0.0.7/README.md` & `caesar-rock-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
-df = pd.read_csv('df_p')
+df = pd.read_csv('df_p.csv')
 
 ccs = RockStrengthLog(df = df_p,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
@@ -120,15 +120,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
-df = pd.read_csv('df_dt')
+df = pd.read_csv('df_dt.csv')
 
 ccs = RockStrengthLog(df = df_dt,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
```

### Comparing `caesar-rock-0.0.7/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.8/caesar_rock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.7
-Summary: Package for calculating the confined compressive strength of rock.
+Version: 0.0.8
+Summary: Package for estimating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
@@ -99,15 +99,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
-df = pd.read_csv('df_p')
+df = pd.read_csv('df_p.csv')
 
 ccs = RockStrengthLog(df = df_p,
                       variable = Data.POROSITY,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_porosity,
@@ -130,15 +130,15 @@
 
 O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
-df = pd.read_csv('df_dt')
+df = pd.read_csv('df_dt.csv')
 
 ccs = RockStrengthLog(df = df_dt,
                       variable = Data.DELTA_TC,
                       shale_list = [Lit.CLAYSTONE, Lit.MARL, Lit.SILTSTONE],
                       limestone_list = [Lit.LIMESTONE],
                       sandstone_list = [Lit.SANDSTONE],
                       shale_equation = shale_horsrud_delta_tc,
```

### Comparing `caesar-rock-0.0.7/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.8/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.7/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.8/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.7/caesarrock/ucs.py` & `caesar-rock-0.0.8/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.7/setup.py` & `caesar-rock-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     long_description = f.read()
 
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.7',
+      version='0.0.8',
       license='MIT',
       long_description= long_description,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
-      description='Package for calculating the confined compressive strength of rock.',
+      description='Package for estimating the confined compressive strength of rock.',
       packages= ['caesarrock'],
       install_requires=['pandas', 'matplotlib', 'numpy', 'sympy'],)
```

