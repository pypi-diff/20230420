# Comparing `tmp/avsos-0.0.5.tar.gz` & `tmp/avsos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsos-0.0.5.tar", last modified: Thu Apr 20 03:54:46 2023, max compression
+gzip compressed data, was "avsos-0.0.6.tar", last modified: Thu Apr 20 08:15:56 2023, max compression
```

## Comparing `avsos-0.0.5.tar` & `avsos-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.873309 avsos-0.0.5/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 03:54:46.873309 avsos-0.0.5/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     2775 2023-04-17 22:24:22.000000 avsos-0.0.5/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.861303 avsos-0.0.5/avsos/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.5/avsos/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.5/avsos/config.ini
--rwxrwxr-x   0 kali      (1000) kali      (1000)     1312 2023-04-20 00:32:37.000000 avsos-0.0.5/avsos/config.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     3303 2023-04-15 10:02:24.000000 avsos-0.0.5/avsos/encryption.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.5/avsos/main.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 00:27:49.000000 avsos-0.0.5/avsos/osint.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.5/avsos/portscan.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.5/avsos/setup.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.5/avsos/start_zap.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.5/avsos/utils.py
--rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.5/avsos/zapscan.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 03:54:46.873309 avsos-0.0.5/avsos.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      378 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      192 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 03:54:46.000000 avsos-0.0.5/avsos.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 03:54:46.877311 avsos-0.0.5/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      407 2023-04-20 03:53:50.000000 avsos-0.0.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.925944 avsos-0.0.6/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:15:56.925944 avsos-0.0.6/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     2938 2023-04-20 07:57:35.000000 avsos-0.0.6/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.917940 avsos-0.0.6/avsos/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-04-17 10:34:17.000000 avsos-0.0.6/avsos/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      261 2023-04-17 17:22:40.000000 avsos-0.0.6/avsos/config.ini
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     1440 2023-04-20 08:08:45.000000 avsos-0.0.6/avsos/config.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     3283 2023-04-20 08:11:09.000000 avsos-0.0.6/avsos/encryption.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)    17394 2023-04-20 00:30:11.000000 avsos-0.0.6/avsos/main.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5760 2023-04-20 00:27:49.000000 avsos-0.0.6/avsos/osint.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5584 2023-04-20 00:28:39.000000 avsos-0.0.6/avsos/portscan.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      353 2023-04-17 10:29:11.000000 avsos-0.0.6/avsos/setup.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)      480 2023-04-17 16:53:14.000000 avsos-0.0.6/avsos/start_zap.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     4077 2023-04-13 00:12:44.000000 avsos-0.0.6/avsos/utils.py
+-rwxrwxr-x   0 kali      (1000) kali      (1000)     5492 2023-04-20 00:26:38.000000 avsos-0.0.6/avsos/zapscan.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-20 08:15:56.921942 avsos-0.0.6/avsos.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)       49 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      378 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      208 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-20 08:15:56.000000 avsos-0.0.6/avsos.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-20 08:15:56.925944 avsos-0.0.6/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      407 2023-04-20 08:02:34.000000 avsos-0.0.6/setup.py
```

### Comparing `avsos-0.0.5/README.md` & `avsos-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 OR
 
 1. Open terminal
 2. sudo apt-get update
 3. pip install avsos
 
+## Debug
+- Add the location of avsos in your system to PATH so it can be run from anywhere in the system.
+- Install the latest version 'pip install avsos==x.y.z'
+
 ## Usage
 
 To run all scans on a domain, use the following command:
 
 avsos -d example.com -a
```

### Comparing `avsos-0.0.5/avsos/config.py` & `avsos-0.0.6/avsos/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # config.py
 import configparser
+import os
+import pathlib
 
 
 class ScannerConfig:
     def __init__(self):
         self.config = configparser.ConfigParser()
-        self.config.read("config.ini")
+        config_file_path = pathlib.Path(os.path.dirname(os.path.abspath(__file__))) / "config.ini"
+        self.config.read(config_file_path)
 
     @property
     def output_format(self):
         return self.config.get("general", "output_format", fallback="txt")
 
     @property
     def output_filename(self):
```

### Comparing `avsos-0.0.5/avsos/encryption.py` & `avsos-0.0.6/avsos/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,16 @@
                 key = generate_encryption_key()
             encrypted_data = encrypt_data(content, key)
         encrypted_file_path = f"{file_path}"
         with open(encrypted_file_path, "wb") as f:
             f.write(encrypted_data)
         print(f"Encrypted file saved as {encrypted_file_path}")
         print(f"Encryption key: {key}")
-    except FileNotFoundError:
-        print(f"Error: File {file_path} not found.")
+    except FileNotFoundError as e:
+        print(f"Error:{e}")
        
 def decrypt_report(encrypted_file, decrypted_file, decryption_key=None):
     """
     Decrypts an encrypted file and saves the decrypted content to a new file.
 
     Args:
         encrypted_file (str): Path to the encrypted file.
```

### Comparing `avsos-0.0.5/avsos/main.py` & `avsos-0.0.6/avsos/main.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.5/avsos/osint.py` & `avsos-0.0.6/avsos/osint.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.5/avsos/portscan.py` & `avsos-0.0.6/avsos/portscan.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.5/avsos/utils.py` & `avsos-0.0.6/avsos/utils.py`

 * *Files identical despite different names*

### Comparing `avsos-0.0.5/avsos/zapscan.py` & `avsos-0.0.6/avsos/zapscan.py`

 * *Files identical despite different names*

