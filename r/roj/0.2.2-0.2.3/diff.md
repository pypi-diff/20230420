# Comparing `tmp/roj-0.2.2.tar.gz` & `tmp/roj-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roj-0.2.2.tar", last modified: Mon Mar 20 07:25:41 2023, max compression
+gzip compressed data, was "roj-0.2.3.tar", last modified: Thu Apr 20 03:30:54 2023, max compression
```

## Comparing `roj-0.2.2.tar` & `roj-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-03-20 07:25:41.141693 roj-0.2.2/
--rw-rw-r--   0 ek        (1000) ek        (1000)     1260 2023-02-11 05:57:50.000000 roj-0.2.2/LICENSE
--rw-rw-r--   0 ek        (1000) ek        (1000)     2585 2023-03-20 07:25:41.141693 roj-0.2.2/PKG-INFO
--rw-rw-r--   0 ek        (1000) ek        (1000)     2043 2023-03-20 07:20:37.000000 roj-0.2.2/README.md
--rw-rw-r--   0 ek        (1000) ek        (1000)       89 2023-02-11 05:57:50.000000 roj-0.2.2/pyproject.toml
-drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-03-20 07:25:41.137694 roj-0.2.2/roj/
--rw-rw-r--   0 ek        (1000) ek        (1000)     7066 2023-03-20 06:35:51.000000 roj-0.2.2/roj/__init__.py
--rw-rw-r--   0 ek        (1000) ek        (1000)      142 2023-02-11 06:32:06.000000 roj-0.2.2/roj/__main__.py
-drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-03-20 07:25:41.141693 roj-0.2.2/roj.egg-info/
--rw-rw-r--   0 ek        (1000) ek        (1000)     2585 2023-03-20 07:25:41.000000 roj-0.2.2/roj.egg-info/PKG-INFO
--rw-rw-r--   0 ek        (1000) ek        (1000)      212 2023-03-20 07:25:41.000000 roj-0.2.2/roj.egg-info/SOURCES.txt
--rw-rw-r--   0 ek        (1000) ek        (1000)        1 2023-03-20 07:25:41.000000 roj-0.2.2/roj.egg-info/dependency_links.txt
--rw-rw-r--   0 ek        (1000) ek        (1000)       42 2023-03-20 07:25:41.000000 roj-0.2.2/roj.egg-info/entry_points.txt
--rw-rw-r--   0 ek        (1000) ek        (1000)        4 2023-03-20 07:25:41.000000 roj-0.2.2/roj.egg-info/top_level.txt
--rw-rw-r--   0 ek        (1000) ek        (1000)      673 2023-03-20 07:25:41.141693 roj-0.2.2/setup.cfg
+drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-04-20 03:30:54.559776 roj-0.2.3/
+-rw-rw-r--   0 ek        (1000) ek        (1000)     1260 2023-02-11 05:57:50.000000 roj-0.2.3/LICENSE
+-rw-rw-r--   0 ek        (1000) ek        (1000)     2585 2023-04-20 03:30:54.559776 roj-0.2.3/PKG-INFO
+-rw-rw-r--   0 ek        (1000) ek        (1000)     2043 2023-03-20 07:20:37.000000 roj-0.2.3/README.md
+-rw-rw-r--   0 ek        (1000) ek        (1000)       89 2023-02-11 05:57:50.000000 roj-0.2.3/pyproject.toml
+drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-04-20 03:30:54.559776 roj-0.2.3/roj/
+-rw-rw-r--   0 ek        (1000) ek        (1000)     7065 2023-04-20 03:24:48.000000 roj-0.2.3/roj/__init__.py
+-rw-rw-r--   0 ek        (1000) ek        (1000)      142 2023-02-11 06:32:06.000000 roj-0.2.3/roj/__main__.py
+drwxrwxr-x   0 ek        (1000) ek        (1000)        0 2023-04-20 03:30:54.559776 roj-0.2.3/roj.egg-info/
+-rw-rw-r--   0 ek        (1000) ek        (1000)     2585 2023-04-20 03:30:54.000000 roj-0.2.3/roj.egg-info/PKG-INFO
+-rw-rw-r--   0 ek        (1000) ek        (1000)      212 2023-04-20 03:30:54.000000 roj-0.2.3/roj.egg-info/SOURCES.txt
+-rw-rw-r--   0 ek        (1000) ek        (1000)        1 2023-04-20 03:30:54.000000 roj-0.2.3/roj.egg-info/dependency_links.txt
+-rw-rw-r--   0 ek        (1000) ek        (1000)       42 2023-04-20 03:30:54.000000 roj-0.2.3/roj.egg-info/entry_points.txt
+-rw-rw-r--   0 ek        (1000) ek        (1000)        4 2023-04-20 03:30:54.000000 roj-0.2.3/roj.egg-info/top_level.txt
+-rw-rw-r--   0 ek        (1000) ek        (1000)      673 2023-04-20 03:30:54.559776 roj-0.2.3/setup.cfg
```

### Comparing `roj-0.2.2/LICENSE` & `roj-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `roj-0.2.2/PKG-INFO` & `roj-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roj
-Version: 0.2.2
+Version: 0.2.3
 Summary: roj (run on jail) runs a command (login shell by default) on a local or remote jail
 Home-page: https://github.com/astralblue/roj
 Author: Eugene M. Kim
 Author-email: astralblue@gmail.com
 Project-URL: Bug Tracker, https://github.com/astralblue/roj/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `roj-0.2.2/README.md` & `roj-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `roj-0.2.2/roj/__init__.py` & `roj-0.2.3/roj/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                                 help="""jail host; passed to OpenSSH ssh(1) so
                                         ssh_config(5) aliases also work""")
             user = parser.add_mutually_exclusive_group()
             user.add_argument('--user', '-u', metavar='<USER>',
                               help="""username (in jail) or uid to run as""")
             tty = parser.add_mutually_exclusive_group()
             tty.add_argument('--tty', '-t',
-                             action='store_const', dest='tty', const=False,
+                             action='store_const', dest='tty', const=True,
                              help="""allocate TTY when running remotely""")
             tty.add_argument('--no-tty', '-T',
                              action='store_const', dest='tty', const=False,
                              help="""do not allocate TTY when running
                                      remotely""")
             parser.add_argument('--full', '-f', action='store_const',
                                 dest='full', const=True,
```

### Comparing `roj-0.2.2/roj.egg-info/PKG-INFO` & `roj-0.2.3/roj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roj
-Version: 0.2.2
+Version: 0.2.3
 Summary: roj (run on jail) runs a command (login shell by default) on a local or remote jail
 Home-page: https://github.com/astralblue/roj
 Author: Eugene M. Kim
 Author-email: astralblue@gmail.com
 Project-URL: Bug Tracker, https://github.com/astralblue/roj/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `roj-0.2.2/setup.cfg` & `roj-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = roj
-version = 0.2.2
+version = 0.2.3
 author = Eugene M. Kim
 author_email = astralblue@gmail.com
 description = roj (run on jail) runs a command (login shell by default) on a local or remote jail
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/astralblue/roj
 project_urls =
```

