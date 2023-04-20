# Comparing `tmp/piknik-0.3.6.tar.gz` & `tmp/piknik-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.6.tar", last modified: Thu Apr 20 06:56:42 2023, max compression
+gzip compressed data, was "piknik-0.3.7.tar", last modified: Thu Apr 20 07:00:19 2023, max compression
```

## Comparing `piknik-0.3.6.tar` & `piknik-0.3.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.859983 piknik-0.3.6/
--rw-r--r--   0 lash      (1000) lash      (1000)     1573 2023-04-20 06:55:07.000000 piknik-0.3.6/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.6/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.6/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 06:56:42.859983 piknik-0.3.6/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.6/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.6/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.6/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.6/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      853 2023-04-20 06:52:34.000000 piknik-0.3.6/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.6/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.6/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.6/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.6/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 06:52:34.000000 piknik-0.3.6/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.6/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.6/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.6/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.6/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.6/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 06:52:34.000000 piknik-0.3.6/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 06:52:34.000000 piknik-0.3.6/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.6/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     1972 2023-04-20 06:54:05.000000 piknik-0.3.6/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.6/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.6/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.856649 piknik-0.3.6/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 06:56:42.000000 piknik-0.3.6/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.6/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-20 06:56:42.859983 piknik-0.3.6/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.6/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.6/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:56:42.859983 piknik-0.3.6/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.6/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.6/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.6/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.6/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.6/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.6/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.6/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.6/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.6/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.6/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1622 2023-04-20 07:00:03.000000 piknik-0.3.7/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.7/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.7/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:00:19.896648 piknik-0.3.7/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.7/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.7/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.7/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.7/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      853 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.7/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.7/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2001 2023-04-20 06:59:39.000000 piknik-0.3.7/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.7/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.7/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.7/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-20 07:00:19.899982 piknik-0.3.7/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.7/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.7/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.7/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.7/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.7/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.7/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.7/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.7/tests/test_tag.py
```

### Comparing `piknik-0.3.6/CHANGELOG` & `piknik-0.3.7/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.3.7
+	* Complete incomplete change from 0.3.6
 - 0.3.6
 	* Enable --help display without subcommand
 - 0.3.5
 	* Fix crash using other tools than show on missing --show-missing flag
 - 0.3.4
 	* Fix endless recursion bug for html issue render introduced in v0.3.3
 - 0.3.3
```

### Comparing `piknik-0.3.6/LICENSE` & `piknik-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/PKG-INFO` & `piknik-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.6
+Version: 0.3.7
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.6/ROADMAP` & `piknik-0.3.7/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/basket.py` & `piknik-0.3.7/piknik/basket.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/cli/__init__.py` & `piknik-0.3.7/piknik/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/cli/comment.py` & `piknik-0.3.7/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/cli/mod.py` & `piknik-0.3.7/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/cli/show.py` & `piknik-0.3.7/piknik/cli/show.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/crypto.py` & `piknik-0.3.7/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/issue.py` & `piknik-0.3.7/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/msg.py` & `piknik-0.3.7/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/render/base.py` & `piknik-0.3.7/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/render/html.py` & `piknik-0.3.7/piknik/render/html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/render/plain.py` & `piknik-0.3.7/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/runnable/cmd.py` & `piknik-0.3.7/piknik/runnable/cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 argp = argparse.ArgumentParser()
 argp.add_argument('-d', type=str, help='Data directory')
 argp.add_argument('-f', '--files', dest='f', action='store_true', help='Save attachments to filesystem')
 argp.add_argument('-o', '--files-dir', dest='files_dir', type=str, help='Directory to output saved files to')
 argp.add_argument('-v', action='store_true', help='Turn on debug logs')
 argp.add_argument('-i','--issue-id',  type=str, help='Issue id to show')
-argp.add_argument('cmd', type=str, choices=['show', 'add', 'mod', 'comment'], help='subcommand to execute')
+argp.add_argument('cmd', type=str, nargs='?', choices=['show', 'add', 'mod', 'comment'], help='subcommand to execute')
 strargs = copy.copy(sys.argv[1:])
 
 have_help = False
 try:
     strargs.remove('-h')
     have_help = True
 except ValueError:
@@ -51,16 +51,17 @@
     m = importlib.import_module('piknik.cli.mod')
 elif arg.cmd == 'comment':
     m = importlib.import_module('piknik.cli.comment')
 else:
     if not have_help:
         raise ValueError('unknown subcommand')
 
+if m != None:
+    argp = m.subparser(argp)
 
-argp = m.subparser(argp)
 arg = argp.parse_args(sys.argv[1:])
 if arg.v:
     logg.setLevel(logging.DEBUG)
 
 m.ctx = Context(arg, m.assembler)
```

### Comparing `piknik-0.3.6/piknik/store/__init__.py` & `piknik-0.3.7/piknik/store/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik/wrap.py` & `piknik-0.3.7/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/piknik.egg-info/PKG-INFO` & `piknik-0.3.7/piknik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.6
+Version: 0.3.7
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.6/piknik.egg-info/SOURCES.txt` & `piknik-0.3.7/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/setup.py` & `piknik-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_assign.py` & `piknik-0.3.7/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_basic.py` & `piknik-0.3.7/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_crypto.py` & `piknik-0.3.7/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_dep.py` & `piknik-0.3.7/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_html.py` & `piknik-0.3.7/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_issue.py` & `piknik-0.3.7/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_msg.py` & `piknik-0.3.7/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_render.py` & `piknik-0.3.7/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_store.py` & `piknik-0.3.7/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.6/tests/test_tag.py` & `piknik-0.3.7/tests/test_tag.py`

 * *Files identical despite different names*

