# Comparing `tmp/piknik-0.3.3.tar.gz` & `tmp/piknik-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.3.tar", last modified: Wed Apr 19 19:07:27 2023, max compression
+gzip compressed data, was "piknik-0.3.4.tar", last modified: Thu Apr 20 06:42:01 2023, max compression
```

## Comparing `piknik-0.3.3.tar` & `piknik-0.3.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/
--rw-r--r--   0 lash      (1000) lash      (1000)     1361 2023-04-19 18:54:19.000000 piknik-0.3.3/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.3/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.3/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 19:07:27.616628 piknik-0.3.3/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-19 09:43:40.000000 piknik-0.3.3/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.3/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.613295 piknik-0.3.3/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.3/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-19 09:43:40.000000 piknik-0.3.3/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      834 2023-04-19 18:03:40.000000 piknik-0.3.3/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-19 18:03:31.000000 piknik-0.3.3/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.3/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.3/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-19 18:47:55.000000 piknik-0.3.3/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6203 2023-04-19 18:51:30.000000 piknik-0.3.3/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     1842 2023-04-19 17:48:28.000000 piknik-0.3.3/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-19 10:45:31.000000 piknik-0.3.3/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.3/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.613295 piknik-0.3.3/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-19 10:45:31.000000 piknik-0.3.3/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 19:07:27.616628 piknik-0.3.3/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.3/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.3/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.3/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.3/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.3/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.3/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.3/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.3/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.409988 piknik-0.3.4/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1441 2023-04-20 06:37:12.000000 piknik-0.3.4/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.4/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.4/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-20 06:42:01.409988 piknik-0.3.4/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.4/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.4/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.4/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.4/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      834 2023-04-20 06:37:12.000000 piknik-0.3.4/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.4/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.4/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.4/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.4/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 06:37:12.000000 piknik-0.3.4/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.4/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.4/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.4/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.4/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.4/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 06:37:12.000000 piknik-0.3.4/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 06:39:06.000000 piknik-0.3.4/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.4/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1842 2023-04-20 06:37:12.000000 piknik-0.3.4/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.4/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.4/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.406655 piknik-0.3.4/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 06:42:01.000000 piknik-0.3.4/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.4/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-20 06:42:01.409988 piknik-0.3.4/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.4/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.4/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 06:42:01.409988 piknik-0.3.4/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.4/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.4/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.4/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.4/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.4/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.4/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.4/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.4/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.4/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.4/tests/test_tag.py
```

### Comparing `piknik-0.3.3/CHANGELOG` & `piknik-0.3.4/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.3.4
+	* Fix endless recursion bug for html issue render introduced in v0.3.3
 - 0.3.3
 	* Enable state filtering controls from cli
 	* Make finished issues not visible by default
 	* Fix last state category truncate in html rendering
 - 0.3.2
 	* Add handler for setting pending state
 	* Upgrade shep to handle empty tag directories when transferring (empty) state directories over git
```

### Comparing `piknik-0.3.3/LICENSE` & `piknik-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/PKG-INFO` & `piknik-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.3
+Version: 0.3.4
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.3/ROADMAP` & `piknik-0.3.4/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/basket.py` & `piknik-0.3.4/piknik/basket.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/cli/__init__.py` & `piknik-0.3.4/piknik/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/cli/comment.py` & `piknik-0.3.4/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/cli/mod.py` & `piknik-0.3.4/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/cli/show.py` & `piknik-0.3.4/piknik/cli/show.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/crypto.py` & `piknik-0.3.4/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/issue.py` & `piknik-0.3.4/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/msg.py` & `piknik-0.3.4/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/render/base.py` & `piknik-0.3.4/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/render/html.py` & `piknik-0.3.4/piknik/render/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,25 @@
             w = self.w
         if len(v) == 0:
             if self.envelope != None:
                 self.msg.add(self.envelope)
             if self.msg != None:
                 self.category.add(self.msg)
                 #self.doc.add(self.msg)
-            self.doc.add(self.category)
             if self.last_v != None:
                 self.category.add(li(self.last_v))
+            self.doc.add(self.category)
             w.write(self.doc.render())
-            return False
+            self.last_v = None
 
         v_id = getattr(v, 'id', '')
         logg.debug('add id {}'.format(v_id))
         if len(v_id) > 1:
+            if v_id[0] == 's':
+                self.last_v = v
             if v_id[:2] == 's_':
                 if self.issue != None:
                     self.category_content.add(self.issue)
                     self.category.add(li(self.category_content))
                 self.category_content = v
                 self.issue = ul(_id='issue_list_' + v_id[2:])
             elif v_id[:2] == 'i_':
@@ -68,16 +70,14 @@
                 #self.envelope_content = v
                 self.envelope = li()
             elif v_id[:4] == 'd_m_':
                 self.envelope.add(v)
         else:
             self.doc = v
             self.last_v = None
-        self.last_v = v
-        return True
 
 
 class Renderer(BaseRenderer):
 
     def __init__(self, basket, accumulator=None, wrapper=None, outdir=None, states_include=[], states_skip=[]):
         if accumulator == None:
             accumulator = Accumulator().add
@@ -131,15 +131,15 @@
                 o = v[0]
                 ss = o.id()
                 if o == owner:
                     ss += ' (owner)'
                 r_r.add(li(ss))
             s.add(dd(r_r))
 
-        r.add(s)
+        #r.add(s)
 
         deps = issue.get_dependencies()
         s.add(dt('depends on'))
         if len(deps) == 0:
             s.add(dd('no dependencies'))
         else:
             r_r = ul()
```

### Comparing `piknik-0.3.3/piknik/render/plain.py` & `piknik-0.3.4/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/runnable/cmd.py` & `piknik-0.3.4/piknik/runnable/cmd.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/store/__init__.py` & `piknik-0.3.4/piknik/store/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik/wrap.py` & `piknik-0.3.4/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/piknik.egg-info/PKG-INFO` & `piknik-0.3.4/piknik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.3
+Version: 0.3.4
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.3/piknik.egg-info/SOURCES.txt` & `piknik-0.3.4/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/setup.cfg` & `piknik-0.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.3
+version = 0.3.4
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-cache
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.3/setup.py` & `piknik-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_assign.py` & `piknik-0.3.4/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_basic.py` & `piknik-0.3.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_crypto.py` & `piknik-0.3.4/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_dep.py` & `piknik-0.3.4/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_html.py` & `piknik-0.3.4/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_issue.py` & `piknik-0.3.4/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_msg.py` & `piknik-0.3.4/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_render.py` & `piknik-0.3.4/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_store.py` & `piknik-0.3.4/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.3/tests/test_tag.py` & `piknik-0.3.4/tests/test_tag.py`

 * *Files identical despite different names*

