# Comparing `tmp/caesar-rock-0.0.1.tar.gz` & `tmp/caesar-rock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caesar-rock-0.0.1.tar", last modified: Thu Apr 13 03:07:10 2023, max compression
+gzip compressed data, was "caesar-rock-0.0.2.tar", last modified: Thu Apr 20 04:16:34 2023, max compression
```

## Comparing `caesar-rock-0.0.1.tar` & `caesar-rock-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.759302 caesar-rock-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-04-13 02:21:28.000000 caesar-rock-0.0.1/LICENCE
--rw-rw-rw-   0        0        0     6578 2023-04-13 03:07:10.759302 caesar-rock-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6302 2023-04-06 00:32:52.000000 caesar-rock-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.754303 caesar-rock-0.0.1/caesar_rock.egg-info/
--rw-rw-rw-   0        0        0     6578 2023-04-13 03:07:10.000000 caesar-rock-0.0.1/caesar_rock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-04-13 03:07:10.000000 caesar-rock-0.0.1/caesar_rock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:07:10.000000 caesar-rock-0.0.1/caesar_rock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 03:07:10.000000 caesar-rock-0.0.1/caesar_rock.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 03:07:10.000000 caesar-rock-0.0.1/caesar_rock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 03:07:10.758300 caesar-rock-0.0.1/caesarrock/
--rw-rw-rw-   0        0        0       88 2023-04-13 02:11:14.000000 caesar-rock-0.0.1/caesarrock/__init__.py
--rw-rw-rw-   0        0        0     6317 2023-04-13 01:55:29.000000 caesar-rock-0.0.1/caesarrock/rockstrengthlog.py
--rw-rw-rw-   0        0        0      671 2023-04-07 23:47:33.000000 caesar-rock-0.0.1/caesarrock/ucs.py
--rw-rw-rw-   0        0        0       42 2023-04-13 03:07:10.759302 caesar-rock-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-04-13 03:03:44.000000 caesar-rock-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.139693 caesar-rock-0.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-13 20:38:35.000000 caesar-rock-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8724 2023-04-20 04:16:34.137627 caesar-rock-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8178 2023-04-20 03:50:32.000000 caesar-rock-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.107616 caesar-rock-0.0.2/caesar_rock.egg-info/
+-rw-rw-rw-   0        0        0     8724 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 04:16:33.000000 caesar-rock-0.0.2/caesar_rock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 04:16:34.133633 caesar-rock-0.0.2/caesarrock/
+-rw-rw-rw-   0        0        0      112 2023-04-19 16:54:45.000000 caesar-rock-0.0.2/caesarrock/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-19 17:11:13.000000 caesar-rock-0.0.2/caesarrock/pore_pressure_grad.py
+-rw-rw-rw-   0        0        0     6556 2023-04-20 03:53:31.000000 caesar-rock-0.0.2/caesarrock/rockstrengthlog.py
+-rw-rw-rw-   0        0        0      671 2023-04-13 20:38:35.000000 caesar-rock-0.0.2/caesarrock/ucs.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 04:16:34.140640 caesar-rock-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-04-20 04:10:31.000000 caesar-rock-0.0.2/setup.py
```

### Comparing `caesar-rock-0.0.1/caesarrock/ucs.py` & `caesar-rock-0.0.2/caesarrock/ucs.py`

 * *Files identical despite different names*

### Comparing `caesar-rock-0.0.1/setup.py` & `caesar-rock-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
     readme = arq.read()
 
 setup(name='caesar-rock',
-      version='0.0.1',
+      version='0.0.2',
       license='MIT',
       long_description= readme,
       long_description_content_type="text/markdown",
       author='LCCV/UFAL',
       author_email='erasmo.bezerra@lccv.ufal.br',
       description='Module for calculating the confined compressive strength of rock.',
       packages= ['caesarrock'],
```

