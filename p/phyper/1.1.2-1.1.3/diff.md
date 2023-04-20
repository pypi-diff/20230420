# Comparing `tmp/phyper-1.1.2-py3-none-any.whl.zip` & `tmp/phyper-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 28806 bytes, number of entries: 15
+Zip file size: 29225 bytes, number of entries: 15
 -rw-r--r--  2.0 unx      685 b- defN 23-Apr-20 10:38 phyper/__init__.py
 -rw-r--r--  2.0 unx      292 b- defN 23-Apr-20 12:42 phyper/chemometrics/__init__.py
 -rw-r--r--  2.0 unx     9505 b- defN 23-Apr-20 13:00 phyper/chemometrics/_gui.py
 -rw-r--r--  2.0 unx    13252 b- defN 23-Apr-20 10:38 phyper/chemometrics/analysis.py
--rw-r--r--  2.0 unx    48428 b- defN 23-Apr-20 12:55 phyper/chemometrics/dataset.py
+-rw-r--r--  2.0 unx    50208 b- defN 23-Apr-20 14:26 phyper/chemometrics/dataset.py
 -rw-r--r--  2.0 unx     2713 b- defN 23-Apr-20 10:38 phyper/chemometrics/preprocessing.py
 -rw-r--r--  2.0 unx     2298 b- defN 23-Apr-20 10:38 phyper/chemometrics/sampling.py
 -rw-r--r--  2.0 unx      121 b- defN 23-Apr-20 10:38 phyper/lab/__init__.py
 -rw-r--r--  2.0 unx      802 b- defN 23-Apr-20 10:38 phyper/lab/_misc.py
--rw-r--r--  2.0 unx    15275 b- defN 23-Apr-20 10:38 phyper/lab/measurement.py
--rwxrwxrwx  2.0 unx     1075 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2231 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-20 13:03 phyper-1.1.2.dist-info/RECORD
-15 files, 97995 bytes uncompressed, 26796 bytes compressed:  72.7%
+-rw-r--r--  2.0 unx    15275 b- defN 23-Apr-20 13:35 phyper/lab/measurement.py
+-rwxrwxrwx  2.0 unx     1075 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2231 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/RECORD
+15 files, 99775 bytes uncompressed, 27215 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: phyper/lab/_misc.py
 Comment: 
 
 Filename: phyper/lab/measurement.py
 Comment: 
 
-Filename: phyper-1.1.2.dist-info/LICENSE
+Filename: phyper-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: phyper-1.1.2.dist-info/METADATA
+Filename: phyper-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: phyper-1.1.2.dist-info/WHEEL
+Filename: phyper-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: phyper-1.1.2.dist-info/top_level.txt
+Filename: phyper-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: phyper-1.1.2.dist-info/RECORD
+Filename: phyper-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phyper/chemometrics/dataset.py

```diff
@@ -10,14 +10,15 @@
 
 from .preprocessing import _Preprocess
 from ._gui import Gui, MaskCreator, PointsCreator
 from .. import WL_UNIT, WL_UNIT_LONG
 from copy import deepcopy
 from spectral import open_image
 from scipy.signal import medfilt
+import pandas as pd
 
 def _docstring_parameter(*sub):
     def dec(obj):
         obj.__doc__ = obj.__doc__.format(*sub)
         return obj
     return dec
 
@@ -460,17 +461,19 @@
         --------
         get_label_table
         get_labels
         """
 
         if not self._has_label_id(label_id):
             self.label_table.append((label_id, label_name))
-        else:
+        elif self.get_label_name(label_id) != label_name:
             print('Label {0} was already in labeltabel with name {1} (instead of given name {2})'.format(label_id, self.get_label_name(label_id), label_name))
-
+        else:
+            pass
+        
     def get_label_name(self, label_id) -> Optional[str]:
         """ Get the label name beloging to the `label_id`.
         
         Parameters
         ---------
         label_id : int
             Label_id as can be found in the labels from this dataset.
@@ -516,15 +519,27 @@
         else:
             label_table = list()
             for label in self.label_table:
                 label_id, label_name = label
                 label_quantity = sum(self.get_labels()==label_id)
                 label_table.append((label_id, label_name,label_quantity))
             return label_table
+        
+    ############################# Saving and loading #############################
 
+    def to_csv(self, filepath, preproc=True, fill=False, columns=None):
+        data = self.get_data(preproc=preproc, fill_nans=fill)
+        if self._has_labels():
+            labels = self.get_labels(fill=fill)
+            data = np.concatenate([data, labels[:, None]], axis=1)
+        df = pd.DataFrame(data, columns=columns)
+        if self._has_labels():
+            df.label = df.label.apply(lambda x: self.get_label_name(x))
+        df.to_csv(filepath, index=False)
+        
     ############################# Utils #############################
     def _get_mean_data(self, by_label=True) -> Union[tuple, np.ndarray]:
         """ Get data mean. If labels are given, the mean for each label will be returned.
         
         Parameters
         ----------
         by_label : bool, optional
@@ -775,14 +790,42 @@
         if not self._is_valid_wavelength(wavelength):
             raise ValueError('Invalid wavelength {0}{1}.'.format(wavelength, WL_UNIT))
 
         diff = (np.abs(self.get_wl() - wavelength))
 
         idx = diff.argmin()
         return idx
+        
+    ############################# Saving and loading #############################
+
+    def to_csv(self, filepath, preproc=True, fill=False):
+        wl = self.get_wl()
+        wl = np.around(wl, decimals=2)
+        wl = wl.astype(str)
+        columns = list(wl)
+        if self._has_labels():
+            columns.append('label')
+        super().to_csv(filepath, preproc, fill, columns=columns)
+
+    @classmethod
+    def from_csv(cls, path):
+        df = pd.read_csv(path)
+        if 'label' in df.columns:
+            labels = df['label'] #labels are saved as string e.g. 'healthy'
+            label_names = np.sort(np.unique(labels))
+            label_ids = np.arange(len(label_names))
+            label_table = list(zip(list(label_ids), list(label_names)))
+            df['label'].replace(label_names, label_ids, inplace=True)
+            labels = df.pop('label')
+        else:
+            labels=None
+            label_table=None
+        data = df.to_numpy()
+        wl =  np.asarray(df.columns.astype(float))
+        return SpectralDataset(data, wl,labels=labels, label_table=label_table)
 
     def plot(self, nb_spectra=100, labels=True, ax=None, class_ids = [], show=True):
         """ See Dataset.plot """
         if ax is None:
             ax = pyplot.subplot(111)
         ax.set_xlabel('Wavelength [{0}]'.format(WL_UNIT))
         ax.set_ylabel('Reflectance [-]')
```

## Comparing `phyper-1.1.2.dist-info/LICENSE` & `phyper-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phyper-1.1.2.dist-info/METADATA` & `phyper-1.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyper
-Version: 1.1.2
+Version: 1.1.3
 Summary: Package for managing (hyper)spectral datasets
 Home-page: https://gitlab.kuleuven.be/u0123403/pyper
 Author: Remi Van Belleghem
 Author-email: remi.vanbelleghem@kuleuven.be
 Maintainer: MeBios - KULeuven
 Maintainer-email: wouter.saeys@kuleuven.be
 Keywords: hyperspectral,chemometrics
```

## Comparing `phyper-1.1.2.dist-info/RECORD` & `phyper-1.1.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 phyper/__init__.py,sha256=4hYB58cealu01B6FLn3lhRnI0JAPY6Va107e65WXTcs,685
 phyper/chemometrics/__init__.py,sha256=5y7WaXHDvt1RbplvdekletkldO9cMdvYHRFzJkE1ziE,292
 phyper/chemometrics/_gui.py,sha256=3h4jW2pVt-14QTx3g-wFnMzaQTq8SZC2BBabRBZ9bpA,9505
 phyper/chemometrics/analysis.py,sha256=903ZGNPjkmJL_z0CeeorcQkoiCMZLeOYK3_q18CmBnc,13252
-phyper/chemometrics/dataset.py,sha256=cb4A3edpXYI0IEQ-QaCP7o8diph15cNHgF4LkffKsyg,48428
+phyper/chemometrics/dataset.py,sha256=usVvonWQZXK6gdy0jNdjdiTRRJ_tgM2u3IaQbocnjKM,50208
 phyper/chemometrics/preprocessing.py,sha256=lKoB64-a4IdM82pC1OAh9cCy-LXKLOcFbygVYnQCBcM,2713
 phyper/chemometrics/sampling.py,sha256=H-xl0PrAwRoaxwah8DqVSlRJ1gPl9Qm806Zh7MPuu2U,2298
 phyper/lab/__init__.py,sha256=p1f53MLglxawnDhRGT4O1NI5CpL2Rvski2XEyg9ErM8,121
 phyper/lab/_misc.py,sha256=irgAaObHkaIBESTdw-o0e0Eb-z2pUm9Kdc9ujZq8pg8,802
 phyper/lab/measurement.py,sha256=YCQX5YkgWDmwesoELt14JgdWcVYc2vq8cqnjIbxHfSM,15275
-phyper-1.1.2.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
-phyper-1.1.2.dist-info/METADATA,sha256=rsaJ8dFhjWDd87IaeJPwJdq1crlJsJvs_sCKnLjAFtU,2231
-phyper-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-phyper-1.1.2.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
-phyper-1.1.2.dist-info/RECORD,,
+phyper-1.1.3.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
+phyper-1.1.3.dist-info/METADATA,sha256=wtwBal0wXrDPj4jr4I6gUC453-KX9aA2Ss0K6_wHX8E,2231
+phyper-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+phyper-1.1.3.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
+phyper-1.1.3.dist-info/RECORD,,
```

