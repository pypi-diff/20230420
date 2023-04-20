# Comparing `tmp/caesar-rock-0.0.4.tar.gz` & `tmp/caesar-rock-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.4.tar", last modified: Thu Apr 20 04:40:32 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.5.tar", last modified: Thu Apr 20 04:46:59 2023, max compression
```

## Comparing `caesar-rock-0.0.4.tar` & `caesar-rock-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:40:32.936064 caesar-rock-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     8748 2023-04-20 04:40:32.935086 caesar-rock-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8202 2023-04-20 04:39:46.000000 caesar-rock-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:40:32.918978 caesar-rock-0.0.4/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8748 2023-04-20 04:40:32.000000 caesar-rock-0.0.4/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 04:40:32.000000 caesar-rock-0.0.4/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:40:32.000000 caesar-rock-0.0.4/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 04:40:32.000000 caesar-rock-0.0.4/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:40:32.000000 caesar-rock-0.0.4/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 04:40:32.932072 caesar-rock-0.0.4/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.4/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.4/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.4/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.4/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 04:40:32.937063 caesar-rock-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-04-20 04:39:53.000000 caesar-rock-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.527758 caesar-rock-0.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     8478 2023-04-20 04:46:59.525732 caesar-rock-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8202 2023-04-20 04:39:46.000000 caesar-rock-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.510723 caesar-rock-0.0.5/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8478 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:46:59.000000 caesar-rock-0.0.5/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:46:59.522729 caesar-rock-0.0.5/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.5/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.5/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.5/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.5/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:46:59.527758 caesar-rock-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-20 04:46:12.000000 caesar-rock-0.0.5/setup.py
```

### Comparing `caesar-rock-0.0.4/LICENSE` & `caesar-rock-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.4/PKG-INFO` & `caesar-rock-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.4
+Version: 0.0.5
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
 # caesar-rock
 
-caesar-rock Ã© um pacote para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trÃ¢nsito compressional. Inclui o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton e Zamora.
+caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
-caesar-rock inclui as seguintes funÃ§Ãµes:
+caesar-rock inclui as seguintes funções:
 
-  * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
-  * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Zamora (com expoente d corrigido)
-  * FunÃ§Ãµes para a estimativa da resistÃªncia uniaxial Ã  compressÃ£o das rochas por meio de equaÃ§Ãµes empÃ­ricas a partir da porosidade
-  * FunÃ§Ãµes para a estimativa da resistÃªncia uniaxial Ã  compressÃ£o das rochas por meio de equaÃ§Ãµes empÃ­ricas a partir do tempo de trÃ¢nsito compressional
-  * FunÃ§Ã£o para a estimativa do Ã¢ngulo de atrito interno das rochas por meio da correlaÃ§Ã£o empÃ­rica obtida em AL-AWAD (2000)
-  * FunÃ§Ã£o para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada das rochas
-  * FunÃ§Ãµes para geraÃ§Ã£o de dataframe e grÃ¡ficos com os resultados 
+  * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
+  * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
+  * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
+  * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
+  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em AL-AWAD (2000)
+  * Função para o cálculo da resistência à compressão confinada das rochas
+  * Funções para geração de dataframe e gráficos com os resultados 
 
-## InstalaÃ§Ã£o
+## Instalação
 
 ```bash
 pip install caesar-rock
 ```
 
 ## Exemplos
 
-### 1. Gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
+### 1. Gradiente de poro pressão pelo método de Eaton
 
-Os dados de entrada para o cÃ¡lculo dos gradientes de poro pressÃ£o pelo mÃ©todo de Eaton consistem nos perfis de densidade (g/cmÂ³) e tempo de trÃ¢nsito compressional (Âµs/ft) ao longo da profundidade (m), organizados em um dataframe, como o padrÃ£o a seguir. Outro parÃ¢metro necessÃ¡rio Ã© o gradiente de poro pressÃ£o normal (ppg).
+Os dados de entrada para o cálculo dos gradientes de poro pressão pelo método de Eaton consistem nos perfis de densidade (g/cm³) e tempo de trânsito compressional (µs/ft) ao longo da profundidade (m), organizados em um dataframe, como o padrão a seguir. Outro parâmetro necessário é o gradiente de poro pressão normal (ppg).
 
-| Depth - m | Bulk density - g/cmÂ³ | Delta-T Compressional - Âµs/ft |
+| Depth - m | Bulk density - g/cm³ | Delta-T Compressional - µs/ft |
 | -------- | -------- | -------- |
 | 2765.2979 | 2.0542 | 62.5396 |
 | 2765.4504 | 2.0731 | 61.4572 |
 | 2765.6028 | 2.0811 | 60.9234 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe Eaton`, e imprime-se o dataframe com os gradientes de poro pressÃ£o resultantes.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe Eaton`, e imprime-se o dataframe com os gradientes de poro pressão resultantes.
 
 
 ```python
 import pandas as pd
 from caesarrock import Eaton
 
 df = pd.read_csv('df_eaton.csv')
 
 eaton = Eaton(df = df, normal_pore_pressure_gradient = 8.5)
 
 print(eaton.df)
 
 ```
 
-### 2. Gradiente de poro pressÃ£o pelo mÃ©todo de Zamora
+### 2. Gradiente de poro pressão pelo método de Zamora
 
-Os dados de entrada para o cÃ¡lculo dos gradientes de poro pressÃ£o pelo mÃ©todo de Zamora consistem nos valores do expoente d corrigido (adimensional) ao longo da profundidade (m), organizados em um dataframe, como o padrÃ£o a seguir. Outro parÃ¢metro necessÃ¡rio Ã© o gradiente de poro pressÃ£o normal (ppg).
+Os dados de entrada para o cálculo dos gradientes de poro pressão pelo método de Zamora consistem nos valores do expoente d corrigido (adimensional) ao longo da profundidade (m), organizados em um dataframe, como o padrão a seguir. Outro parâmetro necessário é o gradiente de poro pressão normal (ppg).
 
 | Depth - m | Corrected Drilling Exponent - unitless |
 | -------- | -------- |
 | 2751.0 | 1.06 |
 | 2752.0 | 1.04 |
 | 2753.0 | 1.04 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe Zamora`, e imprime-se o dataframe com os gradientes de poro pressÃ£o resultantes.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe Zamora`, e imprime-se o dataframe com os gradientes de poro pressão resultantes.
 
 
 ```python
 import pandas as pd
 from caesarrock import Zamora
 
 df = pd.read_csv('df_zamora.csv')
 
 eaton = Zamora(df = df, normal_pore_pressure_gradient = 8.5)
 
 print(zamora.df)
 
 ```
 
-### 3. ResistÃªncia Ã  compressÃ£o confinada das rochas
+### 3. Resistência à compressão confinada das rochas
 
-Os dados de entrada para o cÃ¡lculo da resistÃªncia confinada das rochas consistem na profundidade (m), litologia, densidade circulante equivalente (ppg), gradiente de poro pressÃ£o (ppg) e um dado geofÃ­sico, ou a porosidade (fr) ou o tempo de trÃ¢nsito compressional (Âµs/ft), conforme os padrÃµes a seguir. O dado geofÃ­sico deve ser informado no parÃ¢metro `variable` como `Data.POROSITY` ou `Data.DELTA_TC`.
+Os dados de entrada para o cálculo da resistência confinada das rochas consistem na profundidade (m), litologia, densidade circulante equivalente (ppg), gradiente de poro pressão (ppg) e um dado geofísico, ou a porosidade (fr) ou o tempo de trânsito compressional (µs/ft), conforme os padrões a seguir. O dado geofísico deve ser informado no parâmetro `variable` como `Data.POROSITY` ou `Data.DELTA_TC`.
 
-AlÃ©m desses dados, Ã© necessÃ¡rio classificar as litologias presentes no dataframe em trÃªs listas de grupos: `shale_list`, `limestone_list` e `sandstone_list`. As litologias nÃ£o enumeradas na estrutura `Lit`: `Lit.CLAYSTONE`, `Lit.SILTSTONE`, `Lit.MARL`, `Lit.LIMESTONE` e `Lit.SANDSTONE`, podem ser descritas pelo tipo string, por exemplo: `'Dolomite'`.
+Além desses dados, é necessário classificar as litologias presentes no dataframe em três listas de grupos: `shale_list`, `limestone_list` e `sandstone_list`. As litologias não enumeradas na estrutura `Lit`: `Lit.CLAYSTONE`, `Lit.SILTSTONE`, `Lit.MARL`, `Lit.LIMESTONE` e `Lit.SANDSTONE`, podem ser descritas pelo tipo string, por exemplo: `'Dolomite'`.
 
-Para cada grupo de litologia, importa-se a equaÃ§Ã£o empÃ­rica para o cÃ¡lculo do UCS com base em suas limitaÃ§Ãµes, isto Ã©, litologia e bacia ou regiÃ£o na qual foram extraÃ­dos os testemunhos usados para obter a correlaÃ§Ã£o. Alternativamente, Ã© possÃ­vel definir uma funÃ§Ã£o e passa-la como parÃ¢metro. As equaÃ§Ãµes adequadas sÃ£o informadas em `shale_equation`, `limestone_equation` e `sandstone_equation`.
+Para cada grupo de litologia, importa-se a equação empírica para o cálculo do UCS com base em suas limitações, isto é, litologia e bacia ou região na qual foram extraídos os testemunhos usados para obter a correlação. Alternativamente, é possível definir uma função e passa-la como parâmetro. As equações adequadas são informadas em `shale_equation`, `limestone_equation` e `sandstone_equation`.
 
-#### Dado geofÃ­sico: porosidade
+#### Dado geofísico: porosidade
 
 | Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Porosity - fr
 | -------- | -------- | -------- |-------- | -------- |
 | 2765.2979 | Limestone | 15.0833 |8.4593| 0.1111 |
 | 2765.4504 | Limestone | 15.0833 |8.1952 | 0.1015 |
 | 2765.6028 | Limestone | 15.0798 |8.0605 | 0.0927 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistÃªncias resultantes. O mÃ©todo `.plot()` plota o grÃ¡fico dos dados fornecidos e calculados.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
 df = pd.read_csv('df_p')
 
@@ -116,23 +116,23 @@
 
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
-#### Dado geofÃ­sico: tempo de trÃ¢nsito compressional
+#### Dado geofísico: tempo de trânsito compressional
 
-| Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Delta T - Compressional - Âµs/ft
+| Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Delta T - Compressional - µs/ft
 | -------- | -------- | -------- |-------- | -------- |
 | 2765.2979 | Limestone | 15.0833 |8.4593| 62.5396 |
 | 2765.4504 | Limestone | 15.0833 |8.1952 | 61.4572 |
 | 2765.6028 | Limestone | 15.0798 |8.0605 | 60.9234 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistÃªncias resultantes. O mÃ©todo `.plot()` plota o grÃ¡fico dos dados fornecidos e calculados.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
 df = pd.read_csv('df_dt')
 
@@ -147,14 +147,14 @@
 
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
-## ReferÃªncias
+## Referências
   * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2022.
   * Edimann, K.; Somerville, J. M.; Smart, B. G. D.; Hamilton, S. A.; B. R. Crawford. Predicting Rock Mechanical Properties from Wireline Porosities. Paper presented at the SPE/ISRM Rock Mechanics in Petroleum Engineering, Trondheim, Norway, July 1998.
   * Farquhar, R. A.; Somerville, J. M; Smart, B. G. D. Porosity as a Geomechanical Indicator: An Application of Core and Log Data and Rock Mechanics. Paper presented at the European Petroleum Conference, London, United Kingdom, October 1994.
   * Golubev, A. A.; Rabinovich, G. Y. 1976. apud Chang, C.; Zpback, M. D.; Khaksar, A. Empirical Relations Between Rock Strength and Physical Properties in Sedimen-tary Rocks. Journal of Petroleum Science and Engineering 51. 2006. 
   * Horshud, P. Estimating Mechanical Properties of Shale From Empirical Correlations. SPE Drill & Compl 16 (02). 2001.
   * MacNally, G. H. The Prediction of Geotechnical Rock Properties from Sonic and Neutron Logs. Exploration Geophysics 21. 1990.
```

### Comparing `caesar-rock-0.0.4/README.md` & `caesar-rock-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.4/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.5/caesar_rock.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.4
+Version: 0.0.5
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
 # caesar-rock
 
-caesar-rock Ã© um pacote para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trÃ¢nsito compressional. Inclui o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton e Zamora.
+caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
-caesar-rock inclui as seguintes funÃ§Ãµes:
+caesar-rock inclui as seguintes funções:
 
-  * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
-  * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Zamora (com expoente d corrigido)
-  * FunÃ§Ãµes para a estimativa da resistÃªncia uniaxial Ã  compressÃ£o das rochas por meio de equaÃ§Ãµes empÃ­ricas a partir da porosidade
-  * FunÃ§Ãµes para a estimativa da resistÃªncia uniaxial Ã  compressÃ£o das rochas por meio de equaÃ§Ãµes empÃ­ricas a partir do tempo de trÃ¢nsito compressional
-  * FunÃ§Ã£o para a estimativa do Ã¢ngulo de atrito interno das rochas por meio da correlaÃ§Ã£o empÃ­rica obtida em AL-AWAD (2000)
-  * FunÃ§Ã£o para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada das rochas
-  * FunÃ§Ãµes para geraÃ§Ã£o de dataframe e grÃ¡ficos com os resultados 
+  * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
+  * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
+  * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
+  * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
+  * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em AL-AWAD (2000)
+  * Função para o cálculo da resistência à compressão confinada das rochas
+  * Funções para geração de dataframe e gráficos com os resultados 
 
-## InstalaÃ§Ã£o
+## Instalação
 
 ```bash
 pip install caesar-rock
 ```
 
 ## Exemplos
 
-### 1. Gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
+### 1. Gradiente de poro pressão pelo método de Eaton
 
-Os dados de entrada para o cÃ¡lculo dos gradientes de poro pressÃ£o pelo mÃ©todo de Eaton consistem nos perfis de densidade (g/cmÂ³) e tempo de trÃ¢nsito compressional (Âµs/ft) ao longo da profundidade (m), organizados em um dataframe, como o padrÃ£o a seguir. Outro parÃ¢metro necessÃ¡rio Ã© o gradiente de poro pressÃ£o normal (ppg).
+Os dados de entrada para o cálculo dos gradientes de poro pressão pelo método de Eaton consistem nos perfis de densidade (g/cm³) e tempo de trânsito compressional (µs/ft) ao longo da profundidade (m), organizados em um dataframe, como o padrão a seguir. Outro parâmetro necessário é o gradiente de poro pressão normal (ppg).
 
-| Depth - m | Bulk density - g/cmÂ³ | Delta-T Compressional - Âµs/ft |
+| Depth - m | Bulk density - g/cm³ | Delta-T Compressional - µs/ft |
 | -------- | -------- | -------- |
 | 2765.2979 | 2.0542 | 62.5396 |
 | 2765.4504 | 2.0731 | 61.4572 |
 | 2765.6028 | 2.0811 | 60.9234 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe Eaton`, e imprime-se o dataframe com os gradientes de poro pressÃ£o resultantes.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe Eaton`, e imprime-se o dataframe com os gradientes de poro pressão resultantes.
 
 
 ```python
 import pandas as pd
 from caesarrock import Eaton
 
 df = pd.read_csv('df_eaton.csv')
 
 eaton = Eaton(df = df, normal_pore_pressure_gradient = 8.5)
 
 print(eaton.df)
 
 ```
 
-### 2. Gradiente de poro pressÃ£o pelo mÃ©todo de Zamora
+### 2. Gradiente de poro pressão pelo método de Zamora
 
-Os dados de entrada para o cÃ¡lculo dos gradientes de poro pressÃ£o pelo mÃ©todo de Zamora consistem nos valores do expoente d corrigido (adimensional) ao longo da profundidade (m), organizados em um dataframe, como o padrÃ£o a seguir. Outro parÃ¢metro necessÃ¡rio Ã© o gradiente de poro pressÃ£o normal (ppg).
+Os dados de entrada para o cálculo dos gradientes de poro pressão pelo método de Zamora consistem nos valores do expoente d corrigido (adimensional) ao longo da profundidade (m), organizados em um dataframe, como o padrão a seguir. Outro parâmetro necessário é o gradiente de poro pressão normal (ppg).
 
 | Depth - m | Corrected Drilling Exponent - unitless |
 | -------- | -------- |
 | 2751.0 | 1.06 |
 | 2752.0 | 1.04 |
 | 2753.0 | 1.04 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe Zamora`, e imprime-se o dataframe com os gradientes de poro pressÃ£o resultantes.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe Zamora`, e imprime-se o dataframe com os gradientes de poro pressão resultantes.
 
 
 ```python
 import pandas as pd
 from caesarrock import Zamora
 
 df = pd.read_csv('df_zamora.csv')
 
 eaton = Zamora(df = df, normal_pore_pressure_gradient = 8.5)
 
 print(zamora.df)
 
 ```
 
-### 3. ResistÃªncia Ã  compressÃ£o confinada das rochas
+### 3. Resistência à compressão confinada das rochas
 
-Os dados de entrada para o cÃ¡lculo da resistÃªncia confinada das rochas consistem na profundidade (m), litologia, densidade circulante equivalente (ppg), gradiente de poro pressÃ£o (ppg) e um dado geofÃ­sico, ou a porosidade (fr) ou o tempo de trÃ¢nsito compressional (Âµs/ft), conforme os padrÃµes a seguir. O dado geofÃ­sico deve ser informado no parÃ¢metro `variable` como `Data.POROSITY` ou `Data.DELTA_TC`.
+Os dados de entrada para o cálculo da resistência confinada das rochas consistem na profundidade (m), litologia, densidade circulante equivalente (ppg), gradiente de poro pressão (ppg) e um dado geofísico, ou a porosidade (fr) ou o tempo de trânsito compressional (µs/ft), conforme os padrões a seguir. O dado geofísico deve ser informado no parâmetro `variable` como `Data.POROSITY` ou `Data.DELTA_TC`.
 
-AlÃ©m desses dados, Ã© necessÃ¡rio classificar as litologias presentes no dataframe em trÃªs listas de grupos: `shale_list`, `limestone_list` e `sandstone_list`. As litologias nÃ£o enumeradas na estrutura `Lit`: `Lit.CLAYSTONE`, `Lit.SILTSTONE`, `Lit.MARL`, `Lit.LIMESTONE` e `Lit.SANDSTONE`, podem ser descritas pelo tipo string, por exemplo: `'Dolomite'`.
+Além desses dados, é necessário classificar as litologias presentes no dataframe em três listas de grupos: `shale_list`, `limestone_list` e `sandstone_list`. As litologias não enumeradas na estrutura `Lit`: `Lit.CLAYSTONE`, `Lit.SILTSTONE`, `Lit.MARL`, `Lit.LIMESTONE` e `Lit.SANDSTONE`, podem ser descritas pelo tipo string, por exemplo: `'Dolomite'`.
 
-Para cada grupo de litologia, importa-se a equaÃ§Ã£o empÃ­rica para o cÃ¡lculo do UCS com base em suas limitaÃ§Ãµes, isto Ã©, litologia e bacia ou regiÃ£o na qual foram extraÃ­dos os testemunhos usados para obter a correlaÃ§Ã£o. Alternativamente, Ã© possÃ­vel definir uma funÃ§Ã£o e passa-la como parÃ¢metro. As equaÃ§Ãµes adequadas sÃ£o informadas em `shale_equation`, `limestone_equation` e `sandstone_equation`.
+Para cada grupo de litologia, importa-se a equação empírica para o cálculo do UCS com base em suas limitações, isto é, litologia e bacia ou região na qual foram extraídos os testemunhos usados para obter a correlação. Alternativamente, é possível definir uma função e passa-la como parâmetro. As equações adequadas são informadas em `shale_equation`, `limestone_equation` e `sandstone_equation`.
 
-#### Dado geofÃ­sico: porosidade
+#### Dado geofísico: porosidade
 
 | Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Porosity - fr
 | -------- | -------- | -------- |-------- | -------- |
 | 2765.2979 | Limestone | 15.0833 |8.4593| 0.1111 |
 | 2765.4504 | Limestone | 15.0833 |8.1952 | 0.1015 |
 | 2765.6028 | Limestone | 15.0798 |8.0605 | 0.0927 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistÃªncias resultantes. O mÃ©todo `.plot()` plota o grÃ¡fico dos dados fornecidos e calculados.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_porosity, limestone_faquhar_porosity, sandstone_edimann_porosity
 
 df = pd.read_csv('df_p')
 
@@ -116,23 +116,23 @@
 
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
-#### Dado geofÃ­sico: tempo de trÃ¢nsito compressional
+#### Dado geofísico: tempo de trânsito compressional
 
-| Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Delta T - Compressional - Âµs/ft
+| Depth - m | Lithology | ECD - ppg | Grad. Poro Pressure - ppg | Delta T - Compressional - µs/ft
 | -------- | -------- | -------- |-------- | -------- |
 | 2765.2979 | Limestone | 15.0833 |8.4593| 62.5396 |
 | 2765.4504 | Limestone | 15.0833 |8.1952 | 61.4572 |
 | 2765.6028 | Limestone | 15.0798 |8.0605 | 60.9234 |
 
-O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrÃ£o anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistÃªncias resultantes. O mÃ©todo `.plot()` plota o grÃ¡fico dos dados fornecidos e calculados.
+O exemplo seguinte mostra a leitura do arquivo `.csv` conforme o padrão anterior, instancia-se a `classe RockStrengthLog`, e imprime-se o dataframe com as resistências resultantes. O método `.plot()` plota o gráfico dos dados fornecidos e calculados.
 
 ```python
 import pandas as pd
 from caesarrock import RockStrengthLog, Data, Lit, shale_horsrud_delta_tc, limestone_golubev_delta_tc, sandstone_macnelly_delta_tc
 
 df = pd.read_csv('df_dt')
 
@@ -147,14 +147,14 @@
 
 print(ccs.df)
 
 ccs.plot()
 
 ```
 
-## ReferÃªncias
+## Referências
   * Al-Awad, M. N. J. Simple Correlation to Evaluate Mohr-Coulomb Failure Criterion Using Uniaxial Compressive Strength. J. King Saud Univ.; Vol. 14, Eng. Sci. (1). 2022.
   * Edimann, K.; Somerville, J. M.; Smart, B. G. D.; Hamilton, S. A.; B. R. Crawford. Predicting Rock Mechanical Properties from Wireline Porosities. Paper presented at the SPE/ISRM Rock Mechanics in Petroleum Engineering, Trondheim, Norway, July 1998.
   * Farquhar, R. A.; Somerville, J. M; Smart, B. G. D. Porosity as a Geomechanical Indicator: An Application of Core and Log Data and Rock Mechanics. Paper presented at the European Petroleum Conference, London, United Kingdom, October 1994.
   * Golubev, A. A.; Rabinovich, G. Y. 1976. apud Chang, C.; Zpback, M. D.; Khaksar, A. Empirical Relations Between Rock Strength and Physical Properties in Sedimen-tary Rocks. Journal of Petroleum Science and Engineering 51. 2006. 
   * Horshud, P. Estimating Mechanical Properties of Shale From Empirical Correlations. SPE Drill & Compl 16 (02). 2001.
   * MacNally, G. H. The Prediction of Geotechnical Rock Properties from Sonic and Neutron Logs. Exploration Geophysics 21. 1990.
```

### Comparing `caesar-rock-0.0.4/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.5/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.4/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.5/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.4/caesarrock/ucs.py` & `caesar-rock-0.0.5/caesarrock/ucs.py`

 * *Files identical despite different names*

