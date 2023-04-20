# Comparing `tmp/ligo-followup-advocate-1.2.0.tar.gz` & `tmp/ligo-followup-advocate-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.0.tar", last modified: Mon Apr 17 01:11:08 2023, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.1.tar", last modified: Thu Apr 20 18:01:03 2023, max compression
```

## Comparing `ligo-followup-advocate-1.2.0.tar` & `ligo-followup-advocate-1.2.1.tar`

### file list

```diff
@@ -1,149 +1,152 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.784361 ligo-followup-advocate-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-17 01:11:08.784361 ligo-followup-advocate-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.747361 ligo-followup-advocate-1.2.0/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    21061 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.751361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2856 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2184 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     8568 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.752361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.745361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.752361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.753361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.754361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.755361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.755361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.756361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.756361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.757361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.758361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.759361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.765361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.766361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.766361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3382 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.768361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.782361 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-17 01:10:53.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     4791 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 01:11:08.783361 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6315 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-17 01:11:08.000000 ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-17 01:11:08.785361 ligo-followup-advocate-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-04-17 01:10:54.000000 ligo-followup-advocate-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.914352 ligo-followup-advocate-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-20 18:01:03.915351 ligo-followup-advocate-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.876350 ligo-followup-advocate-1.2.1/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    21231 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.880350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     8572 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.880350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.874350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.881350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.881350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.883350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.883350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.884350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.884350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.885351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.885351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.888351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.894351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.894351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.895351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.897351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.913351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     4791 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.914352 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.0/COPYING.md` & `ligo-followup-advocate-1.2.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/PKG-INFO` & `ligo-followup-advocate-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.0
+Version: 1.2.1
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.0/README.md` & `ligo-followup-advocate-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,21 @@
 
 def main_dict(gracedb_id, client):
     """Create general dictionary to pass to compose circular"""
 
     event = client.superevent(gracedb_id).json()
     preferred_event = event['preferred_event_data']
     preferred_pipeline = preferred_event['pipeline']
-    other_pipelines = list(event["pipeline_preferred_events"].keys())
-    other_pipelines.remove(preferred_pipeline)
+    other_pipelines = []
+    gw_events = event['gw_events']
+
+    for gw_event in gw_events:
+        pipeline = client.event(gw_event).json()['pipeline']
+        if pipeline not in other_pipelines and pipeline != preferred_pipeline:
+            other_pipelines.append(pipeline)
 
     voevents = client.voevents(gracedb_id).json()['voevents']
     if not voevents:
         raise ValueError(
             "{} has no VOEvent to generate circulars from.".format(
                 gracedb_id))
 
@@ -182,15 +187,15 @@
     if mailto:
         pattern = 'mailto:emfollow@ligo.org,dac@ligo.org?subject={0}&body={1}'
         url = pattern.format(
             urllib.parse.quote(subject),
             urllib.parse.quote(body))
         webbrowser.open(url)
     else:
-        return '{0}\n{1}'.format(subject, body)
+        return '{0}\n\n{1}'.format(subject, body)
 
 
 def compose_raven(gracedb_id, authors=(),
                   service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose EM_COINC RAVEN GCN Circular draft"""
 
     if client is None:
@@ -203,15 +208,15 @@
 
     subject = (
         env.get_template('RAVEN_subject.jinja2').render(**kwargs)
         .strip())
     body = (
         env.get_template('RAVEN_circular.jinja2').render(**kwargs)
         .strip())
-    return '{0}\n{1}'.format(subject, body)
+    return '{0}\n\n{1}'.format(subject, body)
 
 
 def compose_grb_medium_latency(
         gracedb_id, authors=(), service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose GRB Medium Latency GCN Circular draft.
     Here, gracedb_id will be a GRB external trigger ID in GraceDb."""
 
@@ -283,15 +288,15 @@
 
     subject = (
         env.get_template('medium_latency_grb_subject.jinja2').render(**kwargs)
         .strip())
     body = (
         env.get_template('medium_latency_grb_circular.jinja2').render(**kwargs)
         .strip())
-    return '{0}\n{1}'.format(subject, body)
+    return '{0}\n\n{1}'.format(subject, body)
 
 
 def compose_update(gracedb_id, authors=(),
                    service=rest.DEFAULT_SERVICE_URL,
                    update_types=['sky_localization', 'p_astro',
                                  'em_bright', 'raven'],
                    client=None):
@@ -327,15 +332,15 @@
     kwargs.update(change_significance_statement=False)
     kwargs.update(subject='Update')
     kwargs.update(update_types=update_types)
 
     subject = env.get_template('subject.jinja2').render(**kwargs).strip()
     body = env.get_template(
                'update_circular.jinja2').render(**kwargs).strip()
-    return '{0}\n{1}'.format(subject, body)
+    return '{0}\n\n{1}'.format(subject, body)
 
 
 def compose_retraction(gracedb_id, authors=(),
                        service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose GCN retraction circular"""
     if client is None:
         client = rest.GraceDb(service)
@@ -352,15 +357,15 @@
                  group=preferred_event['group'],
                  earlywarning=earlywarning,
                  authors=authors
              )
 
     subject = env.get_template('subject.jinja2').render(**kwargs).strip()
     body = env.get_template('retraction.jinja2').render(**kwargs).strip()
-    return '{0}\n{1}'.format(subject, body)
+    return '{0}\n\n{1}'.format(subject, body)
 
 
 def read_map_gracedb(graceid, filename, client):
     with tempfile.NamedTemporaryFile(mode='w+b') as localfile:
         remotefile = client.files(graceid, filename, raw=True)
         shutil.copyfileobj(remotefile, localfile)
         localfile.flush()
```

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 {{gracedb_id}} and a {% if snews %}SNEWS supernova{% elif grb %}{% if subthreshold %}sub-threshold {% endif %}{{grbmission(external_pipeline)}}{% endif %} {{propername(external_trigger)}} **CITE ORIGINAL GCN FOR THE EXTERNAL TRIGGER FROM https://gcn.gsfc.nasa.gov/gcn3_archive.html, e.g., (Bhalerao et al., GCN Circular XXXXX)**.
 The {% if snews %}neutrino{% elif grb %}GRB{% endif %} trigger time is {{latency}} seconds {{beforeafter}} the GW candidate event.
 {% if grb %}
 The estimated joint false alarm rate for the coincidence using just timing info is {{naturalfar(time_coinc_far)}}.
 {% if subthreshold_targeted %}The GRB candidate was found during a joint targeted search between the LIGO/Virgo/KAGRA collaboration and {{grbmission_targeted(external_pipeline)}}, and has a false alarm rate of {{naturalfar(far_grb)}}. {% endif %}
 {% if other_ext_pipelines %}RAVEN has also identified {% if other_ext_pipelines|length == 1 %}an additional detection{% elif other_ext_pipelines|length > 1%}additional detections{% endif %} from {{naturalotherexternalpipelines(other_ext_pipelines)}}.{% endif %}
 
-
 {% endif %}
 {% if combined_skymap %}
 {% if combined_skymaps|length == 1 %}A combined sky map is{% else %}Combined sky maps are{% endif %} also available:
 {% for skymap in combined_skymaps %}
  * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% else %}updated{% endif %} localization, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
 {% endfor %}
```

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 trigger with ID {{external_trigger}}
 {%- endif -%}
 {%- endmacro -%}
 
 
 Dictionary of common citations.
 
-{% set citations = {'pycbc': 'Nitz et al. PRD 98, 024050 (2018)',
+{% set citations = {'pycbc': 'Dal Canton et al. ApJ 923, 254 (2021)',
                     'mbta': 'Adams et al. CQG 33, 175012 (2016)',
                     'gstlal': 'Messick et al. PRD 95, 042001 (2017)',
                     'spiir': 'Qi Chu, PhD Thesis, The University of Western Australia (2017)',
                     'cwb': 'Klimenko et al. PRD 93, 042004 (2016)',
                     'olib': 'Lynch et al. PRD 95, 104046 (2017)',
                     'mly': 'Skliris et al. arXiv:2009.14611 (2020)',
                     'em_bright': 'Chatterjee et al. The Astrophysical Journal 896, 1 (2020)',
```

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1133/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E1235/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M1234/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/M5678/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S2468/voevents.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/test_tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 def test_medium_latency_cbc_burst_detection(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E1122'])
 
 
 def test_medium_latency_cbc_exclusion(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
-          'compose_grb_medium_latency', 'E1133'])
+          'compose_grb_medium_latency', 'E1134'])
 
 
 def test_medium_latency_cbc_burst_exclusion(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E2244'])
```

### Comparing `ligo-followup-advocate-1.2.0/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.1/ligo/followup_advocate/tool.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.0
+Version: 1.2.1
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.0/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 ligo/followup_advocate/test/data/E1122/files.json
 ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
 ligo/followup_advocate/test/data/E1122/files/distances_x.json
 ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
 ligo/followup_advocate/test/data/E1133/event.json
 ligo/followup_advocate/test/data/E1133/files.json
-ligo/followup_advocate/test/data/E1133/files/distances_pygrb.json
-ligo/followup_advocate/test/data/E1133/files/false_alarm_probability_pygrb.json
+ligo/followup_advocate/test/data/E1134/event.json
+ligo/followup_advocate/test/data/E1134/files.json
+ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E1234/event.json
 ligo/followup_advocate/test/data/E1234/files.json
 ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
 ligo/followup_advocate/test/data/E1234/files/distances_x.json
 ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
 ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
 ligo/followup_advocate/test/data/E1234/files/initial.data
```

### Comparing `ligo-followup-advocate-1.2.0/setup.cfg` & `ligo-followup-advocate-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/setup.py` & `ligo-followup-advocate-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.0/versioneer.py` & `ligo-followup-advocate-1.2.1/versioneer.py`

 * *Files identical despite different names*

