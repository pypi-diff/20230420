# Comparing `tmp/sev3rance_auth_templates-1.5.0.tar.gz` & `tmp/sev3rance_auth_templates-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sev3rance_auth_templates-1.5.0.tar", last modified: Sun Jul 31 00:54:56 2022, max compression
+gzip compressed data, was "sev3rance_auth_templates-1.6.0.tar", last modified: Thu Apr 20 21:53:54 2023, max compression
```

## Comparing `sev3rance_auth_templates-1.5.0.tar` & `sev3rance_auth_templates-1.6.0.tar`

### file list

```diff
@@ -1,140 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.443262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/community-apps-fixes.css
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/community-apps-fixes.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.css
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    22090 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)    35662 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (121)    57617 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-256x256.png
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-36x36.png
--rw-r--r--   0 runner    (1001) docker     (121)   116071 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-384x384.png
--rw-r--r--   0 runner    (1001) docker     (121)     4428 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-48x48.png
--rw-r--r--   0 runner    (1001) docker     (121)   186065 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (121)     7666 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)    11598 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-96x96.png
--rw-r--r--   0 runner    (1001) docker     (121)    12531 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    10889 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (121)    13628 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    11832 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (121)    18685 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    16332 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)    20450 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    17947 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (121)    27309 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    24052 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (121)     4195 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (121)     6001 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     5176 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (121)     6466 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (121)    27309 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (121)    24052 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (121)    15086 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/html_code.html
--rw-r--r--   0 runner    (1001) docker     (121)    22136 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-144x144.png
--rw-r--r--   0 runner    (1001) docker     (121)    19008 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (121)    19974 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x150.png
--rw-r--r--   0 runner    (1001) docker     (121)    63450 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x310.png
--rw-r--r--   0 runner    (1001) docker     (121)    11653 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-70x70.png
--rw-r--r--   0 runner    (1001) docker     (121)    46235 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/safari-pinned-tab.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.js
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/README.markdown
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.css
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/
--rw-r--r--   0 runner    (1001) docker     (121)     3080 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/switch.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/
--rw-r--r--   0 runner    (1001) docker     (121)    19225 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.js
--rw-r--r--   0 runner    (1001) docker     (121)    13870 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    13870 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/
--rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.js
--rw-r--r--   0 runner    (1001) docker     (121)    11656 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     6837 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js.map
--rw-r--r--   0 runner    (1001) docker     (121)    11656 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)    14216 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.js
--rw-r--r--   0 runner    (1001) docker     (121)    11656 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    11656 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.447262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/config.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/data.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/helper.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/select.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slim.d.ts
--rw-r--r--   0 runner    (1001) docker     (121)     6417 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.css
--rw-r--r--   0 runner    (1001) docker     (121)    74827 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.js
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    47237 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     6063 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.css
--rw-r--r--   0 runner    (1001) docker     (121)    47237 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/
--rw-r--r--   0 runner    (1001) docker     (121)     2738 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/icons.html
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/top-menu.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/
--rw-r--r--   0 runner    (1001) docker     (121)     6889 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/add_doctrine.html
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/add_fit.html
--rw-r--r--   0 runner    (1001) docker     (121)     2986 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/create_category.html
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (121)     5963 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_category.html
--rw-r--r--   0 runner    (1001) docker     (121)     6813 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_doctrine.html
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_fit.html
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_all_categories.html
--rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_all_fits.html
--rw-r--r--   0 runner    (1001) docker     (121)     9229 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_category.html
--rw-r--r--   0 runner    (1001) docker     (121)     6727 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_doctrine.html
--rw-r--r--   0 runner    (1001) docker     (121)    55243 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_fit.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.451262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     8757 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     5300 2022-07-31 00:54:35.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/link.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-31 00:54:56.439262 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9426 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-31 00:54:56.000000 sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.108246 sev3rance_auth_templates-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 21:53:54.108246 sev3rance_auth_templates-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-20 21:53:54.108246 sev3rance_auth_templates-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.080245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.080245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/community-apps-fixes.css
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/community-apps-fixes.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.css
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.092246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35662 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57617 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (123)   116071 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-384x384.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (123)   186065 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18685 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27309 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/html_code.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22136 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19008 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19974 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63450 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46235 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/safari-pinned-tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.092246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.js
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.096246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/de.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/de.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/en.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/en.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/es.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/es.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/fr.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/fr.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/it.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/it.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ja.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ja.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ja.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ko.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ko.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ko.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ru.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ru.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/ru.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/uk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/uk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/uk.mjs
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/zh-hans.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/zh-hans.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/zh-hans.mjs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.096246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/switch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.100246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11656 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.076245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.104246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.104246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/config.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/data.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/helper.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/select.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slim.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.css
+-rw-r--r--   0 runner    (1001) docker     (123)    74827 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    47237 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    47237 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.080245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.104246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/top-menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.108246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/add_doctrine.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/add_fit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/create_category.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_category.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_doctrine.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_fit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_all_categories.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_all_fits.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_category.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_doctrine.html
+-rw-r--r--   0 runner    (1001) docker     (123)    57851 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_fit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.108246 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-20 21:53:37.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:53:54.080245 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 21:53:54.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-04-20 21:53:54.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:53:54.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:53:53.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 21:53:54.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 21:53:54.000000 sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/top_level.txt
```

### Comparing `sev3rance_auth_templates-1.5.0/LICENSE` & `sev3rance_auth_templates-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/PKG-INFO` & `sev3rance_auth_templates-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: sev3rance_auth_templates
-Version: 1.5.0
+Version: 1.6.0
 Summary: Sev3rance Template Overrides for Alliance Auth
 Home-page: https://github.com/sev3rance/sev3rance-auth-templates
 Author: Peter Pfeufer
-Author-email: development@ppfeufer.de
+Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/sev3rance/sev3rance-auth-templates/issues
 Project-URL: Changelog, https://github.com/sev3rance/sev3rance-auth-templates/blob/master/CHANGELOG.md
 Keywords: allianceauth,eveonline,template,template_override,sev3rance
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alliance Auth Template Overrides used by Sev3rance Alliance
 
 # Sev3rance Auth Templates
```

### Comparing `sev3rance_auth_templates-1.5.0/README.md` & `sev3rance_auth_templates-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/setup.cfg` & `sev3rance_auth_templates-1.6.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [metadata]
 name = sev3rance_auth_templates
 version = attr: sev3rance_auth_templates.__version__
 description = Sev3rance Template Overrides for Alliance Auth
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Peter Pfeufer
-author_email = development@ppfeufer.de
+author_email = develop@ppfeufer.de
 maintainer = Peter Pfeufer
-maintainer_email = development@ppfeufer.de
+maintainer_email = develop@ppfeufer.de
 license = GPL-3.0
 license_file = LICENSE
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 home_page = https://github.com/sev3rance/sev3rance-auth-templates
@@ -37,16 +35,16 @@
 project_urls = 
 	Issue / Bug Reports = https://github.com/sev3rance/sev3rance-auth-templates/issues
 	Changelog = https://github.com/sev3rance/sev3rance-auth-templates/blob/master/CHANGELOG.md
 
 [options]
 packages = find:
 install_requires = 
-	allianceauth>=2.15.0
-python_requires = ~=3.7
+	allianceauth>=3.0.0
+python_requires = ~=3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = sev3rance_auth_templates
 
 [egg_info]
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/css/sev3rance.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 @media all {
-    .img-circle, img {
+    .img-circle,
+    img {
         border-radius: 6px;
         height: auto;
         max-width: 100%;
     }
 
     .navbar-nav > li.top-user-menu.with-main-character > .dropdown-menu {
         min-width: 225px;
@@ -15,15 +16,15 @@
     }
 }
 
 /* eve time in navbar
 ------------------------------------------------------------------------------------- */
 @media all {
     .nav-item-eve-time .eve-time-wrapper {
-        color: rgb(255, 255, 255);
+        color: rgb(255 255 255);
         display: block;
         line-height: 21px;
         padding: 10px 15px;
         position: relative;
     }
 }
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/README.md` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/README.md`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-144x144.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-144x144.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-192x192.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-256x256.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-256x256.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-36x36.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-36x36.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-384x384.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-384x384.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-48x48.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-48x48.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-512x512.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-72x72.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-72x72.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-96x96.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/android-chrome-96x96.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-precomposed.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/browserconfig.xml` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/browserconfig.xml`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-16x16.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-32x32.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon.ico` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/html_code.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/html_code.html`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-144x144.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-150x150.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x150.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x310.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-70x70.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/safari-pinned-tab.svg` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/site.webmanifest` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/favicons/site.webmanifest`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/js/sev3rance.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.min.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.min.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/switch.png` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/img/switch.png`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/Gruntfile.min.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/LICENSE` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/README.md` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js.map` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js.map`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/quicksearch/2.4.0/src/jquery.quicksearch.min.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/LICENSE` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/README.md` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/README.md`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/config.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/config.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/data.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/data.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/helper.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/helper.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/index.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/index.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/select.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/select.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slim.d.ts` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slim.d.ts`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.css` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.css`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.js` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/static/sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.min.js`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/base.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/base.html`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/icons.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/icons.html`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/allianceauth/top-menu.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/allianceauth/top-menu.html`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/add_doctrine.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/add_doctrine.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
 
 {% block more_css %}
-    <link rel="stylesheet" href="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css' %}" />
+    <link rel="stylesheet" href="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css' %}">
 
     <style>
         .ms-container {
             width: 100% !important;
         }
     </style>
 {% endblock %}
@@ -53,15 +53,15 @@
 
                             <div class="form-group">
                                 <label for="name" class="col-sm-2 control-label">
                                     {% translate "Doctrine Name" %}
                                 </label>
 
                                 <div class="col-sm-10">
-                                    <input type="text" class="form-control" name="name" id="name" required/>
+                                    <input type="text" class="form-control" name="name" id="name" required>
                                 </div>
                             </div>
 
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">
                                     {% translate "Doctrine Description" %}
                                 </label>
@@ -75,39 +75,43 @@
                                 <label for="fitSelect" class="col-sm-2 control-label">
                                     {% translate "Select Fits" %}
                                 </label>
 
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <select multiple="multiple" id="fitSelect" name="fitSelect">
                                         {% for fit in fittings %}
-                                            <option value="{{ fit.pk }}">{{ fit.name }} ({{fit.ship_type.type_name}})</option>
+                                            <option value="{{ fit.pk }}">
+                                                {{ fit.name }} ({{fit.ship_type.name}})
+                                            </option>
                                         {% endfor %}
                                     </select>
                                 </div>
                             </div>
 
                             <div class="form-group">
                                 <label for="iconSelect" class="col-sm-2 control-label">
                                     {% translate "Select Doctrine Icon" %}
                                 </label>
 
                                 <div class="col-sm-10">
                                     <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
                                         {% for ship in ships %}
-                                            <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__type_name}}</option>
+                                            <option value="{{ ship.ship_type|type_render_url:64 }}">
+                                                {{ship.ship_type__name}}
+                                            </option>
                                         {% endfor %}
                                     </select>
 
                                     <span id="helpBlock" class="help-block">
                                         {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}
                                     </span>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">
                                 {% translate "Submit" %}
                             </button>
                         </form>
                     </div>
                 </div>
             </div>
@@ -115,18 +119,21 @@
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js' %}"></script>
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js' %}"></script>
 
-    <script type="application/javascript">
+    <script>
+        const translation_search = '{% translate "Search" %}';
+
         $('#fitSelect').multiSelect({
-            selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
-            selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
+            selectableHeader: '<input type="text" class="form-control" autocomplete="off" placeholder="' + translation_search + '" style="margin-bottom: 3px;">',
+            selectionHeader: '<input type="text" class="form-control" autocomplete="off" placeholder="' + translation_search + '" style="margin-bottom: 3px;">',
+
             afterInit: function(ms) {
                 let that = this,
                     $selectableSearch = that.$selectableUl.prev(),
                     $selectionSearch = that.$selectionUl.prev(),
                     selectableSearchString = '#'+that.$container.attr('id')+' .ms-elem-selectable:not(.ms-selected)',
                     selectionSearchString = '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected';
```

#### html2text {}

```diff
@@ -11,19 +11,19 @@
 {% translate "New Doctrine" %}
 {% csrf_token %}
  {% translate "Doctrine Name" %}
 [name                ]
  {% translate "Doctrine Description" %}
  {% translate "Select Fits" %}
 {% for fit in fittings %}
-{{ fit.name }} ({{fit.ship_type.type_name}})
+{{ fit.name }} ({{fit.ship_type.name}})
 {% endfor %}
  {% translate "Select Doctrine Icon" %}
 {% for ship in ships %}
-{{ship.ship_type__type_name}}
+{{ship.ship_type__name}}
 {% endfor %}
   {% translate "If you do not see the ship type that you would like to use for
 the icon, add a fit that uses that ship type and try again." %}
 
  {% translate "Submit" %}
 {% endblock %} {% block extra_javascript %}
  {% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/add_fit.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/add_fit.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 {% extends 'fittings/base.html' %}
+
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
+
 {% block page_title %}{% translate "Add Fit" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
         <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
             <button type="button" class="close" data-dismiss="alert" aria-label="close">
                 <span aria-hidden="true">&times</span>
@@ -43,26 +45,26 @@
                                 </label>
 
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3"></textarea>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <div class="form-group form-row">
                                 <label for="eft" class="col-sm-2 control-label">
                                     {% translate "Fitting" %}
                                 </label>
 
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <textarea class="form-control" name="eft" id="eft" rows="5"></textarea>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/create_category.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_category.html`

 * *Files 6% similar despite different names*

```diff
@@ -15,103 +15,104 @@
             border: none;
             height:100%;
             width: 100%;
         }
     </style>
 {% endblock %}
 
-{% block page_title %}{% translate "Add Category" %}{% endblock %}
+{% block page_title %}{% translate "Edit Category" %}{% endblock %}
 
 {% block fittings_block %}
     <div>
         <div class="panel panel-primary">
             <div class="panel-heading">
-                <div class="panel-title">{% translate "New Category" %}</div>
+                <div class="panel-title">{% translate "Edit Category" %}</div>
             </div>
 
             <div class="panel-body">
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form" role="form" action="" method="POST">
                             {% csrf_token %}
 
                             <div class="row">
                                 <div class="col-sm-10">
                                     <div class="form-group">
                                         <label for="name">{% translate "Category Name" %}</label>
-                                        <input type="text" class="form-control" name="name" id="name" required/>
+                                        <input type="text" class="form-control" name="name" id="name" value="{{cat.name}}" required>
                                     </div>
                                 </div>
 
                                 <div class="col-sm-2">
                                     <div class="form-group">
                                         <label for="color">{% translate "Category Color" %}</label>
-                                        <div class="form-control col-sm-1" id="color-wrapper" style="padding:0 !important;">
-                                            <input type="color" name="color" id="color" value="#39CCCC" required/>
+
+                                        <div class="form-control col-sm-1" id="color-wrapper" style="padding: 0 !important;">
+                                            <input type="color" name="color" id="color" value="{{cat.color}}" required>
                                         </div>
                                     </div>
                                 </div>
                             </div>
 
                             <div class="row">
                                 <div class="col-sm-12">
                                     <div class="form-group">
                                         <label for="groupSelect" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
 
                                         <span class="help-block" style="margin-top: 0; margin-bottom: 0; font-size: 10pt; font-style: italic;">{% translate "Only selected groups will have access to fittings and doctrines in this category. If no groups are selected the category will be visible to all with fittings module access." %}</span>
 
                                         <select name="groupSelect" id="groupSelect" multiple>
                                             {% for group in groups %}
-                                            <option value="{{group.pk}}">{{group.name}}</option>
+                                            <option value="{{group.pk}}" {% if group in cat.groups.all %} selected {%endif%}>{{group.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
 
                             <div class="row">
                                 <div class="col-sm-6">
                                     <div class="form-group">
                                         <label for="fitSelect">{% translate "Select Fits" %}</label>
 
                                         <select name="fitSelect" id="fitSelect" multiple>
                                             {% for fit in fits %}
-                                            <option value="{{fit.pk}}">{{fit.name}}</option>
+                                            <option value="{{fit.pk}}" {% if fit in cat.fittings.all %} selected {% endif %}>{{fit.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
 
                                 <div class="col-sm-6">
                                     <div class="form-group">
                                         <label for="docSelect">{% translate "Select Doctrines" %}</label>
 
                                         <select name="docSelect" id="docSelect" multiple>
                                             {% for doc in docs %}
-                                            <option value="{{doc.pk}}">{{doc.name}}</option>
+                                            <option value="{{doc.pk}}" {% if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js' %}"></script>
 
-    <script type="application/javascript">
+    <script>
         let color_picker = document.getElementById("color");
         let color_picker_wrapper = document.getElementById("color-wrapper");
 
         color_picker.onchange = function () {
             color_picker_wrapper.style.backgroundColor = color_picker.value;
         }
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
 filters %} {% load static %} {% block more_css %}
- {% endblock %} {% block page_title %}{% translate "Add Category" %}{% endblock
-%} {% block fittings_block %}
-{% translate "New Category" %}
+ {% endblock %} {% block page_title %}{% translate "Edit Category" %}{%
+endblock %} {% block fittings_block %}
+{% translate "Edit Category" %}
 {% csrf_token %}
-{% translate "Category Name" %} [name                ]
+{% translate "Category Name" %} [{{cat.name}}        ]
 {% translate "Category Color" %}
 [Unknown INPUT type]
 {% for group in groups %}
-{{group.name}}
+% if group in cat.groups.all %} selected {%endif%}>{{group.name}}
 {% endfor %}
 {% for fit in fits %}
-{{fit.name}}
+% if fit in cat.fittings.all %} selected {% endif %}>{{fit.name}}
 {% endfor %}
 {% for doc in docs %}
-{{doc.name}}
+% if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}
 {% endfor %}
 
 {% translate "Submit" %}
 {% endblock %} {% block extra_javascript %}
  {% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/dashboard.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/dashboard.html`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         <div class="panel panel-default">
             <div class="panel-heading">
                 <div class="panel-title">{% translate "Doctrines" %}</div>
             </div>
 
             <div class="panel-body">
                 {% if not docs %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Doctrines Found" %} </div>
+                    <div class="alert alert-warning text-center">{% translate "No Doctrines Found" %}</div>
                 {% else %}
                     <table class="table table-striped table-hover dataTable" id="docTable">
                         <thead>
                             <tr>
                                 <th> </th>
                                 <th>{% translate "Name" %}</th>
                                 <th>{% translate "Categories" %}</th>
@@ -51,27 +51,29 @@
                         </thead>
 
                         <tbody>
                             {% for doc in docs %}
                                 <tr>
                                     <td>
                                         <a href="{% url 'fittings:view_doctrine' doc.pk %}">
-                                            <img src="{{ doc.icon_url }}" class="img-rounded" style="display: block; margin: auto;"/>
+                                            <img src="{{ doc.icon_url }}" class="img-rounded" style="display: block; margin: auto;" alt="{{ doc.name }}">
                                         </a>
                                     </td>
                                     <td> <a href="{% url 'fittings:view_doctrine' doc.pk %}">{{ doc.name }}</a> </td>
                                     <td>
                                         {% for cat in doc.category.all %}
-                                            <span class="label" style="background-color: {{ cat.color }}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
+                                            <span class="label" style="background-color: {{ cat.color }};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
                                         {% endfor %}
                                     </td>
-                                    <td> {{ doc.description|linebreaks|urlize }} </td>
+                                    <td>
+                                        {{ doc.description|linebreaks|urlize }}
+                                    </td>
                                     <td>
                                         {% for fitting in doc_dict|get_item:doc.pk %}
-                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-rounded" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.type_name }}"/>
+                                            <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-rounded" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.name }}" alt="{{ fitting.ship_type.name }}">
                                         {% endfor %}
                                     </td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 {% endif %}
@@ -79,23 +81,22 @@
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         $(document).ready(function(){
             {% if docs %}
                 $('#docTable').DataTable({
-                    "order": [[ 1, "asc" ]],
+                    language: {
+                        url: '{{ STATIC_URL }}/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/{{ LANGUAGE_CODE }}.json'
+                    },
+                    order: [[ 1, "asc" ]],
                 });
             {% endif %}
 
             $('[data-toggle="tooltip"]').tooltip();
         });
     </script>
 {% endblock %}
-
-{% block extra_script %}
-
-{% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_category.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/create_category.html`

 * *Files 12% similar despite different names*

```diff
@@ -15,115 +15,129 @@
             border: none;
             height:100%;
             width: 100%;
         }
     </style>
 {% endblock %}
 
-{% block page_title %}{% translate "Edit Category" %}{% endblock %}
+{% block page_title %}{% translate "Add Category" %}{% endblock %}
 
 {% block fittings_block %}
     <div>
         <div class="panel panel-primary">
             <div class="panel-heading">
-                <div class="panel-title">{% translate "Edit Category" %}</div>
+                <div class="panel-title">{% translate "New Category" %}</div>
             </div>
 
             <div class="panel-body">
                 <div class="row">
                     <div class="col-md-10 col-md-offset-1">
                         <form class="form" role="form" action="" method="POST">
                             {% csrf_token %}
 
                             <div class="row">
                                 <div class="col-sm-10">
                                     <div class="form-group">
                                         <label for="name">{% translate "Category Name" %}</label>
-                                        <input type="text" class="form-control" name="name" id="name" value="{{cat.name}}" required/>
+                                        <input type="text" class="form-control" name="name" id="name" required>
                                     </div>
                                 </div>
 
                                 <div class="col-sm-2">
                                     <div class="form-group">
                                         <label for="color">{% translate "Category Color" %}</label>
-
                                         <div class="form-control col-sm-1" id="color-wrapper" style="padding:0 !important;">
-                                            <input type="color" name="color" id="color" value="{{cat.color}}" required/>
+                                            <input type="color" name="color" id="color" value="#39CCCC" required>
                                         </div>
                                     </div>
                                 </div>
                             </div>
 
                             <div class="row">
                                 <div class="col-sm-12">
                                     <div class="form-group">
                                         <label for="groupSelect" style="margin-bottom: 0;">{% translate "Select Groups" %}</label>
 
                                         <span class="help-block" style="margin-top: 0; margin-bottom: 0; font-size: 10pt; font-style: italic;">{% translate "Only selected groups will have access to fittings and doctrines in this category. If no groups are selected the category will be visible to all with fittings module access." %}</span>
 
                                         <select name="groupSelect" id="groupSelect" multiple>
                                             {% for group in groups %}
-                                            <option value="{{group.pk}}" {% if group in cat.groups.all %} selected {%endif%}>{{group.name}}</option>
+                                            <option value="{{group.pk}}">{{group.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
 
                             <div class="row">
                                 <div class="col-sm-6">
                                     <div class="form-group">
                                         <label for="fitSelect">{% translate "Select Fits" %}</label>
 
                                         <select name="fitSelect" id="fitSelect" multiple>
                                             {% for fit in fits %}
-                                            <option value="{{fit.pk}}" {% if fit in cat.fittings.all %} selected {% endif %}>{{fit.name}}</option>
+                                            <option value="{{fit.pk}}">{{fit.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
 
                                 <div class="col-sm-6">
                                     <div class="form-group">
                                         <label for="docSelect">{% translate "Select Doctrines" %}</label>
 
                                         <select name="docSelect" id="docSelect" multiple>
                                             {% for doc in docs %}
-                                            <option value="{{doc.pk}}" {% if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}</option>
+                                            <option value="{{doc.pk}}">{{doc.name}}</option>
                                             {% endfor %}
                                         </select>
                                     </div>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/slim-select/1.26.0/dist/slimselect.min.js' %}"></script>
 
-    <script type="application/javascript">
-        let color_picker = document.getElementById("color");
-        let color_picker_wrapper = document.getElementById("color-wrapper");
+    <script>
+        const color_picker = document.getElementById('color');
+        const color_picker_wrapper = document.getElementById('color-wrapper');
 
-        color_picker.onchange = function () {
+        color_picker.onchange = function() {
             color_picker_wrapper.style.backgroundColor = color_picker.value;
         }
-
         color_picker_wrapper.style.backgroundColor = color_picker.value;
 
         new SlimSelect({
             select: "#groupSelect",
-            hideSelectedOption: true
+            hideSelectedOption: true,
+            placeholder: '{% translate "Select Value" %}',
+            searchText: '{% translate "No Results" %}',
+            searchPlaceholder: '{% translate "Search" %}'
         });
 
-        new SlimSelect({select: "#fitSelect", hideSelectedOption: true});
-        new SlimSelect({select: "#docSelect", hideSelectedOption: true});
+        new SlimSelect({
+            select: "#fitSelect",
+            hideSelectedOption: true,
+            placeholder: '{% translate "Select Value" %}',
+            searchText: '{% translate "No Results" %}',
+            searchPlaceholder: '{% translate "Search" %}'
+        });
+
+        new SlimSelect({
+            select: "#docSelect",
+            hideSelectedOption: true,
+            placeholder: '{% translate "Select Value" %}',
+            searchText: '{% translate "No Results" %}',
+            searchPlaceholder: '{% translate "Search" %}'
+        });
     </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
 filters %} {% load static %} {% block more_css %}
- {% endblock %} {% block page_title %}{% translate "Edit Category" %}{%
-endblock %} {% block fittings_block %}
-{% translate "Edit Category" %}
+ {% endblock %} {% block page_title %}{% translate "Add Category" %}{% endblock
+%} {% block fittings_block %}
+{% translate "New Category" %}
 {% csrf_token %}
-{% translate "Category Name" %} [{{cat.name}}        ]
+{% translate "Category Name" %} [name                ]
 {% translate "Category Color" %}
 [Unknown INPUT type]
 {% for group in groups %}
-% if group in cat.groups.all %} selected {%endif%}>{{group.name}}
+{{group.name}}
 {% endfor %}
 {% for fit in fits %}
-% if fit in cat.fittings.all %} selected {% endif %}>{{fit.name}}
+{{fit.name}}
 {% endfor %}
 {% for doc in docs %}
-% if doc in cat.doctrines.all %} selected {% endif %}>{{doc.name}}
+{{doc.name}}
 {% endfor %}
 
 {% translate "Submit" %}
 {% endblock %} {% block extra_javascript %}
  {% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_doctrine.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_doctrine.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
 
 {% block more_css %}
-    <link rel="stylesheet" href="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css' %}" />
+    <link rel="stylesheet" href="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/css/multi-select.min.css' %}">
 
     <style>
         .ms-container {
             width: 100% !important;
         }
     </style>
 {% endblock %}
@@ -47,15 +47,15 @@
                         <form class="form-signin" role="form" action="" method="POST">
                             {% csrf_token %}
 
                             <div class="form-group">
                                 <label for="name" class="col-sm-2 control-label">{% translate "Doctrine Name" %}</label>
 
                                 <div class="col-sm-10">
-                                    <input type="text" class="form-control" name="name" id="name" value="{{ doctrine.name }}" required/>
+                                    <input type="text" class="form-control" name="name" id="name" value="{{ doctrine.name }}" required>
                                 </div>
                             </div>
 
                             <div class="form-group">
                                 <label for="description" class="col-sm-2 control-label">{% translate "Doctrine Description" %}</label>
 
                                 <div class="col-sm-10">
@@ -84,63 +84,71 @@
                                 <div class="col-sm-10">
                                     <select class="form-control" name="iconSelect" id="iconSelect" aria-describedby="helpBlock">
                                         <option value="{{ doctrine.icon_url }}" selected> {% translate "Current Icon" %} </option>
                                         {% for ship in ships %}
                                             <option value="{{ ship.ship_type|type_render_url:64 }}">{{ship.ship_type__type_name}}</option>
                                         {% endfor %}
                                     </select>
-                                    <span id="helpBlock" class="help-block"> {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}</span>
+
+                                    <span id="helpBlock" class="help-block">
+                                        {% translate "If you do not see the ship type that you would like to use for the icon, add a fit that uses that ship type and try again." %}
+                                    </span>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/multi-select/0.9.12/js/jquery.multi-select.min.js' %}"></script>
     <script type="application/javascript" src="{% static 'sev3rance_auth_templates/libs/quicksearch/2.4.0/dist/jquery.quicksearch.min.js' %}"></script>
 
-    <script type="application/javascript">
+    <script>
+        const translation_search = '{% translate "Search" %}';
+
         $('#fitSelect').multiSelect({
-            selectableHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
-            selectionHeader: "<input type='text' class='form-control' autocomplete='off' placeholder='Search' style='margin-bottom: 3px;'>",
-            afterInit: function(ms) {
+            selectableHeader: '<input type="text" class="form-control" autocomplete="off" placeholder="' + translation_search + '" style="margin-bottom: 3px;">',
+            selectionHeader: '<input type="text" class="form-control" autocomplete="off" placeholder="' + translation_search + '" style="margin-bottom: 3px;">',
+
+            afterInit: function (ms) {
                 let that = this,
                     $selectableSearch = that.$selectableUl.prev(),
                     $selectionSearch = that.$selectionUl.prev(),
                     selectableSearchString = '#'+that.$container.attr('id')+' .ms-elem-selectable:not(.ms-selected)',
                     selectionSearchString = '#'+that.$container.attr('id')+' .ms-elem-selection.ms-selected';
 
-                that.qs1 = $selectableSearch.quicksearch(selectableSearchString) .on('keydown', function(e) {
-                    if (e.which === 40){
-                        that.$selectableUl.focus();
-
-                        return false;
-                    }
-                });
-
-                that.qs2 = $selectionSearch.quicksearch(selectionSearchString).on('keydown', function(e) {
-                    if (e.which === 40){
-                        that.$selectionUl.focus();
-
-                        return false;
-                    }
-                });
+                that.qs1 = $selectableSearch.quicksearch(selectableSearchString)
+                    .on('keydown', function (e) {
+                        if (e.which === 40){
+                            that.$selectableUl.focus();
+
+                            return false;
+                        }
+                    });
+
+                that.qs2 = $selectionSearch.quicksearch(selectionSearchString)
+                    .on('keydown', function (e) {
+                        if (e.which === 40) {
+                            that.$selectionUl.focus();
+
+                            return false;
+                        }
+                    });
             },
-            afterSelect: function() {
+            afterSelect: function () {
                 this.qs1.cache();
                 this.qs2.cache();
             },
-            afterDeselect: function() {
+            afterDeselect: function () {
                 this.qs1.cache();
                 this.qs2.cache();
             }
         });
     </script>
 {% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/edit_fit.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/edit_fit.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'fittings/base.html' %}
+
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 
 {% block page_title %}{% translate "Update Fitting" %}{% endblock %}
 
 {% block fittings_block %}
@@ -38,24 +39,24 @@
                                 <label for="description" class="col-sm-2 control-label">{% translate "Description" %}</label>
 
                                 <div class="col-sm-10">
                                     <textarea class="form-control" name="description" id="description" maxlength="500" rows="3">{{ fit.description }}</textarea>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <div class="form-group" >
                                 <label for="eft" class="col-sm-2 control-label">{% translate "Fit" %}</label>
 
                                 <div class="col-sm-10" style="margin-top: 5px; margin-bottom: 5px;">
                                     <textarea class="form-control" name="eft" id="eft" rows="5">{{ fit.eft }}</textarea>
                                 </div>
                             </div>
 
-                            <br />
+                            <br>
                             <button class="btn btn-primary btn-block" type="submit">{% translate "Submit" %}</button>
                         </form>
                     </div>
                 </div>
             </div>
         </div>
     </div>
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_all_categories.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_all_categories.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'fittings/base.html' %}
+
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 
-
 {% block page_title %}{% translate "View All Categories" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
         <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
             <button type="button" class="close" data-dismiss="alert" aria-label="close">
                 <span aria-hidden="true">&times</span>
@@ -31,49 +31,52 @@
         <div class="panel panel-default">
             <div class="panel-heading">
                 <div class="panel-title">{% translate "Fits" %}</div>
             </div>
 
             <div class="panel-body">
                 {% if not cats %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Categories Found" %}</div>
+                    <div class="alert alert-warning text-center">{% translate "No Categories Found" %}</div>
                 {% else %}
                     <table class="table table-striped table-hover dataTable" id="fitTable">
                         <thead>
-                            <th>{% translate "Name" %}</th>
-                            <th>{% translate "Doctrines Assigned" %}</th>
-                            <th>{% translate "Fittings Assigned" %}</th>
-                            {% if perms.fittings.manage %}
-                                <th>{% translate "Groups Assigned" %}</th>
-                                <th> </th>
-                            {% endif %}
+                            <tr>
+                                <th>{% translate "Name" %}</th>
+                                <th>{% translate "Doctrines Assigned" %}</th>
+                                <th>{% translate "Fittings Assigned" %}</th>
+
+                                {% if perms.fittings.manage %}
+                                    <th>{% translate "Groups Assigned" %}</th>
+                                    <th> </th>
+                                {% endif %}
+                            </tr>
                         </thead>
 
                         <tbody>
-                            {% for cat in cats %}
-                                <tr>
-                                    <td> <span class="label" style="background-color: {{cat.color}}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span> </td>
-                                    <td> {{ cat.doctrines_count }}</td>
-                                    <td> {{ cat.total_fits }} </td>
-                                    {% if perms.fittings.manage %}
-                                        <td> {{ cat.groups_count }}</td>
-                                        <td>
-                                            <a href="{% url 'fittings:view_category' cat.pk %}" type="button" class="btn btn-sm btn-primary" data-toggle="tooltip" data-placement="top" title="{% translate 'View Category' %}">
-                                                <span class="fa fas fa-eye"></span>
-                                            </a>
-                                            <a href="{% url 'fittings:edit_category' cat.pk %}" type="button" class="btn btn-sm btn-warning" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Category' %}">
-                                                <span class="fa fas fa-pencil-alt"></span>
-                                            </a>
-                                            <a href="{% url 'fittings:delete_category' cat.pk %}" type="button" class="btn btn-sm btn-danger" data-toggle="tooltip" data-placement="top" title="{% translate 'Delete Category' %}">
-                                                <span class="fa fas fa-times"></span>
-                                            </a>
-                                        </td>
-                                    {% endif %}
-                                </tr>
-                            {% endfor %}
+                        {% for cat in cats %}
+                            <tr>
+                                <td> <span class="label" style="background-color: {{cat.color}};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{cat.name}}</a></span> </td>
+                                <td> {{ cat.doctrines_count }}</td>
+                                <td> {{ cat.total_fits }} </td>
+                                {% if perms.fittings.manage %}
+                                    <td> {{ cat.groups_count }}</td>
+                                    <td>
+                                        <a href="{% url 'fittings:view_category' cat.pk %}" type="button" class="btn btn-sm btn-primary" data-toggle="tooltip" data-placement="top" title="{% translate 'View Category' %}">
+                                            <span class="fa fas fa-eye"></span>
+                                        </a>
+                                        <a href="{% url 'fittings:edit_category' cat.pk %}" type="button" class="btn btn-sm btn-warning" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Category' %}">
+                                            <span class="fa fas fa-pencil-alt"></span>
+                                        </a>
+                                        <a href="{% url 'fittings:delete_category' cat.pk %}" type="button" class="btn btn-sm btn-danger" data-toggle="tooltip" data-placement="top" title="{% translate 'Delete Category' %}">
+                                            <span class="fa fas fa-times"></span>
+                                        </a>
+                                    </td>
+                                {% endif %}
+                            </tr>
+                        {% endfor %}
                         </tbody>
                     </table>
 
                     <h6>
                         <i class="fas fa-exclamation-triangle"></i>
                         <i>{% translate "*Note: Fit counts may be inaccurate as fits marked independently of doctrines may be counted more than once." %}</i>
                     </h6>
@@ -81,21 +84,22 @@
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
-    <script type="application/javascript">
+
+    <script>
         $(document).ready(function() {
             {% if cats %}
-                $('#fitTable').DataTable();
+                $('#fitTable').DataTable({
+                    language: {
+                        url: '{{ STATIC_URL }}/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/{{ LANGUAGE_CODE }}.json'
+                    },
+                });
             {% endif %}
 
             $('[data-toggle="tooltip"]').tooltip();
         });
     </script>
 {% endblock %}
-
-{% block extra_script %}
-
-{% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_all_fits.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_all_fits.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 {% extends 'fittings/base.html' %}
+
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
 {% load evelinks %}
 
-{% block page_title %}{% translate "View All Fits" %}{% endblock %}
+{% block page_title %}{% translate "View All Fittings" %}{% endblock %}
 
 {% block fittings_block %}
     {% if msg %}
         <div class="alert alert-{{ msg.0 }} alert-dismissible" role="alert">
             <button type="button" class="close" data-dismiss="alert" aria-label="close">
                 <span aria-hidden="true">&times</span>
             </button>
@@ -35,15 +36,15 @@
         <div class="panel panel-default">
             <div class="panel-heading">
                 <div class="panel-title">{% translate "Fits" %}</div>
             </div>
 
             <div class="panel-body">
                 {% if not fits %}
-                    <div class="alert alert-warning" style="text-align: center">{% translate "No Fits Found" %}</div>
+                    <div class="alert alert-warning text-center">{% translate "No Fittings Found" %}</div>
                 {% else %}
                     <table class="table table-striped table-hover dataTable" id="fitTable">
                         <thead>
                             <tr>
                                 <th>{% translate "Ship Type" %}</th>
                                 <th>{% translate "Name" %}</th>
                                 <th>{% translate "Categories" %}</th>
@@ -52,22 +53,26 @@
                         </thead>
 
                         <tbody>
                             {% for fit in fits %}
                                 <tr>
                                     <td>
                                         <a href="{% url 'fittings:view_fit' fit.pk %}" class="text-decoration-none d-inline-block">
-                                            <img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}">
+                                            <img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}" alt="{{ fit.ship_type.type_name }}">
                                         </a>
                                         {{ fit.ship_type.type_name }}
                                     </td>
-                                    <td><a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a></td>
+                                    <td>
+                                        <a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a>
+                                    </td>
                                     <td>
                                         {% for cat in cats|get_item:fit.pk %}
-                                        <span class="label" style="background-color: {{ cat.color }}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
+                                            <span class="label" style="background-color: {{ cat.color }};">
+                                                <a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a>
+                                            </span>
                                         {% endfor %}
                                     </td>
                                     <td>{{ fit.description|linebreaks|urlize }}</td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
@@ -76,21 +81,21 @@
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         $(document).ready(function() {
             {% if fits %}
-                $('#fitTable').DataTable();
+                $('#fitTable').DataTable({
+                    language: {
+                        url: '{{ STATIC_URL }}/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/{{ LANGUAGE_CODE }}.json'
+                    },
+                });
             {% endif %}
 
             $('[data-toggle="tooltip"]').tooltip();
         });
     </script>
 {% endblock %}
-
-{% block extra_script %}
-
-{% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_category.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_category.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 {% extends 'fittings/base.html' %}
 
 {% load i18n %}
 {% load humanize %}
 {% load filters %}
-{% load static %}
 {% load evelinks %}
 
 {% block more_css %}
     <style>
         .tp {
             padding-bottom: 0;
         }
@@ -20,14 +19,15 @@
             padding-left: 15px;
             padding-right: 15px;
         }
         .mv {
             margin-left: 15px;
         }
     </style>
+
     {% include 'bundles/datatables-css.html' %}
 {% endblock %}
 
 {% block page_title %}{% translate "View Category" %}{% endblock %}
 
 {% block fittings_block %}
     <div>
@@ -47,24 +47,26 @@
                         </div>
                     {% endif %}
                 </div>
             </div>
 
             <div class="panel-body tp">
                 <strong>{% translate "Name" %}: </strong>
-                <br/>
-                <span class="label" style="background-color: {{cat.color}}">{{cat.name}}</span>
+                <br>
+                <span class="label" style="background-color: {{cat.color}};">{{cat.name}}</span>
 
                 <div id="spacer" style="padding-top: 5px;"></div>
                 {% if perms.fittings.manage %}
                     <strong>{% translate "Groups" %}: </strong>
-                    <br />
+                    <br>
 
                     {% if cat.groups.all|length != 0 %}
-                        {% for group in cat.groups.all %} <span class="label label-primary">{{group.name}}</span> {% endfor %}
+                        {% for group in cat.groups.all %}
+                            <span class="label label-primary">{{group.name}}</span>
+                        {% endfor %}
                     {% else %}
                         <span class="label label-warning">{% translate "Category is public" %}</span>
                     {% endif %}
                 {% endif %}
             </div>
 
             <p>&nbsp;</p>
@@ -88,39 +90,43 @@
                                 </tr>
                             </thead>
 
                             <tbody>
                                 {% if not docs %}
                                     <tr>
                                         <td colspan="5">
-                                            <div class="alert alert-warning" style="text-align: center"> {% translate "No Doctrines Found" %} </div>
+                                            <div class="alert alert-warning text-center">
+                                                {% translate "No Doctrines Found" %}
+                                            </div>
                                         </td>
                                     </tr>
                                 {% else %}
                                     {% for doc in docs %}
                                         <tr>
                                             <td>
                                                 <a href="{% url 'fittings:view_doctrine' doc.pk %}">
-                                                    <img src="{{ doc.icon_url }}" class="img-rounded" style="display: block; margin: auto;"/>
+                                                    <img src="{{ doc.icon_url }}" class="img-rounded" style="display: block; margin: auto;" alt="{{ doc.name }}">
                                                 </a>
                                             </td>
                                             <td>
                                                 <a href="{% url 'fittings:view_doctrine' doc.pk %}">{{ doc.name }}</a>
                                             </td>
                                             <td>
                                                 {% for cate in doc.category.all %}
-                                                    <span class="label" style="background-color: {{ cate.color }}">
+                                                    <span class="label" style="background-color: {{ cate.color }};">
                                                         <a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{ cate.name }}</a>
                                                     </span>
                                                 {% endfor %}
                                             </td>
-                                            <td> {{ doc.description|linebreaks|urlize }} </td>
+                                            <td>
+                                                {{ doc.description|linebreaks|urlize }}
+                                            </td>
                                             <td>
                                                 {% for fitting in doc_dict|get_item:doc.pk %}
-                                                    <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-rounded" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.type_name }}"/>
+                                                    <img src="{{ fitting.ship_type_type_id|type_render_url:32 }}" class="img-rounded" data-toggle="tooltip" data-placement="bottom" title="{{ fitting.ship_type.type_name }}" alt="{{ fitting.ship_type.type_name }}">
                                                 {% endfor %}
                                             </td>
                                         </tr>
                                     {% endfor %}
                                 {% endif %}
                             </tbody>
                         </table>
@@ -137,30 +143,35 @@
                                 </tr>
                             </thead>
 
                             <tbody>
                                 {% if not fits %}
                                     <tr>
                                         <td colspan="4">
-                                            <div class="alert alert-warning" style="text-align: center"> {% translate "No Fits Found" %} </div>
+                                            <div class="alert alert-warning text-center">
+                                                {% translate "No Fits Found" %}
+                                            </div>
                                         </td>
                                     </tr>
                                 {% else %}
                                     {% for fit in fits %}
                                         <tr>
                                             <td><a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a></td>
                                             <td>
                                                 {% for cate in cats|get_item:fit.pk %}
-                                                    <span class="label" style="background-color: {{ cate.color }}">
+                                                    <span class="label" style="background-color: {{ cate.color }};">
                                                         <a href="{% url 'fittings:view_category' cate.pk %}" class="nostyle">{{ cate.name }}</a>
                                                     </span>
                                                 {% endfor %}
                                             </td>
                                             <td>{{ fit.description|linebreaks|urlize }}</td>
-                                            <td><img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:128 }}" style="height: 32px; width: 32px;" title="{{ fit.ship_type.type_name }}"> {{ fit.ship_type.type_name }}</td>
+                                            <td>
+                                                <img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:128 }}" style="height: 32px; width: 32px;" title="{{ fit.ship_type.type_name }}" alt="{{ fit.ship_type.type_name }}">
+                                                {{ fit.ship_type.type_name }}
+                                            </td>
                                         </tr>
                                     {% endfor %}
                                 {% endif %}
                             </tbody>
                         </table>
                     </div>
                 </div>
@@ -168,15 +179,15 @@
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         $(document).ready(function() {
             {% if docs %}
                 $('#docTable').DataTable({
                     "order": [[ 1, "asc" ]],
                 });
             {% endif %}
 
@@ -184,11 +195,7 @@
                 $('#fitTable').DataTable();
             {% endif %}
 
             $('[data-toggle="tooltip"]').tooltip();
         });
     </script>
 {% endblock %}
-
-{% block extra_script %}
-
-{% endblock %}
```

#### html2text {}

```diff
@@ -1,37 +1,40 @@
 {% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% load evelinks %} {% block more_css %}
+filters %} {% load evelinks %} {% block more_css %}
  {% include 'bundles/datatables-css.html' %} {% endblock %} {% block page_title
 %}{% translate "View Category" %}{% endblock %} {% block fittings_block %}
 {% translate "Category" %} {% if perms.fittings.manage %}
 
 {% endif %}
 {% translate "Name" %}:
 {{cat.name}}
 {% if perms.fittings.manage %} {% translate "Groups" %}:
 {% if cat.groups.all|length != 0 %} {% for group in cat.groups.all %} {
 {group.name}} {% endfor %} {% else %} {% translate "Category is public" %} {%
 endif %} {% endif %}
  
     * {%_translate_"Doctrines"_%}
     * {%_translate_"Fittings"_%}
-             {%        {% translate
-             translate "Categories" %}  {% translate "Description" %}     {% translate "Ships" %}
-             "Name" %}
+         {%        {% translate
+         translate "Categories" %}  {% translate "Description" %}     {% translate "Ships" %}
+         "Name" %}
 {% translate "No Doctrines Found" %}
-[{           {         {% for cate in   {                                 {% for fitting in doc_dict|get_item:doc.pk
-{            {         doc.category.all {                                 %} [{
-doc.icon_url doc.name  %}  {{_cate.name doc.description|linebreaks|urlize {
-}}]          }}        }}  {% endfor %} }}                                fitting.ship_type_type_id|type_render_url:
-                                                                          32 }}] {% endfor %}
-{%        {% translate
-translate "Categories"   {% translate "Description" %}     {% translate "Ship Type" %}
+                                                                      {% for fitting in
+[{       {         {% for cate in   {                                 doc_dict|get_item:doc.pk %}
+{        {         doc.category.all {                                 [{
+doc.name doc.name  %}  {{_cate.name doc.description|linebreaks|urlize {
+}}]      }}        }}  {% endfor %} }}                                fitting.ship_type.type_name
+                                                                      }}] {% endfor %}
+{%        {% translate                                     {% translate "Ship
+translate "Categories"   {% translate "Description" %}     Type" %}
 "Name" %} %}
 {% translate "No Fits Found" %}
-{         {% for cate in {                                 [{
-{         cats|get_item: {                                 {
-fit.name  fit.pk %}  {   fit.description|linebreaks|urlize fit.ship_type_type_id|type_render_url:
-}}        {_cate.name_}} }}                                128 }}] {{ fit.ship_type.type_name }}
-          {% endfor %}
+                                                           [{
+{         {% for cate in {                                 {
+{         cats|get_item: {                                 fit.ship_type.type_name
+fit.name  fit.pk %}  {   fit.description|linebreaks|urlize }}] {
+}}        {_cate.name_}} }}                                {
+          {% endfor %}                                     fit.ship_type.type_name
+                                                           }}
 {% endblock %} {% block extra_javascript %} {% include 'bundles/datatables-
 js.html' %}
- {% endblock %} {% block extra_script %} {% endblock %}
+ {% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_doctrine.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_doctrine.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 {% extends 'fittings/base.html' %}
 
 {% load i18n %}
-{% load humanize %}
 {% load filters %}
-{% load static %}
 {% load evelinks %}
 
 {% block page_title %}{{ doctrine.name }} {% translate "Doctrine" %}{% endblock %}
 
 {% block fittings_block %}
     {# modal start #}
     <div class="modal fade" id="deleteModal" role="dialog" tabindex="-1" aria-labelledby="modalTitle">
@@ -15,128 +13,148 @@
             <div class="modal-content">
                 <div class="modal-header">
                     <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                     <h4 class="modal-title" id="modalTitle">{% translate "Are you sure?" %}</h4>
                 </div>
 
                 <div class="modal-body">
-                    <p style="white-space: pre-line">
+                    <p style="white-space: pre-line;">
                         {% translate "Are you sure you wish to delete this doctrine?" %}
                         <i><strong>{% translate "This action is permanent." %}</strong></i>
                     </p>
                 </div>
 
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">{% translate "No - Close" %}</button>
                     <a href="{% url 'fittings:delete_doctrine' doctrine.pk %}" type="button" class="btn btn-danger">{% translate "Yes - Delete" %}</a>
                 </div>
             </div>
         </div>
     </div>
     {# modal end #}
 
-    <br />
+    <br>
     <div class="row">
         <div class="col-md-3">
             <div class="panel panel-primary">
                 <div class="panel-heading">
                     <div class="panel-title">
                         {% translate "Doctrine Information" %}
 
                         {% if perms.fittings.manage %}
                             <span data-toggle="modal" data-target="#deleteModal">
                                 <button class="btn btn-xs btn-danger" style="float: right; margin-left: 5px;" data-toggle="tooltip" data-placement="top" title="{% translate 'Delete Doctrine' %}"><span class="fa fas fa-times"></span> </button>
                             </span>
-                            <a href="{% url 'fittings:edit_doctrine' doctrine.pk %}" class="btn btn-xs btn-warning" style="float: right" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Doctrine' %}"><span class="fa fas fa-pencil-alt"></span> </a>
+                            <a href="{% url 'fittings:edit_doctrine' doctrine.pk %}" class="btn btn-xs btn-warning" style="float: right;" data-toggle="tooltip" data-placement="top" title="{% translate 'Edit Doctrine' %}"><span class="fa fas fa-pencil-alt"></span> </a>
                         {% endif %}
                     </div>
                 </div>
 
                 <div class="panel-body">
-                    <img src="{{ doctrine.icon_url }}" class="img-rounded center-block" style="text-align: center"/>
-                    <div style="text-align: center">{{ doctrine.name }}</div>
-                    <div style="text-align: center">
+                    <img src="{{ doctrine.icon_url }}" class="img-rounded center-block text-center" alt="{{ doctrine.name }}">
+                    <div class="text-center">{{ doctrine.name }}</div>
+                    <div class="text-center">
                         {% for cat in d_cats %}
-                            <span class="label" style="background-color: {{ cat.color }}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
+                            <span class="label" style="background-color: {{ cat.color }};"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
                         {% endfor %}
                     </div>
 
-                    <hr />
+                    <hr>
 
                     <dl>
                         <dt>{% translate "Description" %}</dt>
                         <dd>{{ doctrine.description|break_html_lines|striptags }}</dd>
-                        <dt>{% translate "Created" %}</dt>
-                        <dd>{{ doctrine.created|date:'d M Y H:i:s' }}</dd>
+
+                        {% if doctrine.created %}
+                            <dt>{% translate "Created" %}</dt>
+                            {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                                <dd>{{ doctrine.created|date:'Y-m-d / H:i:s' }}</dd>
+                            {% else %}
+                                <dd>{{ doctrine.created|date:'d M Y H:i:s' }}</dd>
+                            {% endif %}
+                        {% endif %}
+
                         {% if doctrine.last_updated %}
                             <dt>{% translate "Last Updated" %}</dt>
-                            <dd>{{ doctrine.last_updated|date:'d M Y H:i:s' }}</dd>
+                            {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                                <dd>{{ doctrine.last_updated|date:'Y-m-d / H:i:s' }}</dd>
+                            {% else %}
+                                <dd>{{ doctrine.last_updated|date:'d M Y H:i:s' }}</dd>
+                            {% endif %}
                         {% endif %}
                     </dl>
                 </div>
             </div>
         </div>
 
         <div class="col-md-9">
             <div class="panel panel-default">
                 <div class="panel-heading">
                     <div class="panel-title">{% translate "Doctrine Fits" %}</div>
                 </div>
 
                 <div class="panel-body">
                     {% if not fits %}
-                        <div class="alert alert-warning" style="text-align: center">{% translate "No Fits Found" %}</div>
+                        <div class="alert alert-warning text-center">{% translate "No Fits Found" %}</div>
                     {% else %}
-                        <table class="table table-striped table-hover dataTable" id="fitsTable">
+                        <table class="table table-hover dataTable" id="fitsTable">
                             <thead>
                                 <tr>
                                     <th>{% translate "Ship Type" %}</th>
                                     <th>{% translate "Name" %}</th>
                                     <th>{% translate "Category" %}</th>
                                     <th>{% translate "Description" %}</th>
                                 </tr>
                             </thead>
 
                             <tbody>
-                                {% for fit in fits %}
-                                    <tr>
-                                        <td>
-                                            <a href="{% url 'fittings:view_fit' fit.pk %}" class="text-decoration-none d-inline-block">
-                                                <img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.type_name }}">
-                                            </a>
-                                            {{ fit.ship_type.type_name }}
-                                        </td>
-                                        <td><a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a></td>
-                                        <td>
-                                            {% for cat in f_cats|get_item:fit.pk %}
-                                                <span class="label" style="background-color: {{ cat.color }}"><a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a></span>
-                                            {% endfor %}
-                                        </td>
-                                        <td>{{ fit.description|linebreaks|urlize }}</td>
-                                    </tr>
-                                {% endfor %}
+                            {% for fit in fits %}
+                                <tr>
+                                    <td>
+                                        <a href="{% url 'fittings:view_fit' fit.pk %}" class="text-decoration-none d-inline-block">
+                                            <img class="img-rounded" src="{{ fit.ship_type_type_id|type_render_url:32 }}" title="{{ fit.ship_type.name }}" alt="{{ fit.ship_type.name }}">
+                                        </a>
+                                        {{ fit.ship_type.name }}
+                                    </td>
+
+                                    <td>
+                                        <a href="{% url 'fittings:view_fit' fit.pk %}">{{ fit.name }}</a>
+                                    </td>
+                                    <td>
+                                        {% for cat in f_cats|get_item:fit.pk %}
+                                            <span class="label" style="background-color: {{ cat.color }};">
+                                                <a href="{% url 'fittings:view_category' cat.pk %}" class="nostyle">{{ cat.name }}</a>
+                                            </span>
+                                        {% endfor %}
+                                    </td>
+                                    <td>{{ fit.description|linebreaks|urlize }}</td>
+                                </tr>
+                            {% endfor %}
                             </tbody>
                         </table>
                     {% endif %}
                 </div>
             </div>
         </div>
     </div>
 {% endblock %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
 
-    <script type="application/javascript">
+    <script>
         $(document).ready(function() {
             {% if fits %}
-                $('#fitsTable').DataTable();
+                $('#fitsTable').DataTable({
+                    language: {
+                        url: '{{ STATIC_URL }}/sev3rance_auth_templates/libs/DataTables-Plugins/1.13.4/i18n/{{ LANGUAGE_CODE }}.json'
+                    },
+                    paging: false,
+                    searching: false,
+                    order: [[1, 'asc']]
+                });
             {% endif %}
 
             $('[data-toggle="tooltip"]').tooltip();
         });
     </script>
 {% endblock %}
-
-{% block extra_script %}
-
-{% endblock %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/fittings/view_fit.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/fittings/view_fit.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends 'fittings/base.html' %}
 
 {% load i18n %}
-{% load humanize %}
 {% load filters %}
 {% load static %}
 {% load evelinks %}
 
 {% block page_title %}{{ fitting.name }} {% translate "Fit" %}{% endblock %}
 
 {% block fittings_block %}
@@ -50,31 +49,32 @@
                         <span aria-hidden="true">&times;</span>
                     </button>
 
                     <h4 class="modal-title" id="modalTitle">{{ fit.name }}</h4>
                 </div>
 
                 <div class="modal-body">
-                    <label for="eft-fitting">
+                    <label for="eft-fitting" style="margin-bottom: 1rem;">
                         {% translate "EFT Formatted Fitting" %}
                     </label>
-                    <textarea id="eft-fitting" style="width: 100%; height: 100%;" rows="25" onclick="this.select()">{{ fit.eft }}</textarea>
+
+                    <textarea id="eft-fitting" style="width: 100%; height: 100%;" rows="25" onclick="this.select()" readonly>{{ fit.eft }}</textarea>
                 </div>
 
                 <div class="modal-footer">
                     <button type="button" class="btn btn-default" data-dismiss="modal">
                         {% translate "Close" %}
                     </button>
                 </div>
             </div>
         </div>
     </div>
     {# modal end #}
 
-    <br />
+    <br>
     <div class="row">
         <div class="col-md-3">
             <div class="panel panel-primary">
                 <div class="panel-heading">
                     <div class="panel-title">
                         {% translate "Fit Information" %}
 
@@ -103,14 +103,32 @@
                                             {{ doctrine.name }}
                                         </a>
                                     </li>
                                 {% endfor %}
                             </ul>
                         </dd>
                     </dl>
+
+                    {% if fit.created %}
+                        <dt>{% translate "Created" %}</dt>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ fit.created|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ fit.created|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
+                    {% endif %}
+
+                    {% if fit.last_updated %}
+                        <dt>{% translate "Last Updated" %}</dt>
+                        {% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+                            <dd>{{ fit.last_updated|date:'Y-m-d / H:i:s' }}</dd>
+                        {% else %}
+                            <dd>{{ fit.last_updated|date:'d M Y H:i:s' }}</dd>
+                        {% endif %}
+                    {% endif %}
                 </div>
             </div>
         </div>
 
         <div class="col-md-9">
             <div class="panel panel-default">
                 <div class="panel-heading">
@@ -122,15 +140,19 @@
                         <div class="col-sm-12 col-md-6 text-center">
                             <div id="Fitting_Panel" style="position: relative; height: 398px; width: 398px; z-index: 3; margin: 0 auto;" >
                                 <div id="mask" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index: -1;">
                                     <img class="img-rounded" style="position:absolute; left: 0; top: 0; height: 398px; width: 398px; border: 0;" src="{% static 'fittings/img/pannel/tyrannis.png' %}" alt="">
                                 </div>
 
                                 <div id="highx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index: -1;">
-                                    <img class="img-rounded" src="/static/fittings/img/pannel/{{ slots.high }}h.png" alt="" style="border: 0;">
+                                    {% with slots.high|stringformat:"s" as high_slot_id %}
+                                        {% with "fittings/img/pannel/"|add:high_slot_id|add:"h.png" as high_slots_grid %}
+                                            <img class="img-rounded" src="{% static high_slots_grid %}" alt="High Slots" style="border: 0;">
+                                        {% endwith %}
+                                    {% endwith %}
                                 </div>
 
                                 <div id="high1" style="position:absolute; left:73px; top:60px; width:32px; height:32px;">
                                     {% if fitting.HiSlot0 %}
                                         <img class="img-rounded" src="{{ fitting.HiSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot0.item_name }}" alt="{{ fitting.HiSlot0.item_name }}">
                                     {% endif %}
                                 </div>
@@ -170,15 +192,19 @@
                                         <img class="img-rounded" src="{{ fitting.HiSlot6.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot6.item_name }}" alt="{{ fitting.HiSlot6.item_name }}">
                                     {% endif %}
                                 </div>
 
                                 <div id="high8" style="position:absolute; left:295px; top:64px; width:32px; height:32px;">{% if fitting.HiSlot7 %}<img src="{{ fitting.HiSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.HiSlot7.item_name }}" alt="{{ fitting.HiSlot7.item_name }}">{% endif %}</div>
 
                                 <div id="midx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index: -1;">
-                                    <img class="img-rounded" src="/static/fittings/img/pannel/{{ slots.med }}m.png" alt="" style="border: 0;" />
+                                    {% with slots.med|stringformat:"s" as med_slot_id %}
+                                        {% with "fittings/img/pannel/"|add:med_slot_id|add:"m.png" as med_slots_grid %}
+                                            <img class="img-rounded" src="{% static med_slots_grid %}" alt="Med Slots" style="border: 0;">
+                                        {% endwith %}
+                                    {% endwith %}
                                 </div>
 
                                 <div id="mid1" style="position:absolute; left:26px; top:140px; width:32px; height:32px;">
                                     {% if fitting.MedSlot0 %}
                                         <img class="img-rounded" src="{{ fitting.MedSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot0.item_name }}" alt="{{ fitting.MedSlot0.item_name }}">
                                     {% endif %}
                                 </div>
@@ -222,15 +248,19 @@
                                 <div id="mid8" style="position:absolute; left:133px; top:342px; width:32px; height:32px;">
                                     {% if fitting.MedSlot7 %}
                                         <img class="img-rounded" src="{{ fitting.MedSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.MedSlot7.item_name }}" alt="{{ fitting.MedSlot7.item_name }}">
                                     {% endif %}
                                 </div>
 
                                 <div id="lowx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
-                                    <img class="img-rounded" src="/static/fittings/img/pannel/{{ slots.low }}l.png" alt="" style="border: 0;">
+                                    {% with slots.low|stringformat:"s" as low_slot_id %}
+                                        {% with "fittings/img/pannel/"|add:low_slot_id|add:"l.png" as low_slots_grid %}
+                                            <img class="img-rounded" src="{% static low_slots_grid %}" alt="Low Slots" style="border: 0;">
+                                        {% endwith %}
+                                    {% endwith %}
                                 </div>
 
                                 <div id="low1" style="position:absolute; left:344px; top:143px; width:32px; height:32px;">
                                     {% if fitting.LoSlot0 %}
                                         <img class="img-rounded" src="{{ fitting.LoSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot0.item_name }}" alt="{{ fitting.LoSlot0.item_name }}">
                                     {% endif %}
                                 </div>
@@ -274,15 +304,19 @@
                                 <div id="low8" style="position:absolute; left:234px; top:338px; width:32px; height:32px;">
                                     {% if fitting.LoSlot7 %}
                                         <img class="img-rounded" src="{{ fitting.LoSlot7.type_id|type_icon_url:32 }}" title="{{ fitting.LoSlot7.item_name }}" alt="{{ fitting.LoSlot7.item_name }}">
                                     {% endif %}
                                 </div>
 
                                 <div id="rigxx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index:-1;">
-                                    <img class="img-rounded" src="/static/fittings/img/pannel/{{ slots.rig }}r.png" alt="" style="border: 0;">
+                                    {% with slots.rig|stringformat:"s" as rig_slot_id %}
+                                        {% with "fittings/img/pannel/"|add:rig_slot_id|add:"r.png" as rig_slots_grid %}
+                                            <img class="img-rounded" src="{% static rig_slots_grid %}" alt="Rig Slots" style="border: 0;">
+                                        {% endwith %}
+                                    {% endwith %}
                                 </div>
 
                                 <div id="rig1" style="position:absolute; left:148px; top:259px; width:32px; height:32px;">
                                     {% if fitting.RigSlot0 %}
                                         <img class="img-rounded" src="{{ fitting.RigSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.RigSlot0.item_name }}" alt="{{ fitting.RigSlot0.item_name }}">
                                     {% endif %}
                                 </div>
@@ -297,15 +331,19 @@
                                     {% if fitting.RigSlot2 %}
                                         <img class="img-rounded" src="{{ fitting.RigSlot2.type_id|type_icon_url:32 }}" title="{{ fitting.RigSlot2.item_name }}" alt="{{ fitting.RigSlot2.item_name }}">
                                     {% endif %}
                                 </div>
 
                                 {% if slots.sub %}
                                     <div id="subx" style="position:absolute; left: 0; top: 0; width: 398px; height: 398px; z-index: -1;">
-                                        <img class="img-rounded" src="/static/fittings/img/pannel/{{ slots.sub }}s.png" alt="" style="border: 0;">
+                                        {% with slots.sub|stringformat:"s" as sub_slot_id %}
+                                            {% with "fittings/img/pannel/"|add:sub_slot_id|add:"s.png" as sub_slots_grid %}
+                                                <img class="img-rounded" src="{% static sub_slots_grid %}" alt="Subsystem Slots" style="border: 0;">
+                                            {% endwith %}
+                                        {% endwith %}
                                     </div>
 
                                     <div id="sub1" style="position:absolute; left:117px; top:131px; width:32px; height:32px;">
                                         {% if fitting.SubSystemSlot0 %}
                                             <img class="img-rounded" src="{{ fitting.SubSystemSlot0.type_id|type_icon_url:32 }}" title="{{ fitting.SubSystemSlot0.item_name }}" alt="{{ fitting.SubSystemSlot0.item_name }}">
                                         {% endif %}
                                     </div>
@@ -354,25 +392,27 @@
                                 </div>
 
                                 <div class="panel-body text-center">
                                     {{ fit.ship_type.type_name }}
                                 </div>
                             </div>
 
-                            <div class="panel panel-warning">
-                                <div class="panel-heading">
-                                    <div class="panel-title">{% translate "Fitting Notes" %}</div>
-                                </div>
+                            {% if fit.description %}
+                                <div class="panel panel-warning">
+                                    <div class="panel-heading">
+                                        <div class="panel-title">{% translate "Fitting Notes" %}</div>
+                                    </div>
 
-                                <div class="panel-body">
-                                    <div class="well">
-                                        {{ fit.description|linebreaks|urlize }}
+                                    <div class="panel-body">
+                                        <div class="well">
+                                            {{ fit.description|linebreaks|urlize }}
+                                        </div>
                                     </div>
                                 </div>
-                            </div>
+                            {% endif %}
                         </div>
                     </div>
                 </div>
             </div>
 
             <div class="panel panel-default">
                 <div class="panel-heading">
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
-{% extends 'fittings/base.html' %} {% load i18n %} {% load humanize %} {% load
-filters %} {% load static %} {% load evelinks %} {% block page_title %}{
-{ fitting.name }} {% translate "Fit" %}{% endblock %} {% block fittings_block
-%} {# modal start #}
+{% extends 'fittings/base.html' %} {% load i18n %} {% load filters %} {% load
+static %} {% load evelinks %} {% block page_title %}{{ fitting.name }} {%
+translate "Fit" %}{% endblock %} {% block fittings_block %} {# modal start #}
  ×
 *** {% translate "Are you sure?" %} ***
 {% translate "Are you sure you wish to delete this fit?" %} {% translate "This
 action is permanent." %}
  {% translate "No - Close" %}  {%_translate_"Yes_-_Delete"_%}
  ×
 *** {{ fit.name }} ***
@@ -15,59 +14,89 @@
 {# modal end #}
 {% translate "Fit Information" %} {% if perms.fittings.manage %}       {% endif
 %}
   {% translate "Doctrines" %}
           * {% for doctrine in doctrines %}
           * {{_doctrine.name_}}
           * {% endfor %}
+{% if fit.created %}
+{% translate "Created" %}
+{% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+{{ fit.created|date:'Y-m-d / H:i:s' }}
+{% else %}
+{{ fit.created|date:'d M Y H:i:s' }}
+{% endif %} {% endif %} {% if fit.last_updated %}
+{% translate "Last Updated" %}
+{% if LANGUAGE_CODE == 'ko' or LANGUAGE_CODE == 'ja' %}
+{{ fit.last_updated|date:'Y-m-d / H:i:s' }}
+{% else %}
+{{ fit.last_updated|date:'d M Y H:i:s' }}
+{% endif %} {% endif %}
 {% translate "Fitting" %}
+{% with slots.high|stringformat:"s" as high_slot_id %} {% with "fittings/img/
+pannel/"|add:high_slot_id|add:"h.png" as high_slots_grid %} [High Slots] {%
+endwith %} {% endwith %}
 {% if fitting.HiSlot0 %} [{{ fitting.HiSlot0.item_name }}] {% endif %}
 {% if fitting.HiSlot1 %} [{{ fitting.HiSlot1.item_name }}] {% endif %}
 {% if fitting.HiSlot2 %} [{{ fitting.HiSlot2.item_name }}] {% endif %}
 {% if fitting.HiSlot3 %} [{{ fitting.HiSlot3.item_name }}] {% endif %}
 {% if fitting.HiSlot4 %} [{{ fitting.HiSlot4.item_name }}] {% endif %}
 {% if fitting.HiSlot5 %} [{{ fitting.HiSlot5.item_name }}] {% endif %}
 {% if fitting.HiSlot6 %} [{{ fitting.HiSlot6.item_name }}] {% endif %}
 {% if fitting.HiSlot7 %}[{{ fitting.HiSlot7.item_name }}]{% endif %}
+{% with slots.med|stringformat:"s" as med_slot_id %} {% with "fittings/img/
+pannel/"|add:med_slot_id|add:"m.png" as med_slots_grid %} [Med Slots] {%
+endwith %} {% endwith %}
 {% if fitting.MedSlot0 %} [{{ fitting.MedSlot0.item_name }}] {% endif %}
 {% if fitting.MedSlot1 %} [{{ fitting.MedSlot1.item_name }}] {% endif %}
 {% if fitting.MedSlot2 %} [{{ fitting.MedSlot2.item_name }}] {% endif %}
 {% if fitting.MedSlot3 %} [{{ fitting.MedSlot3.item_name }}] {% endif %}
 {% if fitting.MedSlot4 %} [{{ fitting.MedSlot4.item_name }}] {% endif %}
 {% if fitting.MedSlot5 %} [{{ fitting.MedSlot5.item_name }}] {% endif %}
 {% if fitting.MedSlot6 %} [{{ fitting.MedSlot6.item_name }}] {% endif %}
 {% if fitting.MedSlot7 %} [{{ fitting.MedSlot7.item_name }}] {% endif %}
+{% with slots.low|stringformat:"s" as low_slot_id %} {% with "fittings/img/
+pannel/"|add:low_slot_id|add:"l.png" as low_slots_grid %} [Low Slots] {%
+endwith %} {% endwith %}
 {% if fitting.LoSlot0 %} [{{ fitting.LoSlot0.item_name }}] {% endif %}
 {% if fitting.LoSlot1 %} [{{ fitting.LoSlot1.item_name }}] {% endif %}
 {% if fitting.LoSlot2 %} [{{ fitting.LoSlot2.item_name }}] {% endif %}
 {% if fitting.LoSlot3 %} [{{ fitting.LoSlot3.item_name }}] {% endif %}
 {% if fitting.LoSlot4 %} [{{ fitting.LoSlot4.item_name }}] {% endif %}
 {% if fitting.LoSlot5 %} [{{ fitting.LoSlot5.item_name }}] {% endif %}
 {% if fitting.LoSlot6 %} [{{ fitting.LoSlot6.item_name }}] {% endif %}
 {% if fitting.LoSlot7 %} [{{ fitting.LoSlot7.item_name }}] {% endif %}
+{% with slots.rig|stringformat:"s" as rig_slot_id %} {% with "fittings/img/
+pannel/"|add:rig_slot_id|add:"r.png" as rig_slots_grid %} [Rig Slots] {%
+endwith %} {% endwith %}
 {% if fitting.RigSlot0 %} [{{ fitting.RigSlot0.item_name }}] {% endif %}
 {% if fitting.RigSlot1 %} [{{ fitting.RigSlot1.item_name }}] {% endif %}
 {% if fitting.RigSlot2 %} [{{ fitting.RigSlot2.item_name }}] {% endif %}
 {% if slots.sub %}
+{% with slots.sub|stringformat:"s" as sub_slot_id %} {% with "fittings/img/
+pannel/"|add:sub_slot_id|add:"s.png" as sub_slots_grid %} [Subsystem Slots] {%
+endwith %} {% endwith %}
 {% if fitting.SubSystemSlot0 %} [{{ fitting.SubSystemSlot0.item_name }}] {%
 endif %}
 {% if fitting.SubSystemSlot1 %} [{{ fitting.SubSystemSlot1.item_name }}] {%
 endif %}
 {% if fitting.SubSystemSlot2 %} [{{ fitting.SubSystemSlot2.item_name }}] {%
 endif %}
 {% if fitting.SubSystemSlot3 %} [{{ fitting.SubSystemSlot3.item_name }}] {%
 endif %}
 {% endif %}
 [{{ fit.ship_type.type_name }}]
 **** {{ fit.name }} ****
 {% for cat in cats %}  {{_cat.name_}}  {% endfor %}
 {% translate "Hull" %}
 {{ fit.ship_type.type_name }}
+{% if fit.description %}
 {% translate "Fitting Notes" %}
 {{ fit.description|linebreaks|urlize }}
+{% endif %}
 {% translate "Fitting Details" %}
 {%_translate_"Save_to_EVE"_%}  {% translate "Copy Buy All" %}   {% translate
 "Copy Fit (EFT)" %}
     * {% translate "Hull" %}
     * [{{ fit.ship_type.type_name }}] {{ fit.ship_type.type_name }}
     * {% if fitting.SubSystemSlot0 %}
     * {% translate "SubSystems" %}
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/index.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             <div class="col-md-12">
                 <div class="panel panel-success">
                     <div class="panel-heading">
                         <div class="panel-title">New Link</div>
                     </div>
                     <div class="panel-body text-center" style="min-height: 100px;">
                         <p>Expires in: <span id="countdown{{ tl.link_ref }}hot"></span></p>
-                        <pre>{{ request.scheme }}://{{ request.get_host }}{% url 'mumbletemps:join' tl.link_ref %}</pre>
+                        <pre>{{ SITE_URL }}{% url 'mumbletemps:join' tl.link_ref %}</pre>
                         <button class="btn btn-info col-md-12" id="clipboard-new" data-clipboard-text="{{ request.scheme }}://{{request.get_host}}{% url 'mumbletemps:join' tl.link_ref %}">Copy to Clipboard!</button>
                     </div>
                 </div>
             </div>
         </div>
     {% endif %}
 
@@ -83,15 +83,15 @@
                                 <tr>
                                     <td class="valign-middle">
                                         <img class="ra-avatar img-rounded" src="{{ lnk.creator.portrait_url_32 }}" alt="{{ lnk.creator.character_name }}">
                                         {{ lnk.creator.character_name }}
                                     </td>
                                     <td class="valign-middle">{{ lnk.link_ref }}</td>
                                     <td class=valign-middle" id="countdown{{ lnk.link_ref }}"></td>
-                                    <td class="text-center valign-middle"><button class="btn btn-info" id="clipboard-{{ lnk.link_ref }}" data-clipboard-text="{{ request.scheme }}://{{ request.get_host }}{% url 'mumbletemps:join' lnk.link_ref %}">Copy to Clipboard!</button></td>
+                                    <td class="text-center valign-middle"><button class="btn btn-info" id="clipboard-{{ lnk.link_ref }}" data-clipboard-text="{{ SITE_URL }}{% url 'mumbletemps:join' lnk.link_ref %}">Copy to Clipboard!</button></td>
                                     <td class="text-center valign-middle"><a class="btn btn-danger" href="{% url 'mumbletemps:nuke' lnk.link_ref %}">Nuke Link!</a></td>
                                 </tr>
                             {% endfor %}
                         </tbody>
                     </table>
                 </div>
             </div>
```

#### html2text {}

```diff
@@ -8,16 +8,15 @@
 Create New Link
 Your link will be displayed on the next page for easy copy and paste
 {% csrf_token %} Duration (hours) [One of: 3/6/12/24]
 [OK]
 {% if tl %}
 New Link
 Expires in:
-{{ request.scheme }}://{{ request.get_host }}{% url 'mumbletemps:join'
-tl.link_ref %}
+{{ SITE_URL }}{% url 'mumbletemps:join' tl.link_ref %}
 Copy to Clipboard!
 {% endif %}
 Current Links
 [{
 { lnk.creator.character_name
 }}] {                        {{ lnk.link_ref }}  Copy to Clipboard! Nuke_Link!
 { lnk.creator.character_name
```

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates/templates/mumbletemps/link.html` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates/templates/mumbletemps/link.html`

 * *Files identical despite different names*

### Comparing `sev3rance_auth_templates-1.5.0/sev3rance_auth_templates.egg-info/PKG-INFO` & `sev3rance_auth_templates-1.6.0/sev3rance_auth_templates.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: sev3rance-auth-templates
-Version: 1.5.0
+Version: 1.6.0
 Summary: Sev3rance Template Overrides for Alliance Auth
 Home-page: https://github.com/sev3rance/sev3rance-auth-templates
 Author: Peter Pfeufer
-Author-email: development@ppfeufer.de
+Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
-Maintainer-email: development@ppfeufer.de
+Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
 Project-URL: Issue / Bug Reports, https://github.com/sev3rance/sev3rance-auth-templates/issues
 Project-URL: Changelog, https://github.com/sev3rance/sev3rance-auth-templates/blob/master/CHANGELOG.md
 Keywords: allianceauth,eveonline,template,template_override,sev3rance
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Alliance Auth Template Overrides used by Sev3rance Alliance
 
 # Sev3rance Auth Templates
```

