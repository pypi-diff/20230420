# Comparing `tmp/riskCalculator-0.0.4.tar.gz` & `tmp/riskCalculator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riskCalculator-0.0.4.tar", last modified: Thu Apr 20 02:22:56 2023, max compression
+gzip compressed data, was "riskCalculator-0.0.5.tar", last modified: Thu Apr 20 06:14:37 2023, max compression
```

## Comparing `riskCalculator-0.0.4.tar` & `riskCalculator-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 02:22:56.924646 riskCalculator-0.0.4/
--rw-r--r--   0 angusleck   (501) staff       (20)    34523 2023-04-17 22:36:31.000000 riskCalculator-0.0.4/LICENSE
--rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-20 02:22:56.924502 riskCalculator-0.0.4/PKG-INFO
--rw-r--r--   0 angusleck   (501) staff       (20)     1018 2023-04-20 02:22:47.000000 riskCalculator-0.0.4/README.md
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 02:22:56.923804 riskCalculator-0.0.4/riskCalculator/
--rw-r--r--   0 angusleck   (501) staff       (20)       37 2023-04-19 04:39:42.000000 riskCalculator-0.0.4/riskCalculator/__init__.py
--rw-r--r--   0 angusleck   (501) staff       (20)      363 2023-04-19 04:33:42.000000 riskCalculator-0.0.4/riskCalculator/expectedSurvivors.py
--rw-r--r--   0 angusleck   (501) staff       (20)      380 2023-04-19 04:33:42.000000 riskCalculator-0.0.4/riskCalculator/likelihoodOfVictory.py
--rw-r--r--   0 angusleck   (501) staff       (20)     1059 2023-04-19 04:56:17.000000 riskCalculator-0.0.4/riskCalculator/parseArguments.py
--rw-r--r--   0 angusleck   (501) staff       (20)      718 2023-04-18 00:54:01.000000 riskCalculator-0.0.4/riskCalculator/probabilityOfLosses.py
--rw-r--r--   0 angusleck   (501) staff       (20)      871 2023-04-18 03:27:18.000000 riskCalculator-0.0.4/riskCalculator/readWriteData.py
--rw-r--r--   0 angusleck   (501) staff       (20)      937 2023-04-19 04:33:42.000000 riskCalculator-0.0.4/riskCalculator/recursiveMarkovChain.py
--rw-r--r--   0 angusleck   (501) staff       (20)     1483 2023-04-20 02:21:22.000000 riskCalculator-0.0.4/riskCalculator/risk.py
-drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 02:22:56.924322 riskCalculator-0.0.4/riskCalculator.egg-info/
--rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-20 02:22:56.000000 riskCalculator-0.0.4/riskCalculator.egg-info/PKG-INFO
--rw-r--r--   0 angusleck   (501) staff       (20)      444 2023-04-20 02:22:56.000000 riskCalculator-0.0.4/riskCalculator.egg-info/SOURCES.txt
--rw-r--r--   0 angusleck   (501) staff       (20)        1 2023-04-20 02:22:56.000000 riskCalculator-0.0.4/riskCalculator.egg-info/dependency_links.txt
--rw-r--r--   0 angusleck   (501) staff       (20)       15 2023-04-20 02:22:56.000000 riskCalculator-0.0.4/riskCalculator.egg-info/top_level.txt
--rw-r--r--   0 angusleck   (501) staff       (20)       38 2023-04-20 02:22:56.924693 riskCalculator-0.0.4/setup.cfg
--rw-r--r--   0 angusleck   (501) staff       (20)      947 2023-04-20 02:22:18.000000 riskCalculator-0.0.4/setup.py
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 06:14:37.523460 riskCalculator-0.0.5/
+-rw-r--r--   0 angusleck   (501) staff       (20)    34523 2023-04-17 22:36:31.000000 riskCalculator-0.0.5/LICENSE
+-rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-20 06:14:37.523336 riskCalculator-0.0.5/PKG-INFO
+-rw-r--r--   0 angusleck   (501) staff       (20)     1016 2023-04-20 06:13:18.000000 riskCalculator-0.0.5/README.md
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 06:14:37.522741 riskCalculator-0.0.5/riskCalculator/
+-rw-r--r--   0 angusleck   (501) staff       (20)       37 2023-04-19 04:39:42.000000 riskCalculator-0.0.5/riskCalculator/__init__.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      363 2023-04-19 04:33:42.000000 riskCalculator-0.0.5/riskCalculator/expectedSurvivors.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      380 2023-04-19 04:33:42.000000 riskCalculator-0.0.5/riskCalculator/likelihoodOfVictory.py
+-rw-r--r--   0 angusleck   (501) staff       (20)     1059 2023-04-19 04:56:17.000000 riskCalculator-0.0.5/riskCalculator/parseArguments.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      793 2023-04-20 06:12:01.000000 riskCalculator-0.0.5/riskCalculator/probabilityOfLosses.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      871 2023-04-18 03:27:18.000000 riskCalculator-0.0.5/riskCalculator/readWriteData.py
+-rw-r--r--   0 angusleck   (501) staff       (20)      937 2023-04-19 04:33:42.000000 riskCalculator-0.0.5/riskCalculator/recursiveMarkovChain.py
+-rw-r--r--   0 angusleck   (501) staff       (20)     1483 2023-04-20 02:21:22.000000 riskCalculator-0.0.5/riskCalculator/risk.py
+drwxr-xr-x   0 angusleck   (501) staff       (20)        0 2023-04-20 06:14:37.523180 riskCalculator-0.0.5/riskCalculator.egg-info/
+-rw-r--r--   0 angusleck   (501) staff       (20)      601 2023-04-20 06:14:37.000000 riskCalculator-0.0.5/riskCalculator.egg-info/PKG-INFO
+-rw-r--r--   0 angusleck   (501) staff       (20)      444 2023-04-20 06:14:37.000000 riskCalculator-0.0.5/riskCalculator.egg-info/SOURCES.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)        1 2023-04-20 06:14:37.000000 riskCalculator-0.0.5/riskCalculator.egg-info/dependency_links.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)       15 2023-04-20 06:14:37.000000 riskCalculator-0.0.5/riskCalculator.egg-info/top_level.txt
+-rw-r--r--   0 angusleck   (501) staff       (20)       38 2023-04-20 06:14:37.523502 riskCalculator-0.0.5/setup.cfg
+-rw-r--r--   0 angusleck   (501) staff       (20)      947 2023-04-20 06:13:56.000000 riskCalculator-0.0.5/setup.py
```

### Comparing `riskCalculator-0.0.4/LICENSE` & `riskCalculator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.4/PKG-INFO` & `riskCalculator-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskCalculator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple python package for calculating expected outcome of a risk battle
 Author: Angus Leck
 Author-email: aleck42@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `riskCalculator-0.0.4/README.md` & `riskCalculator-0.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 ```sh
 yarn risk <attackers> <defenders>
 ```
 
 ## Returns
 The likelihood of victory and the average number of survivors (attackers).
 ```sh
-likelihood of victory 52.8% with 2.41 survivors on average
+Likelihood of victory 57.7% with 2.7 survivors on average.
 ```
 
 ## Usage
 I have an 11 stack, should I attack that 10 stack? Let's find out!
 
 We can't attack with all 11 stacks, because we have to leave one behind. So when we attack we'll have 10 attacking into 10:
 
 ```sh
 ./risk --attackers 10 --defenders 10
 ```
 
 We see the following output:
 ```sh
-likelihood of victory 52.8% with 2.41 survivors on average
+Likelihood of victory 57.7% with 2.7 survivors on average.
 ```
 
-The script tells us we have a 52.8% chance of winning, and on average we'll have 2.41 survivors (3.41 if you include the stack left behind).
+The script tells us we have a 57.7% chance of winning, and on average we'll have 2.7 survivors (3.7 if you include the stack left behind).
 
 
 ## build & deploy
 bump version in `setup.py`
 `g a . && g c -m "bump version"`
 `python setup.py sdist bdist_wheel`
 `twine upload dist/* --skip-existing`
```

### Comparing `riskCalculator-0.0.4/riskCalculator/parseArguments.py` & `riskCalculator-0.0.5/riskCalculator/parseArguments.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.4/riskCalculator/probabilityOfLosses.py` & `riskCalculator-0.0.5/riskCalculator/probabilityOfLosses.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 def probabilityOfLosses(attackDie: int, defenseDie: int, losses: int):
     if (defenseDie == 0):
-        return 0
+        return 0 if losses > 0 else 1
     if (defenseDie == 1):
         return probabilityOfXLossesOneDefender(attackDie, losses)
     return probabilityOfXLossesTwoDefenders(attackDie, losses)
 
 
 def probabilityOfXLossesOneDefender(attackDie: int, losses: int):
+    if (losses > 1):
+        return 0
     if (losses == 0):
-        return [0.417, 0.579, 0.66][attackDie - 1]
-    return [0.583, 0.421, 0.34][attackDie - 1]
+        return [0.4167, 0.5787, 0.6597][attackDie - 1]
+    return [0.5833, 0.4213, 0.3403][attackDie - 1]
 
 
 def probabilityOfXLossesTwoDefenders(attackDie: int, losses: int):
     if (losses == 0):
-        return [0.255, 0.228, 0.372][attackDie - 1]
+        return [0.2546, 0.2276, 0.3717][attackDie - 1]
     if (losses == 1):
-        return [0, 0.448, 0.292][attackDie - 1]
-    return [0.745, 0.448, 0.336][attackDie - 1]
+        return [0.7454, 0.3241, 0.3358][attackDie - 1]
+    return [0, 0.4483, 0.2926][attackDie - 1]
```

### Comparing `riskCalculator-0.0.4/riskCalculator/readWriteData.py` & `riskCalculator-0.0.5/riskCalculator/readWriteData.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.4/riskCalculator/recursiveMarkovChain.py` & `riskCalculator-0.0.5/riskCalculator/recursiveMarkovChain.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.4/riskCalculator/risk.py` & `riskCalculator-0.0.5/riskCalculator/risk.py`

 * *Files identical despite different names*

### Comparing `riskCalculator-0.0.4/riskCalculator.egg-info/PKG-INFO` & `riskCalculator-0.0.5/riskCalculator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskCalculator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple python package for calculating expected outcome of a risk battle
 Author: Angus Leck
 Author-email: aleck42@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `riskCalculator-0.0.4/setup.py` & `riskCalculator-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Simple python package for calculating expected outcome of a risk battle'
 LONG_DESCRIPTION = 'Simple python package for calculating expected outcome of a risk battle'
 
 # Setting up
 setup(
     name="riskCalculator",
     version=VERSION,
```

