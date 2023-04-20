# Comparing `tmp/kurzgesagt-1.1.1.tar.gz` & `tmp/kurzgesagt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurzgesagt-1.1.1.tar", last modified: Sun Apr  9 20:32:59 2023, max compression
+gzip compressed data, was "kurzgesagt-1.1.2.tar", last modified: Thu Apr 20 21:02:23 2023, max compression
```

## Comparing `kurzgesagt-1.1.1.tar` & `kurzgesagt-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-09 20:32:59.484851 kurzgesagt-1.1.1/
--rw-rw-r--   0 edgar     (1000) edgar     (1000)      605 2023-04-09 20:32:59.488851 kurzgesagt-1.1.1/PKG-INFO
--rw-rw-r--   0 edgar     (1000) edgar     (1000)      169 2023-02-08 20:19:27.000000 kurzgesagt-1.1.1/README.md
--rw-rw-r--   0 edgar     (1000) edgar     (1000)       89 2023-04-09 20:32:59.488851 kurzgesagt-1.1.1/setup.cfg
--rw-rw-r--   0 edgar     (1000) edgar     (1000)      854 2023-04-09 20:32:22.000000 kurzgesagt-1.1.1/setup.py
-drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-09 20:32:59.484851 kurzgesagt-1.1.1/src/
-drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-09 20:32:59.484851 kurzgesagt-1.1.1/src/kurzgesagt/
--rw-rw-r--   0 edgar     (1000) edgar     (1000)     1960 2023-04-09 20:32:29.000000 kurzgesagt-1.1.1/src/kurzgesagt/__init__.py
-drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-09 20:32:59.484851 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/
--rw-rw-r--   0 edgar     (1000) edgar     (1000)      605 2023-04-09 20:32:59.000000 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/PKG-INFO
--rw-rw-r--   0 edgar     (1000) edgar     (1000)      244 2023-04-09 20:32:59.000000 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/SOURCES.txt
--rw-rw-r--   0 edgar     (1000) edgar     (1000)        1 2023-04-09 20:32:59.000000 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/dependency_links.txt
--rw-rw-r--   0 edgar     (1000) edgar     (1000)       31 2023-04-09 20:32:59.000000 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/requires.txt
--rw-rw-r--   0 edgar     (1000) edgar     (1000)       11 2023-04-09 20:32:59.000000 kurzgesagt-1.1.1/src/kurzgesagt.egg-info/top_level.txt
+drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)      605 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/PKG-INFO
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)      169 2023-02-08 20:19:27.000000 kurzgesagt-1.1.2/README.md
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)       89 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/setup.cfg
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)      854 2023-04-09 20:32:22.000000 kurzgesagt-1.1.2/setup.py
+drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/src/
+drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/src/kurzgesagt/
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)     1822 2023-04-20 21:00:02.000000 kurzgesagt-1.1.2/src/kurzgesagt/__init__.py
+drwxrwxr-x   0 edgar     (1000) edgar     (1000)        0 2023-04-20 21:02:23.983161 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)      605 2023-04-20 21:02:23.000000 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/PKG-INFO
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)      244 2023-04-20 21:02:23.000000 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/SOURCES.txt
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)        1 2023-04-20 21:02:23.000000 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/dependency_links.txt
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)       31 2023-04-20 21:02:23.000000 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/requires.txt
+-rw-rw-r--   0 edgar     (1000) edgar     (1000)       11 2023-04-20 21:02:23.000000 kurzgesagt-1.1.2/src/kurzgesagt.egg-info/top_level.txt
```

### Comparing `kurzgesagt-1.1.1/PKG-INFO` & `kurzgesagt-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kurzgesagt
-Version: 1.1.1
+Version: 1.1.2
 Summary: A puzzle.
 Home-page: https://gitlab.com/eklenske/kurzgesagt
 Author: Carl Friedrich
 Author-email: carl-friedrich@mailbox.org
 Keywords: puzzle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `kurzgesagt-1.1.1/setup.py` & `kurzgesagt-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `kurzgesagt-1.1.1/src/kurzgesagt/__init__.py` & `kurzgesagt-1.1.2/src/kurzgesagt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """The Kurzgesagt Package"""
 import os
 import webbrowser
 from random import shuffle
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 ALPHA = list("Z(Uf!tEn:kGIAismuWeK?)oFwcyrzXRM JqOBNH,aDTgQxSCljvhpdbYPVL.")
 MESSAGE = "NujR!hioe(FEwiMc)sMAE!WoWsZWh At HMcWLfmkyKoM,MC)dMAEZWrxAuwKRTjWnrgeUFkmr:E)ofM miZMsiEh su HMpOZclkCXxWyiI)EM)Ur!hiMAomccuMcWleXbnxiMFvuyWM!v:i iycoyRiAMtSoo)LdXcWhCHwWM!v:i GWAs,DeRFiZS FiGwrsWiA,TWM!WMmiLROURc?mrki,XEqEiMimcWMc)m'yermAiED fverkaAkymUwycv!A)EMGWtS)h.ME)"
 MAGIC = 12021055047710724565076463829
 
 print(
-    "Dear friend, thanks for starting this puzzle journey with me! There are still some steps ahead of you. Most puzzles are just a joke, but not this one, so please don't give up too soon. There will be a reward at the end, if you push through. Good luck!"
+    "Dear friend, thanks for starting this puzzle journey with me! There are still some steps ahead of you. Good luck!"
 )
 
 
 def gauss(prime: int = 2) -> None:
     """Gauss what."""
 
     if MAGIC % prime == 0 and not MAGIC == prime:  # check for the correct prime factor
```

### Comparing `kurzgesagt-1.1.1/src/kurzgesagt.egg-info/PKG-INFO` & `kurzgesagt-1.1.2/src/kurzgesagt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kurzgesagt
-Version: 1.1.1
+Version: 1.1.2
 Summary: A puzzle.
 Home-page: https://gitlab.com/eklenske/kurzgesagt
 Author: Carl Friedrich
 Author-email: carl-friedrich@mailbox.org
 Keywords: puzzle
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

