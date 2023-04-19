# Comparing `tmp/avsos-0.0.3.tar.gz` & `tmp/avsos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.3.tar", last modified: Mon Apr 17 22:08:54 2023, max compression
+gzip compressed data, was "avsos-0.0.4.tar", last modified: Wed Apr 19 23:37:15 2023, max compression
```

## Comparing `avsos-0.0.3.tar` & `avsos-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.061499 avsos-0.0.3/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 22:08:54.061499 avsos-0.0.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1469 2023-04-17 20:18:08.000000 avsos-0.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.053503 avsos-0.0.3/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.3/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.3/avsos/config.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.3/avsos/encryption.py
--rw-r--r--   0 kali      (1000) kali      (1000)    17539 2023-04-17 22:03:35.000000 avsos-0.0.3/avsos/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.3/avsos/osint.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5577 2023-04-17 22:07:00.000000 avsos-0.0.3/avsos/portscan.py
--rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.3/avsos/setup.py
--rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.3/avsos/start_zap.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.3/avsos/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5485 2023-04-17 22:04:18.000000 avsos-0.0.3/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-17 22:08:54.061499 avsos-0.0.3/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      117 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-17 22:08:53.000000 avsos-0.0.3/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-17 22:08:54.061499 avsos-0.0.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-17 22:07:25.000000 avsos-0.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.927120 avsos-0.0.4/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-19 23:37:15.927120 avsos-0.0.4/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2775 2023-04-17 22:24:22.000000 avsos-0.0.4/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.923122 avsos-0.0.4/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.4/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.4/avsos/config.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.4/avsos/encryption.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    17544 2023-04-19 23:35:45.000000 avsos-0.0.4/avsos/main.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.4/avsos/osint.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5577 2023-04-17 22:07:00.000000 avsos-0.0.4/avsos/portscan.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.4/avsos/setup.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.4/avsos/start_zap.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.4/avsos/utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5485 2023-04-17 22:04:18.000000 avsos-0.0.4/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.927120 avsos-0.0.4/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      207 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-19 23:37:15.927120 avsos-0.0.4/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-19 23:37:11.000000 avsos-0.0.4/setup.py
```

### Comparing `avsos-0.0.3/avsos/config.py` & `avsos-0.0.4/avsos/config.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.3/avsos/encryption.py` & `avsos-0.0.4/avsos/encryption.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.3/avsos/main.py` & `avsos-0.0.4/avsos/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                 amass_output = subprocess.run(["amass", "enum", "-df", args.subdomains_file], check=True, text=True)
                 amass_results = amass_output.stdout.splitlines()
                 subdomains = amass_results
                 report_data["File Subdomains"] = subdomains
         except FileNotFoundError:
             print(f"Error: File {args.subdomains_file} not found.")
 
-    if args.enum or args.all:  # subdomain enumeration
+        if args.enum or args.all:  # subdomain enumeration
         try:
             if args.whois or args.all:
                 # Run Amass and Whois concurrently
                 with concurrent.futures.ThreadPoolExecutor() as executor:
                     amass_future = executor.submit(osint.amass, target)
                     whois_future = executor.submit(osint.get_whois_info, target)
 
@@ -265,14 +265,15 @@
             domains_at_risk_list = osint.check_domain_hijacking(whois_info)
             domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
             report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
             report_data["Domains at risk of hijacking"] = domains_at_risk_text
         except Exception as e:
             print(f"Error running the selected scans: {e}")
 
+
     if args.zap or args.all:
         try:
             logging.debug("Running ZAP...")
             print("\nRunning ZAP Scan...")
             if api_key is None:
                 print("Error retrieving ZAP API key.")
                 return
```

### Comparing `avsos-0.0.3/avsos/osint.py` & `avsos-0.0.4/avsos/osint.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.3/avsos/portscan.py` & `avsos-0.0.4/avsos/portscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.3/avsos/utils.py` & `avsos-0.0.4/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.3/avsos/zapscan.py` & `avsos-0.0.4/avsos/zapscan.py`

 * *Files identical despite different names*

