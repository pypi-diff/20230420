# Comparing `tmp/EclipsingBinaries-2.8.3.tar.gz` & `tmp/EclipsingBinaries-2.8.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.3.tar", last modified: Thu Apr  6 03:14:20 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a2.tar", last modified: Thu Apr 20 19:20:35 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.3.tar` & `EclipsingBinaries-2.8.4a2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    17229 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/color_light_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/tesscut.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-06 03:14:20.000000 EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:14:20.068507 EclipsingBinaries-2.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-06 03:14:04.000000 EclipsingBinaries-2.8.3/tests/test_OC_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.089782 EclipsingBinaries-2.8.4a2/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17137 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/color_light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23469 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/tesscut.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.089782 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-20 19:20:35.000000 EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-20 19:20:11.000000 EclipsingBinaries-2.8.4a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-20 19:20:16.000000 EclipsingBinaries-2.8.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:20:35.093782 EclipsingBinaries-2.8.4a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-20 19:20:16.000000 EclipsingBinaries-2.8.4a2/tests/test_OC_plot.py
```

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,98 @@
 """
 Author: Kyle Koeller
 Created: 11/08/2022
-Last Edited: 04/05/2023
+Last Edited: 04/17/2023
 
 This program is meant to automatically do the data reduction of the raw images from the
 Ball State University Observatory (BSUO) and SARA data. The new calibrated images are placed into a new folder as to
 not overwrite the original images.
 """
 # import sys
 from pathlib import Path
 import time
 import warnings
 
 from astropy import wcs
 from astropy.stats import mad_std
 from astropy import units as u
+from astropy.nddata import CCDData
+from astropy.io import fits
+from astropy.time import Time
+from astropy.coordinates import SkyCoord, EarthLocation
+
 import ccdproc as ccdp
 import numpy as np
-from astropy.nddata import CCDData
 import matplotlib.pyplot as plt
 
 # turn off this warning that just tells the user,
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 # global variables for combining, to either play with or set depending on the run
 sigma_clip_low_thresh = None
 sigma_clip_high_thresh = 3
 sigclip = 5  # sigclip for cosmic ray removal
 rdnoise = 10.83  # * u.electron  # gathered from fits headers manually
-gain = 1.43  # * (u.electron / u.adu)  # gathered from fits headers manually
+gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
 overwrite = True  # if the user wants to overwrite already existing files or not, by default it is set to True
-mem_limit = 450e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
+mem_limit = 1600e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
 dark_bool = "True"
+location = "bsuo"
 
 
 def main():
     """
     This function calls all other functions in order of the calibration.
 
     :return: outputs all calibration images into a new reduced folder designated by the user.
     """
 
     # allows the user to input where the raw images are and where the calibrated images go to
     path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the raw images are or type "
                  "the word 'Close' to leave: ")
+    # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration2"
     if path.lower() == "close":
         exit()
     # path = "Calibration2"
     calibrated = input("Please enter a file pathway for a new calibrated folder to not overwrite the original images "
-                       "(C:\\folder1\\folder2\\[calibrated]): ")
-
+                        "(C:\\folder1\\folder2\\[calibrated]): ")
+    # calibrated = "C:\\test"
     # checks whether the file paths from above are real
     while True:
         try:
             images_path = Path(path)
             calibrated_data = Path(calibrated)
             break
         except FileNotFoundError:
             print("Files were not found. Please try again.\n")
             path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
             calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
-    print("\nDo you want to load default options like gain and readnoise? The defaults are for BSUO")
+    print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
     while True:
-        default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
+        # default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
+        default_ans = "default"
         if default_ans.lower() == "default":
             break
         elif default_ans.lower() == "new":
             default()
             break
         else:
-            print("Please either enter 'Default' or 'New'\n.")
+            print("Please either enter 'Default' or 'New'.\n")
 
     calibrated_data.mkdir(exist_ok=True)
     files = ccdp.ImageFileCollection(images_path)
 
     zero, overscan_region, trim_region = bias(files, calibrated_data, path)
     if not dark_bool:
         master_dark = None
     else:
         master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
+
     flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
     science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
 
 
 def default():
     """
     Generates new values that the user can enter
@@ -93,14 +101,15 @@
     """
     global sigma_clip_high_thresh
     global sigma_clip_low_thresh
     global gain
     global rdnoise
     global sigclip
     global dark_bool
+    global location
 
     sigma_clip_low_thresh = (input("\nEnter a sigma clip low threshold, default is 'None': "))
     if sigma_clip_low_thresh.lower() == "none":
         sigma_clip_low_thresh = None
     else:
         sigma_clip_low_thresh = int(sigma_clip_high_thresh)
     sigma_clip_high_thresh = int(input("Enter a sigma clip high threshold, default is '3': "))
@@ -108,14 +117,15 @@
     rdnoise = float(input("Enter a readnoise value, default is '10.83' electrons: "))
     sigclip = int(input("Enter a sigma clip value for cosmic ray removal, default is '5': "))
     dark_bool = input("Are you using Dark Frames, default is True (enter 'True' or 'False'): ")
     if dark_bool.lower == "false":
         dark_bool = False
     elif dark_bool.lower == "true":
         dark_bool = True
+    location = input("What is your observation location, default is bsuo (ctip, kpno, lapalma")
 
 
 def reduce(ccd, overscan_region, trim_region, num, zero, combined_dark, good_flat):
     """
     This function takes the information for each section of the reduction process into a singular function for
     limits in duplication of the code.
 
@@ -124,130 +134,149 @@
     :param trim_region: region of the image to trim
     :param num: tells the program what stage of the process it is in
     :param zero: master bias
     :param combined_dark: master dark
     :param good_flat: master flat
     :return: depends on the stage of process, but will return a final image for each process
     """
-    # Subtract the overscan, ccd[columns, rows] I think?
+
+    # subtract overscan, trims image, and gain corrects
     if overscan_region.lower() == "none":
         pass
     else:
-        ccd = ccdp.subtract_overscan(ccd, fits_section=overscan_region, median=True, overscan_axis=1)
+        new_ccd = ccdp.ccd_process(ccd, oscan=overscan_region, trim=trim_region, gain=gain * u.electron / u.adu,
+                                   readnoise=rdnoise * u.electron, error=False)
+        # ccd = ccdp.subtract_overscan(ccd, fits_section=overscan_region, median=True, overscan_axis=None)
 
-    # Trim the overscan and gain correct the image
-    ccd = ccdp.trim_image(ccd, fits_section=trim_region)
-    new_ccd = ccdp.gain_correct(ccd, gain=gain)  # gain correct the image
+    # Subtract the overscan, ccd[columns, rows] I think?
+    # # Trim the overscan and gain correct the image
+    # while True:
+    #     try:
+    #         ccd = ccdp.trim_image(ccd, fits_section=trim_region)
+    #         break
+    #     except ValueError:
+    #         print("You have entered the wrong format for the Data Section. Please try again.\n")
+    #         trim_region = input("Please enter the data region. Example '[20:2060, 12:2057]': ")
+    #
+    # new_ccd = ccdp.gain_correct(ccd, gain=gain * u.electron / u.adu)  # gain correct the image
 
     # this if statement checks whether the input is bias, dark, flat, or science reduction
     # bias combining
     if num == 0:
         return new_ccd
     # dark combining
     elif num == 1:
+        # print(new_ccd.unit, zero.unit)
         # Subtract bias
         sub_ccd = ccdp.subtract_bias(new_ccd, zero)
 
         return sub_ccd
     # flat combining
     elif num == 2:
+        # print(new_ccd.unit, zero.unit)
         # Subtract bias
         sub_ccd = ccdp.subtract_bias(new_ccd, zero)
 
         # Subtract the dark current
         if not dark_bool:
             final_ccd = sub_ccd
         else:
             final_ccd = ccdp.subtract_dark(sub_ccd, combined_dark, exposure_time='exptime', exposure_unit=u.second,
                                            scale=True)
         return final_ccd
     # science calibration
     elif num == 3:
         # Subtract bias
-        sub_ccd = ccdp.subtract_bias(new_ccd, zero)
-
+        if location.lower() == "bsuo":
+            sub_ccd = ccdp.subtract_bias(new_ccd, zero)
+        else:
+            sub_ccd = ccdp.subtract_bias(new_ccd, zero)
         # Subtract the dark current
         if not dark_bool:
             reduced = sub_ccd
         else:
             reduced = ccdp.subtract_dark(sub_ccd, combined_dark, exposure_time='exptime', exposure_unit=u.second,
                                          scale=True)
         # flat field correct the science image based on filter
         reduced = ccdp.flat_correct(ccd=reduced, flat=good_flat, min_value=1.0)
 
         # cosmic ray reject above 5 sigmas and gain_apply is set to false because it changes the units of the image
-        new_reduced = ccdp.cosmicray_lacosmic(reduced, gain_apply=False, readnoise=rdnoise, gain=gain, sigclip=sigclip)
+        # new_reduced = ccdp.cosmicray_lacosmic(reduced, gain_apply=False, readnoise=rdnoise, gain=gain, sigclip=sigclip)
 
-        return new_reduced
+        return reduced
 
 
 def bias(files, calibrated_data, path):
     """
     Calibrates the bias images
 
     :param path: the raw images folder path
     :param files: file location where all raw images are
     :param calibrated_data: file location where the new images go
     :return: the combined bias image and the trim and overscan regions
     """
 
     # plots one of the flat image mean count values across all columns to find the trim and overscan regions
     print("\n\nThe flat image that you enter next should be inside the " + "\033[1m" + "\033[93m" + "FIRST" +
-          "\033[00m" + " folder that you entered above or this will crash.\n")
+          "\033[00m" + " folder that you entered above or this will crash.")
     while True:
         try:
             image = input(
-                "Please enter the name of one of the flat image to be looked at for overscan and trim regions: ")
+                "Please enter the name of one of the flat image to be looked at for overscan and data regions: ")
             cryo_path = Path(path)
             bias_1 = CCDData.read(cryo_path / image, unit='adu')
             break
         except FileNotFoundError:
             print("\nThe file you entered could not be found, please try entering " 
                   "\033[1m" + "\033[93m" + "JUST" + "\033[00m" + " the file name only.\n")
     # bias_1 = CCDData.read(cryo_path / 'bias-0001.fits', unit='adu')  # testing
 
-    print("\n\nFor the overscan region, [rows, columns], and if you want all the columns then you want would enter, \n"
+    print("\n\nFor the overscan region, [columns, rows], and if you want all the columns then you want would enter, \n"
           "[1234:5678, 1234:5678] and this would say rows between those values and all the columns. \n"
-          "This would also work if you wanted all the rows ([: , 1234:5678]).\n")
+          "This would also work if you wanted all the columns ([: , 1234:5678]).\n")
     bias_plot(bias_1)
 
     overscan_region = input("Please enter the overscan region you determined from the figure.\n"
                             "Example '[2073:2115, :]' or if you do not have an overscan region enter 'None': ")
-    trim_region = input("Please enter the trim region. Example '[20:2060, 12:2057]': ")
+    trim_region = input("Please enter the data section. Example '[20:2060, 12:2057]': ")
     print()
 
     print("\nStarting overscan on bias.\n")
     for ccd, file_name in files.ccds(imagetyp='BIAS', return_fname=True, ccd_kwargs={'unit': 'adu'}):
         new_ccd = reduce(ccd, overscan_region, trim_region, 0, zero=None, combined_dark=None, good_flat=None)
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
-        # new_fname = "bias_o_{}.fits".format(list_of_words[3])
-        # new_fname = "bias_o_{}.fits".format(list_of_words[1])  # testing
+
         # Save the result
         new_ccd.write(calibrated_data / new_fname, overwrite=overwrite)
 
+        add_header(calibrated_data, new_fname, "BIAS", "None", None, None, None)
+
         # output that an image is finished for updates to the user
         print("Finished overscan correction for " + str(new_fname))
 
     print("\nFinished overscan correcting bias frames.")
     # combine all the output bias images into a master bias
     reduced_images = ccdp.ImageFileCollection(calibrated_data)
     calibrated_biases = reduced_images.files_filtered(imagetyp='BIAS', include_path=True)
 
     combined_bias = ccdp.combine(calibrated_biases,
                                  method='average',
                                  sigma_clip=True, sigma_clip_low_thresh=sigma_clip_low_thresh,
                                  sigma_clip_high_thresh=sigma_clip_high_thresh,
                                  sigma_clip_func=np.ma.median, signma_clip_dev_func=mad_std,
-                                 mem_limit=450e6
+                                 mem_limit=mem_limit
                                  )
 
+    fname = "zero.fits"
     combined_bias.meta['combined'] = True
-    combined_bias.write(calibrated_data / 'zero.fits', overwrite=overwrite)
+    combined_bias.write(calibrated_data / fname, overwrite=overwrite)
+
+    add_header(calibrated_data, fname, "BIAS", "None", None, None, None)
 
     print("\nFinished creating zero.fits\n")
 
     return combined_bias, overscan_region, trim_region
 
 
 def bias_plot(ccd):
@@ -285,36 +314,42 @@
     # calibrating a combining the dark frames
     for ccd, file_name in files.ccds(imagetyp='DARK', ccd_kwargs={'unit': 'adu'}, return_fname=True):
         sub_ccd = reduce(ccd, overscan_region, trim_region, 1, zero, combined_dark=None, good_flat=None)
 
         # new file name that uses the number from the original image
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
-        # new_fname = "dark_o_b_{}.fits".format(list_of_words[3])
+
         # Save the result
         sub_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
+        add_header(calibrated_path, new_fname, "DARK", "None", None, None, None)
+
         print("Finished overscan correction and bias subtraction for " + str(new_fname))
 
     print("\nFinished overscan correcting and bias subtracting all dark frames.")
     print("\nStarting combining dark frames.\n")
     time.sleep(10)
     reduced_images = ccdp.ImageFileCollection(calibrated_path)
     calibrated_darks = reduced_images.files_filtered(imagetyp='dark', include_path=True)
 
     combined_dark = ccdp.combine(calibrated_darks,
                                  method='average',
                                  sigma_clip=True, sigma_clip_low_thresh=sigma_clip_low_thresh,
                                  sigma_clip_high_thresh=sigma_clip_high_thresh,
                                  sigma_clip_func=np.ma.median, signma_clip_dev_func=mad_std,
-                                 rdnoise=rdnoise, gain=gain, mem_limit=450e6
+                                 rdnoise=rdnoise * u.electron, gain=gain * u.electron / u.adu, mem_limit=mem_limit
                                  )
 
+    fname = "master_dark.fits"
     combined_dark.meta['combined'] = True
-    combined_dark.write(calibrated_path / 'master_dark.fits', overwrite=overwrite)
+    combined_dark.write(calibrated_path / fname, overwrite=overwrite)
+
+    add_header(calibrated_path, fname, "DARK", "None", None, None, None)
+
     print("Finished creating a master dark.\n")
     return combined_dark
 
 
 def flat(files, zero, combined_dark, calibrated_path, overscan_region, trim_region):
     """
     Calibrate flat images.
@@ -324,79 +359,150 @@
     :param combined_dark: combined bias image
     :param calibrated_path: file location for new images
     :param trim_region: trim region for images
     :param overscan_region: overscan region for images
     :return: master flat files in each filter
     """
     print("Starting flat calibration.\n")
-    print()
 
     # calibrating and combining the flat frames
     for ccd, file_name in files.ccds(imagetyp='FLAT', return_fname=True, ccd_kwargs={'unit': 'adu'}):
         final_ccd = reduce(ccd, overscan_region, trim_region, 2, zero, combined_dark, good_flat=None)
 
         # new file name with the filter and number from the original file
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
-        # new_fname = "flat_o_b_d_{}{}.fits".format(list_of_words[2], list_of_words[4])
-        # new_fname = "flat_o_b_d_{}_{}.fits".format(list_of_words[1], list_of_words[0])  # testing
 
         # Save the result
         final_ccd.write(calibrated_path / new_fname, overwrite=overwrite)
 
+        add_header(calibrated_path, new_fname, "FLAT", "None", None, None, None)
+
         print("Finished overscan correction, bias subtraction, and dark subtraction for " + str(new_fname))
 
     print("\nFinished overscan, bias subtracting, and dark subtracting of flat frames.\n")
     print("Starting flat combination.\n")
     time.sleep(10)
 
     ifc = ccdp.ImageFileCollection(calibrated_path)
     flat_filters = set(h['FILTER'] for h in ifc.headers(imagetyp="FLAT"))
     for filt in flat_filters:
         to_combine = ifc.files_filtered(imagetyp="flat", filter=filt, include_path=True)
         combined_flats = ccdp.combine(to_combine,
-                                      method='average',
+                                      method='median',
                                       sigma_clip_high_thresh=sigma_clip_high_thresh,
                                       sigma_clip_func=np.ma.median, signma_clip_dev_func=mad_std,
-                                      rdnoise=rdnoise, gain=gain, mem_limit=450e6
+                                      rdnoise=rdnoise * u.electron, gain=gain * u.electron / u.adu,
+                                      mem_limit=mem_limit
                                       )
 
         combined_flats.meta['combined'] = True
         flat_file_name = 'master_flat_{}.fits'.format(filt.replace("Empty/", ""))
 
         combined_flats.write(calibrated_path / flat_file_name, overwrite=overwrite)
 
+        add_header(calibrated_path, flat_file_name, "FLAT", "None", None, None, None)
+
         print("Finished combining flat " + str(flat_file_name))
 
     print("\nFinished creating the master flats by filter.\n")
 
-    return combined_flats
-
 
 def science_images(files, calibrated_data, zero, combined_dark, trim_region, overscan_region):
     all_reds = []
     science_imagetyp = 'LIGHT'
     flat_imagetyp = 'FLAT'
 
     ifc_reduced = ccdp.ImageFileCollection(calibrated_data)
     combined_flats = {ccd.header['filter']: ccd for ccd in ifc_reduced.ccds(imagetyp=flat_imagetyp, combined=True)}
 
     print("Starting reduction of science images.\n")
 
-    for light, file_name in files.ccds(imagetyp=science_imagetyp, return_fname=True, ccd_kwargs={'unit': 'electron'}):
+    for light, file_name in files.ccds(imagetyp=science_imagetyp, return_fname=True, ccd_kwargs={'unit': 'adu'}):
         good_flat = combined_flats[light.header['filter']]
         reduced = reduce(light, overscan_region, trim_region, 3, zero, combined_dark, good_flat)
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
-        # new_fname = "{}_o_b_d_f_{}_{}_{}.fits".format(list_of_words[0], list_of_words[2], list_of_words[5], list_of_words[6].replace(".fts", ""))
-        # new_fname = "{}_o_b_d_{}.fits".format(list_of_words[0], list_of_words[1])  # testing
 
         all_reds.append(reduced)
         reduced.write(calibrated_data / new_fname, overwrite=overwrite)
 
+        hjd = light.header["JD-HELIO"]
+        ra = light.header["RA"]
+        dec = light.header["DEC"]
+
+        add_header(calibrated_data, new_fname, science_imagetyp, "None", hjd, ra, dec)
+
         print("Finished calibration of " + str(new_fname))
     print("\nFinished calibrating all science images.")
 
 
+def add_header(pathway, fname, imagetyp, filter_name, hjd, ra, dec):
+    """
+    Adds values to the header of each image reduced
+
+    :param dec: declination of target object
+    :param ra: right ascension of target object
+    :param hjd: time of mid-exposure for each image
+    :param pathway: pathway to the new file
+    :param fname: file name
+    :param imagetyp: image type (bias, flat, dark, light)
+    :param filter_name: filter type (B, V, R)
+    :return: None
+    """
+    # bias_image = get_pkg_data_filename(pathway + "\\" + fname)
+    image_name = pathway / fname
+    fits.setval(image_name, "GAIN", value=gain, comment="Units of e-/ADU")
+    fits.setval(image_name, "RDNOISE", value=rdnoise, comment="UNits of e-")
+    fits.setval(image_name, "OBSERVAT", value=location, comment="Obs. loc.")
+    fits.setval(image_name, "IMAGETYP", value=imagetyp, comment="Image type")
+    # BIASSEC
+    # DATASEC
+    # EPOCH
+    # fits.setval(bias_image, "FILTER", value=filter_name)
+    if imagetyp == "LIGHT":
+        bjd = BJD_TDB(hjd, location, ra, dec)
+        fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
+
+
+def BJD_TDB(hjd, loc, ra, dec):
+    """
+    Converts HJD to BJD_TDB
+
+    :param ra: right ascension of target object
+    :param dec: declination of target object
+    :param hjd: HJD time for the mid-exposure image
+    :param loc: location of the observations
+    :return: Newly calculated BJD_TDB that is light time corrected
+    """
+    # Define the HJD time in JD format
+    hjd = hjd * u.day
+
+    # Convert HJD to TDB
+    if loc.lower() == "ctio" or loc.lower() == "kpno" or loc.lower() == "lapalma":
+        t = Time(hjd.value, format='jd', scale='utc', location=loc)
+        t = t.tdb
+        # obs_location = EarthLocation.from_geodetic(obs_longitude, obs_latitude, obs_height)
+    elif loc.lower() == "bsuo":
+        # Define the location of the Ball State University Observatory (BSUO)
+        obs_latitude = 40.199910 * u.deg  # lat of the BSUO site
+        obs_longitude = -85.411513 * u.deg  # long of the BSUO site
+        obs_height = 292 * u.m  # height above sea level of the BSUO site
+        obs_location = EarthLocation.from_geodetic(obs_longitude, obs_latitude, obs_height)
+        t = Time(hjd, format='jd', scale='utc', location=obs_location)
+        t = t.tdb
+    else:
+        pass
+
+    # Compute the light travel time from the target to the observer
+    coord = SkyCoord(ra=ra, dec=dec, unit=(u.h, u.deg), obstime=t, frame='icrs')
+
+    ltt = Time.light_travel_time(coord, obs_location, kind='barycentric')
+    bjd_corr = t + ltt
+
+    # bjd_tdb_time = t
+    return bjd_corr
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/tess_data_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Look up the TESS data and download that data onto a local drive.
 Author: Kyle Koeller
 Created: 2/19/2022
-Last Updated: 03/23/2023
+Last Updated: 04/20/2023
 """
 
 # import required packages
 import astroquery.exceptions
 from astroquery.mast import Tesscut
-import astropy.units as u
-from .tesscut import main as tCut
-# from tesscut import main as tCut  # testing purposes
+# from .tesscut import main as tCut
+from tesscut import main as tCut  # testing purposes
 from os.path import exists
+import pandas as pd
+
+from astropy import units as u
 
 
 def main():
     """
     This function allows the user to enter a TIC ID to be entered, and it also makes sure that number is valid or exists.
     This program will also list off the sector data to be downloaded for cross-referencing if needed.
     :return: Downloaded pixel data in the form of .fits files to be extracted later
@@ -31,16 +33,54 @@
             break
         except astroquery.exceptions.ResolverError:
             print("\nThe TIC number you entered is invalid or there is no data for this given system.\n")
 
     if system_name.lower() == "close":
         exit()
 
+    dc = pd.read_csv("tess_ccd_info.txt", header=None, sep="\t", skiprows=[0])
+
+    gain = dc[6]  # gain for the individual camera/ccd
+    tess_camera = dc[0]  # camera number
+    tess_ccd = dc[1]  # ccd number
+    # slice = dc[2]  # could be used in the future
+
+    sector_camera = []
+    sector_ccd = []
+    for count, val in enumerate(sector_table["camera"]):
+        sector_camera.append(val)
+        sector_ccd.append(sector_table["ccd"][count])
+
+    # create a tuple form of the sector and TESS camera/ccd data
+    list_gain = []
+    a = list(zip(tess_camera, tess_ccd))  # tess cam and ccd's
+    b = list(zip(sector_camera, sector_ccd))  # sect cam and ccd's
+
+    # compare the TESS and sector information
+    for _, sect in enumerate(b):
+        for y, tess in enumerate(a):
+            if sect == tess:
+                list_gain.append(gain[y])
+
+    # splits up list_gain into lists by every 1, 2, 3, or 4th value since there are 4 slices for each camera and ccd
+    A = list_gain[::4]
+    B = list_gain[1::4]
+    C = list_gain[2::4]
+    D = list_gain[3::4]
+
+    # append the gain values to the sector table list
+    sector_table.add_column(A, name="A gain")
+    sector_table.add_column(B, name="B gain")
+    sector_table.add_column(C, name="C gain")
+    sector_table.add_column(D, name="D gain")
+
+    # sector_table.add_columns(["Gain"])
     # prints off the sector table to let the user know what sectors TESS has observed the object
     while True:
+        print("\n The read noise for the cameras is between 7-11 electrons/pixel.")
         print(sector_table)
         print("\nDo you want to download " + "\033[1m" + "\033[93m" + "ALL" + "\033[00m" +
               " the TESS data?")
         download_ans = input("Type 'Yes' to download all Sector data or type 'No' to specify a sector that you want. "
                              "Or type 'Close' to leave: ")
         # prints the word 'ALL' in bold '\033[1m' and in yellow '\033[93m' must return to normal with '\033[0m'
         if download_ans.lower() == "yes":
@@ -51,16 +91,16 @@
             for i in sector_table["sector"]:
                 download(system_name, i)
                 print("\nFinished downloading Sector " + str(i))
         elif download_ans.lower() == "no":
             sector_num = int(input("Which Sector would you like to download: "))
             download(system_name, sector_num)
         elif download_ans.lower() == 'close':
-            print("The program will not exit.\n")
-            exit()
+            print("The program will now exit.\n")
+            break
         else:
             print("\nPlease enter 'Yes' or 'No' only.\n")
 
     print("Finished downloading all sector data related to " + system_name + "\n")
 
 
 def download(system_name, i):
```

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.3
+Version: 2.8.4a2
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.3/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a2/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,9 +16,8 @@
 EclipsingBinaries/vseq_updated.py
 EclipsingBinaries.egg-info/PKG-INFO
 EclipsingBinaries.egg-info/SOURCES.txt
 EclipsingBinaries.egg-info/dependency_links.txt
 EclipsingBinaries.egg-info/entry_points.txt
 EclipsingBinaries.egg-info/requires.txt
 EclipsingBinaries.egg-info/top_level.txt
-tests/__init__.py
 tests/test_OC_plot.py
```

### Comparing `EclipsingBinaries-2.8.3/LICENSE` & `EclipsingBinaries-2.8.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/PKG-INFO` & `EclipsingBinaries-2.8.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.3
+Version: 2.8.4a2
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.3/README.md` & `EclipsingBinaries-2.8.4a2/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.3/setup.py` & `EclipsingBinaries-2.8.4a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     name="EclipsingBinaries",
     description="Binary Star Package for Ball State University's Astronomy Research Group",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kjkoeller/EclipsingBinaries',
     author='Kyle Koeller',
 
-    packages=find_packages(),
+    # packages=find_packages(),
 
     entry_points={'console_scripts': [
         'EclipsingBinaries = EclipsingBinaries.menu:main'
     ],
     },
 
     license="MIT",
@@ -84,12 +84,15 @@
     extras_require={
         'testing': [
             'pytest>=7.2.2',
         ],
     },
 
     include_package_data=True,
+    packages=['EclipsingBinaries'],
+    package_dir={'EclipsingBinaries': 'EclipsingBinaries'},
     package_data={
         'EclipsingBinaries': ['tests/*'],
+        'EclipsingBinaries': ['examples/*'],
     },
 
 )
```

### Comparing `EclipsingBinaries-2.8.3/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a2/tests/test_OC_plot.py`

 * *Files identical despite different names*

