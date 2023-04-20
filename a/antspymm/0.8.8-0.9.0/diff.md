# Comparing `tmp/antspymm-0.8.8.tar.gz` & `tmp/antspymm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspymm-0.8.8.tar", last modified: Mon Mar 20 13:01:52 2023, max compression
+gzip compressed data, was "antspymm-0.9.0.tar", last modified: Thu Apr 20 13:41:02 2023, max compression
```

## Comparing `antspymm-0.8.8.tar` & `antspymm-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-20 13:01:52.331429 antspymm-0.8.8/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.8.8/LICENSE
--rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.8.8/MANIFEST.in
--rw-r--r--   0 stnava     (501) staff       (20)     8019 2023-03-20 13:01:52.331234 antspymm-0.8.8/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     7662 2023-03-20 13:01:18.000000 antspymm-0.8.8/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-20 13:01:52.320417 antspymm-0.8.8/antspymm/
--rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.8.8/antspymm/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)   280383 2023-03-20 12:19:56.000000 antspymm-0.8.8/antspymm/mm.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-20 13:01:52.321991 antspymm-0.8.8/antspymm.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     8019 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)      588 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)      129 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)        9 2023-03-20 13:01:52.000000 antspymm-0.8.8/antspymm.egg-info/top_level.txt
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-20 13:01:52.326299 antspymm-0.8.8/docs/
--rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.8.8/docs/antspymm_data_dictionary.csv
--rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.8.8/docs/make_dict_table.Rmd
--rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.8.8/docs/outlierness.py
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-03-20 13:01:52.331481 antspymm-0.8.8/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)      681 2023-03-17 14:32:52.000000 antspymm-0.8.8/setup.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-03-20 13:01:52.330862 antspymm-0.8.8/tests/
--rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.8.8/tests/mm.py
--rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.8.8/tests/mm_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.8.8/tests/test_bids_2_nrg.py
--rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.8.8/tests/test_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.8.8/tests/test_dwi_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.8.8/tests/test_flair_run.py
--rw-r--r--   0 stnava     (501) staff       (20)     2618 2023-02-20 13:16:33.000000 antspymm-0.8.8/tests/test_joint_dti_recon.py
--rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.8.8/tests/test_mm_csv.py
--rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.8.8/tests/test_rsfmri_run.py
--rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.8.8/tests/testsr.py
--rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.8.8/tests/visualize_tractogram.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.797792 antspymm-0.9.0/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2021-11-01 09:20:32.000000 antspymm-0.9.0/LICENSE
+-rw-r--r--   0 stnava     (501) staff       (20)       33 2023-01-29 13:38:57.000000 antspymm-0.9.0/MANIFEST.in
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-04-20 13:41:02.797531 antspymm-0.9.0/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)     9827 2023-04-12 13:23:21.000000 antspymm-0.9.0/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.790246 antspymm-0.9.0/antspymm/
+-rw-r--r--   0 stnava     (501) staff       (20)     2690 2023-03-20 11:54:16.000000 antspymm-0.9.0/antspymm/__init__.py
+-rw-r--r--   0 stnava     (501) staff       (20)   284711 2023-04-20 13:37:06.000000 antspymm-0.9.0/antspymm/mm.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.791689 antspymm-0.9.0/antspymm.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    10184 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      741 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/not-zip-safe
+-rw-r--r--   0 stnava     (501) staff       (20)      112 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        9 2023-04-20 13:41:02.000000 antspymm-0.9.0/antspymm.egg-info/top_level.txt
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.795134 antspymm-0.9.0/docs/
+-rw-r--r--   0 stnava     (501) staff       (20)  1939802 2023-01-29 13:48:53.000000 antspymm-0.9.0/docs/antspymm_data_dictionary.csv
+-rw-r--r--   0 stnava     (501) staff       (20)      567 2023-04-12 13:06:30.000000 antspymm-0.9.0/docs/bids_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-04-08 18:52:17.000000 antspymm-0.9.0/docs/example_run_from_directory.py
+-rw-r--r--   0 stnava     (501) staff       (20)      478 2023-02-19 10:57:50.000000 antspymm-0.9.0/docs/make_dict_table.Rmd
+-rw-r--r--   0 stnava     (501) staff       (20)      632 2023-04-12 13:06:30.000000 antspymm-0.9.0/docs/nrg_cohort_example.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2082 2023-03-20 13:00:28.000000 antspymm-0.9.0/docs/outlierness.py
+-rw-r--r--   0 stnava     (501) staff       (20)     3643 2023-04-15 22:47:31.000000 antspymm-0.9.0/docs/ukbb_to_nrg_processing.py
+-rw-r--r--   0 stnava     (501) staff       (20)     4546 2023-04-16 12:24:12.000000 antspymm-0.9.0/docs/ukbb_to_nrg_processing2.py
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2023-04-20 13:41:02.797845 antspymm-0.9.0/setup.cfg
+-rw-r--r--   0 stnava     (501) staff       (20)      681 2023-04-20 13:39:29.000000 antspymm-0.9.0/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-04-20 13:41:02.797260 antspymm-0.9.0/tests/
+-rw-r--r--   0 stnava     (501) staff       (20)     5589 2022-10-21 12:35:02.000000 antspymm-0.9.0/tests/mm.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2087 2022-12-17 20:51:01.000000 antspymm-0.9.0/tests/mm_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      440 2023-03-15 12:39:26.000000 antspymm-0.9.0/tests/test_bids_2_nrg.py
+-rw-r--r--   0 stnava     (501) staff       (20)      394 2022-06-09 14:57:05.000000 antspymm-0.9.0/tests/test_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2507 2023-02-05 20:18:30.000000 antspymm-0.9.0/tests/test_dwi_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      445 2023-02-05 00:06:28.000000 antspymm-0.9.0/tests/test_flair_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2618 2023-02-20 13:16:33.000000 antspymm-0.9.0/tests/test_joint_dti_recon.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1497 2023-03-15 12:44:41.000000 antspymm-0.9.0/tests/test_mm_csv.py
+-rw-r--r--   0 stnava     (501) staff       (20)     2101 2022-11-16 16:52:51.000000 antspymm-0.9.0/tests/test_rsfmri_run.py
+-rw-r--r--   0 stnava     (501) staff       (20)      597 2021-11-02 19:50:00.000000 antspymm-0.9.0/tests/testsr.py
+-rw-r--r--   0 stnava     (501) staff       (20)     1439 2023-03-02 15:01:53.000000 antspymm-0.9.0/tests/visualize_tractogram.py
```

### Comparing `antspymm-0.8.8/LICENSE` & `antspymm-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/PKG-INFO` & `antspymm-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-Metadata-Version: 2.1
-Name: antspymm
-Version: 0.8.8
-Summary: multi-channel/time-series medical image processing with antspyx
-Home-page: https://github.com/stnava/ANTsPyMM
-Author: Avants, Gosselin, Tustison, Reardon
-Author-email: stnava@gmail.com
-License: Apache 2.0
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENSE
-
 # ANTsPyMM
 
 ## processing utilities for timeseries/multichannel images - mostly neuroimaging
 
 the outputs of these processes can be used for data inspection/cleaning/triage
 as well for interrogating hypotheses.
 
 this package also keeps track of the latest preferred algorithm variations for
 production environments.
 
-install by calling (within the source directory):
+install the `dev` version by calling (within the source directory):
 
 ```
 python setup.py install
 ```
 
-or install via `pip install antspymm` **FIXME**
+or install the latest release via 
+
+```
+pip install antspymm
+```
 
 # what this will do
 
 ANTsPyMM will process several types of brain MRI into tabular form as well as normalized (standard template) space.  The processing includes:
 
 * T1wHier uses hierarchical processing from ANTsPyT1w organized around these measurements
 
@@ -75,21 +68,25 @@
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
 # first time setup
 
 ```python
+import antspyt1w
 import antspymm
-antspymm.get_data()
+antspyt1w.get_data(force_download=True)
+antspymm.get_data(force_download=True)
 ```
 
 NOTE: `get_data` has a `force_download` option to make sure the latest
 package data is installed.
 
+NOTE: some functions in `antspynet` will download deep network model weights on the fly.  if one is containerizing, then it would be worth running a test case through in the container to make sure all the relevant weights are pre-downloaded.
+
 # example processing
 
 see the latest help but this snippet gives an idea of how one might use the package:
 
 ```python
 import os
 os.environ["TF_NUM_INTEROP_THREADS"] = "8"
@@ -119,19 +116,22 @@
 
 antspymm.write_mm( '/tmp/test_output', t1wide, tabPro, normPro )
 
 ```
 
 ## blind quality control
 
-automatically qc, filter and match multiple modality images at each time point.
+this package also provides tools to identify the *best* multi-modality image set at a given visit.
+
+the code below provides guidance on how to automatically qc, filter and match multiple modality images at each time point.  these tools are based on standard unsupervised approaches and are not perfect so we recommend using the associated plotting/visualization techniques to check the quality characterizations for each modality.
 
 ```python
 ## run the qc on all images - requires a relatively large sample per modality to be effective
 ## then aggregate
+qcdf=pd.DataFrame()
 for fn in fns:
   qcdf=pd.concat( [qcdf,antspymm.blind_image_assessment(fn)], axis=0)
 qcdfa=antspymm.average_blind_qc_by_modality(qcdf,verbose=True) ## reduce the time series qc
 qcdfaol=antspymm.outlierness_by_modality(qcdfa) # estimate outlier scores
 print( qcdfaol.shape )
 print( qcdfaol.keys )
 matched_mm_data=antspymm.match_modalities( qcdfaol  )
@@ -152,15 +152,14 @@
     alldf = pd.concat( [alldf, jjj ], axis=0 )
     jjj.to_csv( "mm_outlierness_"+m+".csv")
     print(m+" done")
 # write the joined data out
 alldf.to_csv( "mm_outlierness.csv", index=False )
 # find the best mm collection
 matched_mm_data=antspymm.match_modalities( alldf, verbose=True )
-matched_mm_data
 matched_mm_data.to_csv( "matched_mm_data.csv", index=False )
 matched_mm_data['negative_outlier_factor'] = 1.0 - matched_mm_data['ol_loop'].astype("float")
 matched_mm_data2 = antspymm.highest_quality_repeat( matched_mm_data, 'subjectID', 'date', qualityvar='negative_outlier_factor')
 matched_mm_data2.to_csv( "matched_mm_data2.csv", index=False )
 ```
 
 ## an example on open neuro (BIDS) data
@@ -190,23 +189,24 @@
 import antspymm
 import pandas as pd
 import glob as glob
 fns = glob.glob("imagesBIDS/ANTPD/sub-RC4125/ses-*/*/*gz")
 fns.sort()
 randid='000' # BIDS does not have unique image ids - so we assign one
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     randid,
     'T1w',
     '/Users/stnava/data/openneuro/imagesBIDS/',
     '/Users/stnava/data/openneuro/processed/',
     t1_filename=fns[0],
-    dti_filenames=[fns[2]],
-    rsf_filenames=[fns[1]])
+    dti_filenames=[fns[1]],
+    rsf_filenames=[fns[2]])
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
 ## NRG example
 
 NRG format details [here](https://htmlpreview.github.io/?https://github.com/stnava/biomedicalDataOrganization/blob/master/src/nrg_data_organization_summary.html)
@@ -233,38 +233,91 @@
 
 
 ```python
 import antspymm
 import pandas as pd
 import glob as glob
 t1fn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*T1w*gz")[0]
+# flair also takes a single image
 dtfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*DTI*gz")
 rsfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*rsfMRI*gz")
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     '000',
     'T1w',
     '/Users/stnava/data/openneuro/imagesNRG/',
     '/Users/stnava/data/openneuro/processed/',
     t1fn,
     rsf_filenames=rsfn,
     dti_filenames=dtfn
 )
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
+## useful tools for converting dicom to nifti
+
+* [dcm2niix](https://github.com/rordenlab/dcm2niix)
+
+* [dicom2nifti](https://dicom2nifti.readthedocs.io/en/latest/)
+
+```python
+import dicom2nifti
+
+dicom2nifti.convert_directory(dicom_directory, output_folder, compression=True, reorient=True)
+```
+
+* [simpleitk](https://pypi.org/project/SimpleITK/)
+
+```python
+import SimpleITK as sitk
+import sys
+import os
+import glob as glob
+import ants
+dd='dicom'
+oo='dicom2nifti'
+folders=glob.glob('dicom/*')
+k=0
+for f in folders:
+    print(f)    
+    reader = sitk.ImageSeriesReader()
+    ff=glob.glob(f+"/*")
+    dicom_names = reader.GetGDCMSeriesFileNames(ff[0])
+    if len(ff) > 0:
+        fnout='dicom2nifti/image_'+str(k).zfill(4)+'.nii.gz'
+        if not exists(fnout):
+            failed=False
+            reader.SetFileNames(dicom_names)
+            try:
+                image = reader.Execute()
+            except:
+                failed=True
+                pass
+            if not failed:
+                size = image.GetSpacing()
+                print( image.GetMetaDataKeys( ) )
+                print( size )
+                sitk.WriteImage(image, fnout )
+                img=ants.image_read( fnout )
+                img=ants.iMath(img,'TruncateIntensity',0.02,0.98)
+                ants.plot( img, nslices=21,ncol=7,axis=2, crop=True )
+        else:
+            print(f+ ": "+'empty')
+    k=k+1
+```
+
 ## build docs
 
 ```
 pdoc -o ./docs antspymm --html
 ```
 
 ## to publish a release
 
 ```
 rm -r -f build/ antspymm.egg-info/ dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload -u username -p password  dist/*
 ```
-
```

### Comparing `antspymm-0.8.8/README.md` & `antspymm-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,39 @@
+Metadata-Version: 2.1
+Name: antspymm
+Version: 0.9.0
+Summary: multi-channel/time-series medical image processing with antspyx
+Home-page: https://github.com/stnava/ANTsPyMM
+Author: Avants, Gosselin, Tustison, Reardon
+Author-email: stnava@gmail.com
+License: Apache 2.0
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENSE
+
 # ANTsPyMM
 
 ## processing utilities for timeseries/multichannel images - mostly neuroimaging
 
 the outputs of these processes can be used for data inspection/cleaning/triage
 as well for interrogating hypotheses.
 
 this package also keeps track of the latest preferred algorithm variations for
 production environments.
 
-install by calling (within the source directory):
+install the `dev` version by calling (within the source directory):
 
 ```
 python setup.py install
 ```
 
-or install via `pip install antspymm` **FIXME**
+or install the latest release via 
+
+```
+pip install antspymm
+```
 
 # what this will do
 
 ANTsPyMM will process several types of brain MRI into tabular form as well as normalized (standard template) space.  The processing includes:
 
 * T1wHier uses hierarchical processing from ANTsPyT1w organized around these measurements
 
@@ -64,21 +79,25 @@
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
 # first time setup
 
 ```python
+import antspyt1w
 import antspymm
-antspymm.get_data()
+antspyt1w.get_data(force_download=True)
+antspymm.get_data(force_download=True)
 ```
 
 NOTE: `get_data` has a `force_download` option to make sure the latest
 package data is installed.
 
+NOTE: some functions in `antspynet` will download deep network model weights on the fly.  if one is containerizing, then it would be worth running a test case through in the container to make sure all the relevant weights are pre-downloaded.
+
 # example processing
 
 see the latest help but this snippet gives an idea of how one might use the package:
 
 ```python
 import os
 os.environ["TF_NUM_INTEROP_THREADS"] = "8"
@@ -108,19 +127,22 @@
 
 antspymm.write_mm( '/tmp/test_output', t1wide, tabPro, normPro )
 
 ```
 
 ## blind quality control
 
-automatically qc, filter and match multiple modality images at each time point.
+this package also provides tools to identify the *best* multi-modality image set at a given visit.
+
+the code below provides guidance on how to automatically qc, filter and match multiple modality images at each time point.  these tools are based on standard unsupervised approaches and are not perfect so we recommend using the associated plotting/visualization techniques to check the quality characterizations for each modality.
 
 ```python
 ## run the qc on all images - requires a relatively large sample per modality to be effective
 ## then aggregate
+qcdf=pd.DataFrame()
 for fn in fns:
   qcdf=pd.concat( [qcdf,antspymm.blind_image_assessment(fn)], axis=0)
 qcdfa=antspymm.average_blind_qc_by_modality(qcdf,verbose=True) ## reduce the time series qc
 qcdfaol=antspymm.outlierness_by_modality(qcdfa) # estimate outlier scores
 print( qcdfaol.shape )
 print( qcdfaol.keys )
 matched_mm_data=antspymm.match_modalities( qcdfaol  )
@@ -141,15 +163,14 @@
     alldf = pd.concat( [alldf, jjj ], axis=0 )
     jjj.to_csv( "mm_outlierness_"+m+".csv")
     print(m+" done")
 # write the joined data out
 alldf.to_csv( "mm_outlierness.csv", index=False )
 # find the best mm collection
 matched_mm_data=antspymm.match_modalities( alldf, verbose=True )
-matched_mm_data
 matched_mm_data.to_csv( "matched_mm_data.csv", index=False )
 matched_mm_data['negative_outlier_factor'] = 1.0 - matched_mm_data['ol_loop'].astype("float")
 matched_mm_data2 = antspymm.highest_quality_repeat( matched_mm_data, 'subjectID', 'date', qualityvar='negative_outlier_factor')
 matched_mm_data2.to_csv( "matched_mm_data2.csv", index=False )
 ```
 
 ## an example on open neuro (BIDS) data
@@ -179,23 +200,24 @@
 import antspymm
 import pandas as pd
 import glob as glob
 fns = glob.glob("imagesBIDS/ANTPD/sub-RC4125/ses-*/*/*gz")
 fns.sort()
 randid='000' # BIDS does not have unique image ids - so we assign one
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     randid,
     'T1w',
     '/Users/stnava/data/openneuro/imagesBIDS/',
     '/Users/stnava/data/openneuro/processed/',
     t1_filename=fns[0],
-    dti_filenames=[fns[2]],
-    rsf_filenames=[fns[1]])
+    dti_filenames=[fns[1]],
+    rsf_filenames=[fns[2]])
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
 ## NRG example
 
 NRG format details [here](https://htmlpreview.github.io/?https://github.com/stnava/biomedicalDataOrganization/blob/master/src/nrg_data_organization_summary.html)
@@ -222,38 +244,91 @@
 
 
 ```python
 import antspymm
 import pandas as pd
 import glob as glob
 t1fn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*T1w*gz")[0]
+# flair also takes a single image
 dtfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*DTI*gz")
 rsfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*rsfMRI*gz")
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     '000',
     'T1w',
     '/Users/stnava/data/openneuro/imagesNRG/',
     '/Users/stnava/data/openneuro/processed/',
     t1fn,
     rsf_filenames=rsfn,
     dti_filenames=dtfn
 )
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
+## useful tools for converting dicom to nifti
+
+* [dcm2niix](https://github.com/rordenlab/dcm2niix)
+
+* [dicom2nifti](https://dicom2nifti.readthedocs.io/en/latest/)
+
+```python
+import dicom2nifti
+
+dicom2nifti.convert_directory(dicom_directory, output_folder, compression=True, reorient=True)
+```
+
+* [simpleitk](https://pypi.org/project/SimpleITK/)
+
+```python
+import SimpleITK as sitk
+import sys
+import os
+import glob as glob
+import ants
+dd='dicom'
+oo='dicom2nifti'
+folders=glob.glob('dicom/*')
+k=0
+for f in folders:
+    print(f)    
+    reader = sitk.ImageSeriesReader()
+    ff=glob.glob(f+"/*")
+    dicom_names = reader.GetGDCMSeriesFileNames(ff[0])
+    if len(ff) > 0:
+        fnout='dicom2nifti/image_'+str(k).zfill(4)+'.nii.gz'
+        if not exists(fnout):
+            failed=False
+            reader.SetFileNames(dicom_names)
+            try:
+                image = reader.Execute()
+            except:
+                failed=True
+                pass
+            if not failed:
+                size = image.GetSpacing()
+                print( image.GetMetaDataKeys( ) )
+                print( size )
+                sitk.WriteImage(image, fnout )
+                img=ants.image_read( fnout )
+                img=ants.iMath(img,'TruncateIntensity',0.02,0.98)
+                ants.plot( img, nslices=21,ncol=7,axis=2, crop=True )
+        else:
+            print(f+ ": "+'empty')
+    k=k+1
+```
+
 ## build docs
 
 ```
 pdoc -o ./docs antspymm --html
 ```
 
 ## to publish a release
 
 ```
 rm -r -f build/ antspymm.egg-info/ dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload -u username -p password  dist/*
 ```
-
```

### Comparing `antspymm-0.8.8/antspymm/__init__.py` & `antspymm-0.9.0/antspymm/__init__.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/antspymm/mm.py` & `antspymm-0.9.0/antspymm/mm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 __all__ = ['version',
     'mm_read',
     'mm_read_to_3d',
     'image_write_with_thumbnail',
     'nrg_format_path',
-    'higest_quality_repeat',
+    'highest_quality_repeat',
     'match_modalities',
     'mc_resample_image_to_target',
     'nrg_filelist_to_dataframe',
     'merge_timeseries_data',
     'timeseries_reg',
     'merge_dwi_data',
     'outlierness_by_modality',
@@ -166,22 +166,23 @@
     else:
         mymodchar=""
         for x in mymod:
             mymodchar = mymodchar + " " + str(x)
         return mymodchar
 
 def generate_mm_dataframe(
+        projectID,
         subjectID,
         date,
         imageUniqueID,
         modality,
         source_image_directory,
         output_image_directory,
         t1_filename,
-        flair_filename=None,
+        flair_filename=[],
         rsf_filenames=[],
         dti_filenames=[],
         nm_filenames=[]
 ):
     from os.path import exists
     valid_modalities = get_valid_modalities()
     if not isinstance(t1_filename, str):
@@ -202,14 +203,21 @@
             dti_filenames.append(None)
     if len( nm_filenames ) < 10:
         for k in range(len(nm_filenames),10):
             nm_filenames.append(None)
     # check modality names
     if not "T1w" in t1_filename:
         raise ValueError("T1w is not in t1 filename " + t1_filename)
+    if flair_filename is not None:
+        if isinstance(flair_filename,list):
+            if (len(flair_filename) == 0):
+                flair_filename=None
+            else:
+                print("Take first entry from flair_filename list")
+                flair_filename=flair_filename[0]
     if flair_filename is not None and not "lair" in flair_filename:
             raise ValueError("flair is not flair filename " + flair_filename)
     for k in nm_filenames:
         if k is not None:
             if not "NM" in k:
                 raise ValueError("NM is not flair filename " + k)
     for k in dti_filenames:
@@ -224,25 +232,27 @@
     for k in allfns:
         if k is not None:
             if not isinstance(k, str):
                 raise ValueError(str(k) + " is not a string")
             if not exists( k ):
                 raise ValueError( "image " + k + " does not exist")
     coredata = [
+        projectID,
         subjectID,
         date,
         imageUniqueID,
         modality,
         source_image_directory,
         output_image_directory,
         t1_filename,
         flair_filename]
     mydata0 = coredata +  rsf_filenames + dti_filenames
     mydata = mydata0 + nm_filenames
     corecols = [
+        'projectID',
         'subjectID',
         'date',
         'imageID',
         'modality',
         'sourcedir',
         'outputdir',
         'filename',
@@ -715,19 +725,27 @@
     metasubq = highest_quality_repeat(metasub, 'fn', 'date', 'negol')
 
     if verbose:
         print(f"{wmod} {metasubq.shape[0]} post")
 
     return {'raw': metasub, 'filt': metasubq}
 
-def mm_read( x, modality='' ):
+def mm_read( x, standardize_intensity=False, modality='' ):
     """
     read an image from a filename - same as ants.image_read (for now)
+
+    standardize_intensity : boolean ; if True will set negative values to zero and normalize into the range of zero to one
+
+    modality : not used
     """
-    return ants.image_read( x, reorient=False )
+    img = ants.image_read( x, reorient=False )
+    if standardize_intensity:
+        img[img<0.0]=0.0
+        img=ants.iMath(img,'Normalize')
+    return img
 
 def mm_read_to_3d( x, slice=None, modality='' ):
     """
     read an image from a filename - and return as 3d or None if that is not possible
     """
     img = ants.image_read( x, reorient=False )
     if img.dimension < 3:
@@ -858,15 +876,15 @@
 
 
 def timeseries_reg(
     image,
     avg_b0,
     type_of_transform="Rigid",
     total_sigma=1.0,
-    fdOffset=10.0,
+    fdOffset=2.0,
     trim = 0,
     output_directory=None,
     verbose=False, **kwargs
 ):
     """
     Correct time-series data for motion - with deformation.
 
@@ -1111,21 +1129,22 @@
     image,
     avg_b0,
     avg_dwi,
     bvals=None,
     bvecs=None,
     b0_idx=None,
     type_of_transform="Rigid",
-    total_sigma=1.0,
-    fdOffset=10.0,
+    total_sigma=3.0,
+    fdOffset=2.0,
+    mask_csf=False,
     output_directory=None,
     verbose=False, **kwargs
 ):
     """
-    Correct time-series data for motion - with deformation.
+    Correct time-series data for motion - with optional deformation.
 
     Arguments
     ---------
         image: antsImage, usually ND where D=4.
 
         avg_b0: Fixed image b0 image
 
@@ -1139,14 +1158,16 @@
 
         type_of_transform : string
             A linear or non-linear registration type. Mutual information metric and rigid transformation by default.
             See ants registration for details.
 
         fdOffset: offset value to use in framewise displacement calculation
 
+        mask_csf: boolean
+
         output_directory : string
             output will be placed in this directory plus a numeric extension.
 
         verbose: boolean
 
         kwargs: keyword args
             extra arguments - these extra arguments will control the details of registration that is performed. see ants registration for more.
@@ -1250,15 +1271,15 @@
                     outprefix=ofnL+str(k).zfill(4)+"_",
                     **kwargs
                 )
             if type_of_transform == 'SyN':
                 myreg = ants.registration(
                     fixed, temp,
                     type_of_transform='SyNOnly',
-                    total_sigma=total_sigma,
+                    total_sigma=total_sigma, grad_step=0.1,
                     initial_transform=myrig['fwdtransforms'][0],
                     outprefix=ofnL+str(k).zfill(4)+"_",
                     **kwargs
                 )
             else:
                 myreg = myrig
             fdptsTxI = ants.apply_transforms_to_points(
@@ -1275,19 +1296,24 @@
             motion_parameters.append(myreg["fwdtransforms"])
         else:
             motion_parameters.append("NA")
 
     if verbose:
         print("begin global distortion correction")
     # initrig = tra_initializer(avg_b0, ab0, max_rotation=60, transform=['rigid'], verbose=verbose)
-    initrig = ants.registration( avg_b0, ab0,'BOLDRigid',outprefix=ofnG)
-    deftx = ants.registration( avg_dwi, adw, 'SyNOnly',
+    if mask_csf:
+        bcsf = ants.threshold_image( avg_b0,"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
+    else:
+        bcsf = avg_b0[0] * 0 + 1
+
+    initrig = ants.registration( avg_b0, ab0*bcsf,'BOLDRigid',outprefix=ofnG)
+    deftx = ants.registration( avg_dwi, adw*bcsf, 'SyNOnly',
         syn_metric='CC', syn_sampling=2,
         reg_iterations=[50,50,20],
-        multivariate_extras=[ [ "CC", avg_b0, ab0, 1, 2 ]],
+        multivariate_extras=[ [ "CC", avg_b0, ab0*bcsf, 1, 2 ]],
         initial_transform=initrig['fwdtransforms'][0],
         outprefix=ofnG
         )['fwdtransforms']
     if verbose:
         print("end global distortion correction")
 
     for k in range(nTimePoints):
@@ -1337,15 +1363,15 @@
 
 def mc_reg(
     image,
     fixed=None,
     type_of_transform="Rigid",
     mask=None,
     total_sigma=3.0,
-    fdOffset=10.0,
+    fdOffset=2.0,
     output_directory=None,
     verbose=False, **kwargs
 ):
     """
     Correct time-series data for motion - with deformation.
 
     Arguments
@@ -1840,15 +1866,16 @@
     import shutil
     shutil.rmtree(output_directory, ignore_errors=True )
     return ants.n4_bias_field_correction(bavg)
 
 
 def get_average_dwi_b0( x, fixed_b0=None, fixed_dwi=None, fast=False ):
     """
-    automatically generates the average b0 and dwi and outputs both
+    automatically generates the average b0 and dwi and outputs both;
+    maps dwi to b0 space at end.
 
     x : input image
 
     fixed_b0 : alernative reference space
 
     fixed_dwi : alernative reference space
 
@@ -1887,21 +1914,26 @@
                 xavg = xavg + b0
             else:
                 bavg = bavg + b0
     bavg = ants.iMath( bavg, 'Normalize' )
     xavg = ants.iMath( xavg, 'Normalize' )
     import shutil
     shutil.rmtree(output_directory, ignore_errors=True )
-    return ants.n4_bias_field_correction(bavg), ants.n4_bias_field_correction(xavg)
+    avgb0=ants.n4_bias_field_correction(bavg)
+    avgdwi=ants.n4_bias_field_correction(xavg)
+    avgdwi=ants.registration( avgb0, avgdwi, 'Rigid' )['warpedmovout']
+    return avgb0, avgdwi
 
 def dti_template(
     b_image_list=None,
     w_image_list=None,
     iterations=5,
     gradient_step=0.5,
+    mask_csf=False,
+    average_both=True,
     verbose=False
 ):
     """
     two channel version of build_template
 
     returns:
         avg_b0, avg_dwi
@@ -1914,38 +1946,49 @@
     comptx = tmp2.name
     weights = np.repeat(1.0 / len(b_image_list), len(b_image_list))
     weights = [x / sum(weights) for x in weights]
     w_initial_template = w_image_list[0]
     b_initial_template = b_image_list[0]
     b_initial_template = ants.iMath(b_initial_template,"Normalize")
     w_initial_template = ants.iMath(w_initial_template,"Normalize")
-    bavg = b_initial_template.clone()
-    wavg = w_initial_template.clone()
+    if mask_csf:
+        bcsf0 = ants.threshold_image( b_image_list[0],"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
+        bcsf1 = ants.threshold_image( b_image_list[1],"Otsu",2).threshold_image(1,1).morphology("open",1).iMath("GetLargestComponent")
+    else:
+        bcsf0 = b_image_list[0] * 0 + 1
+        bcsf1 = b_image_list[1] * 0 + 1
+    bavg = b_initial_template.clone() * bcsf0
+    wavg = w_initial_template.clone() * bcsf0
+    bcsf = [ bcsf0, bcsf1 ]
     for i in range(iterations):
         for k in range(len(w_image_list)):
+            fimg=wavg
+            mimg=w_image_list[k] * bcsf[k]
+            fimg2=bavg
+            mimg2=b_image_list[k] * bcsf[k]
             w1 = ants.registration(
-                wavg, w_image_list[k], type_of_transform='antsRegistrationSyNQuick[s]',
-                    multivariate_extras= [ [ "mattes", bavg, b_image_list[k], 1, 32 ]],
+                fimg, mimg, type_of_transform='antsRegistrationSyNQuick[s]',
+                    multivariate_extras= [ [ "mattes", fimg2, mimg2, 1, 32 ]],
                     outprefix=mydeftx,
                     verbose=0 )
             txname = ants.apply_transforms(wavg, wavg,
                 w1["fwdtransforms"], compose=comptx )
             if k == 0:
                 txavg = ants.image_read(txname) * weights[k]
                 wavgnew = ants.apply_transforms( wavg,
-                    w_image_list[k], txname ).iMath("Normalize")
+                    w_image_list[k] * bcsf[k], txname ).iMath("Normalize")
                 bavgnew = ants.apply_transforms( wavg,
-                    b_image_list[k], txname ).iMath("Normalize")
+                    b_image_list[k] * bcsf[k], txname ).iMath("Normalize")
             else:
                 txavg = txavg + ants.image_read(txname) * weights[k]
-                if i >= (iterations-2):
+                if i >= (iterations-2) and average_both:
                     wavgnew = wavgnew+ants.apply_transforms( wavg,
-                        w_image_list[k], txname ).iMath("Normalize")
+                        w_image_list[k] * bcsf[k], txname ).iMath("Normalize")
                     bavgnew = bavgnew+ants.apply_transforms( wavg,
-                        b_image_list[k], txname ).iMath("Normalize")
+                        b_image_list[k] * bcsf[k], txname ).iMath("Normalize")
         if verbose:
             print("iteration:",str(i),str(txavg.abs().mean()))
         wscl = (-1.0) * gradient_step
         txavg = txavg * wscl
         ants.image_write( txavg, wavgfn )
         wavg = ants.apply_transforms(wavg, wavgnew, wavgfn).iMath("Normalize")
         bavg = ants.apply_transforms(bavg, bavgnew, wavgfn).iMath("Normalize")
@@ -3775,15 +3818,15 @@
       'NM_q0pt95' : np.quantile( nm_avg_cropped.numpy(), 0.95 ),
       'NM_substantianigra_z_coordinate' : sn_z,
       'NM_evr' : nm_evr,
       'NM_count': len( list_nm_images )
        }
 
 def resting_state_fmri_networks( fmri, fmri_template, t1, t1segmentation,
-    f=[0.03,0.08],   spa = 1.5, spt = 0.5, nc = 6, type_of_transform='SyN',
+    f=[0.03,0.08], FD_threshold=0.5, spa = 1.5, spt = 0.5, nc = 6, type_of_transform='SyN',
     verbose=False ):
 
   """
   Compute resting state network correlation maps based on the J Power labels.
   This will output a map for each of the major network systems.
 
   Arguments
@@ -3825,15 +3868,15 @@
   bmask = antspynet.brain_extraction( fmri_template, 'bold' ).threshold_image(0.5,1).iMath("FillHoles")
   if verbose:
       print("Begin rsfmri motion correction")
   corrmo = timeseries_reg(
     fmri, fmri_template,
     type_of_transform=type_of_transform,
     total_sigma=0.0,
-    fdOffset=10.0,
+    fdOffset=2.0,
     trim = 8,
     output_directory=None,
     verbose=False,
     syn_metric='cc',
     syn_sampling=2,
     reg_iterations=[40,20,5] )
   if verbose:
@@ -3983,14 +4026,20 @@
   A_wide = pd.DataFrame( A_wide )
   A_wide.columns = newnames_wide
   outdict['corr'] = A
   outdict['corr_wide'] = A_wide
   outdict['brainmask'] = bmask
   outdict['alff'] = myfalff['alff']
   outdict['falff'] = myfalff['falff']
+  # add global mean and standard deviation for post-hoc z-scoring
+  outdict['alff_mean'] = (myfalff['alff'][myfalff['alff']!=0]).mean()
+  outdict['alff_sd'] = (myfalff['alff'][myfalff['alff']!=0]).std()
+  outdict['falff_mean'] = (myfalff['falff'][myfalff['falff']!=0]).mean()
+  outdict['falff_sd'] = (myfalff['falff'][myfalff['falff']!=0]).std()
+
   for k in range(1,270):
     anatname=( pts2bold['AAL'][k] )
     if isinstance(anatname, str):
         anatname = re.sub("_","",anatname)
     else:
         anatname='Unk'
     fname='falffPoint'+str(k)+anatname
@@ -4006,15 +4055,16 @@
   edgemask = ants.iMath( bmask, "ME",1) - trimmask
   outdict['motion_corrected'] = corrmo['motion_corrected']
   outdict['brain_mask'] = bmask
   outdict['nuisance'] = rsfNuisance
   outdict['tsnr'] = mytsnr
   outdict['ssnr'] = slice_snr( corrmo['motion_corrected'], csfAndWM, gmseg )
   outdict['dvars'] = dvars( corrmo['motion_corrected'], gmseg )
-  outdict['high_motion_count'] = (rsfNuisance['FD'] > 0.5 ).sum()
+  outdict['high_motion_count'] = (rsfNuisance['FD'] > FD_threshold ).sum()
+  outdict['high_motion_pct'] = (rsfNuisance['FD'] > FD_threshold ).sum() / rsfNuisance.shape[0]
   outdict['FD_max'] = rsfNuisance['FD'].max()
   outdict['FD_mean'] = rsfNuisance['FD'].mean()
   outdict['bold_evr'] =  antspyt1w.patch_eigenvalue_ratio( und, 512, [16,16,16], evdepth = 0.9, mask = bmask )
   return outdict
 
 
 
@@ -4085,14 +4135,16 @@
     nm_image_list=None,
     dw_image=[], bvals=[], bvecs=[],
     srmodel=None,
     do_tractography = False,
     do_kk = False,
     do_normalization = None,
     target_range = [0,1],
+    dti_motion_correct = 'Rigid',
+    dti_denoise = False,
     test_run = False,
     verbose = False ):
     """
     Multiple modality processing and normalization
 
     aggregates modality-specific processing under one roof.  see individual
     modality specific functions for details.
@@ -4125,14 +4177,20 @@
     do_normalization : template transformation if available
 
     target_range : 2-element tuple
         a tuple or array defining the (min, max) of the input image
         (e.g., [-127.5, 127.5] or [0,1]).  Output images will be scaled back to original
         intensity. This range should match the mapping used in the training
         of the network.
+    
+    dti_motion_correct : None Rigid or SyN
+
+    dti_denoise : boolean
+
+    test_run : boolean 
 
     verbose : boolean
 
     """
     from os.path import exists
     ex_path = os.path.expanduser( "~/.antspyt1w/" )
     ex_path_mm = os.path.expanduser( "~/.antspymm/" )
@@ -4278,22 +4336,22 @@
                 bvecs[0],
                 jhu_atlas=JHU_atlas,
                 jhu_labels=JHU_labels,
                 brain_mask = dwimask,
                 reference_B0 = btpB0,
                 reference_DWI = btpDW,
                 srmodel=srmodel,
-                motion_correct='SyN', # set to False if using input from qsiprep
-                denoise=True,
+                motion_correct=dti_motion_correct, # set to False if using input from qsiprep
+                denoise=dti_denoise,
                 verbose = verbose)
         else :  # use phase encoding acquisitions for distortion correction and T1 for brain extraction
             if verbose:
                 print("We have both DTI_LR and DTI_RL: " + str(len(dw_image)))
-            a1b,a1w=get_average_dwi_b0(dw_image[0])
-            a2b,a2w=get_average_dwi_b0(dw_image[1])
+            a1b,a1w=antspymm.get_average_dwi_b0(dw_image[0])
+            a2b,a2w=antspymm.get_average_dwi_b0(dw_image[1],fixed_b0=a1b,fixed_dwi=a1w)
             btpB0, btpDW = dti_template(
                 b_image_list=[a1b,a2b],
                 w_image_list=[a1w,a2w],
                 iterations=7, verbose=verbose )
             initrig = ants.registration( btpDW, hier['brain_n4_dnz'], 'BOLDRigid' )['fwdtransforms'][0]
             tempreg = ants.registration( btpDW, hier['brain_n4_dnz'], 'SyNOnly',
                 syn_metric='mattes', syn_sampling=32,
@@ -4530,17 +4588,22 @@
         alffkeys = [key for key, val in rsfpro.items() if search_key in key]
         for myalf in alffkeys:
             mm_wide[ myalf ]=rsfpro[myalf]
         mm_wide['rsf_tsnr_mean'] =  rsfpro['tsnr'].mean()
         mm_wide['rsf_dvars_mean'] =  rsfpro['dvars'].mean()
         mm_wide['rsf_ssnr_mean'] =  rsfpro['ssnr'].mean()
         mm_wide['rsf_high_motion_count'] =  rsfpro['high_motion_count']
+        # mm_wide['rsf_high_motion_pct'] = rsfpro['rsf_high_motion_pct'] # BUG : rsf_high_motion_pct does not exist
         mm_wide['rsf_evr'] =  rsfpro['bold_evr']
         mm_wide['rsf_FD_mean'] = rsfpro['FD_mean']
         mm_wide['rsf_FD_max'] = rsfpro['FD_max']
+        mm_wide['rsf_alff_mean'] = rsfpro['alff_mean']
+        mm_wide['rsf_alff_sd'] = rsfpro['alff_sd']
+        mm_wide['rsf_falff_mean'] = rsfpro['falff_mean']
+        mm_wide['rsf_falff_sd'] = rsfpro['falff_sd']
         ofn = output_prefix + separator + 'rsfcorr.csv'
         rsfpro['corr'].to_csv( ofn )
         # apply same principle to new correlation matrix, doesn't need to be incorporated with mm_wide
         ofn2 = output_prefix + separator + 'nodescorr.csv'
         rsfpro['fullCorrMat'].to_csv( ofn2 )
     if mm['DTI'] is not None:
         mydti = mm['DTI']
@@ -5077,14 +5140,17 @@
 
 def mm_csv(
     studycsv,   # pandas data frame
     mysep = '-', # or "_" for BIDS
     srmodel_T1 = False, # optional - will add a great deal of time
     srmodel_NM = False, # optional - will add a great deal of time
     srmodel_DTI = False, # optional - will add a great deal of time
+    dti_motion_correct = 'Rigid',
+    dti_denoise = False,
+    nrg_modality_list = None
 ):
     """
     too dangerous to document ... use with care.
 
     processes multiple modality MRI specifically:
 
     * T1w
@@ -5130,26 +5196,33 @@
 
     srmodel_T1 : False (default) - will add a great deal of time - or h5 filename, 2 chan
 
     srmodel_NM : False (default) - will add a great deal of time - or h5 filename, 1 chan
 
     srmodel_DTI : False (default) - will add a great deal of time - or h5 filename, 1 chan
 
+    dti_motion_correct : None, Rigid or SyN
+
+    dti_denoise : boolean
+
+    nrg_modality_list : optional; defaults to None; use to focus on a given modality
+
     Returns
     ---------
 
     writes output to disk and produces figures
 
     """
     visualize = True
     verbose = True
-    nrg_modality_list = get_valid_modalities()
+    if nrg_modality_list is None:
+        nrg_modality_list = get_valid_modalities()
     if studycsv.shape[0] < 1:
         raise ValueError('studycsv has no rows')
-    musthavecols = ['subjectID','date','imageID','modality','sourcedir','outputdir','filename']
+    musthavecols = ['projectID', 'subjectID','date','imageID','modality','sourcedir','outputdir','filename']
     for k in range(len(musthavecols)):
         if not musthavecols[k] in studycsv.keys():
             raise ValueError('studycsv is missing column ' +musthavecols[k] )
     def makewideout( x, separator = mysep ):
         return x + separator + 'mmwide.csv'
     testloop = False
     counter=0
@@ -5163,25 +5236,27 @@
         antspyt1w.get_data( force_download=True )
         get_data( force_download=True )
     template = mm_read( templatefn ) # Read in template
     test_run = False
     if test_run:
         visualize=False
     # get sid and dtid from studycsv
-    # musthavecols = ['subjectID','date','imageID','modality','sourcedir','outputdir','filename']
+    # musthavecols = ['projectID','subjectID','date','imageID','modality','sourcedir','outputdir','filename']
+    projid = str(studycsv['projectID'].iloc[0])
     sid = str(studycsv['subjectID'].iloc[0])
     dtid = str(studycsv['date'].iloc[0])
     iid = str(studycsv['imageID'].iloc[0])
+    t1iidUse=iid
     modality = str(studycsv['modality'].iloc[0])
     sourcedir = str(studycsv['sourcedir'].iloc[0])
     outputdir = str(studycsv['outputdir'].iloc[0])
     filename = str(studycsv['filename'].iloc[0])
     if not exists(filename):
             raise ValueError('mm_nrg cannot find filename ' + filename + ' in mm_csv' )
-    def docsamson( locmod, verbose=True ):
+    def docsamson( locmod, t1iid=None, verbose=True ):
         myimgsInput = []
         myoutputPrefix = None
         imfns = [ 'filename', 'rsfid1', 'rsfid2', 'dtid1', 'dtid2', 'flairid' ]
         if locmod == 'T1w':
             imfns=['filename']
         elif locmod == 'T2Flair':
             imfns=['flairid']
@@ -5207,15 +5282,18 @@
                 if exists( fni ):
                     myimgsInput.append( fni )
                     temp = os.path.basename( fni )
                     mysplit = temp.split( mysep )
                     iid = re.sub( ".nii.gz", "", mysplit[len(mysplit)-1] )
                     iid = re.sub( ".mha", "", iid )
                     iid = re.sub( ".nii", "", iid )
-                    myoutputPrefix = outputdir + "/" + sid + "/" + dtid + "/" + locmod + '/' + iid + "/" + sid + mysep + dtid + mysep + locmod + mysep + iid
+                    iid2 = iid
+                    if locmod != 'T1w' and t1iid is not None:
+                        iid2=iid+"_"+t1iid
+                    myoutputPrefix = outputdir + "/" + projid + "/" + sid + "/" + dtid + "/" + locmod + '/' + iid + "/" + projid + mysep + sid + mysep + dtid + mysep + locmod + mysep + iid2
         if verbose:
             print("VERBOSE in docsamson")
             print( locmod )
             print( myimgsInput )
             print( myoutputPrefix )
         return {
             'modality': locmod,
@@ -5225,16 +5303,16 @@
     # hierarchical
     # NOTE: if there are multiple T1s for this time point, should take
     # the one with the highest resnetGrade
     t1fn = filename
     if not exists( t1fn ):
         raise ValueError('mm_nrg cannot find the T1w with uid ' + t1fn )
     t1 = mm_read( t1fn )
-    hierfn = outputdir + "/" + sid + "/" + dtid + "/" + "T1wHierarchical" + '/' + iid + "/" + sid + mysep + dtid + mysep + "T1wHierarchical" + iid + mysep
-    hierfnSR = outputdir + "/" + sid + "/" + dtid + "/" + "T1wHierarchicalSR" + '/' + iid + "/" + sid + mysep + dtid + mysep + "T1wHierarchicalSR" + iid + mysep
+    hierfn = outputdir + "/"  + projid + "/" + sid + "/" + dtid + "/" + "T1wHierarchical" + '/' + iid + "/" + projid + mysep + sid + mysep + dtid + mysep + "T1wHierarchical" + mysep + iid + mysep
+    hierfnSR = outputdir + "/" + projid + "/"  + sid + "/" + dtid + "/" + "T1wHierarchicalSR" + '/' + iid + "/" + projid + mysep + sid + mysep + dtid + mysep + "T1wHierarchicalSR" + mysep + iid + mysep
     hierfntest = hierfn + 'snseg.csv'
     if verbose:
         print( hierfntest )
     regout = hierfn + "syn"
     templateTx = {
         'fwdtransforms': [ regout+'1Warp.nii.gz', regout+'0GenericAffine.mat'],
         'invtransforms': [ regout+'0GenericAffine.mat', regout+'1InverseWarp.nii.gz']  }
@@ -5301,15 +5379,15 @@
         t1imgbrn = hier['brain_n4_dnz']
         t1atropos = hier['dkt_parc']['tissue_segmentation']
     # loop over modalities and then unique image IDs
     # we treat NM in a "special" way -- aggregating repeats
     # other modalities (beyond T1) are treated individually
     for overmodX in nrg_modality_list:
         # define 1. input images 2. output prefix
-        mydoc = docsamson( overmodX )
+        mydoc = docsamson( overmodX, t1iid=t1iidUse )
         myimgsr = mydoc['images']
         mymm = mydoc['outprefix']
         mymod = mydoc['modality']
         if verbose:
             print( mydoc )
         if len(myimgsr) > 0:
             dowrite=False
@@ -5517,14 +5595,16 @@
                                     dw_image=imgList,
                                     bvals = bvalfnList,
                                     bvecs = bvecfnList,
                                     srmodel=srmodel_DTI_mdl,
                                     do_tractography=not test_run,
                                     do_kk=False,
                                     do_normalization=templateTx,
+                                    dti_motion_correct = dti_motion_correct,
+                                    dti_denoise = dti_denoise,
                                     test_run=test_run,
                                     verbose=True )
                                 mydti = tabPro['DTI']
                                 if visualize:
                                     maxslice = np.min( [21, mydti['recon_fa'] ] )
                                     ants.plot( mydti['recon_fa'],  axis=2, nslices=maxslice, ncol=7, crop=True, title='FA (supposed to be better)', filename=mymm+mysep+"FAbetter.png"  )
                                     ants.plot( mydti['recon_fa'], mydti['jhu_labels'], axis=2, nslices=maxslice, ncol=7, crop=True, title='FA + JHU', filename=mymm+mysep+"FAJHU.png"  )
@@ -5848,15 +5928,15 @@
     mytr = ants.get_spacing( x )[3]
     for n in range( xmat.shape[1] ):
         temp = alffmap( xmat[:,n], flo=flo, fhi=fhi, tr=mytr )
         alffvec[n]=temp['alff']
         falffvec[n]=temp['falff']
     alffi=ants.make_image( mask, alffvec )
     falffi=ants.make_image( mask, falffvec )
-    return {  'alff':alffi, 'falff': falffi }
+    return {  'alff': alffi, 'falff': falffi }
 
 
 def down2iso( x, interpolation='linear', takemin=False ):
     """
     will downsample an anisotropic image to an isotropic resolution
 
     x: input image
@@ -5932,35 +6012,35 @@
             xdf = pd.DataFrame(ddnum, columns=xdfcols )
     if xdf.shape[1] == 0:
         return None
     if colprefix is not None:
         xdf.columns=colprefix + xdf.columns
     return pd.concat( [df,xdf], axis=1 )
 
-def assemble_modality_specific_dataframes( mm_wide_csvs, hierdfin, nrg_modality, progress=None, verbose=False ):
+def assemble_modality_specific_dataframes( mm_wide_csvs, hierdfin, nrg_modality, separator='-', progress=None, verbose=False ):
     moddersub = re.sub( "[*]","",nrg_modality)
     nmdf=pd.DataFrame()
     for k in range( hierdfin.shape[0] ):
         if progress is not None:
             if k % progress == 0:
                 progger = str( np.round( k / hierdfin.shape[0] * 100 ) )
                 print( progger, end ="...", flush=True)
         temp = mm_wide_csvs[k]
         mypartsf = temp.split("T1wHierarchical")
         myparts = mypartsf[0]
         t1iid = str(mypartsf[1].split("/")[1])
         fnsnm = glob.glob(myparts+"/" + nrg_modality + "/*/*" + t1iid + "*wide.csv")
         if len( fnsnm ) > 0 :
             for y in fnsnm:
-                temp=read_mm_csv( y, colprefix=moddersub+'_', is_t1=False, verbose=verbose )
+                temp=read_mm_csv( y, colprefix=moddersub+'_', is_t1=False, separator=separator, verbose=verbose )
                 if temp is not None:
                     nmdf=pd.concat( [nmdf, temp], axis=0)
     return nmdf
 
-def bind_wide_mm_csvs( mm_wide_csvs, merge=True, verbose = 0 ) :
+def bind_wide_mm_csvs( mm_wide_csvs, merge=True, separator='-', verbose = 0 ) :
     """
     will convert a list of t1w hierarchical csv filenames to a merged dataframe
 
     returns a pair of data frames, the left side having all entries and the
         right side having row averaged entries i.e. unique values for each visit
 
     set merge to False to return individual dataframes ( for debugging )
@@ -5972,15 +6052,15 @@
         print("No files found with specified pattern")
         return
     # 1. row-bind the t1whier data
     # 2. same for each other modality
     # 3. merge the modalities by the keys
     hierdf = pd.DataFrame()
     for y in mm_wide_csvs:
-        temp=read_mm_csv( y, colprefix='T1Hier_', is_t1=True )
+        temp=read_mm_csv( y, colprefix='T1Hier_', separator=separator, is_t1=True )
         if temp is not None:
             hierdf=pd.concat( [hierdf, temp], axis=0)
     if verbose > 0:
         mypro=50
     else:
         mypro=None
     if verbose > 0:
@@ -6297,38 +6377,63 @@
                 joinDiagnostics = pd.concat( [joinDiagnostics, joinDiagnosticsLoc], axis=0)
 
     return jmmUniq, jmm, joinDiagnostics
 
 
 
 def quick_viz_mm_nrg(
-    sourcedir, # folder
+    sourcedir, # root folder
+    projectid, # project name
     sid , # subject unique id
     dtid, # date
-    sourcedatafoldername = 'images', # root for source data
     extract_brain=True,
     slice_factor = 0.55,
-    show_it = None,
+    show_it = None, # output path
     verbose = True
 ):
+    """
+    This function creates visualizations of brain images for a specific subject in a project using ANTsPy.
+
+    Args:
+
+    sourcedir (str): Root folder.
+    
+    projectid (str): Project name.
+    
+    sid (str): Subject unique id.
+    
+    dtid (str): Date.
+    
+    extract_brain (bool): If True, the function extracts the brain from the T1w image. Default is True.
+    
+    slice_factor (float): The slice to be visualized is determined by multiplying the image size by this factor. Default is 0.55.
+    
+    show_it (str): Output path. If not None, the visualizations will be saved at this location. Default is None.
+    
+    verbose (bool): If True, information will be printed while running the function. Default is True.
+
+    Returns:
+    vizlist (list): List of image visualizations.
+
+    """
     iid='*'
     import glob as glob
     from os.path import exists
     import ants
     ex_path = os.path.expanduser( "~/.antspyt1w/" )
     ex_pathmm = os.path.expanduser( "~/.antspymm/" )
     templatefn = ex_path + 'CIT168_T1w_700um_pad_adni.nii.gz'
     if not exists( templatefn ):
         print( "**missing files** => call get_data from latest antspyt1w and antspymm." )
         antspyt1w.get_data( force_download=True )
         get_data( force_download=True )
     temp = sourcedir.split( "/" )
     splitCount = len( temp )
     template = mm_read( templatefn ) # Read in template
-    subjectrootpath = os.path.join(sourcedir,sid, dtid)
+    subjectrootpath = os.path.join(sourcedir, projectid, sid, dtid)
     myimgsInput = glob.glob( subjectrootpath+"/*" )
     myimgsInput.sort( )
     if verbose:
         print( myimgsInput )
     t1_search_path = os.path.join(subjectrootpath, "T1w", "*", "*nii.gz")
     if verbose:
         print(f"t1 search path: {t1_search_path}")
@@ -6820,21 +6925,21 @@
 def novelty_detection_ee(df_train, df_test, contamination=0.05):
     """
     This function performs novelty detection using Elliptic Envelope.
 
     Parameters:
 
     - df_train (pandas dataframe): training data used to fit the model
-    
+
     - df_test (pandas dataframe): test data used to predict novelties
-    
+
     - contamination (float): parameter controlling the proportion of outliers in the data (default: 0.05)
 
     Returns:
-    
+
     predictions (pandas series): predicted labels for the test data (1 for novelties, 0 for inliers)
     """
     import pandas as pd
     from sklearn.covariance import EllipticEnvelope
     # Fit the model on the training data
     clf = EllipticEnvelope(contamination=contamination,support_fraction=1)
     df_train[ df_train == math.inf ] = 0
@@ -6864,15 +6969,15 @@
     - df_test (pandas dataframe): test data used to predict novelties
 
     - nu (float): parameter controlling the fraction of training errors and the fraction of support vectors (default: 0.05)
 
     - kernel (str): kernel type used in the SVM algorithm (default: 'rbf')
 
     Returns:
-    
+
     predictions (pandas series): predicted labels for the test data (1 for novelties, 0 for inliers)
     """
     from sklearn.svm import OneClassSVM
     # Fit the model on the training data
     df_train[ df_train == math.inf ] = 0
     df_test[ df_test == math.inf ] = 0
     clf = OneClassSVM(nu=nu, kernel=kernel)
@@ -6891,17 +6996,17 @@
 
 
 def novelty_detection_lof(df_train, df_test, n_neighbors=20):
     """
     This function performs novelty detection using Local Outlier Factor (LOF).
 
     Parameters:
-    
+
     - df_train (pandas dataframe): training data used to fit the model
-    
+
     - df_test (pandas dataframe): test data used to predict novelties
 
     - n_neighbors (int): number of neighbors used to compute the LOF (default: 20)
 
     Returns:
 
     - predictions (pandas series): predicted labels for the test data (1 for novelties, 0 for inliers)
@@ -6926,27 +7031,27 @@
 
 
 def novelty_detection_loop(df_train, df_test, n_neighbors=20, distance_metric='minkowski'):
     """
     This function performs novelty detection using Local Outlier Factor (LOF).
 
     Parameters:
-    
+
     - df_train (pandas dataframe): training data used to fit the model
-    
+
     - df_test (pandas dataframe): test data used to predict novelties
 
     - n_neighbors (int): number of neighbors used to compute the LOOP (default: 20)
 
     - distance_metric : default minkowski
 
     Returns:
 
     - predictions (pandas series): predicted labels for the test data (1 for novelties, 0 for inliers)
-    
+
     """
     from PyNomaly import loop
     from sklearn.neighbors import NearestNeighbors
     from sklearn.preprocessing import StandardScaler
     scaler = StandardScaler()
     scaler.fit(df_train)
     data = np.vstack( [scaler.transform(df_test),scaler.transform(df_train)])
@@ -6959,24 +7064,24 @@
 
 
 def novelty_detection_quantile(df_train, df_test):
     """
     This function performs novelty detection using quantiles for each column.
 
     Parameters:
-    
+
     - df_train (pandas dataframe): training data used to fit the model
-    
+
     - df_test (pandas dataframe): test data used to predict novelties
 
     Returns:
 
-    - quantiles for the test sample at each column where values range in [0,1] 
+    - quantiles for the test sample at each column where values range in [0,1]
         and higher values mean the column is closer to the edge of the distribution
-    
+
     """
     myqs = df_test.copy()
     n = df_train.shape[0]
     df_trainkeys = df_train.keys()
     for k in range( df_train.shape[1] ):
         mykey = df_trainkeys[k]
         temp = (myqs[mykey][0] >  df_train[mykey]).sum() / n
```

### Comparing `antspymm-0.8.8/antspymm.egg-info/PKG-INFO` & `antspymm-0.9.0/antspymm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antspymm
-Version: 0.8.8
+Version: 0.9.0
 Summary: multi-channel/time-series medical image processing with antspyx
 Home-page: https://github.com/stnava/ANTsPyMM
 Author: Avants, Gosselin, Tustison, Reardon
 Author-email: stnava@gmail.com
 License: Apache 2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE
@@ -15,21 +15,25 @@
 
 the outputs of these processes can be used for data inspection/cleaning/triage
 as well for interrogating hypotheses.
 
 this package also keeps track of the latest preferred algorithm variations for
 production environments.
 
-install by calling (within the source directory):
+install the `dev` version by calling (within the source directory):
 
 ```
 python setup.py install
 ```
 
-or install via `pip install antspymm` **FIXME**
+or install the latest release via 
+
+```
+pip install antspymm
+```
 
 # what this will do
 
 ANTsPyMM will process several types of brain MRI into tabular form as well as normalized (standard template) space.  The processing includes:
 
 * T1wHier uses hierarchical processing from ANTsPyT1w organized around these measurements
 
@@ -75,21 +79,25 @@
 will all modalities will take around 2 hours on an average laptop.
 
 documentation of functions [here](http://htmlpreview.github.io/?https://github.com/stnava/ANTsPyMM/blob/main/docs/antspymm/mm.html).
 
 # first time setup
 
 ```python
+import antspyt1w
 import antspymm
-antspymm.get_data()
+antspyt1w.get_data(force_download=True)
+antspymm.get_data(force_download=True)
 ```
 
 NOTE: `get_data` has a `force_download` option to make sure the latest
 package data is installed.
 
+NOTE: some functions in `antspynet` will download deep network model weights on the fly.  if one is containerizing, then it would be worth running a test case through in the container to make sure all the relevant weights are pre-downloaded.
+
 # example processing
 
 see the latest help but this snippet gives an idea of how one might use the package:
 
 ```python
 import os
 os.environ["TF_NUM_INTEROP_THREADS"] = "8"
@@ -119,19 +127,22 @@
 
 antspymm.write_mm( '/tmp/test_output', t1wide, tabPro, normPro )
 
 ```
 
 ## blind quality control
 
-automatically qc, filter and match multiple modality images at each time point.
+this package also provides tools to identify the *best* multi-modality image set at a given visit.
+
+the code below provides guidance on how to automatically qc, filter and match multiple modality images at each time point.  these tools are based on standard unsupervised approaches and are not perfect so we recommend using the associated plotting/visualization techniques to check the quality characterizations for each modality.
 
 ```python
 ## run the qc on all images - requires a relatively large sample per modality to be effective
 ## then aggregate
+qcdf=pd.DataFrame()
 for fn in fns:
   qcdf=pd.concat( [qcdf,antspymm.blind_image_assessment(fn)], axis=0)
 qcdfa=antspymm.average_blind_qc_by_modality(qcdf,verbose=True) ## reduce the time series qc
 qcdfaol=antspymm.outlierness_by_modality(qcdfa) # estimate outlier scores
 print( qcdfaol.shape )
 print( qcdfaol.keys )
 matched_mm_data=antspymm.match_modalities( qcdfaol  )
@@ -152,15 +163,14 @@
     alldf = pd.concat( [alldf, jjj ], axis=0 )
     jjj.to_csv( "mm_outlierness_"+m+".csv")
     print(m+" done")
 # write the joined data out
 alldf.to_csv( "mm_outlierness.csv", index=False )
 # find the best mm collection
 matched_mm_data=antspymm.match_modalities( alldf, verbose=True )
-matched_mm_data
 matched_mm_data.to_csv( "matched_mm_data.csv", index=False )
 matched_mm_data['negative_outlier_factor'] = 1.0 - matched_mm_data['ol_loop'].astype("float")
 matched_mm_data2 = antspymm.highest_quality_repeat( matched_mm_data, 'subjectID', 'date', qualityvar='negative_outlier_factor')
 matched_mm_data2.to_csv( "matched_mm_data2.csv", index=False )
 ```
 
 ## an example on open neuro (BIDS) data
@@ -190,23 +200,24 @@
 import antspymm
 import pandas as pd
 import glob as glob
 fns = glob.glob("imagesBIDS/ANTPD/sub-RC4125/ses-*/*/*gz")
 fns.sort()
 randid='000' # BIDS does not have unique image ids - so we assign one
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     randid,
     'T1w',
     '/Users/stnava/data/openneuro/imagesBIDS/',
     '/Users/stnava/data/openneuro/processed/',
     t1_filename=fns[0],
-    dti_filenames=[fns[2]],
-    rsf_filenames=[fns[1]])
+    dti_filenames=[fns[1]],
+    rsf_filenames=[fns[2]])
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
 ## NRG example
 
 NRG format details [here](https://htmlpreview.github.io/?https://github.com/stnava/biomedicalDataOrganization/blob/master/src/nrg_data_organization_summary.html)
@@ -233,38 +244,91 @@
 
 
 ```python
 import antspymm
 import pandas as pd
 import glob as glob
 t1fn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*T1w*gz")[0]
+# flair also takes a single image
 dtfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*DTI*gz")
 rsfn=glob.glob("imagesNRG/ANTPD/sub-RC4125/ses-*/*/*/*rsfMRI*gz")
 studycsv = antspymm.generate_mm_dataframe(
+    'ANTPD',
     'sub-RC4125',
     'ses-1',
     '000',
     'T1w',
     '/Users/stnava/data/openneuro/imagesNRG/',
     '/Users/stnava/data/openneuro/processed/',
     t1fn,
     rsf_filenames=rsfn,
     dti_filenames=dtfn
 )
 studycsv2 = studycsv.dropna(axis=1)
 mmrun = antspymm.mm_csv( studycsv2, mysep='_' )
 ```
 
+## useful tools for converting dicom to nifti
+
+* [dcm2niix](https://github.com/rordenlab/dcm2niix)
+
+* [dicom2nifti](https://dicom2nifti.readthedocs.io/en/latest/)
+
+```python
+import dicom2nifti
+
+dicom2nifti.convert_directory(dicom_directory, output_folder, compression=True, reorient=True)
+```
+
+* [simpleitk](https://pypi.org/project/SimpleITK/)
+
+```python
+import SimpleITK as sitk
+import sys
+import os
+import glob as glob
+import ants
+dd='dicom'
+oo='dicom2nifti'
+folders=glob.glob('dicom/*')
+k=0
+for f in folders:
+    print(f)    
+    reader = sitk.ImageSeriesReader()
+    ff=glob.glob(f+"/*")
+    dicom_names = reader.GetGDCMSeriesFileNames(ff[0])
+    if len(ff) > 0:
+        fnout='dicom2nifti/image_'+str(k).zfill(4)+'.nii.gz'
+        if not exists(fnout):
+            failed=False
+            reader.SetFileNames(dicom_names)
+            try:
+                image = reader.Execute()
+            except:
+                failed=True
+                pass
+            if not failed:
+                size = image.GetSpacing()
+                print( image.GetMetaDataKeys( ) )
+                print( size )
+                sitk.WriteImage(image, fnout )
+                img=ants.image_read( fnout )
+                img=ants.iMath(img,'TruncateIntensity',0.02,0.98)
+                ants.plot( img, nslices=21,ncol=7,axis=2, crop=True )
+        else:
+            print(f+ ": "+'empty')
+    k=k+1
+```
+
 ## build docs
 
 ```
 pdoc -o ./docs antspymm --html
 ```
 
 ## to publish a release
 
 ```
 rm -r -f build/ antspymm.egg-info/ dist/
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload -u username -p password  dist/*
 ```
-
```

### Comparing `antspymm-0.8.8/antspymm.egg-info/SOURCES.txt` & `antspymm-0.9.0/antspymm.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,21 @@
 antspymm.egg-info/PKG-INFO
 antspymm.egg-info/SOURCES.txt
 antspymm.egg-info/dependency_links.txt
 antspymm.egg-info/not-zip-safe
 antspymm.egg-info/requires.txt
 antspymm.egg-info/top_level.txt
 docs/antspymm_data_dictionary.csv
+docs/bids_cohort_example.py
+docs/example_run_from_directory.py
 docs/make_dict_table.Rmd
+docs/nrg_cohort_example.py
 docs/outlierness.py
+docs/ukbb_to_nrg_processing.py
+docs/ukbb_to_nrg_processing2.py
 tests/mm.py
 tests/mm_nrg.py
 tests/test_bids_2_nrg.py
 tests/test_dti_recon.py
 tests/test_dwi_run.py
 tests/test_flair_run.py
 tests/test_joint_dti_recon.py
```

### Comparing `antspymm-0.8.8/docs/antspymm_data_dictionary.csv` & `antspymm-0.9.0/docs/antspymm_data_dictionary.csv`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/docs/outlierness.py` & `antspymm-0.9.0/docs/outlierness.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/setup.py` & `antspymm-0.9.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = open("README.md").read()
 
 with open("./requirements.txt") as f:
       requirements = f.read().splitlines()
 
 setup(name='antspymm',
-      version='0.8.8',
+      version='0.9.0',
       description='multi-channel/time-series medical image processing with antspyx',
       long_description=long_description,
       long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
       url='https://github.com/stnava/ANTsPyMM',
       author='Avants, Gosselin, Tustison, Reardon',
       author_email='stnava@gmail.com',
       license='Apache 2.0',
```

### Comparing `antspymm-0.8.8/tests/mm.py` & `antspymm-0.9.0/tests/mm.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/mm_nrg.py` & `antspymm-0.9.0/tests/mm_nrg.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/test_dwi_run.py` & `antspymm-0.9.0/tests/test_dwi_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/test_joint_dti_recon.py` & `antspymm-0.9.0/tests/test_joint_dti_recon.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/test_mm_csv.py` & `antspymm-0.9.0/tests/test_mm_csv.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/test_rsfmri_run.py` & `antspymm-0.9.0/tests/test_rsfmri_run.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/testsr.py` & `antspymm-0.9.0/tests/testsr.py`

 * *Files identical despite different names*

### Comparing `antspymm-0.8.8/tests/visualize_tractogram.py` & `antspymm-0.9.0/tests/visualize_tractogram.py`

 * *Files identical despite different names*

