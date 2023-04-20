# Comparing `tmp/caesar-rock-0.0.5.tar.gz` & `tmp/caesar-rock-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.5.tar", last modified: Thu Apr 20 04:46:59 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.6.tar", last modified: Thu Apr 20 04:52:05 2023, max compression
```

## Comparing `caesar-rock-0.0.5.tar` & `caesar-rock-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.527758 caesar-rock-0.0.5/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     8478 2023-04-20 04:46:59.525732 caesar-rock-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     8202 2023-04-20 04:39:46.000000 caesar-rock-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.510723 caesar-rock-0.0.5/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8478 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.522729 caesar-rock-0.0.5/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.5/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.5/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.5/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.5/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 04:46:59.527758 caesar-rock-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-20 04:46:12.000000 caesar-rock-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.301753 caesar-rock-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     8478 2023-04-20 04:52:05.299745 caesar-rock-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8202 2023-04-20 04:51:11.000000 caesar-rock-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.281751 caesar-rock-0.0.6/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8478 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.295760 caesar-rock-0.0.6/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.6/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.6/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.6/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.6/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:52:05.302744 caesar-rock-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-20 04:51:18.000000 caesar-rock-0.0.6/setup.py
```

### Comparing `caesar-rock-0.0.5/LICENSE` & `caesar-rock-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.5/PKG-INFO` & `caesar-rock-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.5
+Version: 0.0.6
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,15 +15,15 @@
 
 caesar-rock inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
-  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em AL-AWAD (2000)
+  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
   * Funções para geração de dataframe e gráficos com os resultados 
 
 ## Instalação
 
 ```bash
 pip install caesar-rock
@@ -148,13 +148,13 @@
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
 ## Referências
-  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2022.
+  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2002.
   * Edimann, K.; Somerville, J. M.; Smart, B. G. D.; Hamilton, S. A.; B. R. Crawford. Predicting Rock Mechanical Properties from Wireline Porosities. Paper presented at the SPE/ISRM Rock Mechanics in Petroleum Engineering, Trondheim, Norway, July 1998.
   * Farquhar, R. A.; Somerville, J. M; Smart, B. G. D. Porosity as a Geomechanical Indicator: An Application of Core and Log Data and Rock Mechanics. Paper presented at the European Petroleum Conference, London, United Kingdom, October 1994.
   * Golubev, A. A.; Rabinovich, G. Y. 1976. apud Chang, C.; Zpback, M. D.; Khaksar, A. Empirical Relations Between Rock Strength and Physical Properties in Sedimen-tary Rocks. Journal of Petroleum Science and Engineering 51. 2006. 
   * Horshud, P. Estimating Mechanical Properties of Shale From Empirical Correlations. SPE Drill & Compl 16 (02). 2001.
   * MacNally, G. H. The Prediction of Geotechnical Rock Properties from Sonic and Neutron Logs. Exploration Geophysics 21. 1990.
```

### Comparing `caesar-rock-0.0.5/README.md` & `caesar-rock-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 caesar-rock inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
-  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em AL-AWAD (2000)
+  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
   * Funções para geração de dataframe e gráficos com os resultados 
 
 ## Instalação
 
 ```bash
 pip install caesar-rock
@@ -138,13 +138,13 @@
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
 ## Referências
-  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2022.
+  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2002.
   * Edimann, K.; Somerville, J. M.; Smart, B. G. D.; Hamilton, S. A.; B. R. Crawford. Predicting Rock Mechanical Properties from Wireline Porosities. Paper presented at the SPE/ISRM Rock Mechanics in Petroleum Engineering, Trondheim, Norway, July 1998.
   * Farquhar, R. A.; Somerville, J. M; Smart, B. G. D. Porosity as a Geomechanical Indicator: An Application of Core and Log Data and Rock Mechanics. Paper presented at the European Petroleum Conference, London, United Kingdom, October 1994.
   * Golubev, A. A.; Rabinovich, G. Y. 1976. apud Chang, C.; Zpback, M. D.; Khaksar, A. Empirical Relations Between Rock Strength and Physical Properties in Sedimen-tary Rocks. Journal of Petroleum Science and Engineering 51. 2006. 
   * Horshud, P. Estimating Mechanical Properties of Shale From Empirical Correlations. SPE Drill & Compl 16 (02). 2001.
   * MacNally, G. H. The Prediction of Geotechnical Rock Properties from Sonic and Neutron Logs. Exploration Geophysics 21. 1990.
```

### Comparing `caesar-rock-0.0.5/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.6/caesar_rock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.5
+Version: 0.0.6
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,15 +15,15 @@
 
 caesar-rock inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
-  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em AL-AWAD (2000)
+  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
   * Funções para geração de dataframe e gráficos com os resultados 
 
 ## Instalação
 
 ```bash
 pip install caesar-rock
@@ -148,13 +148,13 @@
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
 ## Referências
-  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2022.
+  * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2002.
   * Edimann, K.; Somerville, J. M.; Smart, B. G. D.; Hamilton, S. A.; B. R. Crawford. Predicting Rock Mechanical Properties from Wireline Porosities. Paper presented at the SPE/ISRM Rock Mechanics in Petroleum Engineering, Trondheim, Norway, July 1998.
   * Farquhar, R. A.; Somerville, J. M; Smart, B. G. D. Porosity as a Geomechanical Indicator: An Application of Core and Log Data and Rock Mechanics. Paper presented at the European Petroleum Conference, London, United Kingdom, October 1994.
   * Golubev, A. A.; Rabinovich, G. Y. 1976. apud Chang, C.; Zpback, M. D.; Khaksar, A. Empirical Relations Between Rock Strength and Physical Properties in Sedimen-tary Rocks. Journal of Petroleum Science and Engineering 51. 2006. 
   * Horshud, P. Estimating Mechanical Properties of Shale From Empirical Correlations. SPE Drill & Compl 16 (02). 2001.
   * MacNally, G. H. The Prediction of Geotechnical Rock Properties from Sonic and Neutron Logs. Exploration Geophysics 21. 1990.
```

### Comparing `caesar-rock-0.0.5/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.6/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.5/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.6/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.5/caesarrock/ucs.py` & `caesar-rock-0.0.6/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.5/setup.py` & `caesar-rock-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.5',
+      version='0.0.6',
       license='MIT',
       long_description= long_description,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
       description='Module for calculating the confined compressive strength of rock.',
       packages= ['caesarrock'],
```

