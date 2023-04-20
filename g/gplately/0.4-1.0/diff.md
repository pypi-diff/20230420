# Comparing `tmp/gplately-0.4.tar.gz` & `tmp/gplately-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplately-0.4.tar", last modified: Tue Apr 11 11:35:46 2023, max compression
+gzip compressed data, was "gplately-1.0.tar", last modified: Thu Apr 20 02:58:06 2023, max compression
```

## Comparing `gplately-0.4.tar` & `gplately-1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.211823 gplately-0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-11 11:34:21.000000 gplately-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    15922 2023-04-11 11:35:46.211823 gplately-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13290 2023-04-11 11:34:22.000000 gplately-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.207822 gplately-0.4/gplately/
--rw-r--r--   0 runner    (1001) docker     (122)     6279 2023-04-11 11:34:22.000000 gplately-0.4/gplately/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15195 2023-04-11 11:34:22.000000 gplately-0.4/gplately/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    80675 2023-04-11 11:34:22.000000 gplately-0.4/gplately/download.py
--rw-r--r--   0 runner    (1001) docker     (122)    20072 2023-04-11 11:34:22.000000 gplately-0.4/gplately/geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-04-11 11:34:22.000000 gplately-0.4/gplately/gpml.py
--rw-r--r--   0 runner    (1001) docker     (122)    75773 2023-04-11 11:34:22.000000 gplately-0.4/gplately/grids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-04-11 11:34:22.000000 gplately-0.4/gplately/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    68818 2023-04-11 11:34:22.000000 gplately-0.4/gplately/oceans.py
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-11 11:34:22.000000 gplately-0.4/gplately/parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)   126380 2023-04-11 11:34:22.000000 gplately-0.4/gplately/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-04-11 11:34:22.000000 gplately-0.4/gplately/pygplates.py
--rw-r--r--   0 runner    (1001) docker     (122)   105151 2023-04-11 11:34:22.000000 gplately-0.4/gplately/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (122)    24596 2023-04-11 11:34:22.000000 gplately-0.4/gplately/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.207822 gplately-0.4/gplately.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15922 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-11 11:35:46.000000 gplately-0.4/gplately.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 11:35:46.211823 gplately-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-04-11 11:34:22.000000 gplately-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.211823 gplately-0.4/test/
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-11 11:34:22.000000 gplately-0.4/test/test_0_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-04-11 11:34:22.000000 gplately-0.4/test/test_1_reconstructions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-11 11:34:22.000000 gplately-0.4/test/test_2_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     6359 2023-04-11 11:34:22.000000 gplately-0.4/test/test_3_plottopologies.py
--rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-04-11 11:34:22.000000 gplately-0.4/test/test_4_rasters.py
--rw-r--r--   0 runner    (1001) docker     (122)     6011 2023-04-11 11:34:22.000000 gplately-0.4/test/test_5_seafloorgrid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-04-11 11:34:22.000000 gplately-0.4/test/test_6_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 02:58:06.703575 gplately-1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-20 02:55:40.000000 gplately-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    16028 2023-04-20 02:58:06.703575 gplately-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13388 2023-04-20 02:55:41.000000 gplately-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 02:58:06.703575 gplately-1.0/gplately/
+-rw-r--r--   0 runner    (1001) docker     (122)    12163 2023-04-20 02:55:41.000000 gplately-1.0/gplately/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16690 2023-04-20 02:55:41.000000 gplately-1.0/gplately/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    89693 2023-04-20 02:55:41.000000 gplately-1.0/gplately/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20072 2023-04-20 02:55:41.000000 gplately-1.0/gplately/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-04-20 02:55:41.000000 gplately-1.0/gplately/gpml.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75773 2023-04-20 02:55:41.000000 gplately-1.0/gplately/grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-04-20 02:55:41.000000 gplately-1.0/gplately/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68818 2023-04-20 02:55:41.000000 gplately-1.0/gplately/oceans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-20 02:55:41.000000 gplately-1.0/gplately/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)   133059 2023-04-20 02:55:41.000000 gplately-1.0/gplately/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31456 2023-04-20 02:55:41.000000 gplately-1.0/gplately/pygplates.py
+-rw-r--r--   0 runner    (1001) docker     (122)   112928 2023-04-20 02:55:41.000000 gplately-1.0/gplately/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24599 2023-04-20 02:55:41.000000 gplately-1.0/gplately/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 02:58:06.703575 gplately-1.0/gplately.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16028 2023-04-20 02:58:06.000000 gplately-1.0/gplately.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-20 02:58:06.000000 gplately-1.0/gplately.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-20 02:58:06.000000 gplately-1.0/gplately.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-20 02:58:06.000000 gplately-1.0/gplately.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-20 02:58:06.000000 gplately-1.0/gplately.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-20 02:58:06.703575 gplately-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-04-20 02:55:41.000000 gplately-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-20 02:58:06.703575 gplately-1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-20 02:55:41.000000 gplately-1.0/test/test_0_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5927 2023-04-20 02:55:41.000000 gplately-1.0/test/test_1_reconstructions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1891 2023-04-20 02:55:41.000000 gplately-1.0/test/test_2_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6359 2023-04-20 02:55:41.000000 gplately-1.0/test/test_3_plottopologies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3553 2023-04-20 02:55:41.000000 gplately-1.0/test/test_4_rasters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6011 2023-04-20 02:55:41.000000 gplately-1.0/test/test_5_seafloorgrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-04-20 02:55:41.000000 gplately-1.0/test/test_6_geometry.py
```

### Comparing `gplately-0.4/LICENSE` & `gplately-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gplately-0.4/PKG-INFO` & `gplately-1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gplately
-Version: 0.4
+Version: 1.0
 Summary: Object-orientated Python interface to pyGPlates for plate tectonic reconstructions
 Home-page: https://github.com/GPlates/gplately
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 License: UNKNOWN
 Description: <p align="center">
         <picture>
@@ -12,14 +12,15 @@
           <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
           <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
         </picture>
         </p>
         
         ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
         ![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+        ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gplately?style=for-the-badge)
         ![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
         
         
         GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
         
         ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
```

### Comparing `gplately-0.4/README.md` & `gplately-1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
   <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
 </picture>
 </p>
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
 ![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gplately?style=for-the-badge)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
 
 
 GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
 
 ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
```

### Comparing `gplately-0.4/gplately/data.py` & `gplately-1.0/gplately/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,14 +145,18 @@
             "Pehrsson2015" : ["https://www.geolsoc.org.uk/~/media/Files/GSL/shared/Sup_pubs/2015/18822_7.zip"],
             "TorsvikCocks2017" : ["http://www.earthdynamics.org/earthhistory/bookdata/CEED6.zip"],
             "Young2019" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Young_etal_2018_GeoscienceFrontiers/Young_etal_2018_GeoscienceFrontiers_GPlatesPlateMotionModel.zip"], 
             "Scotese2008" : ["https://static.cambridge.org/content/id/urn:cambridge.org:id:article:S0016756818000110/resource/name/S0016756818000110sup001.zip"],      
             "Golonka2007" : ["https://static.cambridge.org/content/id/urn:cambridge.org:id:article:S0016756818000110/resource/name/S0016756818000110sup001.zip"],
             "Clennett2020_M2019" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Clennett_etal_2020_G3/Clennett_etal_2020_M2019.zip"],
             "Clennett2020_S2013" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Clennett_etal_2020_G3/Clennett_etal_2020_S2013.zip"],
+            "Muller2008" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Muller2008/Global_Model_Rigid_Internal_Release_2010.zip"],
+            "Scotese2016" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Scotese2016/PALEOMAP_GlobalPlateModel.zip"],
+            "Shephard2013" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Shephard2013/GPlates.zip"],
+            "Muller2022" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Muller2022/Muller_etal_2022_SE_1Ga_Opt.zip"],
 
         }
 
         return database
 
 
     def plate_model_valid_reconstruction_times(self):
@@ -171,14 +175,18 @@
             # "Pehrsson2015" : [25], (First implement continuous rotation)
             "TorsvikCocks2017" : [0, 410],
             "Young2019" : [0, 410], 
             "Scotese2008" : [0, 410],      
             "Golonka2007" : [0, 410],
             "Clennett2020_M2019" : [0, 170],
             "Clennett2020_S2013" : [0, 170],
+            "Scotese2016" : [0,410],
+            "Shephard2013" : [0,200],
+            "Muller2008" : [0,141], #GPlates static polygons reconstruct to this time
+            "Muller2022" : [0,1000],
 
         }  
         return database
 
 
     def rotation_strings_to_ignore(self):
 
@@ -220,14 +228,15 @@
             "Kula",
             "North_America",
             "South_America",
             "Western_Jurassic",
             "Clennett_2020_Isochrons",
             "Clennett_2020_Coastlines",
             "Clennett_2020_NAm_boundaries",
+            "Shephard_etal_ESR2013_Global_EarthByte_2013", # For Shephard et al. 2013
 
         ]
         return strings 
 
 
     def dynamic_polygon_strings_to_ignore(self):
 
@@ -237,14 +246,15 @@
             "DO_NOT",
             "9_Point", # Muller et al 2019
             "9_Point_Density", # Clennett et al 2020
             "Density", # Clennett et al 2020
             "Inactive_Meshes_and_Topologies", # Clennett et al 2020
             "ContinentOceanBoundaries", # Seton 2012
             "Seton_etal_ESR2012_Coastline_2012", # Seton 2012
+            "PALEOMAP_PoliticalBoundaries", # Scotese 2016
         ]
         return strings
 
 
     def static_polygon_strings_to_include(self):
 
         strings = [
@@ -255,14 +265,15 @@
             "RodiniaBlocks_WithPlateIDColumnAndIDs",
             # "PlatePolygons.shp",
             "CEED6_TERRANES.shp",
             "CEED6_MICROCONTINENTS.shp",
             "CEED6_LAND.gpml",
             "Scotese_2008_PresentDay_ContinentalPolygons", # Scotese 2008
             "Golonka_2007_PresentDay_ContinentalPolygons.shp", # Golonka 2007
+            "PALEOMAP_PlatePolygons.gpml", # For Scotese 2016
         ]
         return strings
 
 
     def static_polygon_strings_to_ignore(self):
 
         strings = [
@@ -293,25 +304,30 @@
             "Pehrsson2015" : ["https://www.geolsoc.org.uk/~/media/Files/GSL/shared/Sup_pubs/2015/18822_7.zip"],
             "TorsvikCocks2017" : ["http://www.earthdynamics.org/earthhistory/bookdata/CEED6.zip"],
             "Young2019" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Young_etal_2018_GeoscienceFrontiers/Young_etal_2018_GeoscienceFrontiers_GPlatesPlateMotionModel.zip"],
             "Scotese2008" : ["https://static.cambridge.org/content/id/urn:cambridge.org:id:article:S0016756818000110/resource/name/S0016756818000110sup001.zip"],
             "Golonka2007" : ["https://static.cambridge.org/content/id/urn:cambridge.org:id:article:S0016756818000110/resource/name/S0016756818000110sup001.zip"],
             "Clennett2020_M2019" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Clennett_etal_2020_G3/Clennett_etal_2020_M2019.zip"],
             "Clennett2020_S2013" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Clennett_etal_2020_G3/Clennett_etal_2020_S2013.zip"],
+            "Muller2008" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Muller2008/Global_Model_Rigid_Internal_Release_2010.zip"],
+            "Scotese2016" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Scotese2016/PALEOMAP_GlobalPlateModel.zip"],
+            "Shephard2013" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Shephard2013/GPlates.zip"],
+            "Muller2022" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Muller2022/Muller_etal_2022_SE_1Ga_Opt.zip"],
 
         }
         return database
 
 
     def coastline_strings_to_include(self):
 
         strings = [
 
             "coastline",
-            "CEED6_LAND.gpml" # for TorsvikCocks2017
+            "CEED6_LAND.gpml", # for TorsvikCocks2017
+            "PALEOMAP_PoliticalBoundaries", # For Scotese 2016
         ]
         return strings
 
 
     def coastline_strings_to_ignore(self):
 
         strings = [
```

### Comparing `gplately-0.4/gplately/download.py` & `gplately-1.0/gplately/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -465,14 +465,20 @@
                 # creates an e-tag textfile for this version.
                 if not etag_exists:
                     if _os.path.isdir(full_path):
                         _shutil.rmtree(str(full_path))
                     elif _os.path.isfile(full_path):
                         _os.remove(full_path)
 
+                    if unprocessed_path:
+                        if _os.path.isdir(unprocessed_path):
+                            _shutil.rmtree(str(unprocessed_path))
+                        elif _os.path.isfile(unprocessed_path):
+                            _os.remove(unprocessed_path)
+
                     fnames, etag, local_etag_txtfile, used_fname = _first_time_download_from_web(
                         url, 
                         model_name=model_name,
                         verbose=verbose
                     )
                     return(fnames)
 
@@ -489,35 +495,43 @@
                     remote_etag, remote_etag_textfile = _get_url_etag(url)
 
                     # If the local and remote e-tags are unequal, the web-server URL 
                     # contains an updated version of the cached files.
                     if str(remote_etag) != str(local_etag):
                         if verbose:
                             print("Yes - updating requested files...")
-                        
+
                         # Update the e-tag textfile with this newly-identified URL e-tag
                         _save_url_etag_to_txt(remote_etag, local_etag_txtfile)
 
-                        # Re-download the file, and process it if need-be.
-                        with _pooch.utils.temporary_file(path=str(full_path.parent)) as tmp:
-                            downloader = _HTTPDownloader(progressbar=verbose)
-                            downloader(url, tmp, _pooch) 
-                            _shutil.move(tmp, str(full_path))
-                            processor=_determine_processor(url)[0]
-
-                            # If the file to update needs processing, pass the unprocessed file's
-                            # absolute path to the processor
-                            if unprocessed_path:
-                                processor(str(unprocessed_path), "update", None)
+                        # Delete existing version of the files...
+                        # If it didn't need processing, i.e. 'unzipping', just delete as-is
+                        if _os.path.isdir(full_path):
+                            _shutil.rmtree(str(full_path))
+                        elif _os.path.isfile(full_path):
+                            _os.remove(full_path)
                             
-                        # full_path holds the files to return to the user, irrespective of whether
-                        # proceessing was needed
+                        # If it's the kind of file that needs processing, delete the 
+                        # unprocessed version so we can re-download it
+                        if unprocessed_path:
+                            if _os.path.isdir(unprocessed_path):
+                                _shutil.rmtree(str(unprocessed_path))
+                            elif _os.path.isfile(unprocessed_path):
+                                _os.remove(unprocessed_path)
+
+                        # Treat as if downloading the file(s) from the URL for the first time
+                        fnames, etag, local_etag_txtfile, used_fname = _first_time_download_from_web(
+                            url, 
+                            model_name=model_name,
+                            verbose=verbose
+                        )
+
                         if verbose:
-                            print("Requested files downloaded to the GPlately cache folder!")
-                        return(_extract_processed_files(str(full_path)))
+                            print("Updated requested files downloaded to the GPlately cache folder!")
+                        return(fnames)
 
                     # If the e-tags are equal, the local and remote files are the same.
                     # Just return the file(s) as-is.
                     else:
                         if verbose:
                             print("Requested files are up-to-date!")
 
@@ -747,18 +761,19 @@
 
         import gplately
         import numpy as np
         import matplotlib.pyplot as plt
         import cartopy.crs as ccrs
 
         etopo1 = gplately.download.get_raster("ETOPO1_tif")
+        etopo1_data = etopo1.data
 
         fig = plt.figure(figsize=(18,14), dpi=300)
         ax = fig.add_subplot(111, projection=ccrs.Mollweide(central_longitude = -150))
-        etopo1.imshow(ax) 
+        etopo1.imshow(ax)
 
     """
     from matplotlib import image
     if raster_id_string is None:
         raise ValueError(
             "Please specify which raster to download."
         )
@@ -804,14 +819,27 @@
 def get_feature_data(feature_data_id_string=None, verbose=True):
     """Downloads assorted geological feature data from web servers (i.e. 
     [GPlates 2.3 sample data](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/))
     into the "gplately" cache.
 
     Currently, gplately supports the following feature data:
 
+    --------------
+
+    | **Feature data string identifier** | **Description**                                                                                                                                                                              |
+    |------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+    | Johansson2018                      | Large igneous provinces from  Johansson et al. (2018)                                                                                                                                        |
+    | Whittaker2015                      | Large igneous province products  interpreted as plume products  from Whittaker et al. (2015).                                                                                                |
+    | SeafloorFabric                     | Seafloor tectonic fabric  (fracture zones, discordant zones,  V-shaped structures, unclassified  V-anomalies, propagating ridge  lineations and extinct ridges)  from Matthews et al. (2011) |
+    | Hotspots                           | Present day surface hotspot/plume  locations from Whittaker et al. (2013)                                                                                                                    |
+   
+    ---------------
+
+    Detailed descriptions can be found below:
+
     * __Large igneous provinces from Johansson et al. (2018)__
 
         Information
         -----------
         * Formats: .gpmlz
         * `feature_data_id_string` = `Johansson2018`
 
@@ -936,16 +964,43 @@
         # string identifier to access the Muller et al. 2019 model
         gDownload = gplately.download.DataServer("Muller2019")
 
     all requested files are downloaded into the user's 'gplately' cache folder only _once_. If the same
     object and method(s) are re-run, the files will be re-accessed from the cache provided they have not been 
     moved or deleted. 
 
-    Currently, `DataServer` supports a number of plate reconstruction models. To call the object,
-    supply a `file_collection` string from one of the following models:
+    Currently, `DataServer` supports a number of plate reconstruction models. 
+
+    ------------------
+
+    | **Model name string Identifier** | **Rot. files** | **Topology features** | **Static polygons** | **Coast-lines** | **Cont-inents** | **COB-** | **Age grids** | **SR grids** |
+    |:--------------------------------:|:--------------:|:---------------------:|:-------------------:|:---------------:|:---------------:|:--------:|:-------------:|:------------:|
+    |            Muller2019            |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ✅    |       ✅       |       ❌      |
+    |            Muller2016            |        ✅       |           ✅           |          ✅          |        ✅        |        ❌        |     ❌    |       ✅       |       ❌      |
+    |            Merdith2021           |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |              Cao2020             |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |           Clennett2020           |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ❌    |       ✅       |       ✅      |
+    |             Seton2012            |        ✅       |           ✅           |          ❌          |        ✅        |        ❌        |     ✅    |       ✅       |       ❌      |
+    |           Matthews2016           |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |            Merdith2017           |        ✅       |           ✅           |          ❌          |        ❌        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |              Li2008              |        ✅       |           ✅           |          ❌          |        ❌        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |           Pehrsson2015           |        ✅       |           ✅           |          ❌          |        ❌        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |         TorsvikCocks2017         |        ✅       |           ❌           |          ❌          |        ✅        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |             Young2019            |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |            Scotese2008           |        ✅       |           ✅           |          ❌          |        ❌        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |         Clennett2020_M19         |        ✅       |           ✅           |          ❌          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |         Clennett2020_S13         |        ✅       |           ✅           |          ❌          |        ✅        |        ✅        |     ❌    |       ❌       |       ❌      |
+    |            Muller2008            |        ✅       |           ❌           |          ✅          |        ❌        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |            Muller2022            |        ✅       |           ✅           |          ✅          |        ✅        |        ✅        |     ✅    |       ❌       |       ❌      |
+    |            Scotese2016           |        ✅       |           ❌           |          ✅          |        ✅        |        ❌        |     ❌    |       ❌       |       ❌      |
+    |           Shephard2013           |        ✅       |           ✅           |          ✅          |        ✅        |        ❌        |     ❌    |       ❌       |       ❌      |
+
+    ------------------
+
+    To call the object, supply a model name string Identifier, `file_collection`, from one of the following models:
 
     * __[Müller et al. 2019](https://www.earthbyte.org/muller-et-al-2019-deforming-plate-reconstruction-and-seafloor-age-grids-tectonics/):__ 
 
         file_collection = `Muller2019`
     
         Information
         -----------
@@ -1183,15 +1238,15 @@
     - __Clennett et al. 2020 (based on Müller et al. 2019)__: 
 
         file_collection = `Clennett2020_M2019`
 
         Information
         -----------
         * Downloadable files: `rotation_model`, `topology_features`, `continents` and `coastlines`
-        * Maximum reconstruction time: 250 Ma
+        * Maximum reconstruction time: 170 Ma
         
         Citations
         ---------
         * Clennett, E.J., Sigloch, K., Mihalynuk, M.G., Seton, M., Henderson, M.A., Hosseini, K.,
         Mohammadzaheri, A., Johnston, S.T., Müller, R.D., (2020), A Quantitative Tomotectonic Plate 
         Reconstruction of Western North America and the Eastern Pacific Basin. Geochemistry, Geophysics, 
         Geosystems, 21, e2020GC009117. DOI: https://doi.org/10.1029/2020GC009117
@@ -1200,23 +1255,97 @@
     - __Clennett et al. 2020 (rigid topological model based on Shephard et al, 2013)__: 
 
         file_collection = `Clennett2020_S2013`
 
         Information
         -----------
         * Downloadable files: `rotation_model`, `topology_features`, `continents` and `coastlines`
-        * Maximum reconstruction time: 
+        * Maximum reconstruction time: 170
         
         Citations
         ---------
         * Clennett, E.J., Sigloch, K., Mihalynuk, M.G., Seton, M., Henderson, M.A., Hosseini, K.,
         Mohammadzaheri, A., Johnston, S.T., Müller, R.D., (2020), A Quantitative Tomotectonic Plate 
         Reconstruction of Western North America and the Eastern Pacific Basin. Geochemistry, Geophysics, 
         Geosystems, 21, e2020GC009117. DOI: https://doi.org/10.1029/2020GC009117
 
+
+    - __Müller et al. 2008__:
+
+        file_collection = `Muller2008`
+
+        Information
+        -----------
+        * Downloadable files:  `rotation_model`, `static_polygons`
+        * Maximum reconstruction time: 141 Ma
+
+        Citations
+        ---------
+        * Müller, R. D., Sdrolias, M., Gaina, C., & Roest, W. R. (2008). Age, spreading rates, and 
+        spreading asymmetry of the world's ocean crust. Geochemistry, Geophysics, Geosystems, 9(4).
+
+
+
+    - __Müller et al. 2022__:
+
+        file_collection = `Muller2022`
+
+        Information
+        -----------
+        * Downloadable files:  `rotation_model`, `topology_features`, `static_polygons`, `continents`, `coastlines` and `COBs`
+        * Maximum reconstruction time: 1000 Ma
+
+        Citations
+        ---------
+        *  Müller, R. D., Flament, N., Cannon, J., Tetley, M. G., Williams, S. E., Cao, X., Bodur, Ö. F., Zahirovic, S., 
+        and Merdith, A.: A tectonic-rules-based mantle reference frame since 1 billion years ago – implications for 
+        supercontinent cycles and plate–mantle system evolution, Solid Earth, 13, 1127–1159, 
+        https://doi.org/10.5194/se-13-1127-2022, 2022.
+
+
+
+    - __Scotese 2016__:
+
+        file_collection = `Scotese2016`
+
+        Information
+        -----------
+        * Downloadable files:  `rotation_model`, `static_polygons`, `coastlines` 
+        * Maximum reconstruction time: 410 Ma
+
+        Citations
+        ---------
+        * Scotese, C.R., 2016. PALEOMAP PaleoAtlas for GPlates and the PaleoData 
+        Plotter Program, PALEOMAP Project, 
+        http://www.earthbyte.org/paleomappaleoatlas-for-gplates/
+
+
+    - __Shephard et al. 2013__:
+
+        file_collection = `Shephard2013`
+
+        Information
+        -----------
+        * Downloadable files:  `rotation_model`, `topology_features`, `static_polygons`, `coastlines`
+        * Maximum reconstruction time: 200 Ma
+
+        Citations
+        ---------
+        * Shephard, G.E., Müller, R.D., and Seton, M., 2013. The tectonic evolution of the Arctic since 
+        Pangea breakup: Integrating constraints from surface geology and geophysics with mantle structure. 
+        Earth-Science Reviews, Volume 124 p.148-183. doi:10.1016/j.earscirev.2013.05.012 
+        (http://www.sciencedirect.com/science/article/pii/S0012825213001104)
+
+        * M. Seton, R.D. Müller, S. Zahirovic, C. Gaina, T.H. Torsvik, G. Shephard, A. Talsma, M. Gurnis, 
+        M. Turner, S. Maus, M. Chandler, Global continental and ocean basin reconstructions since 200 Ma, 
+        Earth-Science Reviews, Volume 113, p.212-270 doi:10.1016/j.earscirev.2012.03.002.
+        (http://www.sciencedirect.com/science/article/pii/S0012825212000311)
+
+
+
         Parameters
         ----------
         file_collection : str
             name of file collection to use
 
         verbose : bool, default True
             Toggle print messages regarding server/internet connection status, file availability etc.
@@ -1591,15 +1720,15 @@
 
                 gdownload = gplately.DataServer("Muller2019")
 
                 graster = gdownload.get_age_grid(time=100)
 
                 graster_data = graster.data
 
-            where `graster_data` is a numpy ndarray. 
+            where `graster_data` is a numpy ndarray.
 
         Raises
         -----
         ValueError
             If `time` (a single integer, or a list of integers representing reconstruction
             times to extract the age grids from) is not passed.
```

### Comparing `gplately-0.4/gplately/geometry.py` & `gplately-1.0/gplately/geometry.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/gpml.py` & `gplately-1.0/gplately/gpml.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/grids.py` & `gplately-1.0/gplately/grids.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/io.py` & `gplately-1.0/gplately/io.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/oceans.py` & `gplately-1.0/gplately/oceans.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/parallel.py` & `gplately-1.0/gplately/parallel.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/gplately/plot.py` & `gplately-1.0/gplately/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,26 +118,26 @@
             )
         triangles = []
         for p in geometries[polarity_column].unique():
             if p.lower() not in {"left", "l", "right", "r"}:
                 continue
             gdf_polarity = geometries[geometries[polarity_column] == p]
             triangles.extend(
-                _tesselate_triangles(
+                _tessellate_triangles(
                     gdf_polarity,
                     width,
                     p,
                     height,
                     spacing,
                     projection,
                     transform,
                 )
             )
     else:
-        triangles = _tesselate_triangles(
+        triangles = _tessellate_triangles(
             geometries,
             width,
             polarity,
             height,
             spacing,
             projection,
             transform,
@@ -150,15 +150,15 @@
     if hasattr(ax, "add_geometries") and projection is not None:
         ax.add_geometries(triangles, crs=projection, **kwargs)
     else:
         for triangle in triangles:
             ax.fill(*triangle.exterior.xy, **kwargs)
 
 
-def _tesselate_triangles(
+def _tessellate_triangles(
     geometries,
     width,
     polarity="left",
     height=None,
     spacing=None,
     projection=None,
     transform=None,
@@ -282,15 +282,15 @@
     polarity,
 ):
     """Generate vertices of subduction teeth triangles.
 
     Triangle bases are set on shapely BaseGeometry trench instances with their apexes 
     pointing in directions of subduction polarity. Triangle dimensions are set by a 
     specified width, spacing and height (either provided by the user or set as default
-    values from _tesselate_triangles). The teeth are returned as shapely polygons.
+    values from _tessellate_triangles). The teeth are returned as shapely polygons.
 
     Parameters
     ----------
     geometries : list of shapely geometries (instances of the
         shapely.geometry.base.BaseGeometry or shapely.geometry.base.BaseMultipartGeometry
         class)
         Trench geometries projected onto a certain map projection (using a 
@@ -316,37 +316,37 @@
     if isinstance(geometries, BaseGeometry):
         geometries = [geometries]
     triangles = []
     for geometry in geometries:
         if not isinstance(geometry, BaseGeometry):
             continue
         length = geometry.length
-        tesselated_x = []
-        tesselated_y = []
+        tessellated_x = []
+        tessellated_y = []
         for distance in np.arange(spacing, length, spacing):
             point = Point(geometry.interpolate(distance))
-            tesselated_x.append(point.x)
-            tesselated_y.append(point.y)
-        tesselated_x = np.array(tesselated_x)
-        tesselated_y = np.array(tesselated_y)
-
-        for i in range(len(tesselated_x) - 1):
-            normal_x = tesselated_y[i] - tesselated_y[i + 1]
-            normal_y = tesselated_x[i + 1] - tesselated_x[i]
+            tessellated_x.append(point.x)
+            tessellated_y.append(point.y)
+        tessellated_x = np.array(tessellated_x)
+        tessellated_y = np.array(tessellated_y)
+
+        for i in range(len(tessellated_x) - 1):
+            normal_x = tessellated_y[i] - tessellated_y[i + 1]
+            normal_y = tessellated_x[i + 1] - tessellated_x[i]
             normal = np.array((normal_x, normal_y))
             normal_mag = np.sqrt((normal ** 2).sum())
             if normal_mag == 0:
                 continue
             normal *= height / normal_mag
-            midpoint = np.array((tesselated_x[i], tesselated_y[i]))
+            midpoint = np.array((tessellated_x[i], tessellated_y[i]))
             if polarity == "right":
                 normal *= -1.0
             apex = midpoint + normal
 
-            next_midpoint = np.array((tesselated_x[i + 1], tesselated_y[i + 1]))
+            next_midpoint = np.array((tessellated_x[i + 1], tessellated_y[i + 1]))
             line_vector = np.array(next_midpoint - midpoint)
             line_vector_mag = np.sqrt((line_vector ** 2).sum())
             line_vector /= line_vector_mag
             triangle_point_a = midpoint + width * 0.5 * line_vector
             triangle_point_b = midpoint - width * 0.5 * line_vector
             triangle_points = np.array(
                 (
@@ -565,43 +565,51 @@
     * Turn these reconstructed features into Shapely geometries for plotting 
     on `cartopy.mpl.geoaxes.GeoAxes` or `cartopy.mpl.geoaxes.GeoAxesSubplot` map 
     Projections. 
 
     To call the `PlotTopologies` object, supply: 
 
     * an instance of the GPlately `plate_reconstruction` object
-    * a reconstruction `time`
 
     and optionally, 
 
     * a `coastline_filename`
     * a `continent_filename`
     * a `COB_filename`
+    * a reconstruction `time`
     * an `anchor_plate_id`
 
     For example:
 
         # Calling the PlotTopologies object
         gplot = gplately.plot.PlotTopologies(plate_reconstruction,
-                                            time,
-                                            coastline_filename,
-                                            continent_filename,
-                                            COB_filename,
-                                            anchor_plate_id,
+                                            coastline_filename=None,
+                                            continent_filename=None,
+                                            COB_filename=None,
+                                            time=None,
+                                            anchor_plate_id=0,
                 )
 
+        # Setting a new reconstruction time
+        gplot.time = 20 # Ma
+
     The `coastline_filename`, `continent_filename` and `COB_filename` can be single
     strings to GPML and/or shapefiles, as well as instances of `pygplates.FeatureCollection`. 
     If using GPlately's `DataServer` object to source these files, they will be passed as 
     `pygplates.FeatureCollection` items.
 
     Some features for plotting (like plate boundaries) are taken from the `PlateReconstruction` 
     object's`topology_features` attribute. They have already been reconstructed to the given
     `time` using [Plate Tectonic Tools](https://github.com/EarthByte/PlateTectonicTools).
+    Simply provide a new reconstruction time by changing the `time` attribute, e.g.
+
+        gplot.time = 20 # Ma
 
+    which will automatically reconstruct all topologies to the specified time.
+    You __MUST__ set `gplot.time` before plotting anything.
 
     A variety of geological features can be plotted on GeoAxes/GeoAxesSubplot maps 
     as Shapely `MultiLineString` or `MultiPolygon` geometries, including:
     
     * subduction boundaries & subduction polarity teeth
     * mid-ocean ridge boundaries
     * transform boundaries
@@ -694,18 +702,18 @@
         continental rifts, faults, orogenic belts, fracture zones, inferred paleo boundaries, terrane 
         boundaries and passive continental boundaries.
 
     """
     def __init__(
         self,
         plate_reconstruction,
-        time=None,
         coastlines=None,
         continents=None,
         COBs=None,
+        time=None,
         anchor_plate_id=0,
     ):
         self.plate_reconstruction = plate_reconstruction
 
         if self.plate_reconstruction.topology_features is None:
             raise ValueError("Plate model must have topology features.")
 
@@ -917,15 +925,15 @@
 
         if self._COBs:
             self.COBs = self.plate_reconstruction.reconstruct(
                 self._COBs, self.time, from_time=0, anchor_plate_id=self.anchor_plate_id)
 
 
     # subduction teeth
-    def _tesselate_triangles(self, features, tesselation_radians, triangle_base_length, triangle_aspect=1.0):
+    def _tessellate_triangles(self, features, tesselation_radians, triangle_base_length, triangle_aspect=1.0):
         """Places subduction teeth along subduction boundary line segments within a MultiLineString shapefile. 
 
         Parameters
         ----------
         shapefilename  : str  
             Path to shapefile containing the subduction boundary features
 
@@ -1748,20 +1756,20 @@
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with subduction teeth plotted onto the chosen map projection.
         """
         import shapely
 
         # add Subduction Teeth
-        subd_xL, subd_yL = self._tesselate_triangles(
+        subd_xL, subd_yL = self._tessellate_triangles(
             self.trench_left,
             tesselation_radians=spacing,
             triangle_base_length=size,
             triangle_aspect=-aspect)
-        subd_xR, subd_yR = self._tesselate_triangles(
+        subd_xR, subd_yR = self._tessellate_triangles(
             self.trench_right,
             tesselation_radians=spacing,
             triangle_base_length=size,
             triangle_aspect=aspect)
         
         teeth = []
         for tX, tY in zip(subd_xL, subd_yL):
@@ -1773,14 +1781,61 @@
             triangle_xy_points = np.c_[tX, tY]
             shp = shapely.geometry.Polygon(triangle_xy_points)
             teeth.append(shp)
 
         return ax.add_geometries(teeth, crs=self.base_projection, color=color, **kwargs)
 
 
+    def get_subduction_direction(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of trench directions.
+
+        Notes
+        -----
+        The `trench_left` and `trench_right` geometries needed to produce the GeoDataFrame are automatically
+        constructed if the optional `time` parameter is passed to the `PlotTopologies` object before calling
+        this function. `time` can be passed either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `other` geometries are reconstructed, they are 
+        converted into Shapely features whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf_left : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `trench_left` geometry.
+        gdf_right : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `trench_right` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `trench_left` or `trench_right` geometries to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No miscellaneous topologies have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.trench_left is None or self.trench_right is None:
+            raise ValueError("No trench_left or trench_right topologies passed to PlotTopologies.")
+
+        trench_left_features  = shapelify_feature_lines(self.trench_left)
+        trench_right_features = shapelify_feature_lines(self.trench_right)
+
+        gdf_left  = gpd.GeoDataFrame({"geometry": trench_left_features},  geometry="geometry")
+        gdf_right = gpd.GeoDataFrame({"geometry": trench_right_features}, geometry="geometry")
+
+        return gdf_left, gdf_right
+
+
     def plot_subduction_teeth(self, ax, spacing=0.07, size=None, aspect=None, color='black', **kwargs):
         """Plot subduction teeth onto a standard map Projection.  
 
         Notes
         -----
         Subduction teeth are tessellated from `PlotTopologies` object attributes `trench_left` and 
         `trench_right`, and transformed into Shapely polygons for plotting. 
@@ -1814,14 +1869,16 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with subduction teeth plotted onto the chosen map projection.
         """
+        if self._time is None:
+            raise ValueError("No miscellaneous topologies have been resolved. Set `PlotTopologies.time` to construct them.")
 
         spacing = spacing * EARTH_RADIUS * 1e3
 
         if aspect is None:
             aspect = 2.0/3.0
         if size is None:
             size = spacing*0.5
@@ -1874,15 +1931,15 @@
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
             The map should be set at a particular Cartopy projection.
 
-        grid : MaskedArray
+        grid : MaskedArray or `gplately.grids.Raster`
             A `MaskedArray` with elements that define a grid. The number of rows in the raster
             corresponds to the number of latitudinal coordinates, while the number of raster 
             columns corresponds to the number of longitudinal coordinates.
 
         extent : 1d array, default=[-180,180,-90,90]
             A four-element array to specify the [min lon, max lon, min lat, max lat] with 
             which to constrain the grid image. If no extents are supplied, full global 
@@ -1898,16 +1955,27 @@
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with the grid plotted onto the chosen map projection.
         """
         # Override matplotlib default origin ('upper')
         origin = kwargs.pop("origin", "lower")
+
+        from .grids import Raster
+
+        if isinstance(grid, Raster):
+            # extract extent and origin
+            extent = grid.extent
+            origin = grid.origin
+            data = grid.data
+        else:
+            data = grid
+
         return ax.imshow(
-            grid,
+            data,
             extent=extent,
             transform=self.base_projection,
             origin=origin,
             **kwargs,
         )
 
 
@@ -1936,19 +2004,28 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with the netCDF grid plotted onto the chosen map projection.
         """
+        # Override matplotlib default origin ('upper')
+        origin = kwargs.pop("origin", "lower")
+
         from .grids import read_netcdf_grid
 
         raster, lon_coords, lat_coords = read_netcdf_grid(filename, return_grids=True)
-        extent = [lon_coords.min(), lon_coords.max(), lat_coords.min(), lat_coords.max()]
-        return self.plot_grid(ax, raster, extent=extent, **kwargs)
+        extent = [lon_coords[0], lon_coords[-1], lat_coords[0], lat_coords[-1]]
+
+        if lon_coords[0] < lat_coords[-1]:
+            origin = "lower"
+        else:
+            origin = "upper"
+
+        return self.plot_grid(ax, raster, extent=extent, origin=origin, **kwargs)
 
 
     def plot_plate_motion_vectors(self, ax, spacingX=10, spacingY=10, normalise=False, **kwargs):
         """Calculate plate motion velocity vector fields at a particular geological time 
         and plot them onto a standard map Projection. 
         
         Notes
@@ -2990,7 +3067,91 @@
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with unclassified features plotted onto the chosen map projection.
         """
         gdf = self.get_unclassified_features()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
+    def get_all_topologies(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed unclassified feature lines. 
+
+        Notes
+        -----
+        The `topologies` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `topologies` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `topologies` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `topologies` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No topologies have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.topologies is None:
+            raise ValueError("No topologies passed to PlotTopologies.")
+
+        all_topologies = shapelify_features(self.topologies)
+
+        # get plate IDs and feature types to add to geodataframe
+        plate_IDs = []
+        feature_types = []
+        feature_names = []
+        for topo in self.topologies:
+            ft_type = topo.get_feature_type()
+
+            plate_IDs.append(topo.get_reconstruction_plate_id())
+            feature_types.append(ft_type)
+            feature_names.append(ft_type.get_name())
+
+        gdf = gpd.GeoDataFrame({"geometry": all_topologies,
+                                "reconstruction_plate_ID": plate_IDs,
+                                "feature_type": feature_types,
+                                "feature_name": feature_names},
+                                geometry="geometry")
+        return gdf
+
+
+    def plot_all_topologies(self, ax, color='black', **kwargs):
+        """Plot all topologies on a standard map projection.
+
+        Parameters
+        ----------
+        ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
+            A subclass of `matplotlib.axes.Axes` which represents a map Projection.
+            The map should be set at a particular Cartopy projection.
+
+        color : str, default=’black’
+            The colour of the trench lines. By default, it is set to black.
+
+        **kwargs : 
+            Keyword arguments for parameters such as `alpha`, etc. 
+            for plotting trench geometries.
+            See `Matplotlib` keyword arguments 
+            [here](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html).
+
+        Returns
+        -------
+        ax : instance of <geopandas.GeoDataFrame.plot>
+            A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
+            with unclassified features plotted onto the chosen map projection.
+        """
+        gdf = self.get_all_topologies()
+        return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
```

### Comparing `gplately-0.4/gplately/reconstruction.py` & `gplately-1.0/gplately/reconstruction.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,22 +86,22 @@
 
         if 'static_polygons' in state:
             self.static_polygons = _FeatureCollection()
             for polygon in state['static_polygons']:
                 self.static_polygons.add( _FeatureCollection(polygon) )
 
 
-    def tesselate_subduction_zones(self, time, tessellation_threshold_radians=0.001, ignore_warnings=False, **kwargs):
+    def tessellate_subduction_zones(self, time, tessellation_threshold_radians=0.001, ignore_warnings=False, return_geodataframe=False, **kwargs):
         """Samples points along subduction zone trenches and obtains subduction data at a particular
         geological time.
         
         Resolves topologies at `time`, tessellates all resolved subducting features to within 'tessellation_threshold_radians'
         radians and obtains the following information for each sampled point along a trench:
     
-        `tesselate_subduction_zones` returns a list of 10 vertically-stacked tuples with the following data per sampled trench point:
+        `tessellate_subduction_zones` returns a list of 10 vertically-stacked tuples with the following data per sampled trench point:
 
         * Col. 0 - longitude of sampled trench point
         * Col. 1 - latitude of sampled trench point
         * Col. 2 - subducting convergence (relative to trench) velocity magnitude (in cm/yr)
         * Col. 3 - subducting convergence velocity obliquity angle (angle between trench normal vector and convergence velocity vector)
         * Col. 4 - trench absolute (relative to anchor plate) velocity magnitude (in cm/yr)
         * Col. 5 - trench absolute velocity obliquity angle (angle between trench normal vector and trench absolute velocity vector)
@@ -177,15 +177,39 @@
                 self.rotation_model,
                 self.topology_features,
                 tessellation_threshold_radians,
                 float(time),
                 **kwargs)
 
         subduction_data = np.vstack(subduction_data)
-        return subduction_data
+
+        if return_geodataframe:
+            from shapely import geometry
+            import geopandas as gpd
+            coords = [geometry.Point(lon,lat) for lon,lat in zip(subduction_data[:,0], subduction_data[:,1])]
+            d = {"geometry": coords}
+
+            labels = ['convergence velocity (cm/yr)',
+                      'convergence obliquity angle (degrees)',
+                      'trench velocity (cm/yr)',
+                      'trench obliquity angle (degrees)',
+                      'length (degrees)',
+                      'trench normal angle (degrees)',
+                      'subducting plate ID',
+                      'overriding plate ID']
+
+            for i, label in enumerate(labels):
+                index = 2+i
+                d[label] = subduction_data[:,index]
+
+            gdf = gpd.GeoDataFrame(d, geometry="geometry")
+            return gdf
+
+        else:
+            return subduction_data
 
 
     def total_subduction_zone_length(self, time, use_ptt=False, ignore_warnings=False):
         """Calculates the total length of all mid-ocean ridges (km) at the specified geological time (Ma).
 
         if `use_ptt` is True
         
@@ -220,15 +244,15 @@
         total_subduction_zone_length_kms : float
             The total subduction zone length (in km) at the specified `time`.
 
         """
         if use_ptt:
             with warnings.catch_warnings():
                 warnings.simplefilter('ignore')
-                subduction_data = self.tesselate_subduction_zones(time, ignore_warnings=ignore_warnings)
+                subduction_data = self.tessellate_subduction_zones(time, ignore_warnings=ignore_warnings)
 
             trench_arcseg = subduction_data[:,6]
             trench_pt_lat = subduction_data[:,1]
             
             total_subduction_zone_length_kms = 0
             for i, segment in enumerate(trench_arcseg):
                 earth_radius = _tools.geocentric_radius(trench_pt_lat[i])/1e3
@@ -318,15 +342,15 @@
         if (time != graster.time) and (not ignore_warnings):
             raise RuntimeWarning(
                 "`continental_grid.time` ({}) ".format(graster.time)
                 + "does not match `time` ({})".format(time)
             )
 
         # Obtain trench data with Plate Tectonic Tools
-        trench_data = self.tesselate_subduction_zones(time, ignore_warnings=ignore_warnings)
+        trench_data = self.tessellate_subduction_zones(time, ignore_warnings=ignore_warnings)
 
         # Extract trench data
         trench_normal_azimuthal_angle = trench_data[:,7]
         trench_arcseg = trench_data[:,6]
         trench_pt_lon = trench_data[:,0]
         trench_pt_lat = trench_data[:,1]
 
@@ -351,15 +375,15 @@
         point_lats = ilat[continental_indices]
         point_radii = _tools.geocentric_radius(point_lats) * 1.0e-3  # km
         segment_arclens = np.deg2rad(trench_arcseg[continental_indices])
         segment_lengths = point_radii * segment_arclens
         return np.sum(segment_lengths)
 
 
-    def tesselate_mid_ocean_ridges(self, time, tessellation_threshold_radians=0.001, ignore_warnings=False, **kwargs):
+    def tessellate_mid_ocean_ridges(self, time, tessellation_threshold_radians=0.001, ignore_warnings=False, return_geodataframe=False, **kwargs):
         """Samples points along resolved spreading features (e.g. mid-ocean ridges) and calculates spreading rates and 
         lengths of ridge segments at a particular geological time.
          
         Resolves topologies at `time`, tessellates all resolved spreading features to within 'tessellation_threshold_radians'
         radians. Returns a 4-column vertically stacked tuple with the following data.
 
         * Col. 0 - longitude of sampled ridge point
@@ -413,15 +437,28 @@
                 self.topology_features,
                 float(time),
                 tessellation_threshold_radians,
                 spreading_feature_types,
                 **kwargs)
 
         ridge_data = np.vstack(ridge_data)
-        return ridge_data
+
+        if return_geodataframe:
+            from shapely import geometry
+            import geopandas as gpd
+
+            points = [geometry.Point(lon,lat) for lon,lat in zip(ridge_data[:,0], ridge_data[:,1])]
+            gdf = gpd.GeoDataFrame({"geometry": points,
+                                    "velocity (cm/yr)": ridge_data[:,2],
+                                    "length (degrees)": ridge_data[:,3]},
+                                    geometry="geometry")
+            return gdf
+
+        else:
+            return ridge_data
 
 
     def total_ridge_length(self, time, use_ptt=False, ignore_warnings=False):
         """Calculates the total length of all mid-ocean ridges (km) at the specified geological time (Ma).
 
         if `use_ptt` is True
         
@@ -454,15 +491,15 @@
         total_ridge_length_kms : float
             The total length of global mid-ocean ridges (in kilometres) at the specified time.
         """
 
         if use_ptt is True:
             with warnings.catch_warnings():
                 warnings.simplefilter('ignore')
-                ridge_data = self.tesselate_mid_ocean_ridges(time)
+                ridge_data = self.tessellate_mid_ocean_ridges(time)
 
             ridge_arcseg = ridge_data[:,3]
             ridge_pt_lat = ridge_data[:,1]
 
             total_ridge_length_kms = 0
             for i, segment in enumerate(ridge_arcseg):
                 earth_radius = _tools.geocentric_radius(ridge_pt_lat[i])/1e3
@@ -958,21 +995,22 @@
         if not provided.
 
     """
     def __init__(self, plate_reconstruction, lons, lats, time=0, plate_id=None):
         self.lons = lons
         self.lats = lats
         self.time = time
+        self.attributes = dict()
 
         self.plate_reconstruction = plate_reconstruction
 
-        self.update(lons, lats, time, plate_id)
+        self._update(lons, lats, time, plate_id)
 
 
-    def update(self, lons, lats, time=0, plate_id=None):
+    def _update(self, lons, lats, time=0, plate_id=None):
 
         # get Cartesian coordinates
         self.x, self.y, self.z = _tools.lonlat2xyz(lons, lats, degrees=False)
 
         # scale by average radius of the Earth
         self.x *= _tools.EARTH_RADIUS
         self.y *= _tools.EARTH_RADIUS
@@ -1005,48 +1043,220 @@
             plate_id = np.empty(len(self.lons), dtype=int)
             for i, feature in enumerate(partitioned_features):
                 plate_id[i] = feature.get_reconstruction_plate_id()
 
         self.plate_id = plate_id
         self.FeatureCollection = pygplates.FeatureCollection(self.features)
 
+    @property
+    def size(self):
+        """ Number of points
+        """
+        return len(self.lons)
+
 
     def __getstate__(self):
 
         filenames = self.plate_reconstruction.__getstate__()
 
         # add important variables from Points object
         filenames["lons"] = self.lons
         filenames["lats"] = self.lats
         filenames['time'] = self.time
         filenames['plate_id'] = self.plate_id
+        for key in self.attributes:
+            filenames[key] = self.attributes[key]
 
         return filenames
 
     def __setstate__(self, state):
 
         self.plate_reconstruction = PlateReconstruction(state['rotation_model'], state['topology_features'], state['static_polygons'])
 
         # reinstate unpicklable items
         self.lons = state['lons']
         self.lats = state['lats']
         self.time = state['time']
         self.plate_id = state['plate_id']
+        self.attributes = dict()
 
-        self.update(self.lons, self.lats, self.time, self.plate_id)
+        self._update(self.lons, self.lats, self.time, self.plate_id)
+
+        for key in state:
+            if key not in ['lons', 'lats', 'time', 'plate_id']:
+                self.attributes[key] = state[key]
 
     def copy(self):
         """ Returns a copy of the Points object
 
         Returns
         -------
         Points
             A copy of the current Points object
         """
-        return Points(self.plate_reconstruction, self.lons, self.lats, self.time, self.plate_id)
+        gpts = Points(self.plate_reconstruction, self.lons.copy(), self.lats.copy(), self.time, self.plate_id.copy())
+        gpts.add_attributes(**self.attributes.copy())
+
+    def add_attributes(self, **kwargs):
+        """ Adds the value of a feature attribute associated with a key.
+
+        Example
+        -------
+
+            # Define latitudes and longitudes to set up a Points object
+            pt_lons = np.array([140., 150., 160.])
+            pt_lats = np.array([-30., -40., -50.])
+
+            gpts = gplately.Points(model, pt_lons, pt_lats)
+
+            # Add the attributes a, b and c to the points in the Points object
+            gpts.add_attributes(
+                a=[10,2,2], 
+                b=[2,3,3], 
+                c=[30,0,0],
+            )
+
+            print(gpts.attributes)
+
+        The output would be:
+
+            {'a': [10, 2, 2], 'b': [2, 3, 3], 'c': [30, 0, 0]}
+
+        Parameters
+        ----------
+        **kwargs : sequence of key=item/s
+            A single key=value pair, or a sequence of key=value pairs denoting the name and
+            value of an attribute.
+
+
+        Notes
+        -----
+        * An **assertion** is raised if the number of points in the Points object is not equal
+        to the number of values associated with an attribute key. For example, consider an instance
+        of the Points object with 3 points. If the points are ascribed an attribute `temperature`,
+        there must be one `temperature` value per point, i.e. `temperature = [20, 15, 17.5]`.
+
+        """
+        keys = kwargs.keys()
+
+        for key in kwargs:
+            attribute = kwargs[key]
+
+            # make sure attribute is the same size as self.lons
+            if type(attribute) is int or type(attribute) is float:
+                array = np.full(self.lons.size, attribute)
+                attribute = array
+            elif isinstance(attribute, np.ndarray):
+                if attribute.size == 1:
+                    array = np.full(self.lons.size, attribute, dtype=attribute.dtype)
+                    attribute = array
+
+            assert len(attribute) == self.lons.size, "Size mismatch, ensure attributes have the same number of entries as Points"
+            self.attributes[key] = attribute
+
+        if any(kwargs):
+            # add these to the FeatureCollection
+            for f, feature in enumerate(self.FeatureCollection):
+                for key in keys:
+                    # extract value for each row in attribute
+                    val = self.attributes[key][f]
+
+                    # set this attribute on the feature
+                    feature.set_shapefile_attribute(key, val)
+
+    def get_geopandas_dataframe(self):
+        """ Adds a shapely point `geometry` attribute to each point in the `gplately.Points` object.
+        pandas.DataFrame that has a column with geometry
+        Any existing point attributes are kept.
+
+        Returns
+        -------
+        GeoDataFrame : instance of `geopandas.GeoDataFrame`
+            A pandas.DataFrame with rows equal to the number of points in the `gplately.Points` object,
+            and an additional column containing a shapely `geometry` attribute.
+
+        Example
+        -------
+
+            pt_lons = np.array([140., 150., 160.])
+            pt_lats = np.array([-30., -40., -50.])
+
+            gpts = gplately.Points(model, pt_lons, pt_lats)
+
+            # Add sample attributes a, b and c to the points in the Points object
+            gpts.add_attributes(
+                a=[10,2,2], 
+                b=[2,3,3], 
+                c=[30,0,0],
+            )
+
+            gpts.get_geopandas_dataframe()
+
+        ...has the output:
+
+                a  b   c                     geometry
+            0  10  2  30  POINT (140.00000 -30.00000)
+            1   2  3   0  POINT (150.00000 -40.00000)
+            2   2  3   0  POINT (160.00000 -50.00000)
+
+
+        """
+        import geopandas as gpd
+        from shapely import geometry
+
+        # create shapely points
+        points = []
+        for lon, lat in zip(self.lons, self.lats):
+            points.append( geometry.Point(lon, lat) )
+
+        attributes = self.attributes.copy()
+        attributes['geometry'] = points
+
+        return gpd.GeoDataFrame(attributes, geometry='geometry')
+
+    def get_geodataframe(self):
+        """ Returns the output of `Points.get_geopandas_dataframe()`.
+
+        Adds a shapely point `geometry` attribute to each point in the `gplately.Points` object.
+        pandas.DataFrame that has a column with geometry
+        Any existing point attributes are kept.
+
+        Returns
+        -------
+        GeoDataFrame : instance of `geopandas.GeoDataFrame`
+            A pandas.DataFrame with rows equal to the number of points in the `gplately.Points` object,
+            and an additional column containing a shapely `geometry` attribute.
+
+        Example
+        -------
+
+            pt_lons = np.array([140., 150., 160.])
+            pt_lats = np.array([-30., -40., -50.])
+
+            gpts = gplately.Points(model, pt_lons, pt_lats)
+
+            # Add sample attributes a, b and c to the points in the Points object
+            gpts.add_attributes(
+                a=[10,2,2], 
+                b=[2,3,3], 
+                c=[30,0,0],
+            )
+
+            gpts.get_geopandas_dataframe()
+
+        ...has the output:
+
+                a  b   c                     geometry
+            0  10  2  30  POINT (140.00000 -30.00000)
+            1   2  3   0  POINT (150.00000 -40.00000)
+            2   2  3   0  POINT (160.00000 -50.00000)
+
+
+        """
+        return self.get_geopandas_dataframe()
 
     def reconstruct(self, time, anchor_plate_id=0, return_array=False, **kwargs):
         """Reconstructs regular geological features, motion paths or flowlines to a specific geological time and extracts 
         the latitudinal and longitudinal points of these features.
 
         Note: this method accesses and uses the rotation model attribute from the PointReconstruction object, and reconstructs 
         the feature lat-lon point attributes of the Points object.
@@ -1099,15 +1309,17 @@
         reconstructed_features = self.plate_reconstruction.reconstruct(
             self.features, to_time, from_time, anchor_plate_id=anchor_plate_id, **kwargs)
 
         rlons, rlats = _tools.extract_feature_lonlat(reconstructed_features)
         if return_array:
             return rlons, rlats
         else:
-            return Points(self.plate_reconstruction, rlons, rlats, time=to_time, plate_id=self.plate_id)
+            gpts = Points(self.plate_reconstruction, rlons, rlats, time=to_time, plate_id=self.plate_id)
+            gpts.add_attributes(**self.attributes.copy())
+            return gpts
 
 
     def reconstruct_to_birth_age(self, ages, anchor_plate_id=0, **kwargs):
         """ Reconstructs point features supplied to the `Points` object from the supplied initial time (`self.time`)
         to a range of times. The number of supplied times must equal the number of point features supplied to the Points object. 
 
         Attributes
@@ -1390,14 +1602,26 @@
                 right_flowline_longitudes = right_lon[:,i]
                 right_flowline_latitudes = right_lat[:,i]
         """
         model = self.plate_reconstruction
         return model.create_flowline(self.lons, self.lats, time_array, left_plate_ID, right_plate_ID, return_rate_of_motion)
 
 
+    def _get_dataframe(self):
+        import geopandas as gpd
+
+        data = dict()
+        data["Longitude"] = self.lons
+        data["Latitude"]  = self.lats
+        data["Plate_ID"]  = self.plate_id
+        for key in self.attributes:
+            data[key] = self.attributes[key]
+
+        return gpd.GeoDataFrame(data)
+
     def save(self, filename):
         """Saves the feature collection used in the Points object under a given filename to the current directory. 
 
         The needed file format to save to is determined from the filename extension. 
 
         Parameters
         ----------
@@ -1406,30 +1630,31 @@
 
         Returns
         -------
         Feature collection saved under given filename to current directory.
         """
         filename = str(filename)
 
-        numpy_types = {'.csv': ',', '.txt': ' ', '.dat': ' '}
-
-        if filename.endswith(tuple(numpy_types.keys())):
-            data = np.c_[self.lons, self.lats, self.plate_id]
-
-            # find appropriate delimiter
-            delimiter = numpy_types[filename[filename.index('.'):]]
-
-            header = "Longitude{0}Latitude{0}Plate_ID".format(delimiter)
-            np.savetxt(filename, data, header=header, delimiter=delimiter, comments='')
+        if filename.endswith(('.csv', '.txt', '.dat')):
+            df = self._get_dataframe()
+            df.to_csv(filename, index=False)
+
+        elif filename.endswith(('.xls', '.xlsx')):
+            df = self._get_dataframe()
+            df.to_excel(filename, index=False)
+
+        elif filename.endswith('xml'):
+            df = self._get_dataframe()
+            df.to_xml(filename, index=False)
 
-        elif filename.endswith('.gpml'):
+        elif filename.endswith('.gpml') or filename.endswith('.gpmlz'):
             self.FeatureCollection.write(filename)
 
         else:
-            raise ValueError("Cannot save to specified file type, use csv or gpml file extension.")
+            raise ValueError("Cannot save to specified file type. Use csv, gpml, or xls file extension.")
 
 
 # FROM RECONSTRUCT_BY_TOPOLOGIES.PY
 class _DefaultCollision(object):
     """
     Default collision detection function class (the function is the '__call__' method).
     """
```

### Comparing `gplately-0.4/gplately/tools.py` & `gplately-1.0/gplately/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,19 +207,19 @@
     try:
         len(plate_ID)
     except TypeError:
         plate_ID = [plate_ID] * len(lons)
 
     # create point features
     point_features = []
-    for lon, lat, id in zip(lons, lats, plate_ID):
+    for lon, lat, pid in zip(lons, lats, plate_ID):
         point_feature = pygplates.Feature()
         point_feature.set_geometry(pygplates.PointOnSphere(float(lat), float(lon)))
-        if id is not None:
-            point_feature.set_reconstruction_plate_id(id)
+        if pid is not None:
+            point_feature.set_reconstruction_plate_id(pid)
         point_features.append(point_feature)
 
     if len(point_features) == 1:
         return point_features[0]
     return point_features
 
 def extract_feature_lonlat(features):
```

### Comparing `gplately-0.4/gplately.egg-info/PKG-INFO` & `gplately-1.0/gplately.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gplately
-Version: 0.4
+Version: 1.0
 Summary: Object-orientated Python interface to pyGPlates for plate tectonic reconstructions
 Home-page: https://github.com/GPlates/gplately
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 License: UNKNOWN
 Description: <p align="center">
         <picture>
@@ -12,14 +12,15 @@
           <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
           <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
         </picture>
         </p>
         
         ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
         ![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+        ![Conda (channel only)](https://img.shields.io/conda/vn/conda-forge/gplately?style=for-the-badge)
         ![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
         
         
         GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
         
         ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
```

### Comparing `gplately-0.4/gplately.egg-info/SOURCES.txt` & `gplately-1.0/gplately.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gplately-0.4/setup.py` & `gplately-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 link_args = []
  
 if "Windows" in platform.system():
     link_args = ["-static"]
 
 # in development set version to none and ...
-PYPI_VERSION = "0.4"  # Note: don't add any dashes if you want to use conda, use b1 not .b1 
+PYPI_VERSION = "1.0"  # Note: don't add any dashes if you want to use conda, use b1 not .b1 
 
 # Return the git revision as a string (from numpy)
 
 def git_version():
     
     def _minimal_ext_cmd(cmd):
         # construct minimal environment
```

### Comparing `gplately-0.4/test/test_0_imports.py` & `gplately-1.0/test/test_0_imports.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/test/test_1_reconstructions.py` & `gplately-1.0/test/test_1_reconstructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 """ 
 A series of automated tests that ensure GPlately's <DataServer> object collects the necessary
 rotation files, topology features and static polygons to initialise the <PlateReconstruction> 
 object with the Müller et al. (2019) plate reconstruction model. The following methods in the 
 object are tested:
 
     - __init__
-    - tesselate_subduction_zones
-    - tesselate_mid_ocean_ridges
+    - tessellate_subduction_zones
+    - tessellate_mid_ocean_ridges
 
     Using pyGPlates and Plate Tectonic Tools:
     - total_subduction_zone_length
     - total_ridge_length
     - total_continental_arc_length
 
     - get_point_velocities
@@ -36,25 +36,25 @@
     6 - length of arc segment (in degrees) that current point is on
     7 - trench normal azimuth angle (clockwise starting at North, ie, 0 to 360 degrees) at current point
     8 - subducting plate ID
     9 - trench plate ID
 """
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_tessellate_trenches(time, model):
-    subduction_data = model.tesselate_subduction_zones(time, ignore_warnings=True)
+    subduction_data = model.tessellate_subduction_zones(time, ignore_warnings=True)
     # CONDITIONS
     assert subduction_data.any(), "There is no trench data inside Muller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(subduction_data[:,0]) <= 180).all(), "Some trench lons exceed a magnitude of 180 degrees in Muller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(subduction_data[:,1]) <= 90).all(), "Some trench lats exceed a magnitude of 90 degrees in Muller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(subduction_data[:,2]) <= 50).all(), "Some trench convergence velocities exceed 20 cm/yr in Muller et al. (2019) at {} Ma.".format(time)
 
 
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_tessellate_ridges(time, model):
-    ridge_data = model.tesselate_mid_ocean_ridges(time, ignore_warnings=False)
+    ridge_data = model.tessellate_mid_ocean_ridges(time, ignore_warnings=False)
     assert ridge_data.any(), "There is no ridge data inside Müller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(ridge_data[:,0]) <= 180).all(), "Some ridge lons exceed a magnitude of 180 degrees in Muller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(ridge_data[:,1]) <= 90).all(), "Some ridge lats exceed a magnitude of 90 degrees in Muller et al. (2019) at {} Ma.".format(time)
     assert (np.abs(ridge_data[:,2]) <= 50).all(), "Some ridge convergence velocities exceed 20 cm/yr in Muller et al. (2019) at {} Ma.".format(time)
 
 
 # TOTAL TRENCH AND RIDGE LENGTHS: PYGPLATES
```

### Comparing `gplately-0.4/test/test_2_points.py` & `gplately-1.0/test/test_2_points.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,12 +33,20 @@
        
 # TESTING PLATE VELOCITY CALCULATIONS
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_plate_velocity(time, gpts):
     plate_vel = gpts.plate_velocity(time, delta_time=1)
     assert plate_vel, "Unable to calculate plate velocities of point data at {} Ma with Muller et al. (2019).".format(time)
 
+def test_point_attributes(gpts):
+    attr = np.arange(0, gpts.size)
+    gpts.add_attributes(FROMAGE=attr, TOAGE=attr)
 
-def test_pickle_Points():
+def test_pickle_Points(gpts):
     import pickle
     gpts_dump = pickle.dumps(gpts)
+    gpts_load = pickle.loads(gpts_dump)
+
+    attr = np.arange(0, gpts.size)
+    gpts.add_attributes(FROMAGE=attr, TOAGE=attr)
+    gpts_dump = pickle.dumps(gpts)
     gpts_load = pickle.loads(gpts_dump)
```

### Comparing `gplately-0.4/test/test_3_plottopologies.py` & `gplately-1.0/test/test_3_plottopologies.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/test/test_4_rasters.py` & `gplately-1.0/test/test_4_rasters.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import gplately
 from conftest import (
     reconstruction_times,
     pt_lon,
     pt_lat,
     gplately_raster_object as graster,
     gplately_merdith_raster,
     gplately_merdith_static_geometries,
@@ -32,14 +33,41 @@
         pt_lat,
         method='linear',
         return_indices=False,
     )
     assert interpolated_points.any(), "Unable to interpolate points"
 
 
+def test_bilinear_interpolation():
+    array = np.array([[0,1],[1,2]], dtype=float)
+    graster = gplately.Raster(data=array, extent=[0,1,0,1])
+
+    ilon = ilat = 2.0/3
+    result = 1.0 + 1.0/3
+    interp = graster.interpolate(ilon, ilat, method="linear")
+    assert np.isclose(interp, result), "Linear interpolation in x direction failed"
+
+    # get interpolation coordinates
+    interp, (ci,cj) = graster.interpolate(ilon, ilat, method="linear", return_indices=True)
+    assert ci == 1 and cj == 1, "Indices of interpolation are incorrect"
+
+def test_nearest_neighbour_interpolation():
+    array = np.array([[0,1],[1,2]], dtype=float)
+    graster = gplately.Raster(data=array, extent=[0,1,0,1])
+
+    ilon = ilat = 2.0/3
+    result = 2
+    interp = graster.interpolate(ilon, ilat, method="nearest")
+    assert np.isclose(interp, result), "Linear interpolation in x direction failed"
+
+    # get interpolation coordinates
+    interp, (ci,cj) = graster.interpolate(ilon, ilat, method="nearest", return_indices=True)
+    assert ci == 1 and cj == 1, "Indices of interpolation are incorrect"    
+
+
 # TEST AGE GRID RESIZING (AT RESOLUTIONS OF RES_X = 1000, RES_Y = 400)
 def test_resizing(graster):
     resized_agegrid = graster.resize(1000, 400, return_array=True)
     assert np.shape(resized_agegrid)==(400,1000), "Unable to rezise"
 
 
 # TEST FILLING NaNs IN AGE GRIDS
```

### Comparing `gplately-0.4/test/test_5_seafloorgrid.py` & `gplately-1.0/test/test_5_seafloorgrid.py`

 * *Files identical despite different names*

### Comparing `gplately-0.4/test/test_6_geometry.py` & `gplately-1.0/test/test_6_geometry.py`

 * *Files identical despite different names*

