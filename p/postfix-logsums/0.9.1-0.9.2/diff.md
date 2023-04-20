# Comparing `tmp/postfix_logsums-0.9.1.tar.gz` & `tmp/postfix_logsums-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfix_logsums-0.9.1.tar", last modified: Thu Apr 20 07:50:26 2023, max compression
+gzip compressed data, was "postfix_logsums-0.9.2.tar", last modified: Thu Apr 20 08:27:56 2023, max compression
```

## Comparing `postfix_logsums-0.9.1.tar` & `postfix_logsums-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      987 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/de/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)    20693 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/locale/de/LC_MESSAGES/postfix_logsums.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/locale/en/LC_MESSAGES/
--rw-r--r--   0 root         (0) root         (0)      940 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/locale/en/LC_MESSAGES/postfix_logsums.mo
--rwxr-xr-x   0 root         (0) root         (0)     1091 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix-logsums
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/postfix_logsums/
--rw-r--r--   0 root         (0) root         (0)    63893 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74500 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/app.py
--rw-r--r--   0 root         (0) root         (0)     7699 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/errors.py
--rw-r--r--   0 root         (0) root         (0)     7965 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/results.py
--rw-r--r--   0 root         (0) root         (0)    31716 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/stats.py
--rw-r--r--   0 root         (0) root         (0)     2943 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/postfix_logsums/xlate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.471744 postfix_logsums-0.9.1/postfix_logsums.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 07:50:26.000000 postfix_logsums-0.9.1/postfix_logsums.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1203 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6273 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 07:50:26.475744 postfix_logsums-0.9.1/test/
--rwxr-xr-x   0 root         (0) root         (0)     7285 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_00_errors.py
--rwxr-xr-x   0 root         (0) root         (0)    13220 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_05_stats_collections.py
--rwxr-xr-x   0 root         (0) root         (0)     2411 2023-04-20 07:49:58.000000 postfix_logsums-0.9.1/test/test_10_results.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.929724 postfix_logsums-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 08:27:56.929724 postfix_logsums-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)    20694 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/locale/de/LC_MESSAGES/postfix_logsums.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/locale/en/LC_MESSAGES/
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/locale/en/LC_MESSAGES/postfix_logsums.mo
+-rwxr-xr-x   0 root         (0) root         (0)     1091 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix-logsums
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.925724 postfix_logsums-0.9.2/postfix_logsums/
+-rw-r--r--   0 root         (0) root         (0)    63893 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74500 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/app.py
+-rw-r--r--   0 root         (0) root         (0)     7699 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/results.py
+-rw-r--r--   0 root         (0) root         (0)    31716 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/stats.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/postfix_logsums/xlate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.929724 postfix_logsums-0.9.2/postfix_logsums.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/postfix_logsums.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/postfix_logsums.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/postfix_logsums.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-20 08:27:56.000000 postfix_logsums-0.9.2/postfix_logsums.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-04-20 08:27:56.929724 postfix_logsums-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6273 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:27:56.929724 postfix_logsums-0.9.2/test/
+-rwxr-xr-x   0 root         (0) root         (0)     7285 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/test/test_00_errors.py
+-rwxr-xr-x   0 root         (0) root         (0)    13220 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/test/test_05_stats_collections.py
+-rwxr-xr-x   0 root         (0) root         (0)     2411 2023-04-20 08:27:35.000000 postfix_logsums-0.9.2/test/test_10_results.py
```

### Comparing `postfix_logsums-0.9.1/LICENSE` & `postfix_logsums-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/PKG-INFO` & `postfix_logsums-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix_logsums
-Version: 0.9.1
+Version: 0.9.2
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.9.1/README.md` & `postfix_logsums-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/locale/de/LC_MESSAGES/postfix_logsums.mo` & `postfix_logsums-0.9.2/locale/de/LC_MESSAGES/postfix_logsums.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -473,15 +473,15 @@
 msgid "Postfix log summaries for {}"
 msgstr "Postfix Log-Zusammenfassung für {}"
 
 msgid "Reading uncompressed file {!r} ..."
 msgstr "Lese unkomprimierte Datei {!r} …"
 
 msgid "Reading {w} compressed file {f!r} ..."
-msgstr "Lese {w}-lomprimierte Datei {!r} …"
+msgstr "Lese {w}-lomprimierte Datei {f!r} …"
 
 msgid "Received"
 msgstr "Erhalten"
 
 msgid "Recipients by message count"
 msgstr "Empfänger nach Anzahl der Nachrichten"
```

### Comparing `postfix_logsums-0.9.1/locale/en/LC_MESSAGES/postfix_logsums.mo` & `postfix_logsums-0.9.2/locale/en/LC_MESSAGES/postfix_logsums.mo`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix-logsums` & `postfix_logsums-0.9.2/postfix-logsums`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums/__init__.py` & `postfix_logsums-0.9.2/postfix_logsums/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from .results import PostfixLogSums
 
 from .stats import MessageStats, MessageStatsPerDay, SmtpdStats
 
 from .xlate import XLATOR
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = 'Frank Brehm <frank@brehm-online.com>'
 __copyright__ = '(C) 2023 by Frank Brehm, Berlin'
 
 DEFAULT_TERMINAL_WIDTH = 99
 DEFAULT_TERMINAL_HEIGHT = 40
 MAX_TERMINAL_WIDTH = 150
```

### Comparing `postfix_logsums-0.9.1/postfix_logsums/app.py` & `postfix_logsums-0.9.2/postfix_logsums/app.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums/errors.py` & `postfix_logsums-0.9.2/postfix_logsums/errors.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums/results.py` & `postfix_logsums-0.9.2/postfix_logsums/results.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums/stats.py` & `postfix_logsums-0.9.2/postfix_logsums/stats.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums/xlate.py` & `postfix_logsums-0.9.2/postfix_logsums/xlate.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/postfix_logsums.egg-info/PKG-INFO` & `postfix_logsums-0.9.2/postfix_logsums.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfix-logsums
-Version: 0.9.1
+Version: 0.9.2
 Summary: Produce Postfix MTA logfile summary
 Home-page: https://github.com/pixelpark/postfix-logsums
 Author: Frank Brehm
 Author-email: frank@brehm-online.com
 License: LGPL3+
 Platform: posix
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `postfix_logsums-0.9.1/postfix_logsums.egg-info/SOURCES.txt` & `postfix_logsums-0.9.2/postfix_logsums.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/setup.cfg` & `postfix_logsums-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/setup.py` & `postfix_logsums-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/test/test_00_errors.py` & `postfix_logsums-0.9.2/test/test_00_errors.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/test/test_05_stats_collections.py` & `postfix_logsums-0.9.2/test/test_05_stats_collections.py`

 * *Files identical despite different names*

### Comparing `postfix_logsums-0.9.1/test/test_10_results.py` & `postfix_logsums-0.9.2/test/test_10_results.py`

 * *Files identical despite different names*

