# Comparing `tmp/proteinTools-1.2.6.tar.gz` & `tmp/proteinTools-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.2.6.tar", last modified: Thu Apr 20 16:56:22 2023, max compression
+gzip compressed data, was "proteinTools-1.2.7.tar", last modified: Thu Apr 20 17:23:30 2023, max compression
```

## Comparing `proteinTools-1.2.6.tar` & `proteinTools-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.315647 proteinTools-1.2.6/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.6/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 16:56:22.311140 proteinTools-1.2.6/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.6/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.229270 proteinTools-1.2.6/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    51524 2023-04-20 15:41:31.000000 proteinTools-1.2.6/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.6/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.294686 proteinTools-1.2.6/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 16:56:22.320272 proteinTools-1.2.6/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 16:56:09.000000 proteinTools-1.2.6/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.407026 proteinTools-1.2.7/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.7/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 17:23:30.401889 proteinTools-1.2.7/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.7/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.268824 proteinTools-1.2.7/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    51744 2023-04-20 17:23:15.000000 proteinTools-1.2.7/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.7/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 17:23:30.365679 proteinTools-1.2.7/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 17:23:30.000000 proteinTools-1.2.7/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 17:23:30.415181 proteinTools-1.2.7/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 17:23:22.000000 proteinTools-1.2.7/setup.py
```

### Comparing `proteinTools-1.2.6/LICENSE` & `proteinTools-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.2.6/proteinTools/PT.py` & `proteinTools-1.2.7/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,18 +465,22 @@
                     elif line[0:5] == 'SHEET':
                         line = [i for i in line.split(' ') if i != '']
                         try:
                             start = int(line[5])
                             end = int(line[8])
                             chain = line[4]
                         except:
-                            start = int(line[6])
-                            end = int(line[9])
-                            chain = line[5]
-                        
+                            try:
+                                start = int(line[6])
+                                end = int(line[9])
+                                chain = line[5]
+                            except:
+                                start = int(line[5][1:])
+                                end = int(line[8])
+                                chain = line[5][:1]
                         chainindex = chainkeys.index(chain)
                         for i in range(0, chainindex):
                             start += self.chains[chainkeys[i]]
                             end += self.chains[chainkeys[i]]
 
                         for i in range(start, end + 1):
                             sheet.append(i)
```

### Comparing `proteinTools-1.2.6/setup.py` & `proteinTools-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.2.6",
+    version = "1.2.7",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

