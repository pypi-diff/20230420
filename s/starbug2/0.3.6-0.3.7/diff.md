# Comparing `tmp/starbug2-0.3.6.tar.gz` & `tmp/starbug2-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.3.6.tar", last modified: Thu Apr  6 11:40:12 2023, max compression
+gzip compressed data, was "starbug2-0.3.7.tar", last modified: Thu Apr 20 10:28:36 2023, max compression
```

## Comparing `starbug2-0.3.6.tar` & `starbug2-0.3.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-06 11:39:57.000000 starbug2-0.3.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 11:39:57.000000 starbug2-0.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-06 11:39:57.000000 starbug2-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-06 11:40:12.725770 starbug2-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-06 11:39:57.000000 starbug2-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2023-04-06 11:39:57.000000 starbug2-0.3.6/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-06 11:39:57.000000 starbug2-0.3.6/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-06 11:39:57.000000 starbug2-0.3.6/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 11:39:57.000000 starbug2-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-06 11:40:12.725770 starbug2-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-06 11:39:57.000000 starbug2-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    28078 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-06 11:39:57.000000 starbug2-0.3.6/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-06 11:40:12.000000 starbug2-0.3.6/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-06 11:40:12.000000 starbug2-0.3.6/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 11:40:12.000000 starbug2-0.3.6/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-06 11:40:12.000000 starbug2-0.3.6/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 11:40:12.000000 starbug2-0.3.6/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 11:40:12.725770 starbug2-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-06 11:39:57.000000 starbug2-0.3.6/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-06 11:39:57.000000 starbug2-0.3.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.088748 starbug2-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-20 10:28:21.000000 starbug2-0.3.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 10:28:21.000000 starbug2-0.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 10:28:21.000000 starbug2-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 10:28:36.088748 starbug2-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-20 10:28:21.000000 starbug2-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.084748 starbug2-0.3.7/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10896 2023-04-20 10:28:21.000000 starbug2-0.3.7/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-20 10:28:21.000000 starbug2-0.3.7/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.084748 starbug2-0.3.7/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-20 10:28:21.000000 starbug2-0.3.7/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 10:28:21.000000 starbug2-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-20 10:28:36.088748 starbug2-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 10:28:21.000000 starbug2-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.084748 starbug2-0.3.7/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14164 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.088748 starbug2-0.3.7/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28295 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-20 10:28:21.000000 starbug2-0.3.7/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.088748 starbug2-0.3.7/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 10:28:36.000000 starbug2-0.3.7/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-20 10:28:36.000000 starbug2-0.3.7/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:28:36.000000 starbug2-0.3.7/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 10:28:36.000000 starbug2-0.3.7/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 10:28:36.000000 starbug2-0.3.7/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:28:36.088748 starbug2-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-20 10:28:21.000000 starbug2-0.3.7/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-20 10:28:21.000000 starbug2-0.3.7/tests/test_utils.py
```

### Comparing `starbug2-0.3.6/LICENSE.txt` & `starbug2-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/PKG-INFO` & `starbug2-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.6
+Version: 0.3.7
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
@@ -88,9 +88,10 @@
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-
-
+* findpeaks on convl method
+* rickerwavelet radius
+* psf dither match dropping apMag
```

### Comparing `starbug2-0.3.6/README.md` & `starbug2-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,9 +79,10 @@
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-
-
+* findpeaks on convl method
+* rickerwavelet radius
+* psf dither match dropping apMag
```

### Comparing `starbug2-0.3.6/bin/starbug2` & `starbug2-0.3.7/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/bin/starbug2-match` & `starbug2-0.3.7/bin/starbug2-match`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/extras/starbug2.completion` & `starbug2-0.3.7/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/starbug2/__init__.py` & `starbug2-0.3.7/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/starbug2/matching.py` & `starbug2-0.3.7/starbug2/matching.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/starbug2/misc.py` & `starbug2-0.3.7/starbug2/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,14 @@
     INPUT: fname=local file to update
     """
     default_fname="%s/default.param"%pkg_resources.resource_filename("starbug2","param/")
     default_param=load_params(default_fname)
     current_param=load_params(fname)
 
     if default_fname==fname:
-        #perror("cannot change default parameter file")
         return 
 
     if os.path.exists(fname):
         printf("Updating \"%s\"\n"%fname)
         fpi=open(fname, 'r')
         fpd=open(default_fname, 'r')
         fpo=open("/tmp/starbug.param",'w')
@@ -154,12 +153,14 @@
             key=key.strip().rstrip()
 
             if key not in add_keys:
                 value=current_param[key]
 
             outline="%-24s"%("%-12s"%key+"= "+str(value))+" //"+comment+"\n"
             fpo.write(outline)
-
+        fpi.close()
+        fpo.close()
+        fpd.close()
         os.system("mv /tmp/starbug.param %s"%fname)
     else: perror("local parameter file '%s' does not exist\n"%fname)
```

### Comparing `starbug2-0.3.6/starbug2/param/default.param` & `starbug2-0.3.7/starbug2/param/default.param`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 BOX_SIZE	=2    // (int>0) Background estimation kernal size (pix)
 DOBGD2D     =1    // Run background2D estimation (usually finds more sources but takes time)
 CLEANSRC    =1    // Run source cleaning after detection (removes likely contaminants)
 SHARP_LO    = 0.4 // cutoff in detection
 SHARP_HI    = 0.9 // cutoff in detection
 ROUND_LO    =-1.0 // cutoff in detection
 ROUND_HI    = 1.0 // cutoff in detection
+RICKER_R    = 1.0 // Radius (pix) of ricker wavelet 
 
 ## APERTURE PHOTOMOETRY
 APPHOT_R    =1.5   //Radius in number of pixels
 ENCENERGY	=0.5   //Fraction encircled energy (mutually exclusive with APPHOT_R)
 FIT_APP_R	=1	   //Fit APPHOT_R to the aperture correction CRDS (if =0, use ENCENRGY instead)
 SKY_RIN     =3     //Sky annulus inner radius
 SKY_ROUT    =4.5   //Sky annulus outer radius
```

### Comparing `starbug2-0.3.6/starbug2/routines.py` & `starbug2-0.3.7/starbug2/routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from scipy.stats import norm#, mode
 from scipy.optimize import curve_fit
 from scipy.ndimage import convolve
 from skimage.feature import match_template
 
 from astropy.stats import sigma_clipped_stats, sigma_clip
 from astropy.coordinates import SkyCoord
-from astropy.table import Column, Table, QTable, hstack
+from astropy.table import Column, Table, QTable, hstack, vstack
 from astropy.modeling.fitting import LevMarLSQFitter
 from astropy.convolution import RickerWavelet2DKernel
 
 from photutils.background import Background2D, BackgroundBase
 from photutils.aperture import CircularAperture, CircularAnnulus, aperture_photometry
-from photutils.detection import StarFinderBase, DAOStarFinder
+from photutils.detection import StarFinderBase, DAOStarFinder, find_peaks
 from photutils.psf.groupstars import DAOGroup
 from photutils.psf import BasicPSFPhotometry
 
 from photutils.datasets import make_model_sources_image, make_random_models_table
 from starbug2.utils import loading, printf, perror, warn
 from starbug2 import *
 
@@ -33,51 +33,57 @@
     A standalone detection that runs on a 2D image.
     It uses DAOStarFinder as the base for peak detection but run
     several times on a series of background subtracted images.
     Each run the background subtraction is differemt, bringing out a
     different set of sources
     """
     def __init__(self,  sig_src=5, sig_sky=3, fwhm=1,
-                        sharplo=0.2, sharphi=1, roundlo=-1, roundhi=1,
+                        sharplo=0.2, sharphi=1, roundlo=-1, roundhi=1, ricker_r=1.0,
                         verbose=0, cleansrc=1, bgd2d=1, boxsize=2):
         self.sig_src=sig_src
         self.sig_sky=sig_sky
         self.fwhm = fwhm
         self.sharphi=sharphi
         self.sharplo=sharplo
         self.roundhi=roundhi
         self.roundlo=roundlo
+        self.ricker_r=ricker_r
         self.cleansrc=cleansrc
 
         #self.match_threshold=u.Quantity(match_threshold)*u.dimensionless_unscaled
         self.catalogue=Table()
         self.verbose=verbose
 
         self.bgd2d=bgd2d
         self.boxsize=boxsize
         #self.filtersize=filtersize
 
-    def detect(self, data, bkg_estimator=None, xycoords=None):
+    def detect(self, data, bkg_estimator=None, xycoords=None, method=None):
         """
         The core detection step (DAOStarFinder
         INPUT:  
                 data=array to detect on
                 bkg_estimator=background array the same shape as data array
                 xycorrds= table of initial guesses (xcentroid,ycentroid)
         RETURNS:
                 Sourcelist Table
         """
         bkg=np.zeros(data.shape)
         if bkg_estimator:
             bkg=bkg_estimator(data)
 
-        _,_,std=sigma_clipped_stats(data,sigma=self.sig_sky)
-        daofind=DAOStarFinder(std*self.sig_src, self.fwhm, sharplo=self.sharplo, sharphi=self.sharphi,
+        _,median,std=sigma_clipped_stats(data,sigma=self.sig_sky)
+        if method=="findpeaks":
+            return find_peaks(data-bkg, median+std*self.sig_src, box_size=11)
+
+        else:
+            find=DAOStarFinder(std*self.sig_src, self.fwhm, sharplo=self.sharplo, sharphi=self.sharphi,
                 roundlo=self.roundlo, roundhi=self.roundhi, peakmax=np.inf, xycoords=xycoords)
-        return daofind(data - bkg)
+            return find(data - bkg)
+
 
     def _bkg2d(self, data):
         return Background2D(data, self.boxsize, filter_size=3).background
 
     def match(self, base, cat):
         """
         Internal function to class
@@ -86,19 +92,17 @@
         is above the threshold self.match_threshold
         """
 
         added=0
         base_sky=SkyCoord(x=base["xcentroid"], y=base["ycentroid"], z=np.zeros(len(base)), representation_type="cartesian")
         cat_sky=SkyCoord(x=cat["xcentroid"], y=cat["ycentroid"], z=np.zeros(len(cat)), representation_type="cartesian")
         _,separation,_=cat_sky.match_to_catalog_3d(base_sky)
-        for src,sep in zip(cat,separation.to_value()):
-            if sep>self.fwhm:#1 pixel?
-                base.add_row(src)
-                added+=1
-        return added
+        mask= separation.to_value() >self.fwhm
+        return vstack((base,cat[mask]))
+
 
     def find_stars(self, data, mask=None):
         """
         Main function of Routine
         FUNC:
             This routine runs source detection several times, but on a different form
             of the data array each time. Each form has been "skewed" somehow to brighten the
@@ -115,25 +119,26 @@
         if mask is None: mask=np.where(np.isnan(data))
         _,median,_=sigma_clipped_stats(data,sigma=self.sig_sky)
         data[mask]=median
 
         self.catalogue=self.detect(data)
         if self.verbose: printf("-> [PLAIN] pass: %d sources\n"%len(self.catalogue))
 
-        self.match(self.catalogue, self.detect(data, self._bkg2d))
+        self.catalogue=self.match(self.catalogue, self.detect(data, self._bkg2d))
         if self.verbose: printf("-> [BGD2D] pass: %d sources\n"%len(self.catalogue))
 
         ## 2nd order differential detection
-        kernel=RickerWavelet2DKernel(1)
+        kernel=RickerWavelet2DKernel(self.ricker_r)
         conv=convolve(data, kernel)
         corr=match_template(conv/np.amax(conv), kernel.array)
-        _detections=self.detect(corr)
-        _detections["xcentroid"]+=kernel.shape[0]//2
-        _detections["ycentroid"]+=kernel.shape[0]//2
-        self.match(self.catalogue, _detections)
+        _detections=self.detect(corr, method="findpeaks")
+        _detections["x_peak"]+=kernel.shape[0]//2
+        _detections["y_peak"]+=kernel.shape[0]//2
+        _detections.rename_columns( ("x_peak","y_peak"),("xcentroid","ycentroid"))
+        self.catalogue=self.match(self.catalogue, _detections)
         if self.verbose: printf("-> [CONVL] pass: %d sources\n"%len(self.catalogue))
 
         ## Now with xycoords DAOStarfinder will refit the sharp and round values at the detected locations
         #self.catalogue=self.detect(data, xycoords=np.array([self.catalogue["xcentroid"],self.catalogue["ycentroid"]]).T)#, clean=0)
         tmp=SourceProperties(data,self.catalogue, verbose=self.verbose).calculate_geometry(self.fwhm)
         if tmp: self.catalogue=tmp
```

### Comparing `starbug2-0.3.6/starbug2/starbug.py` & `starbug2-0.3.7/starbug2/starbug.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
             detector=Detection_Routine( sig_src=self.options["SIGSRC"],
                                         sig_sky=self.options["SIGSKY"],
                                         fwhm=FWHM,
                                         sharplo=self.options["SHARP_LO"],
                                         sharphi=self.options["SHARP_HI"],
                                         roundlo=self.options["ROUND_LO"],
                                         roundhi=self.options["ROUND_HI"],
+                                        ricker_r=self.options["RICKER_R"],
                                         bgd2d=self.options["DOBGD2D"],
                                         boxsize=int(self.options["BOX_SIZE"]),
                                         cleansrc=self.options["CLEANSRC"],
                                         verbose=self.options["VERBOSE"])
 
             self.detections=detector(self.image.data.copy())["xcentroid","ycentroid","sharpness","roundness1","roundness2"]
 
@@ -482,14 +483,16 @@
             #mag-=dmag
             #self.log("Photometric offset: %f\n"%dmag)
 
             psf_cat.add_column(mag,name=self.filter)
             psf_cat.add_column(magerr,name="e%s"%self.filter)
             self.psfcatalogue=tabppend(self.psfcatalogue, psf_cat)
             self.psfcatalogue.meta=dict(self.header.items())
+            self.psfcatalogue.meta["AP_FILE"]=self.options["AP_FILE"]
+            self.psfcatalogue.meta["BGD_FILE"]=self.options["BGD_FILE"]
             #self.background=fits.ImageHDU(data=phot.bkg_estimator.bgd, name="BACKGROUND", header=self.wcs.to_header()) ##So is it supposed to be a fits image or a numpy array?!
 
     def cleanup(self):
         """
         """
         self.log("Cleaning up..\n")
```

### Comparing `starbug2-0.3.6/starbug2/utils.py` & `starbug2-0.3.7/starbug2/utils.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/starbug2.egg-info/PKG-INFO` & `starbug2-0.3.7/starbug2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.3.6
+Version: 0.3.7
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
@@ -88,9 +88,10 @@
 
 See [starbug-manual](https://github.com/conornally/starbug2/blob/main/docs/starbug-manual.md) for more detailed instructions.
 
 ## TODO
 
 * Need to really figure out setup.cfg to include the extras files
 * MIRI Background masking
-
-
+* findpeaks on convl method
+* rickerwavelet radius
+* psf dither match dropping apMag
```

### Comparing `starbug2-0.3.6/tests/test_routines.py` & `starbug2-0.3.7/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.3.6/tests/test_utils.py` & `starbug2-0.3.7/tests/test_utils.py`

 * *Files identical despite different names*

