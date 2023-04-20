# Comparing `tmp/proteinTools-1.1.6.tar.gz` & `tmp/proteinTools-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.1.6.tar", last modified: Wed Apr 19 22:39:46 2023, max compression
+gzip compressed data, was "proteinTools-1.1.7.tar", last modified: Thu Apr 20 04:14:51 2023, max compression
```

## Comparing `proteinTools-1.1.6.tar` & `proteinTools-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 22:39:46.916699 proteinTools-1.1.6/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.6/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 22:39:46.914130 proteinTools-1.1.6/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.6/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 22:39:46.853638 proteinTools-1.1.6/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    50482 2023-04-19 22:39:30.000000 proteinTools-1.1.6/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.6/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 22:39:46.901920 proteinTools-1.1.6/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 22:39:46.000000 proteinTools-1.1.6/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-19 22:39:46.000000 proteinTools-1.1.6/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-19 22:39:46.000000 proteinTools-1.1.6/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-19 22:39:46.000000 proteinTools-1.1.6/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-19 22:39:46.000000 proteinTools-1.1.6/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-19 22:39:46.920469 proteinTools-1.1.6/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-19 22:24:41.000000 proteinTools-1.1.6/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 04:14:50.983177 proteinTools-1.1.7/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.7/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 04:14:50.979325 proteinTools-1.1.7/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.7/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 04:14:50.907026 proteinTools-1.1.7/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    50587 2023-04-20 04:14:08.000000 proteinTools-1.1.7/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.7/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 04:14:50.962792 proteinTools-1.1.7/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 04:14:50.000000 proteinTools-1.1.7/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 04:14:50.000000 proteinTools-1.1.7/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 04:14:50.000000 proteinTools-1.1.7/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 04:14:50.000000 proteinTools-1.1.7/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 04:14:50.000000 proteinTools-1.1.7/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 04:14:50.988992 proteinTools-1.1.7/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 04:14:43.000000 proteinTools-1.1.7/setup.py
```

### Comparing `proteinTools-1.1.6/LICENSE` & `proteinTools-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.1.6/proteinTools/PT.py` & `proteinTools-1.1.7/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,15 +554,18 @@
                         if site != '' and '\n' not in site and line[18:21] != 'HOH':
                             sites.append(site)
                     if firstRun == True:
                         curr_site = line[11:14]
                         firstRun = False
                     if line[11:14] != curr_site or data[count + 1][0:4] != 'SITE':
                         curr_site = line[11:14]
-                        self.ligand_list[counter].sites = sites
+                        try:
+                            self.ligand_list[counter].sites = sites
+                        except:
+                            continue
                         sites = []
                         counter += 1    
     
         #Generates FASTA sequence based on protein file
         self.FASTA = ''
         for id_residue in self.residue_list:
             self.FASTA += FASTAdict[id_residue.amino_acid]
@@ -1118,13 +1121,13 @@
     TODO
     - Add more ID conversions
     '''
 
 '''
 #For unit testing    
 if __name__ == '__main__':
-    p = Protein('11ba')
+    p = Protein('3akm')
     p.download()
     for res in p.residue_list:
         for atom in res.atoms:
             print(atom.radius)
 '''
```

### Comparing `proteinTools-1.1.6/setup.py` & `proteinTools-1.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.1.6",
+    version = "1.1.7",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

