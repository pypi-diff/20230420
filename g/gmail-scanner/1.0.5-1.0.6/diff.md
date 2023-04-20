# Comparing `tmp/gmail_scanner-1.0.5.tar.gz` & `tmp/gmail_scanner-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_scanner-1.0.5.tar", last modified: Thu Apr 20 03:45:20 2023, max compression
+gzip compressed data, was "gmail_scanner-1.0.6.tar", last modified: Thu Apr 20 09:47:27 2023, max compression
```

## Comparing `gmail_scanner-1.0.5.tar` & `gmail_scanner-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:45:20.532666 gmail_scanner-1.0.5/
--rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.5/LICENSE
--rw-r--r--   0 ziji       (501) staff       (20)     3193 2023-04-20 03:45:20.532372 gmail_scanner-1.0.5/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)     2117 2023-04-20 03:45:08.000000 gmail_scanner-1.0.5/README.md
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:45:20.530368 gmail_scanner-1.0.5/gmail_scanner/
--rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.5/gmail_scanner/__init__.py
--rw-r--r--   0 ziji       (501) staff       (20)     6928 2023-04-20 03:44:43.000000 gmail_scanner-1.0.5/gmail_scanner/gmail_scanner.py
-drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 03:45:20.532118 gmail_scanner-1.0.5/gmail_scanner.egg-info/
--rw-r--r--   0 ziji       (501) staff       (20)     3193 2023-04-20 03:45:20.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/PKG-INFO
--rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 03:45:20.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 03:45:20.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/not-zip-safe
--rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 03:45:20.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/requires.txt
--rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 03:45:20.000000 gmail_scanner-1.0.5/gmail_scanner.egg-info/top_level.txt
--rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 03:45:20.532726 gmail_scanner-1.0.5/setup.cfg
--rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 03:44:49.000000 gmail_scanner-1.0.5/setup.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 09:47:27.295251 gmail_scanner-1.0.6/
+-rw-r--r--   0 ziji       (501) staff       (20)     1070 2023-04-18 15:24:45.000000 gmail_scanner-1.0.6/LICENSE
+-rw-r--r--   0 ziji       (501) staff       (20)     3249 2023-04-20 09:47:27.294934 gmail_scanner-1.0.6/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)     2173 2023-04-20 09:46:10.000000 gmail_scanner-1.0.6/README.md
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 09:47:27.293358 gmail_scanner-1.0.6/gmail_scanner/
+-rw-r--r--   0 ziji       (501) staff       (20)      136 2023-04-19 10:03:30.000000 gmail_scanner-1.0.6/gmail_scanner/__init__.py
+-rw-r--r--   0 ziji       (501) staff       (20)    11785 2023-04-20 09:39:29.000000 gmail_scanner-1.0.6/gmail_scanner/gmail_scanner.py
+drwxr-xr-x   0 ziji       (501) staff       (20)        0 2023-04-20 09:47:27.294705 gmail_scanner-1.0.6/gmail_scanner.egg-info/
+-rw-r--r--   0 ziji       (501) staff       (20)     3249 2023-04-20 09:47:27.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 ziji       (501) staff       (20)      303 2023-04-20 09:47:27.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-20 09:47:27.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 ziji       (501) staff       (20)        1 2023-04-19 10:49:52.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/not-zip-safe
+-rw-r--r--   0 ziji       (501) staff       (20)       51 2023-04-20 09:47:27.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/requires.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       14 2023-04-20 09:47:27.000000 gmail_scanner-1.0.6/gmail_scanner.egg-info/top_level.txt
+-rw-r--r--   0 ziji       (501) staff       (20)       38 2023-04-20 09:47:27.295316 gmail_scanner-1.0.6/setup.cfg
+-rw-r--r--   0 ziji       (501) staff       (20)     1597 2023-04-20 09:43:14.000000 gmail_scanner-1.0.6/setup.py
```

### Comparing `gmail_scanner-1.0.5/LICENSE` & `gmail_scanner-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_scanner-1.0.5/PKG-INFO` & `gmail_scanner-1.0.6/gmail_scanner.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gmail_scanner
-Version: 1.0.5
+Name: gmail-scanner
+Version: 1.0.6
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -46,15 +46,19 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
-### 1.0.4
+### 1.0.6
+
+- Feat: support for special num
+
+### 1.0.5
 
 - Fixed: logs dir
 
 ### 1.0.4
 
 - Feat: add logs dir
 
@@ -123,15 +127,15 @@
 <a href="https://pypi.org/project/GmailScanner/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Docker
 
 ```bash
 git clone https://github.com/Annihilater/gmail_scanner
 cd gmail_scanner
-cp .env.example .env
+cp config-example.yml config.yml
 touch results.csv
 
 # edit the .env file
 
 docker-compose up -d
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.5 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.6 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,28 +12,28 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.4 - Fixed: logs dir ### 1.0.4 - Feat: add logs dir ### 1.0.3 -
-Feat: log to file ### 1.0.2 - Fixed: print None - Feat: print batch num and
-email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record results to a csv file.
-## Usage **You need to install `gmail_scanner` before.** ```bash pip install
-gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file with the following
-codes. ```python from gmail_scanner.gmail_scanner import check_one_gmail # Only
-Print Unregistered Result # admin is email prefix check_one_gmail(f"admin001")
-``` 2. If you want to scan a lots of Gmail, you can use the following codes.
-```python from gmail_scanner.gmail_scanner import scan_int_single,
-scan_int_multi # single process mode(slow) to scan 6-digit gmail mailboxes
-start_num = 0 end_num = 999999 email_length = 6 output_file = f'results.csv'
-scan_int_single(start_num, end_num, email_length, output_file) # multi process
-mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num = 999999
-email_length = 6 output_file = f'results.csv' batch_num = 1000 process_num = 20
-scan_int_multi(start_num, end_num, email_length, output_file, batch_num,
-process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-
-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone https://
-github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example .env
-touch results.csv # edit the .env file docker-compose up -d ``` ## Author
-**GmailScanner** Â© [coo](https://github.com/Annihilater), Released under the
-[MIT](./LICENSE) License.
+Update ### 1.0.6 - Feat: support for special num ### 1.0.5 - Fixed: logs dir
+### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed:
+print None - Feat: print batch num and email num ### 1.0.1 - Fixed some bug ###
+1.0.0 - Record results to a csv file. ## Usage **You need to install
+`gmail_scanner` before.** ```bash pip install gmail_scanner ``` ### Lite Mode
+1. Create a new `.py` file with the following codes. ```python from
+gmail_scanner.gmail_scanner import check_one_gmail # Only Print Unregistered
+Result # admin is email prefix check_one_gmail(f"admin001") ``` 2. If you want
+to scan a lots of Gmail, you can use the following codes. ```python from
+gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi # single
+process mode(slow) to scan 6-digit gmail mailboxes start_num = 0 end_num =
+999999 email_length = 6 output_file = f'results.csv' scan_int_single(start_num,
+end_num, email_length, output_file) # multi process mode(fast) to scan 6-digit
+gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp config-example.yml config.yml touch results.csv # edit the
+.env file docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
+github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.5/README.md` & `gmail_scanner-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
-### 1.0.4
+### 1.0.6
+
+- Feat: support for special num
+
+### 1.0.5
 
 - Fixed: logs dir
 
 ### 1.0.4
 
 - Feat: add logs dir
 
@@ -94,15 +98,15 @@
 <a href="https://pypi.org/project/GmailScanner/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Docker
 
 ```bash
 git clone https://github.com/Annihilater/gmail_scanner
 cd gmail_scanner
-cp .env.example .env
+cp config-example.yml config.yml
 touch results.csv
 
 # edit the .env file
 
 docker-compose up -d
 ```
```

### Comparing `gmail_scanner-1.0.5/gmail_scanner/gmail_scanner.py` & `gmail_scanner-1.0.6/gmail_scanner/gmail_scanner.py`

 * *Files 27% similar despite different names*

```diff
@@ -140,7 +140,101 @@
         for j in range(i, i + batch):
             email_prefix = str(j).zfill(email_length)
             args.append([email_prefix, output_file])
 
         with Pool(processes=processes) as pool:
             list((tqdm(pool.imap(task, args), total=len(args), desc='process')))
         current_batch += 1
+
+
+def scan_int_multi_specific(email_format: dict, output_file: str, batch: int = 1000,
+                            processes: int = 4) -> None:
+    """
+    scan digital gmail for multi process, fast
+    Because the number of gmail is too large, it is processed in batches,
+    and each batch uses a multi-process method to check whether it is registered
+    :param email_format:
+    :param output_file:
+    :param batch: default 1000, When processing in batches, the number of batches
+    :param processes: default 4
+    :return:
+    # email_format = {
+    #     1: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     2: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     3: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     4: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     5: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     6: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    #     7: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+    # }
+    """
+    log_file_name = f"logs/gmail_scanner_{current_time()}.log"
+
+    format_length = len(email_format)
+
+    email_prefix_list = []
+    for i in email_format[1]:
+        for j in email_format[2]:
+            for k in email_format[3]:
+                for m in email_format[4]:
+                    for n in email_format[5]:
+                        for o in email_format[6]:
+                            email_prefix = str(i).zfill(1) + \
+                                           str(j).zfill(1) + \
+                                           str(k).zfill(1) + \
+                                           str(m).zfill(1) + \
+                                           str(n).zfill(1) + \
+                                           str(o).zfill(1)
+
+                            if format_length >= 7:
+                                for p in email_format[7]:
+                                    email_prefix = str(i).zfill(1) + \
+                                                   str(j).zfill(1) + \
+                                                   str(k).zfill(1) + \
+                                                   str(m).zfill(1) + \
+                                                   str(n).zfill(1) + \
+                                                   str(o).zfill(1) + \
+                                                   str(p).zfill(1)
+
+                                    if format_length >= 8:
+                                        for q in email_format[8]:
+                                            email_prefix = str(i).zfill(1) + \
+                                                           str(j).zfill(1) + \
+                                                           str(k).zfill(1) + \
+                                                           str(m).zfill(1) + \
+                                                           str(n).zfill(1) + \
+                                                           str(o).zfill(1) + \
+                                                           str(p).zfill(1) + \
+                                                           str(q).zfill(1)
+
+                                            if format_length >= 9:
+                                                for r in email_format[9]:
+                                                    email_prefix = str(i).zfill(1) + \
+                                                                   str(j).zfill(1) + \
+                                                                   str(k).zfill(1) + \
+                                                                   str(m).zfill(1) + \
+                                                                   str(n).zfill(1) + \
+                                                                   str(o).zfill(1) + \
+                                                                   str(p).zfill(1) + \
+                                                                   str(q).zfill(1) + \
+                                                                   str(r).zfill(1)
+                                            else:
+                                                email_prefix_list.append(email_prefix)
+                                    else:
+                                        email_prefix_list.append(email_prefix)
+                            else:
+                                email_prefix_list.append(email_prefix)
+
+    current_batch = 1
+    for i in range(1, len(email_prefix_list), batch):
+        with open(log_file_name, mode='a', encoding='utf8') as f:
+            text = f"current_batch: {current_batch} current_num: {i} total: {len(email_prefix_list)}\n"
+            f.write(text)
+
+        args = []
+        for j in range(i, i + batch):
+            email_prefix = email_prefix_list[j]
+            args.append([email_prefix, output_file])
+
+        with Pool(processes=processes) as pool:
+            list((tqdm(pool.imap(task, args), total=len(args), desc='process')))
+        current_batch += 1
```

### Comparing `gmail_scanner-1.0.5/gmail_scanner.egg-info/PKG-INFO` & `gmail_scanner-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gmail-scanner
-Version: 1.0.5
+Name: gmail_scanner
+Version: 1.0.6
 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner
 Author: coo
 Author-email: me@coo.lol
 Maintainer: coo
 Maintainer-email: me@coo.lol
 License: MIT
@@ -46,15 +46,19 @@
 
 The program will return only one results:
 
 - `Unregistered`: It means that the Gmail is not registered or is **blocked**.
 
 ## Update
 
-### 1.0.4
+### 1.0.6
+
+- Feat: support for special num
+
+### 1.0.5
 
 - Fixed: logs dir
 
 ### 1.0.4
 
 - Feat: add logs dir
 
@@ -123,15 +127,15 @@
 <a href="https://pypi.org/project/GmailScanner/"><img src="https://img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red" /></a>
 
 ## Docker
 
 ```bash
 git clone https://github.com/Annihilater/gmail_scanner
 cd gmail_scanner
-cp .env.example .env
+cp config-example.yml config.yml
 touch results.csv
 
 # edit the .env file
 
 docker-compose up -d
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gmail-scanner Version: 1.0.5 Summary: gmail scanner
+Metadata-Version: 2.1 Name: gmail_scanner Version: 1.0.6 Summary: gmail scanner
 Home-page: https://github.com/Annihilater/gmail_scanner Author: coo Author-
 email: me@coo.lol Maintainer: coo Maintainer-email: me@coo.lol License: MIT
 Platform: all Classifier: Environment :: Web Environment Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.3 Classifier:
 Programming Language :: Python :: 3.4 Classifier: Programming Language ::
@@ -12,28 +12,28 @@
 Programming Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/
 HTTP :: Dynamic Content Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
 # Gmail Scanner Gmail Scanner is a Gmail mailbox scanner. ## Description Gmail
 Scanner has a multi-process mode that is very fast, and how fast it is depends
 on the performance of your machine. The program will return only one results: -
 `Unregistered`: It means that the Gmail is not registered or is **blocked**. ##
-Update ### 1.0.4 - Fixed: logs dir ### 1.0.4 - Feat: add logs dir ### 1.0.3 -
-Feat: log to file ### 1.0.2 - Fixed: print None - Feat: print batch num and
-email num ### 1.0.1 - Fixed some bug ### 1.0.0 - Record results to a csv file.
-## Usage **You need to install `gmail_scanner` before.** ```bash pip install
-gmail_scanner ``` ### Lite Mode 1. Create a new `.py` file with the following
-codes. ```python from gmail_scanner.gmail_scanner import check_one_gmail # Only
-Print Unregistered Result # admin is email prefix check_one_gmail(f"admin001")
-``` 2. If you want to scan a lots of Gmail, you can use the following codes.
-```python from gmail_scanner.gmail_scanner import scan_int_single,
-scan_int_multi # single process mode(slow) to scan 6-digit gmail mailboxes
-start_num = 0 end_num = 999999 email_length = 6 output_file = f'results.csv'
-scan_int_single(start_num, end_num, email_length, output_file) # multi process
-mode(fast) to scan 6-digit gmail mailboxes start_num = 0 end_num = 999999
-email_length = 6 output_file = f'results.csv' batch_num = 1000 process_num = 20
-scan_int_multi(start_num, end_num, email_length, output_file, batch_num,
-process_num) ``` ## PyPi [https://img.shields.io/badge/Pypi-000000?style=for-
-the-badge&logo=pypi&logoColor=red] ## Docker ```bash git clone https://
-github.com/Annihilater/gmail_scanner cd gmail_scanner cp .env.example .env
-touch results.csv # edit the .env file docker-compose up -d ``` ## Author
-**GmailScanner** Â© [coo](https://github.com/Annihilater), Released under the
-[MIT](./LICENSE) License.
+Update ### 1.0.6 - Feat: support for special num ### 1.0.5 - Fixed: logs dir
+### 1.0.4 - Feat: add logs dir ### 1.0.3 - Feat: log to file ### 1.0.2 - Fixed:
+print None - Feat: print batch num and email num ### 1.0.1 - Fixed some bug ###
+1.0.0 - Record results to a csv file. ## Usage **You need to install
+`gmail_scanner` before.** ```bash pip install gmail_scanner ``` ### Lite Mode
+1. Create a new `.py` file with the following codes. ```python from
+gmail_scanner.gmail_scanner import check_one_gmail # Only Print Unregistered
+Result # admin is email prefix check_one_gmail(f"admin001") ``` 2. If you want
+to scan a lots of Gmail, you can use the following codes. ```python from
+gmail_scanner.gmail_scanner import scan_int_single, scan_int_multi # single
+process mode(slow) to scan 6-digit gmail mailboxes start_num = 0 end_num =
+999999 email_length = 6 output_file = f'results.csv' scan_int_single(start_num,
+end_num, email_length, output_file) # multi process mode(fast) to scan 6-digit
+gmail mailboxes start_num = 0 end_num = 999999 email_length = 6 output_file =
+f'results.csv' batch_num = 1000 process_num = 20 scan_int_multi(start_num,
+end_num, email_length, output_file, batch_num, process_num) ``` ## PyPi [https:
+//img.shields.io/badge/Pypi-000000?style=for-the-badge&logo=pypi&logoColor=red]
+## Docker ```bash git clone https://github.com/Annihilater/gmail_scanner cd
+gmail_scanner cp config-example.yml config.yml touch results.csv # edit the
+.env file docker-compose up -d ``` ## Author **GmailScanner** Â© [coo](https://
+github.com/Annihilater), Released under the [MIT](./LICENSE) License.
```

### Comparing `gmail_scanner-1.0.5/setup.py` & `gmail_scanner-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="gmail_scanner",
-    version="1.0.5",
+    version="1.0.6",
     license='MIT',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="coo",
     author_email="me@coo.lol",
     maintainer="coo",
     maintainer_email="me@coo.lol",
```

