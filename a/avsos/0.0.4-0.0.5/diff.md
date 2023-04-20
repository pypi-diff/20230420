# Comparing `tmp/avsos-0.0.4.tar.gz` & `tmp/avsos-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.4.tar", last modified: Wed Apr 19 23:37:15 2023, max compression
+gzip compressed data, was "avsos-0.0.5.tar", last modified: Thu Apr 20 03:54:46 2023, max compression
```

## Comparing `avsos-0.0.4.tar` & `avsos-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.927120 avsos-0.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-19 23:37:15.927120 avsos-0.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2775 2023-04-17 22:24:22.000000 avsos-0.0.4/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.923122 avsos-0.0.4/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.4/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1308 2023-04-17 10:40:51.000000 avsos-0.0.4/avsos/config.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.4/avsos/encryption.py
--rw-r--r--   0 kali      (1000) kali      (1000)    17544 2023-04-19 23:35:45.000000 avsos-0.0.4/avsos/main.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5753 2023-04-14 19:31:26.000000 avsos-0.0.4/avsos/osint.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5577 2023-04-17 22:07:00.000000 avsos-0.0.4/avsos/portscan.py
--rw-r--r--   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.4/avsos/setup.py
--rw-r--r--   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.4/avsos/start_zap.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.4/avsos/utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5485 2023-04-17 22:04:18.000000 avsos-0.0.4/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-19 23:37:15.927120 avsos-0.0.4/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      361 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      207 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-19 23:37:15.000000 avsos-0.0.4/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-19 23:37:15.927120 avsos-0.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      349 2023-04-19 23:37:11.000000 avsos-0.0.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.873309 avsos-0.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 03:54:46.873309 avsos-0.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2775 2023-04-17 22:24:22.000000 avsos-0.0.5/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.861303 avsos-0.0.5/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.5/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.5/avsos/config.ini
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     1312 2023-04-20 00:32:37.000000 avsos-0.0.5/avsos/config.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.5/avsos/encryption.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.5/avsos/main.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 00:27:49.000000 avsos-0.0.5/avsos/osint.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.5/avsos/portscan.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.5/avsos/setup.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.5/avsos/start_zap.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.5/avsos/utils.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.5/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.873309 avsos-0.0.5/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      378 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      192 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 03:54:46.877311 avsos-0.0.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      407 2023-04-20 03:53:50.000000 avsos-0.0.5/setup.py
```

### Comparing `avsos-0.0.4/README.md` & `avsos-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `avsos-0.0.4/avsos/config.py` & `avsos-0.0.5/avsos/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # config.py
 import configparser
 
+
 class ScannerConfig:
     def __init__(self):
         self.config = configparser.ConfigParser()
         self.config.read("config.ini")
 
     @property
     def output_format(self):
@@ -36,12 +37,12 @@
 
     @property
     def zap_api_key(self):
         return self.config.get("zap", "api_key", fallback=None)
 
     @property
     def zap_path(self):
-    	return self.config.get("zap", "zap_path")
+        return self.config.get("zap", "zap_path")
 
     @property
     def time_interval(self):
         return self.config.getint("schedule", "time_interval", fallback=None)
```

### Comparing `avsos-0.0.4/avsos/encryption.py` & `avsos-0.0.5/avsos/encryption.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.4/avsos/main.py` & `avsos-0.0.5/avsos/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import osint
-import zapscan
-import portscan
-import encryption
-import utils
+from . import osint
+from . import zapscan
+from . import portscan
+from . import encryption
+from . import utils
 import argparse
 import traceback
 import subprocess
-from config import ScannerConfig
+from .config import ScannerConfig
 import configparser
 import json
 from datetime import datetime
 import os
 import time
 import schedule
 import logging
@@ -227,53 +227,49 @@
                 amass_output = subprocess.run(["amass", "enum", "-df", args.subdomains_file], check=True, text=True)
                 amass_results = amass_output.stdout.splitlines()
                 subdomains = amass_results
                 report_data["File Subdomains"] = subdomains
         except FileNotFoundError:
             print(f"Error: File {args.subdomains_file} not found.")
 
-        if args.enum or args.all:  # subdomain enumeration
-        try:
-            if args.whois or args.all:
-                # Run Amass and Whois concurrently
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    amass_future = executor.submit(osint.amass, target)
-                    whois_future = executor.submit(osint.get_whois_info, target)
-
-                subdomains = amass_future.result()
-                whois_info = whois_future.result()
-                report_data["Subdomains"] = subdomains
-                formatted_whois_info = osint.format_whois_output(whois_info)
-                print(formatted_whois_info)
-                domains_at_risk_list = osint.check_domain_hijacking(whois_info)
-                domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
-                report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
-                report_data["Domains at risk of hijacking"] = domains_at_risk_text
-            else:
-                logging.debug("Running Amass...")
-                print("\nRunning Amass...")
-                subdomains = osint.amass(target)
-                report_data["Subdomains"] = subdomains
-        except Exception as e:
-            print(f"Error running the selected scans: {e}")
+    if args.enum or args.all:  # subdomain enumeration
+        if args.whois or args.all:
+            # Run Amass and Whois concurrently
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                amass_future = executor.submit(osint.amass, target)
+                whois_future = executor.submit(osint.get_whois_info, target)
+
+            subdomains = amass_future.result()
+            whois_info = whois_future.result()
+            report_data["Subdomains"] = subdomains
+            formatted_whois_info = osint.format_whois_output(whois_info)
+            print(formatted_whois_info)
+            domains_at_risk_list = osint.check_domain_hijacking(whois_info)
+            domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
+            report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
+            report_data["Domains at risk of hijacking"] = domains_at_risk_text
+        else:
+            logging.debug("Running Amass...")
+            print("\nRunning Amass...")
+            subdomains = osint.amass(target)
+            report_data["Subdomains"] = subdomains
     elif args.whois or args.all:
         try:
             logging.debug("Running WHOIS...")
             print("\nRunning Whois...")
             whois_info = osint.get_whois_info(target)
             formatted_whois_info = osint.format_whois_output(whois_info)
             print(formatted_whois_info)
             domains_at_risk_list = osint.check_domain_hijacking(whois_info)
             domains_at_risk_text = "\n".join(domains_at_risk_list) if domains_at_risk_list else "None"
             report_data['WHOIS'] = formatted_whois_info  # Add Whois information to report_data
             report_data["Domains at risk of hijacking"] = domains_at_risk_text
         except Exception as e:
             print(f"Error running the selected scans: {e}")
 
-
     if args.zap or args.all:
         try:
             logging.debug("Running ZAP...")
             print("\nRunning ZAP Scan...")
             if api_key is None:
                 print("Error retrieving ZAP API key.")
                 return
@@ -331,15 +327,14 @@
                 # Add the subdomains Nmap scan results to the report_data
                 subdomain_nmap_report_str = portscan.print_report(subdomain_nmap_data)
                 print(subdomain_nmap_report_str)
                 report_data['Port Scan']['Subdomains'] = subdomain_nmap_report_str
             except Exception as e:
                 print(f"Error running the selected scans: {e}")
 
-
     if args.debug:
         utils.enable_debugging()
 
     if args.encrypt_file:
         encryption.encrypt_existing_file(args.encrypt_file)
         return
```

### Comparing `avsos-0.0.4/avsos/osint.py` & `avsos-0.0.5/avsos/osint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import dateutil.parser
 import subprocess
 import whois
 from datetime import datetime, timedelta, timezone
-import utils
+from . import utils
 import logging
 import socket
 import json
 import re
 import traceback
 
 # Set up logging
```

### Comparing `avsos-0.0.4/avsos/portscan.py` & `avsos-0.0.5/avsos/portscan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import nmap
 import csv
-import utils
+from . import utils
 import os
 import textwrap
 
 
 # Function to run Nmap scan on a given URL
 def run_nmap(urls, only_vulners=True):
     nm = nmap.PortScanner()
```

### Comparing `avsos-0.0.4/avsos/utils.py` & `avsos-0.0.5/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.4/avsos/zapscan.py` & `avsos-0.0.5/avsos/zapscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from zapv2 import ZAPv2
 import subprocess
-import utils
+from . import utils
 import matplotlib.pyplot as plt
 import datetime
 import logging
 import sys
 
 logging.basicConfig(filename="zapscan.log", level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
```

