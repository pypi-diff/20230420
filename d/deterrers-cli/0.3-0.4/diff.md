# Comparing `tmp/deterrers-cli-0.3.tar.gz` & `tmp/deterrers-cli-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deterrers-cli-0.3.tar", last modified: Mon Apr 17 13:38:13 2023, max compression
+gzip compressed data, was "deterrers-cli-0.4.tar", last modified: Thu Apr 20 14:03:30 2023, max compression
```

## Comparing `deterrers-cli-0.3.tar` & `deterrers-cli-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/
--rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.3/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.3/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-17 13:38:13.508019 deterrers-cli-0.3/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     1908 2023-04-17 13:28:29.000000 deterrers-cli-0.3/README.md
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/deterrers_cli.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/entry_points.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/requires.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-17 13:38:13.000000 deterrers-cli-0.3/deterrers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-17 13:38:13.508019 deterrers-cli-0.3/deterrerscli/
--rw-r--r--   0 lars      (1000) lars      (1000)     2437 2023-04-17 13:23:20.000000 deterrers-cli-0.3/deterrerscli/__main__.py
--rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-17 13:20:44.000000 deterrers-cli-0.3/requirements.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-17 13:38:13.508019 deterrers-cli-0.3/setup.cfg
--rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-17 13:21:20.000000 deterrers-cli-0.3/setup.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/
+-rw-r--r--   0 lars      (1000) lars      (1000)     1135 2023-04-13 21:11:45.000000 deterrers-cli-0.4/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)       43 2023-04-13 21:06:33.000000 deterrers-cli-0.4/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-20 14:03:30.405842 deterrers-cli-0.4/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     1908 2023-04-17 13:28:29.000000 deterrers-cli-0.4/README.md
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/deterrers_cli.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2178 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)      304 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       61 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/requires.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       13 2023-04-20 14:03:30.000000 deterrers-cli-0.4/deterrers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2023-04-20 14:03:30.405842 deterrers-cli-0.4/deterrerscli/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2649 2023-04-20 14:00:49.000000 deterrers-cli-0.4/deterrerscli/__main__.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       32 2023-04-20 13:51:57.000000 deterrers-cli-0.4/requirements.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2023-04-20 14:03:30.405842 deterrers-cli-0.4/setup.cfg
+-rw-r--r--   0 lars      (1000) lars      (1000)      782 2023-04-20 13:51:57.000000 deterrers-cli-0.4/setup.py
```

### Comparing `deterrers-cli-0.3/LICENSE` & `deterrers-cli-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.3/PKG-INFO` & `deterrers-cli-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.3
+Version: 0.4
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.3/README.md` & `deterrers-cli-0.4/README.md`

 * *Files identical despite different names*

### Comparing `deterrers-cli-0.3/deterrers_cli.egg-info/PKG-INFO` & `deterrers-cli-0.4/deterrers_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deterrers-cli
-Version: 0.3
+Version: 0.4
 Summary: Command line client for DETERRERS
 Home-page: https://github.com/virtUOS/proteuscmd
 Author: Lars Kiesow
 Author-email: lkiesow@uos.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `deterrers-cli-0.3/deterrerscli/__main__.py` & `deterrers-cli-0.4/deterrerscli/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,21 +64,26 @@
 def add(ipv4, admin, profile, firewall):
     '''Add IP address to DETERRERS.
     '''
     deterrers.add(ipv4, admin, profile, firewall)
 
 
 @cli.command()
-@click.option('--profile', '-p', default='', type=profiles)
-@click.option('--firewall', '-f', default='', type=host_firewalls)
+@click.option('--admin', '-a', default=None, multiple=True)
+@click.option('--profile', '-p', default=None, type=profiles)
+@click.option('--firewall', '-f', default=None, type=host_firewalls)
 @click.argument('ipv4')
-def update(ipv4, profile, firewall):
+def update(ipv4, admin, profile, firewall):
     '''Update IP address in DETERRERS.
+
+    Fields which are not specified will not be changed.
+    The option `admin` can be used multiple times.
     '''
-    deterrers.update(ipv4, profile, firewall)
+    admin = admin or None
+    deterrers.update(ipv4, profile, firewall, admin)
 
 
 @cli.group()
 def action():
     '''Activate firewall profile or block IP address in perimeter firewall.
     '''
     pass
```

### Comparing `deterrers-cli-0.3/setup.py` & `deterrers-cli-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     path = os.path.abspath(os.path.dirname(__file__))
     with open(os.path.join(path, filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='deterrers-cli',
-    version='0.3',
+    version='0.4',
     description='Command line client for DETERRERS',
     url='https://github.com/virtUOS/proteuscmd',
     author='Lars Kiesow',
     author_email='lkiesow@uos.de',
     license='MIT',
     packages=['deterrerscli'],
     license_files=('LICENSE'),
```

