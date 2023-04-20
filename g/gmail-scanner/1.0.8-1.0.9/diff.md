# Comparing `tmp/gmail_scanner-1.0.8.tar.gz` & `tmp/gmail_scanner-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_scanner-1.0.8.tar", last modified: Thu Apr 20 11:08:38 2023, max compression
+gzip compressed data, was "gmail_scanner-1.0.9.tar", last modified: Thu Apr 20 11:13:43 2023, max compression
```

## Comparing `gmail_scanner-1.0.8.tar` & `gmail_scanner-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:08:38.769479 gmail_scanner-1.0.8/
--rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.8/LICENSE
--rw-r--r--   0 ziji       (501) staff       (20)     3323 2023-04-20 11:08:38.769138 gmail_scanner-1.0.8/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)     2247 2023-04-20 11:08:28.000000 gmail_scanner-1.0.8/README.md
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:08:38.767435 gmail_scanner-1.0.8/gmail_scanner/
--rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.8/gmail_scanner/__init__.py
--rw-r--r--   0 ziji       (501) staff       (20)    11789 2023-04-20 11:07:40.000000 gmail_scanner-1.0.8/gmail_scanner/gmail_scanner.py
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:08:38.768826 gmail_scanner-1.0.8/gmail_scanner.egg-info/
--rw-r--r--   0 ziji       (501) staff       (20)     3323 2023-04-20 11:08:38.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 11:08:38.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 11:08:38.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/not-zip-safe
--rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 11:08:38.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/requires.txt
--rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 11:08:38.000000 gmail_scanner-1.0.8/gmail_scanner.egg-info/top_level.txt
--rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 11:08:38.769538 gmail_scanner-1.0.8/setup.cfg
--rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 11:08:02.000000 gmail_scanner-1.0.8/setup.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:13:43.890371 gmail_scanner-1.0.9/
+-rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.9/LICENSE
+-rw-r--r--   0 ziji       (501) staff       (20)     3352 2023-04-20 11:13:43.890074 gmail_scanner-1.0.9/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)     2276 2023-04-20 11:13:25.000000 gmail_scanner-1.0.9/README.md
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:13:43.888331 gmail_scanner-1.0.9/gmail_scanner/
+-rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.9/gmail_scanner/__init__.py
+-rw-r--r--   0 ziji       (501) staff       (20)    11874 2023-04-20 11:13:25.000000 gmail_scanner-1.0.9/gmail_scanner/gmail_scanner.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 11:13:43.889848 gmail_scanner-1.0.9/gmail_scanner.egg-info/
+-rw-r--r--   0 ziji       (501) staff       (20)     3352 2023-04-20 11:13:43.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 11:13:43.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 11:13:43.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 11:13:43.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/requires.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 11:13:43.000000 gmail_scanner-1.0.9/gmail_scanner.egg-info/top_level.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 11:13:43.890439 gmail_scanner-1.0.9/setup.cfg
+-rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 11:13:32.000000 gmail_scanner-1.0.9/setup.py
```

### Comparing `gmail_scanner-1.0.8/LICENSE` & `gmail_scanner-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_scanner-1.0.8/PKG-INFO` & `gmail_scanner-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail_scanner
-Version: 1.0.8
+Version: 1.0.9
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -46,14 +46,18 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.9
+
+- Fixed some bug
+
 ### 1.0.8
 
 - Fixed some bug
 
 ### 1.0.7
 
 - Fixed: out of range
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.8 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.9 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,29 +12,29 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.8 - Fixed some bug ### 1.0.7 - Fixed: out of range ### 1.0.6 -
-Feat: support for special num ### 1.0.5 - Fixed: logs dir ### 1.0.4 - Feat: add
-logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed: print None - Feat:
-print batch num and email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record
-results to a csv file. ## Usage **You need to install `gmail_scanner` before.**
-```bash pip install gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file
-with the following codes. ```python from gmail_scanner.gmail_scanner import
-check_one_gmail # Only Print Unregistered Result # admin is email prefix
-check_one_gmail(f"admin001") ``` 2. If you want to scan a lots of Gmail, you
-can use the following codes. ```python from gmail_scanner.gmail_scanner import
-scan_int_single, scan_int_multi # single process mode(slow) to scan 6-digit
+Update ### 1.0.9 - Fixed some bug ### 1.0.8 - Fixed some bug ### 1.0.7 - Fixed:
+out of range ### 1.0.6 - Feat: support for special num ### 1.0.5 - Fixed: logs
+dir ### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 -
+Fixed: print None - Feat: print batch num and email num ### 1.0.1 - Fixed some
+bug ### 1.0.0 - Record results to a csv file. ## Usage **You need to install
+`gmail_scanner` before.** ```bash pip install gmail_scanner ``` ### Lite Mode
+1. Create a new `.py` file with the following codes. ```python from
+gmail_scanner.gmail_scanner import check_one_gmail # Only Print Unregistered
+Result # admin is email prefix check_one_gmail(f"admin001") ``` 2. If you want
+to scan a lots of Gmail, you can use the following codes. ```python from
+gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi # single
+process mode(slow) to scan 6-digit gmail mailboxes start_num = 0 end_num =
+999999 email_length = 6 output_file = f'results.csv' scan_int_single(start_num,
+end_num, email_length, output_file) # multi process mode(fast) to scan 6-digit
 gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
-f'results.csv' scan_int_single(start_num, end_num, email_length, output_file) #
-multi process mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num
-= 999999 email_length = 6 output_file = f'results.csv' batch_num = 1000
-process_num = 20 scan_int_multi(start_num, end_num, email_length, output_file,
-batch_num, process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp config-
-example.yml config.yml touch results.csv mkdir logs # edit the .env file
-docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
-github.com/Annihilater), Released under the [MIT](./LICENSE) License.
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp config-example.yml config.yml touch results.csv mkdir logs #
+edit the .env file docker-compose up -d ``` ## Author **GmailScanner** Â© [coo]
+(https://github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.8/README.md` & `gmail_scanner-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.9
+
+- Fixed some bug
+
 ### 1.0.8
 
 - Fixed some bug
 
 ### 1.0.7
 
 - Fixed: out of range
```

### Comparing `gmail_scanner-1.0.8/gmail_scanner/gmail_scanner.py` & `gmail_scanner-1.0.9/gmail_scanner/gmail_scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,16 @@
     current_batch = 1
     for i in range(0, len(email_prefix_list), batch):
         with open(log_file_name, mode='a', encoding='utf8') as f:
             text = f"current_batch: {current_batch} current_num: {i} total: {len(email_prefix_list)}\n"
             f.write(text)
 
         args = []
-        for j in range(i, i + batch - 1):
+        end = len(email_prefix_list) - i if len(email_prefix_list) - i < batch else batch
+
+        for j in range(i, i + end):
             email_prefix = email_prefix_list[j]
             args.append([email_prefix, output_file])
 
         with Pool(processes=processes) as pool:
             list((tqdm(pool.imap(task, args), total=len(args), desc='process')))
         current_batch += 1
```

### Comparing `gmail_scanner-1.0.8/gmail_scanner.egg-info/PKG-INFO` & `gmail_scanner-1.0.9/gmail_scanner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-scanner
-Version: 1.0.8
+Version: 1.0.9
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -46,14 +46,18 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.9
+
+- Fixed some bug
+
 ### 1.0.8
 
 - Fixed some bug
 
 ### 1.0.7
 
 - Fixed: out of range
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.8 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.9 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,29 +12,29 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.8 - Fixed some bug ### 1.0.7 - Fixed: out of range ### 1.0.6 -
-Feat: support for special num ### 1.0.5 - Fixed: logs dir ### 1.0.4 - Feat: add
-logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed: print None - Feat:
-print batch num and email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record
-results to a csv file. ## Usage **You need to install `gmail_scanner` before.**
-```bash pip install gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file
-with the following codes. ```python from gmail_scanner.gmail_scanner import
-check_one_gmail # Only Print Unregistered Result # admin is email prefix
-check_one_gmail(f"admin001") ``` 2. If you want to scan a lots of Gmail, you
-can use the following codes. ```python from gmail_scanner.gmail_scanner import
-scan_int_single, scan_int_multi # single process mode(slow) to scan 6-digit
+Update ### 1.0.9 - Fixed some bug ### 1.0.8 - Fixed some bug ### 1.0.7 - Fixed:
+out of range ### 1.0.6 - Feat: support for special num ### 1.0.5 - Fixed: logs
+dir ### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 -
+Fixed: print None - Feat: print batch num and email num ### 1.0.1 - Fixed some
+bug ### 1.0.0 - Record results to a csv file. ## Usage **You need to install
+`gmail_scanner` before.** ```bash pip install gmail_scanner ``` ### Lite Mode
+1. Create a new `.py` file with the following codes. ```python from
+gmail_scanner.gmail_scanner import check_one_gmail # Only Print Unregistered
+Result # admin is email prefix check_one_gmail(f"admin001") ``` 2. If you want
+to scan a lots of Gmail, you can use the following codes. ```python from
+gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi # single
+process mode(slow) to scan 6-digit gmail mailboxes start_num = 0 end_num =
+999999 email_length = 6 output_file = f'results.csv' scan_int_single(start_num,
+end_num, email_length, output_file) # multi process mode(fast) to scan 6-digit
 gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
-f'results.csv' scan_int_single(start_num, end_num, email_length, output_file) #
-multi process mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num
-= 999999 email_length = 6 output_file = f'results.csv' batch_num = 1000
-process_num = 20 scan_int_multi(start_num, end_num, email_length, output_file,
-batch_num, process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-
-000000?style=for-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp config-
-example.yml config.yml touch results.csv mkdir logs # edit the .env file
-docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
-github.com/Annihilater), Released under the [MIT](./LICENSE) License.
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp config-example.yml config.yml touch results.csv mkdir logs #
+edit the .env file docker-compose up -d ``` ## Author **GmailScanner** Â© [coo]
+(https://github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.8/setup.py` & `gmail_scanner-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="gmail_scanner",
-    version="1.0.8",
+    version="1.0.9",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="coo",
     author_email="me@coo.lol",
     maintainer="coo",
     maintainer_email="me@coo.lol",
```

