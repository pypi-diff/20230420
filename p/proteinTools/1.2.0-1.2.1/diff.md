# Comparing `tmp/proteinTools-1.2.0.tar.gz` & `tmp/proteinTools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.2.0.tar", last modified: Thu Apr 20 05:44:39 2023, max compression
+gzip compressed data, was "proteinTools-1.2.1.tar", last modified: Thu Apr 20 06:05:05 2023, max compression
```

## Comparing `proteinTools-1.2.0.tar` & `proteinTools-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 05:44:39.518430 proteinTools-1.2.0/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.0/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 05:44:39.512719 proteinTools-1.2.0/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.0/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 05:44:39.413085 proteinTools-1.2.0/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    50699 2023-04-20 05:43:28.000000 proteinTools-1.2.0/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.0/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 05:44:39.491356 proteinTools-1.2.0/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 05:44:39.000000 proteinTools-1.2.0/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 05:44:39.000000 proteinTools-1.2.0/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 05:44:39.000000 proteinTools-1.2.0/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 05:44:39.000000 proteinTools-1.2.0/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 05:44:39.000000 proteinTools-1.2.0/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 05:44:39.529523 proteinTools-1.2.0/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 05:44:18.000000 proteinTools-1.2.0/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 06:05:04.993308 proteinTools-1.2.1/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.2.1/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 06:05:04.990318 proteinTools-1.2.1/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.2.1/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 06:05:04.829250 proteinTools-1.2.1/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    50714 2023-04-20 06:04:28.000000 proteinTools-1.2.1/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.2.1/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-20 06:05:04.973505 proteinTools-1.2.1/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-20 06:05:04.000000 proteinTools-1.2.1/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-20 06:05:04.000000 proteinTools-1.2.1/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-20 06:05:04.000000 proteinTools-1.2.1/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-20 06:05:04.000000 proteinTools-1.2.1/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-20 06:05:04.000000 proteinTools-1.2.1/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-20 06:05:04.997638 proteinTools-1.2.1/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-20 06:04:47.000000 proteinTools-1.2.1/setup.py
```

### Comparing `proteinTools-1.2.0/LICENSE` & `proteinTools-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.2.0/proteinTools/PT.py` & `proteinTools-1.2.1/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,16 @@
                         self.chains[chain] = int(line[13:17].strip())
                         
                 elif line[0:4] == 'ATOM':
                     resnum = int(line[23:27].strip())
                     if resnum != curr_residue:
                         curr_residue = resnum
                         chain, AA = line[21:22], line[17:20]
+                        if ' ' in AA:
+                            AA = line[19:22]
                         res = residue(amino_acid = AA, index = resnum, chain = chain)
                         self.residue_list.append(res)
                     element = line[77:79].strip()
                     if element not in atom_keys:
                         element = element[:1]
                     atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), residue = res.chain + str(resnum), data = line)
                     res.atoms.append(atm)
@@ -564,16 +566,14 @@
                             continue
                         sites = []
                         counter += 1    
     
         #Generates FASTA sequence based on protein file
         self.FASTA = ''
         for id_residue in self.residue_list:
-            if id_residue.amino_acid.strip() == 'U':
-                id_residue.amino_acid = 'UNK'
             self.FASTA += FASTAdict[id_residue.amino_acid]
     
     def to_csv(self, destination = os.getcwd()):
         """
         Atoms to CSV
     
         This method returns a .csv file of each individual atom of the protein and all contained attributes within the atom.
@@ -1089,14 +1089,15 @@
                 for act in activities:
                     value = float(act['value'])
                     if act['units'] != 'nM':
                         if act['units'] == 'uM':
                             value *= 1000
                         elif act['units'] == 'pM':
                             value /= 1000
+               
                     try:
                         ligands.append(act['canonical_smiles'])
                         activities.append(value)
                     except:
                         continue
                 ChEMBL = pd.DataFrame.from_dict({'Ligands':ligands, 'IC50 (uM)':activities})
                 ChEMBL = {'ChEMBL':chembl}
@@ -1128,8 +1129,9 @@
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('3akm')
     p.download()
     for res in p.residue_list:
         for atom in res.atoms:
             print(atom.radius)
+            
 '''
```

### Comparing `proteinTools-1.2.0/setup.py` & `proteinTools-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.2.0",
+    version = "1.2.1",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

