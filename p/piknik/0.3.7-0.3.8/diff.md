# Comparing `tmp/piknik-0.3.7.tar.gz` & `tmp/piknik-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.7.tar", last modified: Thu Apr 20 07:00:19 2023, max compression
+gzip compressed data, was "piknik-0.3.8.tar", last modified: Thu Apr 20 07:12:17 2023, max compression
```

## Comparing `piknik-0.3.7.tar` & `piknik-0.3.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/
--rw-r--r--   0 lash      (1000) lash      (1000)     1622 2023-04-20 07:00:03.000000 piknik-0.3.7/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.7/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.7/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:00:19.896648 piknik-0.3.7/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.7/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.7/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.7/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.7/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      853 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.7/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.7/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.7/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 06:58:22.000000 piknik-0.3.7/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.7/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2001 2023-04-20 06:59:39.000000 piknik-0.3.7/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.7/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.7/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 07:00:19.000000 piknik-0.3.7/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.7/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-20 07:00:19.899982 piknik-0.3.7/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.7/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.7/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:00:19.896648 piknik-0.3.7/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.7/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.7/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.7/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.7/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.7/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.7/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.7/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.399977 piknik-0.3.8/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1685 2023-04-20 07:11:27.000000 piknik-0.3.8/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.8/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.8/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:12:17.399977 piknik-0.3.8/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.8/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.8/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.8/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.8/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2023-04-20 07:09:35.000000 piknik-0.3.8/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.8/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.8/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2001 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.8/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.8/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.8/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-20 07:12:17.399977 piknik-0.3.8/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.8/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.8/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.399977 piknik-0.3.8/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.8/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.8/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.8/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.8/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.8/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.8/tests/test_tag.py
```

### Comparing `piknik-0.3.7/CHANGELOG` & `piknik-0.3.8/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- 0.3.8
+	* Fix broken add tool
+	* Add minimal sanity cli tests
 - 0.3.7
 	* Complete incomplete change from 0.3.6
 - 0.3.6
 	* Enable --help display without subcommand
 - 0.3.5
 	* Fix crash using other tools than show on missing --show-missing flag
 - 0.3.4
```

### Comparing `piknik-0.3.7/LICENSE` & `piknik-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/PKG-INFO` & `piknik-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.7
+Version: 0.3.8
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.7/ROADMAP` & `piknik-0.3.8/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/basket.py` & `piknik-0.3.8/piknik/basket.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/cli/__init__.py` & `piknik-0.3.8/piknik/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Context:
 
     def __init__(self, arg, assembler, mode=0, gpg_home=os.environ.get('GPGHOME')):
         self.issue_id = arg.issue_id
         self.files_dir = arg.files_dir
         self.show_finished = getattr(arg, 'show_finished', False)
-        self.show_states = arg.state
+        self.show_states = getattr(arg, 'state', [])
         #self.store_factory = FileStoreFactory(arg.d)
         store_factory = FileStoreFactory(arg.d)
         self.signer = None
         sign_fn = None
         if hasattr(arg, 's'):
             self.signer = PGPSigner(default_key=arg.s, use_agent=True)
             sign_fn = self.signer.sign
```

### Comparing `piknik-0.3.7/piknik/cli/comment.py` & `piknik-0.3.8/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/cli/mod.py` & `piknik-0.3.8/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/cli/show.py` & `piknik-0.3.8/piknik/cli/show.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/crypto.py` & `piknik-0.3.8/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/issue.py` & `piknik-0.3.8/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/msg.py` & `piknik-0.3.8/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/render/base.py` & `piknik-0.3.8/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/render/html.py` & `piknik-0.3.8/piknik/render/html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/render/plain.py` & `piknik-0.3.8/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/runnable/cmd.py` & `piknik-0.3.8/piknik/runnable/cmd.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/store/__init__.py` & `piknik-0.3.8/piknik/store/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik/wrap.py` & `piknik-0.3.8/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/piknik.egg-info/PKG-INFO` & `piknik-0.3.8/piknik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.7
+Version: 0.3.8
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.7/piknik.egg-info/SOURCES.txt` & `piknik-0.3.8/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/setup.cfg` & `piknik-0.3.8/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.7
+version = 0.3.8
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/piknik
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.7/setup.py` & `piknik-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_assign.py` & `piknik-0.3.8/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_basic.py` & `piknik-0.3.8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_crypto.py` & `piknik-0.3.8/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_dep.py` & `piknik-0.3.8/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_html.py` & `piknik-0.3.8/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_issue.py` & `piknik-0.3.8/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_msg.py` & `piknik-0.3.8/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_render.py` & `piknik-0.3.8/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_store.py` & `piknik-0.3.8/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.7/tests/test_tag.py` & `piknik-0.3.8/tests/test_tag.py`

 * *Files identical despite different names*

