# Comparing `tmp/proteinTools-1.2.5.tar.gz` & `tmp/proteinTools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.2.5.tar", last modified: Thu Apr 20 15:14:34 2023, max compression
+gzip compressed data, was "proteinTools-1.2.6.tar", last modified: Thu Apr 20 16:56:22 2023, max compression
```

## Comparing `proteinTools-1.2.5.tar` & `proteinTools-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 15:14:34.767852 proteinTools-1.2.5/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.5/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 15:14:34.763865 proteinTools-1.2.5/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.5/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 15:14:34.677780 proteinTools-1.2.5/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    51524 2023-04-20 15:14:19.000000 proteinTools-1.2.5/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.5/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 15:14:34.748743 proteinTools-1.2.5/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 15:14:34.000000 proteinTools-1.2.5/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 15:14:34.000000 proteinTools-1.2.5/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 15:14:34.000000 proteinTools-1.2.5/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 15:14:34.000000 proteinTools-1.2.5/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 15:14:34.000000 proteinTools-1.2.5/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 15:14:34.771686 proteinTools-1.2.5/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 15:14:27.000000 proteinTools-1.2.5/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.315647 proteinTools-1.2.6/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.6/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 16:56:22.311140 proteinTools-1.2.6/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.6/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.229270 proteinTools-1.2.6/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    51524 2023-04-20 15:41:31.000000 proteinTools-1.2.6/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.6/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 16:56:22.294686 proteinTools-1.2.6/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 16:56:22.000000 proteinTools-1.2.6/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 16:56:22.320272 proteinTools-1.2.6/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 16:56:09.000000 proteinTools-1.2.6/setup.py
```

### Comparing `proteinTools-1.2.5/LICENSE` & `proteinTools-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.2.5/proteinTools/PT.py` & `proteinTools-1.2.6/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
                         self.residue_list.append(res)
                     element = line[77:79].strip()
                     if element not in atom_keys:
                         element = element[:1]
                     try:
                         atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line)
                     except:
-                        atm = atom(element, float(line[29:37].strip()), float(line[37:46].strip()), float(line[46:55].strip()), residue = res.chain + str(resnum), data = line)
+                        atm = atom(element, float(line[30:37].strip()), float(line[38:46].strip()), float(line[47:55].strip()), residue = res.chain + str(resnum), data = line)
                     res.atoms.append(atm)
             
             
             if self.ID_type == 'PDB':
                 #Generates ligands if PDB filetype and ligands in file
                 sheet, helix, chainkeys = [], [], list(self.chains.keys())
                 for count, line in enumerate(data):
```

### Comparing `proteinTools-1.2.5/setup.py` & `proteinTools-1.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.2.5",
+    version = "1.2.6",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

