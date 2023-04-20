# Comparing `tmp/lenspyx-1.0.0.tar.gz` & `tmp/lenspyx-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lenspyx-1.0.0.tar", last modified: Thu Aug  8 17:52:54 2019, max compression
+gzip compressed data, was "dist/lenspyx-2.0.5.tar", last modified: Thu Apr 20 14:56:12 2023, max compression
```

## Comparing `lenspyx-1.0.0.tar` & `lenspyx-2.0.5.tar`

### file list

```diff
@@ -1,30 +1,63 @@
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/
--rw-r--r--   0 jcarron    (501) staff       (20)     1534 2019-08-08 17:52:54.000000 lenspyx-1.0.0/PKG-INFO
--rw-r--r--   0 jcarron    (501) staff       (20)     1125 2019-08-07 21:28:43.000000 lenspyx-1.0.0/README.md
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx/
--rw-r--r--   0 jcarron    (501) staff       (20)       55 2019-08-08 15:50:32.000000 lenspyx-1.0.0/lenspyx/__init__.py
--rw-r--r--   0 jcarron    (501) staff       (20)     3785 2019-08-07 21:16:50.000000 lenspyx-1.0.0/lenspyx/angles.py
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx/bicubic/
--rw-r--r--   0 jcarron    (501) staff       (20)       21 2019-08-07 08:18:55.000000 lenspyx-1.0.0/lenspyx/bicubic/__init__.py
--rw-r--r--   0 jcarron    (501) staff       (20)     2810 2019-08-07 17:51:29.000000 lenspyx-1.0.0/lenspyx/bicubic/bicubic.f90
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx/data/
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx/data/cls/
--rw-r--r--   0 jcarron    (501) staff       (20)   462368 2016-10-11 11:41:44.000000 lenspyx-1.0.0/lenspyx/data/cls/FFP10_wdipole_lensedCls.dat
--rw-r--r--   0 jcarron    (501) staff       (20)   784113 2016-10-11 11:41:44.000000 lenspyx-1.0.0/lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat
--rw-r--r--   0 jcarron    (501) staff       (20)    10924 2019-08-08 16:55:35.000000 lenspyx-1.0.0/lenspyx/lensing.py
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx/shts/
--rw-r--r--   0 jcarron    (501) staff       (20)        2 2019-08-06 21:50:14.000000 lenspyx-1.0.0/lenspyx/shts/__init__.py
--rw-r--r--   0 jcarron    (501) staff       (20)    32729 2019-08-06 21:43:38.000000 lenspyx-1.0.0/lenspyx/shts/shts.f90
--rw-r--r--   0 jcarron    (501) staff       (20)     6353 2019-08-08 17:51:21.000000 lenspyx-1.0.0/lenspyx/shts/shts.py
--rw-r--r--   0 jcarron    (501) staff       (20)     5783 2019-08-08 15:36:07.000000 lenspyx-1.0.0/lenspyx/utils.py
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/
--rw-r--r--   0 jcarron    (501) staff       (20)     1534 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/PKG-INFO
--rw-r--r--   0 jcarron    (501) staff       (20)      505 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/SOURCES.txt
--rw-r--r--   0 jcarron    (501) staff       (20)        1 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/dependency_links.txt
--rw-r--r--   0 jcarron    (501) staff       (20)       20 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/requires.txt
--rw-r--r--   0 jcarron    (501) staff       (20)        8 2019-08-08 17:52:54.000000 lenspyx-1.0.0/lenspyx.egg-info/top_level.txt
--rw-r--r--   0 jcarron    (501) staff       (20)       38 2019-08-08 17:52:54.000000 lenspyx-1.0.0/setup.cfg
--rw-r--r--   0 jcarron    (501) staff       (20)     1226 2019-08-08 17:50:46.000000 lenspyx-1.0.0/setup.py
-drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2019-08-08 17:52:54.000000 lenspyx-1.0.0/tests/
--rw-r--r--   0 jcarron    (501) staff       (20)        0 2019-08-08 16:07:41.000000 lenspyx-1.0.0/tests/__init__.py
--rw-r--r--   0 jcarron    (501) staff       (20)     2029 2019-08-07 20:24:31.000000 lenspyx-1.0.0/tests/test_l.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.314990 lenspyx-2.0.5/
+-rwx------   0 jcarron    (501) staff       (20)     1344 2020-10-09 19:38:38.000000 lenspyx-2.0.5/LICENSE.txt
+-rw-r--r--   0 jcarron    (501) staff       (20)     1834 2023-04-20 14:56:12.314772 lenspyx-2.0.5/PKG-INFO
+-rw-r--r--   0 jcarron    (501) staff       (20)     1622 2023-04-20 14:55:55.000000 lenspyx-2.0.5/README.md
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.284882 lenspyx-2.0.5/lenspyx/
+-rw-r--r--   0 jcarron    (501) staff       (20)       99 2023-04-20 14:32:38.000000 lenspyx-2.0.5/lenspyx/__init__.py
+-rw-r--r--   0 jcarron    (501) staff       (20)       21 2023-04-20 14:50:35.000000 lenspyx-2.0.5/lenspyx/_version.py
+-rwx------   0 jcarron    (501) staff       (20)     3785 2020-10-09 19:38:38.000000 lenspyx-2.0.5/lenspyx/angles.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1981 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/cachers.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.274424 lenspyx-2.0.5/lenspyx/data/
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.290819 lenspyx-2.0.5/lenspyx/data/cls/
+-rwx------   0 jcarron    (501) staff       (20)   462368 2020-10-09 19:38:38.000000 lenspyx-2.0.5/lenspyx/data/cls/FFP10_wdipole_lensedCls.dat
+-rwx------   0 jcarron    (501) staff       (20)   784113 2020-10-09 19:38:38.000000 lenspyx-2.0.5/lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.277377 lenspyx-2.0.5/lenspyx/fortran/
+-rw-r--r--   0 jcarron    (501) staff       (20)    15305 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/fortran/remapping.f90
+-rw-r--r--   0 jcarron    (501) staff       (20)     5972 2023-04-20 13:05:54.000000 lenspyx-2.0.5/lenspyx/lensing.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.299584 lenspyx-2.0.5/lenspyx/remapping/
+-rw-r--r--   0 jcarron    (501) staff       (20)       43 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/__init__.py
+-rw-r--r--   0 jcarron    (501) staff       (20)      102 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/deflection.py
+-rw-r--r--   0 jcarron    (501) staff       (20)    32754 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/deflection_028.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     4398 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/deflection_029.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     3945 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/utils_angles.py
+-rw-r--r--   0 jcarron    (501) staff       (20)    15439 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/remapping/utils_geom.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.301293 lenspyx-2.0.5/lenspyx/shts/
+-rwx------   0 jcarron    (501) staff       (20)        2 2020-10-09 19:38:38.000000 lenspyx-2.0.5/lenspyx/shts/__init__.py
+-rw-r--r--   0 jcarron    (501) staff       (20)    32885 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/shts/shts.f90
+-rw-r--r--   0 jcarron    (501) staff       (20)     6426 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/shts/shts.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     5342 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/sims.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.313767 lenspyx-2.0.5/lenspyx/tests/
+-rw-r--r--   0 jcarron    (501) staff       (20)     5058 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/2829.py
+-rw-r--r--   0 jcarron    (501) staff       (20)        0 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/__init__.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     3652 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/aliasing.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1790 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/anglesatpoles.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1113 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/cmplxvsreal.py
+-rw-r--r--   0 jcarron    (501) staff       (20)      906 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/fibonacci.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     4247 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/gclm2lenmap.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     4139 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/helper.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     5076 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/lensaliasing.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     4026 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/lensgclm.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1676 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/lensing.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     3319 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/polrot.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1111 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/splits.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     2168 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/strongscal_bwd.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     2109 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/strongscal_fwd.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1116 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/test_A.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     4968 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/test_FFP10fwd.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     3722 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/test_epsilon.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1224 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/test_funkypointing.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     3286 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/test_nocurlshts.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1146 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/theta_interpol.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     1982 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/tests/u2nu.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     8471 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/utils.py
+-rw-r--r--   0 jcarron    (501) staff       (20)     7952 2023-04-20 12:33:47.000000 lenspyx-2.0.5/lenspyx/utils_hp.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.287026 lenspyx-2.0.5/lenspyx.egg-info/
+-rw-r--r--   0 jcarron    (501) staff       (20)     1834 2023-04-20 14:56:12.000000 lenspyx-2.0.5/lenspyx.egg-info/PKG-INFO
+-rw-r--r--   0 jcarron    (501) staff       (20)     1363 2023-04-20 14:56:12.000000 lenspyx-2.0.5/lenspyx.egg-info/SOURCES.txt
+-rw-r--r--   0 jcarron    (501) staff       (20)        1 2023-04-20 14:56:12.000000 lenspyx-2.0.5/lenspyx.egg-info/dependency_links.txt
+-rw-r--r--   0 jcarron    (501) staff       (20)        6 2023-04-20 14:56:12.000000 lenspyx-2.0.5/lenspyx.egg-info/requires.txt
+-rw-r--r--   0 jcarron    (501) staff       (20)        8 2023-04-20 14:56:12.000000 lenspyx-2.0.5/lenspyx.egg-info/top_level.txt
+-rw-r--r--   0 jcarron    (501) staff       (20)       38 2023-04-20 14:56:12.315074 lenspyx-2.0.5/setup.cfg
+-rw-r--r--   0 jcarron    (501) staff       (20)      906 2023-04-20 14:50:14.000000 lenspyx-2.0.5/setup.py
+drwxr-xr-x   0 jcarron    (501) staff       (20)        0 2023-04-20 14:56:12.314107 lenspyx-2.0.5/tests/
+-rw-r--r--   0 jcarron    (501) staff       (20)     2387 2023-04-20 12:33:47.000000 lenspyx-2.0.5/tests/test_l.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lenspyx-1.0.0/lenspyx/angles.py` & `lenspyx-2.0.5/lenspyx/angles.py`

 * *Files identical despite different names*

### Comparing `lenspyx-1.0.0/lenspyx/data/cls/FFP10_wdipole_lensedCls.dat` & `lenspyx-2.0.5/lenspyx/data/cls/FFP10_wdipole_lensedCls.dat`

 * *Files identical despite different names*

### Comparing `lenspyx-1.0.0/lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat` & `lenspyx-2.0.5/lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat`

 * *Files identical despite different names*

### Comparing `lenspyx-1.0.0/lenspyx/shts/shts.f90` & `lenspyx-2.0.5/lenspyx/shts/shts.f90`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
      llm_arr_p_lm1(:) = llm_arr_p_lm0(:)
      llm_arr_p_lm0(:) = llm_arr_x_lmt(:)
 
      vtm(:,0) = vtm(:,0) + llm_arr_p_lm0(:)*glm(tl)
   end do
 
   spow_i(:) = 0.d0
-
 !$omp parallel do default(none) &
 !$omp private(j, tl, tm, scal, spow,id, tfac, llm_arr_p_lm0) &
 !$omp private(llm_arr_p_lm1, llm_arr_m_lm0, llm_arr_m_lm1, llm_arr_x_lmt, rl) &
 !$omp firstprivate(l, m, lmax, spow_i, llm_arr_p, llm_arr_m) schedule(dynamic, 1) &
 !$omp shared(htttht, costht, sintht, sfac, s, zl, ntht, tht, glm, vtm)
   ! for m > 0 we first build sLambda_mm:
   do tm=1,lmax
@@ -319,18 +318,19 @@
         end if
      end do
   end do
 !$omp end parallel do
 end subroutine vlm2vtm
 
 
-subroutine vlm2vtm_sym(ntht, lmax, s, tht, vlm, vtm)
+subroutine vlm2vtm_sym(ntht, lmax, s, tht, vlm, vtm, nthreads)
 ! Same as above but produces for all tht the result for 1 - tht as well.
 ! Using sLlm(pi - tht) = (-1) ** (l + s) sLl-m(tht)
-  integer ntht, lmax, s
+  use OMP_LIB
+  integer, intent(in) :: ntht, lmax, s, nthreads
   double precision tht(ntht)
   double complex, intent(in)  :: vlm(0:((lmax+1)*(lmax+1)-1))
   double complex, intent(out) :: vtm(0:2 * ntht -1, -lmax:lmax)
 
   integer l, m, tl, ts, tm, j,sgn
   double precision htttht(ntht), costht(ntht), sintht(ntht)
   double precision scal(ntht), spow(ntht), spow_i(ntht)
@@ -388,14 +388,15 @@
      
      vtm(:ntht-1,0) = vtm(:ntht-1,0) +  llm_arr_p_lm0(:)*vlm(tl*tl+tl)
      vtm(ntht:,0) = vtm(ntht:,0) + sgn *llm_arr_p_lm0(:)*vlm(tl*tl+tl)
      sgn = -sgn
   end do
 
   spow_i(:) = 0.d0
+  call OMP_SET_NUM_THREADS(nthreads)
 
 !$omp parallel do default(none) &
 !$omp private(j, tl, tm, sgn,scal, spow, tfac, llm_arr_p_lm0) &
 !$omp private(llm_arr_p_lm1, llm_arr_m_lm0, llm_arr_m_lm1, llm_arr_x_lmt, rl) &
 !$omp firstprivate(l, m, lmax, spow_i, llm_arr_p, llm_arr_m) schedule(dynamic, 1) &
 !$omp shared(htttht, costht, sintht, sfac, s, zl, ntht, tht, vlm, vtm)
   ! for m > 0 we first build sLambda_mm:
@@ -596,21 +597,22 @@
            end do
         end if
      end do
   end do
 !$omp end parallel do
 end subroutine glm2vtm_s0
 
-subroutine glm2vtm_s0sym(ntht, lmax, tht, glm, vtm)
+subroutine glm2vtm_s0sym(ntht, lmax, tht, glm, vtm, nthreads)
   ! Same as above but outputs only m = 0 to lmax + 1
   ! using for spin 0 vt-m = vtm^*
   ! for each tht, pi -tht is also calculated using Llm(t) = (-)^(l+m)Llm(pi -t)
   ! Not certain it works for tht = 0.
   ! Only 'upper half' of vtm array is used.
-  integer ntht, lmax,sgn
+  use OMP_LIB
+  integer ntht, lmax,sgn, nthreads
   double precision tht(ntht)
   double complex, intent(in)  :: glm(0:((lmax+1)*(lmax+2)/2-1))
   double complex, intent(out) :: vtm(0:2 * ntht-1,0:lmax)
 
   integer l, m, tl, tm, j,id,s
   double precision costht(ntht), sintht(ntht)
   double precision scal(ntht), spow(ntht), spow_i(ntht)
@@ -655,14 +657,15 @@
      llm_cont(:) = llm_arr_p_lm0(:)*glm(tl)
      vtm(0:ntht-1,0) = vtm(0:ntht-1,0) + llm_cont(:)
      vtm(ntht:,0) = vtm(ntht:,0) + sgn * llm_cont(:)
      sgn = -sgn
   end do
 
   spow_i(:) = 0.d0
+  call OMP_SET_NUM_THREADS(nthreads)
 
 !$omp parallel do default(none) &
 !$omp private(j,id,sgn, tl, tm, scal, spow, tfac, llm_arr_p_lm0) &
 !$omp private(llm_arr_p_lm1, llm_arr_x_lmt,llm_cont,rl) &
 !$omp firstprivate(l, m, lmax, spow_i, llm_arr_p) schedule(dynamic, 1) &
 !$omp shared(costht, sintht, sfac, s, zl, ntht, tht, glm, vtm)
   ! for m > 0 we first build sLambda_mm:
```

### Comparing `lenspyx-1.0.0/lenspyx/shts/shts.py` & `lenspyx-2.0.5/lenspyx/shts/shts.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,60 +61,60 @@
     else :
         # Probably no real gain to expect here from pyfftw for the ffts.
         if Nphi > 2 * lmax + 1:
             a = np.zeros((Nt,Nphi),dtype = complex)
             a[:,:2 * lmax + 1] = vtm
             ret = np.fft.ifft(a) * (np.exp(np.arange(Nphi) * (-1j / Nphi * (2. * np.pi) * lmax)) * Nphi)
         else:
-            ret = np.fft.ifft(vtm[:,lmax - Nphi/2:lmax + Nphi/2])
-            ret *= (np.exp(np.arange(Nphi) * (-1j / Nphi * (2. * np.pi) * Nphi/2)) * Nphi)
+            ret = np.fft.ifft(vtm[:,lmax - Nphi//2:lmax + Nphi//2])
+            ret *= (np.exp(np.arange(Nphi) * (-1j / Nphi * (2. * np.pi) * Nphi /2)) * Nphi)
         retmap = ret.real if spin == 0 else ret
     retmap[phiflip, :] = retmap[phiflip, ::-1]
     return retmap
 
 
-def glm2vtm_sym(s, tht, glm):
+def glm2vtm_sym(s, tht, glm, nthreads):
     r"""This produces :math:`\sum_l _s\Lambda_{lm} v_{lm}` for pure gradient input for a range of colatitudes"""
 
     if s == 0:
         lmax = utils.nlm2lmax(len(glm))
         ret = np.empty((2 * len(tht), 2 * lmax + 1), dtype=complex)
-        ret[:, lmax:] = fsht.glm2vtm_s0sym(lmax, tht, -glm)
+        ret[:, lmax:] = fsht.glm2vtm_s0sym(lmax, tht, -glm, nthreads)
         ret[:, 0:lmax] = (ret[:, slice(2 * lmax + 1, lmax, -1)]).conjugate()
         return ret
-    return vlm2vtm_sym(s, tht, utils.alm2vlm(glm))
+    return vlm2vtm_sym(s, tht, utils.alm2vlm(glm), nthreads)
 
 
-def vlm2vtm_sym(s, tht, vlm):
+def vlm2vtm_sym(s, tht, vlm, nthreads):
     r"""This produces :math:`\sum_l _s\Lambda_{lm} v_{lm}` for a range of colatitudes"""
     assert s >= 0
     tht = np.array(tht)
     lmax = int(np.sqrt(len(vlm)) - 1)
     assert (len(vlm) == (lmax + 1) ** 2)
     if s == 0:
         print("Consider using glm2vtm_sym for spin 0 for factor of 2 speed-up")
-        return fsht.vlm2vtm_sym(lmax, s, tht, vlm)
+        return fsht.vlm2vtm_sym(lmax, s, tht, vlm, nthreads)
     else:
         #: resolving poles, since fsht implementation does not handle them.
         north = np.where(tht <= 0.)[0]
         south = np.where(tht >= np.pi)[0]
         if len(north) == 0 and len(south) == 0:
-            return fsht.vlm2vtm_sym(lmax, s, tht, vlm)
+            return fsht.vlm2vtm_sym(lmax, s, tht, vlm, nthreads)
         else:
             nt = len(tht)
             ret = np.zeros( (2 * nt, 2 * lmax + 1), dtype=complex)
             if len(north) > 0:
                 ret[north] = _vlm2vtm_northpole(s, vlm)
                 ret[nt + north] = _vlm2vtm_southpole(s, vlm)
             if len(south) > 0:
                 ret[south] = _vlm2vtm_southpole(s, vlm)
                 ret[nt + south] = _vlm2vtm_northpole(s, vlm)
             if len(north) + len(south) < len(tht):
                 others = np.where( (tht < np.pi) & (tht > 0.))[0]
-                vtm =  fsht.vlm2vtm_sym(lmax, s, tht[others], vlm)
+                vtm =  fsht.vlm2vtm_sym(lmax, s, tht[others], vlm, nthreads)
                 ret[others] = vtm[:len(others)]
                 ret[nt + others] = vtm[len(others):]
             return ret
 
 
 def _vlm2vtm_northpole(s, vlm):
     r"""Spin-weight harmonics on the north pole
```

### Comparing `lenspyx-1.0.0/setup.py` & `lenspyx-2.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 def configuration(parent_package='', top_path=''):
     config = Configuration('', parent_package, top_path)
-    config.add_extension('lenspyx.bicubic.bicubic', ['lenspyx/bicubic/bicubic.f90'])
-    config.add_extension('lenspyx.shts.fsht', ['lenspyx/shts/shts.f90'],
-                extra_link_args=['-lgomp'],libraries=['gomp'], extra_f90_compile_args=['-fopenmp', '-w'])
     return config
 
+exec(open('lenspyx/_version.py').read())
 setup(
     name='lenspyx',
-    version='1.0.0',
-    packages=['lenspyx', 'lenspyx.bicubic', 'lenspyx.shts'],
+    version=__version__,
+    packages=['lenspyx', 'lenspyx.remapping', 'lenspyx.tests'],
     url='https://github.com/carronj/lenspyx',
     author='Julien Carron',
     data_files=[('lenspyx/data/cls', ['lenspyx/data/cls/FFP10_wdipole_lensedCls.dat',
-                                      'lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat',
-                                      'lenspyxs/data/cls/FFP10_wdipole_params.ini'])],
+                                      'lenspyx/data/cls/FFP10_wdipole_lenspotentialCls.dat'])],
     author_email='to.jcarron@gmail.com',
     description='lensed CMB sims pipe',
-    install_requires=['healpy', 'numpy', 'pyfftw'],
+    install_requires=['ducc0'],
     long_description=long_description,
     configuration=configuration)
```

### Comparing `lenspyx-1.0.0/tests/test_l.py` & `lenspyx-2.0.5/tests/test_l.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 from __future__ import print_function
 import healpy as hp
 from lenspyx import lensing
 import numpy as np
 
-def test_t():
+def test_t(experimental=False):
     lmax = 200
     nside = 256
     cls_unl = np.ones(lmax + 1, dtype=float)
     tunl = hp.synalm(cls_unl, new=True)
     dlm = np.zeros_like(tunl)
     hp.almxfl(dlm, np.sqrt(np.arange(lmax + 1) * np.arange(1, lmax + 2, dtype=float)), inplace=True)
     T = hp.alm2map(tunl, nside)
-    T1 = lensing.alm2lenmap(tunl, [dlm, None], nside, verbose=True, nband=8, facres=-2)
+    T1 = lensing.alm2lenmap(tunl, [dlm, None], nside, verbose=True, nband=8, facres=-2, experimental=experimental)
     assert np.max(np.abs(T - T1)) / np.std(T) < 1e-5
-    d1Re, d1Im = hp.alm2map_spin([dlm, np.zeros_like(dlm)], nside, 1, lmax)
-    T2 = lensing.alm2lenmap(tunl, [d1Re, d1Im], nside, verbose=True, nband=8, facres=-2)
-    assert np.max(np.abs(T - T2)) / np.std(T) < 1e-5
-    T3 = lensing.alm2lenmap(tunl, [dlm, dlm.copy()], nside, verbose=True, nband=8, facres=-2)
-    assert np.all(T2 == T3)
+    if not experimental:
+        d1Re, d1Im = hp.alm2map_spin([dlm, np.zeros_like(dlm)], nside, 1, lmax)
+        T2 = lensing.alm2lenmap(tunl, [d1Re, d1Im], nside, verbose=True, nband=8, facres=-2)
+        assert np.max(np.abs(T - T2)) / np.std(T) < 1e-5
+        T3 = lensing.alm2lenmap(tunl, [dlm, dlm.copy()], nside, verbose=True, nband=8, facres=-2)
+        assert np.all(T2 == T3)
 
-def test_pol():
+def test_pol(experimental=False):
     lmax = 200
     nside = 256
     facres= -1
     cls_unl = np.ones(lmax + 1, dtype=float)
     tunl = hp.synalm(cls_unl, new=True)
     dlm = np.zeros_like(tunl)
     hp.almxfl(dlm, np.sqrt(np.arange(lmax + 1) * np.arange(1, lmax + 2, dtype=float)), inplace=True)
     Q, U = hp.alm2map_spin([tunl, np.zeros_like(tunl)], nside, 2, lmax)
-    Q1, U1 = lensing.alm2lenmap_spin([tunl, None], [dlm, None], nside, 2, verbose=True, nband=8, facres=facres)
+    Q1, U1 = lensing.alm2lenmap_spin([tunl, None], [dlm, None], nside, 2, verbose=True, nband=8, facres=facres, experimental=experimental)
 
     assert np.max(np.abs(Q - Q1)) / np.std(Q) < 1e-5, np.max(np.abs(Q - Q1)) / np.std(Q)
     assert np.max(np.abs(U - U1)) / np.std(U) < 1e-5, np.max(np.abs(U - U1)) / np.std(U)
 
-    d1Re, d1Im = hp.alm2map_spin([dlm, np.zeros_like(dlm)], nside, 1, lmax)
-    Q2, U2 = lensing.alm2lenmap_spin([tunl ,None], [d1Re, d1Im], nside, 2, verbose=True, nband=8, facres=facres)
-    assert np.allclose(Q2, Q1, rtol=1e-10)
-    assert np.allclose(U2, U1, rtol=1e-10)
-
-    Q3, U3 = lensing.alm2lenmap_spin([tunl,tunl * 0.], [d1Re, d1Im], nside, 2, verbose=True, nband=8, facres=facres)
-    assert np.all(Q3 == Q2)
-    assert np.all(U3 == U2)
+    if not experimental:
+        #FIXME: this version does not have the Red Imd input caller at the moment
+        d1Re, d1Im = hp.alm2map_spin([dlm, np.zeros_like(dlm)], nside, 1, lmax)
+        Q2, U2 = lensing.alm2lenmap_spin([tunl ,None], [d1Re, d1Im], nside, 2, verbose=True, nband=8, facres=facres, experimental=experimental)
+        assert np.allclose(Q2, Q1, rtol=1e-10)
+        assert np.allclose(U2, U1, rtol=1e-10)
+
+        Q3, U3 = lensing.alm2lenmap_spin([tunl,tunl * 0.], [d1Re, d1Im], nside, 2, verbose=True, nband=8, facres=facres, experimental=experimental)
+        assert np.all(Q3 == Q2)
+        assert np.all(U3 == U2)
 
 
 if __name__ == '__main__':
-    #test_t()
-    test_pol()
+    test_t(experimental=True)
+    test_pol(experimental=True)
```

