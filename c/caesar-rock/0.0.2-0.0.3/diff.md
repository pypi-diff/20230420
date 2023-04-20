# Comparing `tmp/caesar-rock-0.0.2.tar.gz` & `tmp/caesar-rock-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.2.tar", last modified: Thu Apr 20 04:16:34 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.3.tar", last modified: Thu Apr 20 04:34:13 2023, max compression
```

## Comparing `caesar-rock-0.0.2.tar` & `caesar-rock-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.139693 caesar-rock-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     8724 2023-04-20 04:16:34.137627 caesar-rock-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     8178 2023-04-20 03:50:32.000000 caesar-rock-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.107616 caesar-rock-0.0.2/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     8724 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.133633 caesar-rock-0.0.2/caesarrock/
--rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.2/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.2/caesarrock/pore_pressure_grad.py
--rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.2/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.2/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-20 04:16:34.140640 caesar-rock-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-04-20 04:10:31.000000 caesar-rock-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:34:13.213192 caesar-rock-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     8749 2023-04-20 04:34:13.212208 caesar-rock-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8203 2023-04-20 04:27:59.000000 caesar-rock-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:34:13.194095 caesar-rock-0.0.3/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8749 2023-04-20 04:34:12.000000 caesar-rock-0.0.3/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 04:34:13.000000 caesar-rock-0.0.3/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:34:12.000000 caesar-rock-0.0.3/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 04:34:12.000000 caesar-rock-0.0.3/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:34:12.000000 caesar-rock-0.0.3/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:34:13.206632 caesar-rock-0.0.3/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.3/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.3/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.3/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.3/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:34:13.213192 caesar-rock-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-04-20 04:31:29.000000 caesar-rock-0.0.3/setup.py
```

### Comparing `caesar-rock-0.0.2/LICENSE` & `caesar-rock-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.2/PKG-INFO` & `caesar-rock-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# -*- coding: utf-8 -*-
 # caesar-rock
 
 caesar-rock Ã© um pacote para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trÃ¢nsito compressional. Inclui o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton e Zamora.
 
 caesar-rock inclui as seguintes funÃ§Ãµes:
 
   * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
```

### Comparing `caesar-rock-0.0.2/README.md` & `caesar-rock-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 # caesar-rock
 
 caesar-rock é um pacote para o cálculo da resistência à compressão confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trânsito compressional. Inclui o cálculo do gradiente de poro pressão pelo método de Eaton e Zamora.
 
 caesar-rock inclui as seguintes funções:
 
   * Funções para o cálculo do gradiente de poro pressão pelo método de Eaton
```

### Comparing `caesar-rock-0.0.2/caesar_rock.egg-info/PKG-INFO` & `caesar-rock-0.0.3/caesar_rock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: caesar-rock
-Version: 0.0.2
+Version: 0.0.3
 Summary: Module for calculating the confined compressive strength of rock.
 Author: LCCV/UFAL
 Author-email: erasmo.bezerra@lccv.ufal.br
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# -*- coding: utf-8 -*-
 # caesar-rock
 
 caesar-rock Ã© um pacote para o cÃ¡lculo da resistÃªncia Ã  compressÃ£o confinada de rochas (CCS) a partir de dados de perfilagem de porosidade ou do tempo de trÃ¢nsito compressional. Inclui o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton e Zamora.
 
 caesar-rock inclui as seguintes funÃ§Ãµes:
 
   * FunÃ§Ãµes para o cÃ¡lculo do gradiente de poro pressÃ£o pelo mÃ©todo de Eaton
```

### Comparing `caesar-rock-0.0.2/caesarrock/pore_pressure_grad.py` & `caesar-rock-0.0.3/caesarrock/pore_pressure_grad.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.2/caesarrock/rockstrengthlog.py` & `caesar-rock-0.0.3/caesarrock/rockstrengthlog.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.2/caesarrock/ucs.py` & `caesar-rock-0.0.3/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.2/setup.py` & `caesar-rock-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.2',
+      version='0.0.3',
       license='MIT',
       long_description= readme,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
       description='Module for calculating the confined compressive strength of rock.',
       packages= ['caesarrock'],
```

