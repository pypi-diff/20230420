# Comparing `tmp/caesar-rock-0.0.6.tar.gz` & `tmp/caesar-rock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.6.tar", last modified: Thu Apr 20 04:52:05 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.7.tar", last modified: Thu Apr 20 04:58:42 2023, max compression
```

## Comparing `caesar-rock-0.0.6.tar` & `caesar-rock-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.301753 caesar-rock-0.0.6/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     8478 2023-04-20 04:52:05.299745 caesar-rock-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8202 2023-04-20 04:51:11.000000 caesar-rock-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.281751 caesar-rock-0.0.6/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8478 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:52:05.000000 caesar-rock-0.0.6/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 04:52:05.295760 caesar-rock-0.0.6/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.6/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.6/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.6/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.6/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 04:52:05.302744 caesar-rock-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-20 04:51:18.000000 caesar-rock-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.240451 caesar-rock-0.0.7/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     8483 2023-04-20 04:58:42.239447 caesar-rock-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8206 2023-04-20 04:56:33.000000 caesar-rock-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.220490 caesar-rock-0.0.7/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8483 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 04:58:42.000000 caesar-rock-0.0.7/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:58:41.000000 caesar-rock-0.0.7/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:58:42.235459 caesar-rock-0.0.7/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.7/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.7/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.7/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.7/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:58:42.241463 caesar-rock-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      618 2023-04-20 04:57:53.000000 caesar-rock-0.0.7/setup.py
```

### Comparing `caesar-rock-0.0.6/LICENSE` & `caesar-rock-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.6/PKG-INFO` & `caesar-rock-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.6
-Summary: Module for calculating the confined compressive strength of rock.
+Version: 0.0.7
+Summary: Package for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
 # caesar-rock
 
-caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
+`caesar-rock` é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
-caesar-rock inclui as seguintes funções:
+`caesar-rock` inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
   * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
```

### Comparing `caesar-rock-0.0.6/README.md` & `caesar-rock-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!-- coding: utf-8 -->
 # caesar-rock
 
-caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
+`caesar-rock` é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
-caesar-rock inclui as seguintes funções:
+`caesar-rock` inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
   * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
```

### Comparing `caesar-rock-0.0.6/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.7/caesar_rock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.6
-Summary: Module for calculating the confined compressive strength of rock.
+Version: 0.0.7
+Summary: Package for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!-- coding: utf-8 -->
 # caesar-rock
 
-caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
+`caesar-rock` é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
-caesar-rock inclui as seguintes funções:
+`caesar-rock` inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
   * Funções para o cálculo do gradiente de poro pressão pelo método de Zamora (com expoente d corrigido)
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir da porosidade
   * Funções para a estimativa da resistência uniaxial à compressão das rochas por meio de equações empíricas a partir do tempo de trânsito compressional
   * Função para a estimativa do ângulo de atrito interno das rochas por meio da correlação empírica obtida em Al-Awad (2002)
   * Função para o cálculo da resistência à compressão confinada das rochas
```

### Comparing `caesar-rock-0.0.6/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.7/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.6/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.7/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.6/caesarrock/ucs.py` & `caesar-rock-0.0.7/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.6/setup.py` & `caesar-rock-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     long_description = f.read()
 
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.6',
+      version='0.0.7',
       license='MIT',
       long_description= long_description,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
-      description='Module for calculating the confined compressive strength of rock.',
+      description='Package for calculating the confined compressive strength of rock.',
       packages= ['caesarrock'],
       install_requires=['pandas', 'matplotlib', 'numpy', 'sympy'],)
```

