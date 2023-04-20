# Comparing `tmp/gmail_scanner-1.0.3.tar.gz` & `tmp/gmail_scanner-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_scanner-1.0.3.tar", last modified: Thu Apr 20 03:34:02 2023, max compression
+gzip compressed data, was "gmail_scanner-1.0.4.tar", last modified: Thu Apr 20 03:39:01 2023, max compression
```

## Comparing `gmail_scanner-1.0.3.tar` & `gmail_scanner-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:34:02.023835 gmail_scanner-1.0.3/
--rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.3/LICENSE
--rw-r--r--   0 ziji       (501) staff       (20)     3130 2023-04-20 03:34:02.023642 gmail_scanner-1.0.3/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)     2054 2023-04-20 03:32:06.000000 gmail_scanner-1.0.3/README.md
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:34:02.021899 gmail_scanner-1.0.3/gmail_scanner/
--rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.3/gmail_scanner/__init__.py
--rw-r--r--   0 ziji       (501) staff       (20)     6923 2023-04-20 03:28:28.000000 gmail_scanner-1.0.3/gmail_scanner/gmail_scanner.py
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:34:02.023393 gmail_scanner-1.0.3/gmail_scanner.egg-info/
--rw-r--r--   0 ziji       (501) staff       (20)     3130 2023-04-20 03:34:01.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 03:34:01.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 03:34:01.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/not-zip-safe
--rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 03:34:01.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/requires.txt
--rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 03:34:01.000000 gmail_scanner-1.0.3/gmail_scanner.egg-info/top_level.txt
--rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 03:34:02.023892 gmail_scanner-1.0.3/setup.cfg
--rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 03:32:22.000000 gmail_scanner-1.0.3/setup.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:39:01.417702 gmail_scanner-1.0.4/
+-rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.4/LICENSE
+-rw-r--r--   0 ziji       (501) staff       (20)     3163 2023-04-20 03:39:01.417354 gmail_scanner-1.0.4/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)     2087 2023-04-20 03:38:55.000000 gmail_scanner-1.0.4/README.md
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:39:01.413703 gmail_scanner-1.0.4/gmail_scanner/
+-rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.4/gmail_scanner/__init__.py
+-rw-r--r--   0 ziji       (501) staff       (20)     6927 2023-04-20 03:35:44.000000 gmail_scanner-1.0.4/gmail_scanner/gmail_scanner.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:39:01.416458 gmail_scanner-1.0.4/gmail_scanner.egg-info/
+-rw-r--r--   0 ziji       (501) staff       (20)     3163 2023-04-20 03:39:01.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 03:39:01.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 03:39:01.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 03:39:01.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/requires.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 03:39:01.000000 gmail_scanner-1.0.4/gmail_scanner.egg-info/top_level.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 03:39:01.417774 gmail_scanner-1.0.4/setup.cfg
+-rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 03:38:29.000000 gmail_scanner-1.0.4/setup.py
```

### Comparing `gmail_scanner-1.0.3/LICENSE` & `gmail_scanner-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_scanner-1.0.3/PKG-INFO` & `gmail_scanner-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail_scanner
-Version: 1.0.3
+Version: 1.0.4
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
 
+### 1.0.4
+
+- Feat: add logs dir
+
 ### 1.0.3
 
 - Feat: log to file
 
 ### 1.0.2
 
 - Fixed: print None
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.3 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.4 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,27 +12,27 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed: print None - Feat:
-print batch num and email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record
-results to a csv file. ## Usage **You need to install `gmail_scanner` before.**
-```bash pip install gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file
-with the following codes. ```python from gmail_scanner.gmail_scanner import
-check_one_gmail # Only Print Unregistered Result # admin is email prefix
-check_one_gmail(f"admin001") ``` 2. If you want to scan a lots of Gmail, you
-can use the following codes. ```python from gmail_scanner.gmail_scanner import
-scan_int_single, scan_int_multi # single process mode(slow) to scan 6-digit
+Update ### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 -
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
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example
-.env touch results.csv # edit the .env file docker-compose up -d ``` ## Author
-**GmailScanner** Â© [coo](https://github.com/Annihilater), Released under the
-[MIT](./LICENSE) License.
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp .env.example .env touch results.csv # edit the .env file
+docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
+github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.3/README.md` & `gmail_scanner-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
+### 1.0.4
+
+- Feat: add logs dir
+
 ### 1.0.3
 
 - Feat: log to file
 
 ### 1.0.2
 
 - Fixed: print None
```

### Comparing `gmail_scanner-1.0.3/gmail_scanner/gmail_scanner.py` & `gmail_scanner-1.0.4/gmail_scanner/gmail_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     :param end:
     :param email_length:
     :param output_file:
     :param batch: default 1000, When processing in batches, the number of batches
     :param processes: default 4
     :return:
     """
-    log_file_name = f"gmail_scanner_{current_time()}.log"
+    log_file_name = f"log/gmail_scanner_{current_time()}.log"
 
     current_batch = 1
     for i in range(start, end, batch):
         with open(log_file_name, mode='a', encoding='utf8') as f:
             text = f"current_batch: {current_batch} current_num: {i}\n"
             f.write(text)
```

### Comparing `gmail_scanner-1.0.3/gmail_scanner.egg-info/PKG-INFO` & `gmail_scanner-1.0.4/gmail_scanner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-scanner
-Version: 1.0.3
+Version: 1.0.4
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
 
+### 1.0.4
+
+- Feat: add logs dir
+
 ### 1.0.3
 
 - Feat: log to file
 
 ### 1.0.2
 
 - Fixed: print None
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.3 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.4 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,27 +12,27 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed: print None - Feat:
-print batch num and email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record
-results to a csv file. ## Usage **You need to install `gmail_scanner` before.**
-```bash pip install gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file
-with the following codes. ```python from gmail_scanner.gmail_scanner import
-check_one_gmail # Only Print Unregistered Result # admin is email prefix
-check_one_gmail(f"admin001") ``` 2. If you want to scan a lots of Gmail, you
-can use the following codes. ```python from gmail_scanner.gmail_scanner import
-scan_int_single, scan_int_multi # single process mode(slow) to scan 6-digit
+Update ### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 -
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
-https://github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example
-.env touch results.csv # edit the .env file docker-compose up -d ``` ## Author
-**GmailScanner** Â© [coo](https://github.com/Annihilater), Released under the
-[MIT](./LICENSE) License.
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp .env.example .env touch results.csv # edit the .env file
+docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
+github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.3/setup.py` & `gmail_scanner-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="gmail_scanner",
-    version="1.0.3",
+    version="1.0.4",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="coo",
     author_email="me@coo.lol",
     maintainer="coo",
     maintainer_email="me@coo.lol",
```

