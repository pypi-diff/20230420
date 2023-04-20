# Comparing `tmp/avsos-0.0.6.tar.gz` & `tmp/avsos-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.6.tar", last modified: Thu Apr 20 08:15:56 2023, max compression
+gzip compressed data, was "avsos-0.0.7.tar", last modified: Thu Apr 20 08:30:44 2023, max compression
```

## Comparing `avsos-0.0.6.tar` & `avsos-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.925944 avsos-0.0.6/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:15:56.925944 avsos-0.0.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2938 2023-04-20 07:57:35.000000 avsos-0.0.6/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.917940 avsos-0.0.6/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.6/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.6/avsos/config.ini
--rwxrwxr-x   0 kali      (1000) kali      (1000)     1440 2023-04-20 08:08:45.000000 avsos-0.0.6/avsos/config.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     3283 2023-04-20 08:11:09.000000 avsos-0.0.6/avsos/encryption.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.6/avsos/main.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 00:27:49.000000 avsos-0.0.6/avsos/osint.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.6/avsos/portscan.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.6/avsos/setup.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.6/avsos/start_zap.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.6/avsos/utils.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.6/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.921942 avsos-0.0.6/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      378 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      208 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 08:15:56.925944 avsos-0.0.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      407 2023-04-20 08:02:34.000000 avsos-0.0.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:30:44.233373 avsos-0.0.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:30:44.233373 avsos-0.0.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2938 2023-04-20 07:57:35.000000 avsos-0.0.7/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:30:44.225369 avsos-0.0.7/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.7/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.7/avsos/config.ini
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     1440 2023-04-20 08:08:45.000000 avsos-0.0.7/avsos/config.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     3283 2023-04-20 08:11:09.000000 avsos-0.0.7/avsos/encryption.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.7/avsos/main.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 08:28:21.000000 avsos-0.0.7/avsos/osint.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.7/avsos/portscan.py
+-rw-rw-rw-   0 kali      (1000) kali      (1000)  1140036 2023-03-22 16:54:30.000000 avsos-0.0.7/avsos/service-names-port-numbers.csv
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.7/avsos/setup.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.7/avsos/start_zap.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.7/avsos/utils.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.7/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:30:44.233373 avsos-0.0.7/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      415 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      208 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 08:30:44.000000 avsos-0.0.7/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 08:30:44.233373 avsos-0.0.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      441 2023-04-20 08:30:34.000000 avsos-0.0.7/setup.py
```

### Comparing `avsos-0.0.6/README.md` & `avsos-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/config.py` & `avsos-0.0.7/avsos/config.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/encryption.py` & `avsos-0.0.7/avsos/encryption.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/main.py` & `avsos-0.0.7/avsos/main.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/osint.py` & `avsos-0.0.7/avsos/osint.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return domain, whois_data
     except subprocess.CalledProcessError as e:
         logging.error(f"\nError retrieving whois information for {target}: {e}")
         traceback.print_exc()
         return None, None
 
 # Domains at risk
-def domain_at_risk(urls, threshold_days=300):
+def domain_at_risk(urls, threshold_days=150):
     domains_at_risk = []
     current_datetime = datetime.now(timezone.utc)  # Define the current_datetime variable
 
     for url in urls:
         domain, info = get_whois_info(url)
         if domain is None:
             continue
```

### Comparing `avsos-0.0.6/avsos/portscan.py` & `avsos-0.0.7/avsos/portscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/utils.py` & `avsos-0.0.7/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.6/avsos/zapscan.py` & `avsos-0.0.7/avsos/zapscan.py`

 * *Files identical despite different names*

