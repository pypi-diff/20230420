# Comparing `tmp/testit-importer-allure-1.3.0.tar.gz` & `tmp/testit-importer-allure-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-importer-allure-1.3.0.tar", last modified: Thu Mar 30 10:01:22 2023, max compression
+gzip compressed data, was "testit-importer-allure-1.3.1.tar", last modified: Thu Apr 20 13:56:17 2023, max compression
```

## Comparing `testit-importer-allure-1.3.0.tar` & `testit-importer-allure-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 10:01:22.333086 testit-importer-allure-1.3.0/
--rw-rw-rw-   0        0        0     3155 2022-10-20 13:32:36.000000 testit-importer-allure-1.3.0/.gitignore
--rw-rw-rw-   0        0        0       29 2022-10-20 13:32:36.000000 testit-importer-allure-1.3.0/.pylintrc
-drwxrwxrwx   0        0        0        0 2023-03-30 10:01:22.309219 testit-importer-allure-1.3.0/.run/
--rw-rw-rw-   0        0        0     1092 2022-10-20 13:32:36.000000 testit-importer-allure-1.3.0/.run/Debug.run.xml
--rw-rw-rw-   0        0        0      199 2023-03-30 06:26:50.000000 testit-importer-allure-1.3.0/Dockerfile
--rw-rw-rw-   0        0        0     3585 2023-03-30 10:01:22.333086 testit-importer-allure-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2023-03-30 06:26:50.000000 testit-importer-allure-1.3.0/README.md
--rw-rw-rw-   0        0        0      245 2022-11-18 10:32:16.000000 testit-importer-allure-1.3.0/connection_config.ini
--rw-rw-rw-   0        0        0       55 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/debug.py
--rw-rw-rw-   0        0        0      115 2023-03-30 06:26:50.000000 testit-importer-allure-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 10:01:22.333086 testit-importer-allure-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1247 2023-03-30 10:00:27.000000 testit-importer-allure-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:01:22.333086 testit-importer-allure-1.3.0/src/
--rw-rw-rw-   0        0        0        0 2022-11-23 10:45:31.000000 testit-importer-allure-1.3.0/src/__init__.py
--rw-rw-rw-   0        0        0     1310 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/__main__.py
--rw-rw-rw-   0        0        0     3758 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/apiclient.py
--rw-rw-rw-   0        0        0    12055 2023-03-30 06:26:50.000000 testit-importer-allure-1.3.0/src/configurator.py
--rw-rw-rw-   0        0        0     7388 2023-03-30 10:00:27.000000 testit-importer-allure-1.3.0/src/converter.py
--rw-rw-rw-   0        0        0      265 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/filedto.py
--rw-rw-rw-   0        0        0     1479 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/filereader.py
--rw-rw-rw-   0        0        0    11678 2023-03-30 10:00:27.000000 testit-importer-allure-1.3.0/src/importer.py
--rw-rw-rw-   0        0        0     1664 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/minioreader.py
--rw-rw-rw-   0        0        0     2662 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/parser.py
--rw-rw-rw-   0        0        0      909 2023-03-30 06:26:44.000000 testit-importer-allure-1.3.0/src/rabbitmq.py
--rw-rw-rw-   0        0        0      297 2022-10-20 13:32:36.000000 testit-importer-allure-1.3.0/src/reader.py
-drwxrwxrwx   0        0        0        0 2023-03-30 10:01:22.333086 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/
--rw-rw-rw-   0        0        0     3585 2023-03-30 10:01:21.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-03-30 10:01:22.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 10:01:21.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-03-30 10:01:21.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-03-30 10:01:21.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-03-30 10:01:21.000000 testit-importer-allure-1.3.0/testit_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 dmitry.gridnev (1970307760) 1761955536        0 2023-04-20 13:56:17.385494 testit-importer-allure-1.3.1/
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     2899 2023-04-20 13:56:17.385352 testit-importer-allure-1.3.1/PKG-INFO
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     2352 2022-12-30 08:07:25.000000 testit-importer-allure-1.3.1/README.md
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      229 2023-04-20 13:56:04.000000 testit-importer-allure-1.3.1/connection_config.ini
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536       38 2023-04-20 13:56:17.385535 testit-importer-allure-1.3.1/setup.cfg
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     1211 2023-04-20 13:46:27.000000 testit-importer-allure-1.3.1/setup.py
+drwxr-xr-x   0 dmitry.gridnev (1970307760) 1761955536        0 2023-04-20 13:56:17.384058 testit-importer-allure-1.3.1/src/
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536        0 2022-09-01 11:13:09.000000 testit-importer-allure-1.3.1/src/__init__.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     1268 2022-10-21 08:57:33.000000 testit-importer-allure-1.3.1/src/__main__.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     3669 2022-11-18 14:19:51.000000 testit-importer-allure-1.3.1/src/apiclient.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536    11732 2022-11-25 10:23:46.000000 testit-importer-allure-1.3.1/src/configurator.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     7174 2023-04-20 13:46:09.000000 testit-importer-allure-1.3.1/src/converter.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      253 2023-01-20 11:47:56.000000 testit-importer-allure-1.3.1/src/filedto.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     1557 2023-04-20 13:46:19.000000 testit-importer-allure-1.3.1/src/filereader.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536    11405 2023-04-20 13:46:09.000000 testit-importer-allure-1.3.1/src/importer.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     1615 2023-01-20 11:47:56.000000 testit-importer-allure-1.3.1/src/minioreader.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     2588 2023-01-20 11:47:56.000000 testit-importer-allure-1.3.1/src/parser.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      885 2022-10-21 08:57:33.000000 testit-importer-allure-1.3.1/src/rabbitmq.py
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      281 2022-10-21 08:57:33.000000 testit-importer-allure-1.3.1/src/reader.py
+drwxr-xr-x   0 dmitry.gridnev (1970307760) 1761955536        0 2023-04-20 13:56:17.385152 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536     2899 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      523 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536        1 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536      136 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536       63 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 dmitry.gridnev (1970307760) 1761955536       23 2023-04-20 13:56:17.000000 testit-importer-allure-1.3.1/testit_importer_allure.egg-info/top_level.txt
```

### Comparing `testit-importer-allure-1.3.0/PKG-INFO` & `testit-importer-allure-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,86 @@
-Metadata-Version: 2.1
-Name: testit-importer-allure
-Version: 1.3.0
-Summary: Allure report importer for Test IT
-Home-page: https://pypi.org/project/testit-importer-allure/
-Author: Integration team
-Author-email: integrations@testit.software
-License: Apache-2.0
-Description: # Test IT TMS importers
-        ![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
-        
-        # Allure report
-        
-        ## Getting Started
-        
-        ### Installation
-        ```
-        pip install testit-importer-allure
-        ```
-        
-        ## Usage
-        
-        ### API client
-        
-        To use importer you need to install `testit-api-client`:
-        ```
-        pip install testit-api-client
-        ```
-        
-        ### Configuration
-        
-        Use the command `testit --help` to view the configuration setup help:
-        ```
-        testit --url <url>
-        testit --privatetoken <token>
-        testit --projectid <id>
-        testit --configurationid <id>
-        ```
-        
-        And fill parameters with your configuration, where:  
-        `url` - location of the TMS instance  
-        `privatetoken` - API secret key  
-        
-        1. go to the https://{DOMAIN}/user-profile profile  
-        2. copy the API secret key
-        
-        `projectid` - id of project in TMS instance
-        
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request project, Preview tab, copy id field  
-        
-        `configurationid` - id of configuration in TMS instance  
-        
-        1. create a project  
-        2. open DevTools -> network  
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
-        4. GET-request configurations, Preview tab, copy id field 
-        
-        ### Importing
-        
-        Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-        Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-        **Important:** This command initiates the import.
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: testit-importer-allure
+Version: 1.3.1
+Summary: Allure report importer for Test IT
+Home-page: https://pypi.org/project/testit-importer-allure/
+Author: Integration team
+Author-email: integrations@testit.software
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# Test IT TMS importers
+![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
+
+# Allure report
+
+## Getting Started
+
+### Installation
+```
+pip install testit-importer-allure
+```
+
+## Usage
+
+### API client
+
+To use importer you need to install `testit-api-client`:
+```
+pip install testit-api-client
+```
+
+### Configuration
+
+Use the command `testit --help` to view the configuration setup help:
+```
+testit --url <url>
+testit --privatetoken <token>
+testit --projectid <id>
+testit --configurationid <id>
+```
+
+And fill parameters with your configuration, where:  
+`url` - location of the TMS instance  
+`privatetoken` - API secret key  
+
+1. go to the https://{DOMAIN}/user-profile profile  
+2. copy the API secret key
+
+`projectid` - id of project in TMS instance
+
+1. create a project
+2. open DevTools -> network
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+4. GET-request project, Preview tab, copy id field  
+
+`configurationid` - id of configuration in TMS instance  
+
+1. create a project  
+2. open DevTools -> network  
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
+4. GET-request configurations, Preview tab, copy id field 
+
+### Importing
+
+Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
+Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+**Important:** This command initiates the import.
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testit-importer-allure-1.3.0/README.md` & `testit-importer-allure-1.3.1/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# Test IT TMS importers
-![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
-
-# Allure report
-
-## Getting Started
-
-### Installation
-```
-pip install testit-importer-allure
-```
-
-## Usage
-
-### API client
-
-To use importer you need to install `testit-api-client`:
-```
-pip install testit-api-client
-```
-
-### Configuration
-
-Use the command `testit --help` to view the configuration setup help:
-```
-testit --url <url>
-testit --privatetoken <token>
-testit --projectid <id>
-testit --configurationid <id>
-```
-
-And fill parameters with your configuration, where:  
-`url` - location of the TMS instance  
-`privatetoken` - API secret key  
-
-1. go to the https://{DOMAIN}/user-profile profile  
-2. copy the API secret key
-
-`projectid` - id of project in TMS instance
-
-1. create a project
-2. open DevTools -> network
-3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-4. GET-request project, Preview tab, copy id field  
-
-`configurationid` - id of configuration in TMS instance  
-
-1. create a project  
-2. open DevTools -> network  
-3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
-4. GET-request configurations, Preview tab, copy id field 
-
-### Importing
-
-Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-**Important:** This command initiates the import.
-
-# Contributing
-
-You can help to develop the project. Any contributions are **greatly appreciated**.
-
-* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-* Please make sure you check your spelling and grammar.
-* Create individual PR for each suggestion.
-* Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-
-# License
-
-Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
-
+# Test IT TMS importers
+![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
+
+# Allure report
+
+## Getting Started
+
+### Installation
+```
+pip install testit-importer-allure
+```
+
+## Usage
+
+### API client
+
+To use importer you need to install `testit-api-client`:
+```
+pip install testit-api-client
+```
+
+### Configuration
+
+Use the command `testit --help` to view the configuration setup help:
+```
+testit --url <url>
+testit --privatetoken <token>
+testit --projectid <id>
+testit --configurationid <id>
+```
+
+And fill parameters with your configuration, where:  
+`url` - location of the TMS instance  
+`privatetoken` - API secret key  
+
+1. go to the https://{DOMAIN}/user-profile profile  
+2. copy the API secret key
+
+`projectid` - id of project in TMS instance
+
+1. create a project
+2. open DevTools -> network
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+4. GET-request project, Preview tab, copy id field  
+
+`configurationid` - id of configuration in TMS instance  
+
+1. create a project  
+2. open DevTools -> network  
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
+4. GET-request configurations, Preview tab, copy id field 
+
+### Importing
+
+Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
+Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+**Important:** This command initiates the import.
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testit-importer-allure-1.3.0/setup.py` & `testit-importer-allure-1.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from setuptools import setup
-
-setup(
-    name='testit-importer-allure',
-    version='1.3.0',
-    description='Allure report importer for Test IT',
-    long_description=open('README.md', "r").read(),
-    long_description_content_type="text/markdown",
-    url='https://pypi.org/project/testit-importer-allure/',
-    author='Integration team',
-    author_email='integrations@testit.software',
-    license='Apache-2.0',
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    packages=['testit_importer_allure'],
-    package_data={'testit_importer_allure': ['../connection_config.ini']},
-    package_dir={'testit_importer_allure': 'src'},
-    install_requires=[
-        'testit-api-client==3.0.1',
-        'xmltodict',
-        'python-interface',
-        'minio',
-        'pika'
-    ],
-    entry_points={
-        'console_scripts': [
-            'testit = testit_importer_allure.__main__:console_main',
-            'testit-consumer = testit_importer_allure.__main__:consumer_main'
-        ]
-    }
-)
+from setuptools import setup
+
+setup(
+    name='testit-importer-allure',
+    version='1.3.1',
+    description='Allure report importer for Test IT',
+    long_description=open('README.md', "r").read(),
+    long_description_content_type="text/markdown",
+    url='https://pypi.org/project/testit-importer-allure/',
+    author='Integration team',
+    author_email='integrations@testit.software',
+    license='Apache-2.0',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+    ],
+    packages=['testit_importer_allure'],
+    package_data={'testit_importer_allure': ['../connection_config.ini']},
+    package_dir={'testit_importer_allure': 'src'},
+    install_requires=[
+        'testit-api-client==3.0.1',
+        'xmltodict',
+        'python-interface',
+        'minio',
+        'pika'
+    ],
+    entry_points={
+        'console_scripts': [
+            'testit = testit_importer_allure.__main__:console_main',
+            'testit-consumer = testit_importer_allure.__main__:consumer_main'
+        ]
+    }
+)
```

### Comparing `testit-importer-allure-1.3.0/src/configurator.py` & `testit-importer-allure-1.3.1/src/configurator.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-"""The module provides functionality for working with the config"""
-import argparse
-import configparser
-import os
-import re
-
-CONFIG_SECTION = 'testit'
-CONFIG_URL = 'url'
-CONFIG_PRIVATE_TOKEN = 'privateToken'
-CONFIG_PROJECT_ID = 'projectID'
-CONFIG_CONFIGURATION_ID = 'configurationID'
-CONFIG_NAME = 'connection_config.ini'
-
-RABBITMQ_CONFIG_SECTION = 'rabbitmq'
-RABBITMQ_CONFIG_URL = 'host'
-RABBITMQ_CONFIG_USER = 'user'
-RABBITMQ_CONFIG_PASSWORD = 'password'
-RABBITMQ_CONFIG_EXCHANGE = 'exchange'
-
-MINIO_CONFIG_SECTION = 'minio'
-MINIO_CONFIG_URL = 'host'
-MINIO_CONFIG_ACCESS_KEY = 'accessKey'
-MINIO_CONFIG_SECRET_KEY = 'secretKey'
-
-
-class Configurator:
-    """Class representing a configurator"""
-
-    path_to_results = None
-    path_to_config = None
-    specified_testrun = None
-
-    def __init__(self):
-        self.__set_config()
-        self.__set_parser()
-        self.__parse_args()
-        self.__load_env_properties()
-
-    def get_path(self):
-        """Function returns path of result files."""
-        return self.path_to_results
-
-    def get_url(self):
-        """Function returns TMS url."""
-        return self.config.get(CONFIG_SECTION, CONFIG_URL)
-
-    def get_private_token(self):
-        """Function returns private token."""
-        return self.config.get(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN)
-
-    def get_project_id(self):
-        """Function returns project id."""
-        return self.config.get(CONFIG_SECTION, CONFIG_PROJECT_ID)
-
-    def get_configuration_id(self):
-        """Function returns configuration id."""
-        return self.config.get(CONFIG_SECTION, CONFIG_CONFIGURATION_ID)
-
-    def get_rabbitmq_url(self):
-        """Function returns rabbit mq url."""
-        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL)
-
-    def get_rabbitmq_user(self):
-        """Function returns rabbit mq user."""
-        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER)
-
-    def get_rabbitmq_password(self):
-        """Function returns rabbit mq user's password."""
-        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD)
-
-    def get_rabbitmq_exchange(self):
-        """Function returns rabbit mq exchange."""
-        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE)
-
-    def get_minio_url(self):
-        """Function returns minio url."""
-        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL)
-
-    def get_minio_access_key(self):
-        """Function returns minio access key."""
-        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY)
-
-    def get_minio_secret_key(self):
-        """Function returns minio secret key."""
-        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY)
-
-    def __set_config(self):
-        self.config = configparser.RawConfigParser()
-        self.path_to_config = os.path.join(os.path.dirname(__file__)[:os.path.dirname(__file__).rindex(os.sep)],
-                                           CONFIG_NAME)
-
-        self.config.read(self.path_to_config)
-
-    def __set_parser(self):
-        self.parser = argparse.ArgumentParser(description='Test IT importer', add_help=True)
-        self.parser.add_argument(
-            '-u',
-            '--url',
-            action="store",
-            default=None,
-            dest="set_url",
-            metavar="https://demo.testit.software",
-            help='Set location of the Test IT instance'
-        )
-        self.parser.add_argument(
-            '-pt',
-            '--privatetoken',
-            action="store",
-            dest="set_privatetoken",
-            metavar="T2lKd2pLZGI4WHRhaVZUejNl",
-            help='Set API secret key'
-        )
-        self.parser.add_argument(
-            '-pi',
-            '--projectid',
-            action="store",
-            dest="set_project",
-            metavar="5236eb3f-7c05-46f9-a609-dc0278896464",
-            help='Set project ID'
-        )
-        self.parser.add_argument(
-            '-ci',
-            '--configurationid',
-            action="store",
-            dest="set_configuration",
-            metavar="15dbb164-c1aa-4cbf-830c-8c01ae14f4fb",
-            help='Set configuration ID'
-        )
-        self.parser.add_argument(
-            '-ti',
-            '--testrunid',
-            action="store",
-            dest="set_testrun",
-            metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
-            help='Set test run ID'
-        )
-        self.parser.add_argument(
-            '-sh',
-            '--show',
-            action='store_true',
-            dest="show_settings",
-            help='Show the connection_config.ini file'
-        )
-        self.parser.add_argument(
-            '-rd',
-            '--resultsdir',
-            action="store",
-            dest="alluredir",
-            metavar="DIR",
-            default=None,
-            help='Import the Allure report in the specified directory if it exists'
-        )
-        self.parser.add_argument(
-            '-rh',
-            '--rabbitmqhost',
-            action="store",
-            dest="set_rabbitmqhost",
-            metavar="localhost:5672",
-            default=None,
-            help='Host of Rabbit MQ'
-        )
-        self.parser.add_argument(
-            '-ru',
-            '--rabbitmquser',
-            action="store",
-            dest="set_rabbitmquser",
-            metavar="user",
-            default=None,
-            help='User of Rabbit MQ'
-        )
-        self.parser.add_argument(
-            '-rp',
-            '--rabbitmqpassword',
-            action="store",
-            dest="set_rabbitmqpassword",
-            metavar="password",
-            default=None,
-            help='Password of Rabbit MQ'
-        )
-        self.parser.add_argument(
-            '-re',
-            '--rabbitmqexchange',
-            action="store",
-            dest="set_rabbitmqexchange",
-            metavar="exchange",
-            default=None,
-            help='Exchange of Rabbit MQ'
-        )
-        self.parser.add_argument(
-            '-mh',
-            '--miniohost',
-            action="store",
-            dest="set_miniohost",
-            metavar="localhost:9000",
-            default=None,
-            help='Host of Minio'
-        )
-        self.parser.add_argument(
-            '-mak',
-            '--minioaccesskey',
-            action="store",
-            dest="set_minioaccesskey",
-            metavar="accesskey",
-            default=None,
-            help='Access key of Minio'
-        )
-        self.parser.add_argument(
-            '-msk',
-            '--miniosecretkey',
-            action="store",
-            dest="set_miniosecretkey",
-            metavar="secretkey",
-            default=None,
-            help='Secret key of Minio'
-        )
-
-    def __load_env_properties(self):
-        if 'TMS_HOST' in os.environ.keys():
-            self.config.set(CONFIG_SECTION, CONFIG_URL, os.environ.get('TMS_HOST'))
-
-        if 'TMS_PRIVATE_TOKEN' in os.environ.keys():
-            self.config.set(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN, os.environ.get('TMS_PRIVATE_TOKEN'))
-
-        if 'TMS_PROJECT_ID' in os.environ.keys():
-            self.config.set(CONFIG_SECTION, CONFIG_PROJECT_ID, os.environ.get('TMS_PROJECT_ID'))
-
-        if 'TMS_CONFIGURATION_ID' in os.environ.keys():
-            self.config.set(CONFIG_SECTION, CONFIG_CONFIGURATION_ID, os.environ.get('TMS_CONFIGURATION_ID'))
-
-        if 'MINIO_API_HOST' in os.environ.keys():
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL, os.environ.get('MINIO_API_HOST'))
-
-        if 'MINIO_ACCESS_KEY' in os.environ.keys():
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY, os.environ.get('MINIO_ACCESS_KEY'))
-
-        if 'MINIO_SECRET_KEY' in os.environ.keys():
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY, os.environ.get('MINIO_SECRET_KEY'))
-
-        if 'RABBITMQ_HOST' in os.environ.keys():
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, os.environ.get('RABBITMQ_HOST'))
-
-        if 'RABBITMQ_USER' in os.environ.keys():
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER, os.environ.get('RABBITMQ_USER'))
-
-        if 'RABBITMQ_PASSWORD' in os.environ.keys():
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD, os.environ.get('RABBITMQ_PASSWORD'))
-
-        if 'RABBITMQ_EXCHANGE' in os.environ.keys():
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE, os.environ.get('RABBITMQ_EXCHANGE'))
-
-    def __parse_args(self):
-        args = self.parser.parse_args()
-        if args.set_url:
-            if not re.fullmatch(
-                    r"^(ht|f)tp(s?)\:\/\/[0-9a-zA-Z]([-.\w]*[0-9a-zA-Z])*(:(0-9)*)*(\/?)([a-zA-Z0-9\-\.\?\,\'\/\\\+&amp;%\$#_]*)?$",
-                    args.set_url):
-                print('The wrong URL!')
-                raise SystemExit
-
-            self.config.set(CONFIG_SECTION, CONFIG_URL,
-                            args.set_url if args.set_url[-1] != '/' else args.set_url[:-1])
-
-        if args.set_privatetoken:
-            self.config.set(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN, args.set_privatetoken)
-
-        if args.set_project:
-            if not re.fullmatch(r"[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}",
-                                args.set_project):
-                print('The wrong project ID!')
-                raise SystemExit
-
-            self.config.set(CONFIG_SECTION, CONFIG_PROJECT_ID, args.set_project)
-
-        if args.set_configuration:
-            if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
-                                args.set_configuration):
-                print('The wrong configuration ID!')
-                raise SystemExit
-
-            self.config.set(CONFIG_SECTION, CONFIG_CONFIGURATION_ID, args.set_configuration)
-
-        if args.set_testrun:
-            if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
-                                args.set_testrun):
-                print('The wrong testrun ID!')
-                raise SystemExit
-
-            self.specified_testrun = args.set_testrun
-
-        if args.alluredir:
-            self.path_to_results = args.alluredir
-
-        if args.set_rabbitmqhost:
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, args.set_rabbitmqhost)
-
-        if args.set_rabbitmquser:
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER, args.set_rabbitmquser)
-
-        if args.set_rabbitmqpassword:
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD, args.set_rabbitmqpassword)
-
-        if args.set_rabbitmqexchange:
-            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE, args.set_rabbitmqexchange)
-
-        if args.set_miniohost:
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL, args.set_miniohost)
-
-        if args.set_minioaccesskey:
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY, args.set_minioaccesskey)
-
-        if args.set_miniosecretkey:
-            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY, args.set_miniosecretkey)
-
-        if args.show_settings:
-            print(
-                f'url: {self.get_url()}\n'
-                f'privatetoken: {self.get_private_token()}\n'
-                f'projectID: {self.get_project_id()}\n'
-                f'configurationID: {self.get_configuration_id()}')
-
-        if args.set_url or args.set_privatetoken or args.set_project or args.set_configuration:
-            with open(self.path_to_config, "w", encoding='utf-8') as config_file:
-                self.config.write(config_file)
+"""The module provides functionality for working with the config"""
+import argparse
+import configparser
+import os
+import re
+
+CONFIG_SECTION = 'testit'
+CONFIG_URL = 'url'
+CONFIG_PRIVATE_TOKEN = 'privateToken'
+CONFIG_PROJECT_ID = 'projectID'
+CONFIG_CONFIGURATION_ID = 'configurationID'
+CONFIG_NAME = 'connection_config.ini'
+
+RABBITMQ_CONFIG_SECTION = 'rabbitmq'
+RABBITMQ_CONFIG_URL = 'host'
+RABBITMQ_CONFIG_USER = 'user'
+RABBITMQ_CONFIG_PASSWORD = 'password'
+RABBITMQ_CONFIG_EXCHANGE = 'exchange'
+
+MINIO_CONFIG_SECTION = 'minio'
+MINIO_CONFIG_URL = 'host'
+MINIO_CONFIG_ACCESS_KEY = 'accessKey'
+MINIO_CONFIG_SECRET_KEY = 'secretKey'
+
+
+class Configurator:
+    """Class representing a configurator"""
+
+    path_to_results = None
+    path_to_config = None
+    specified_testrun = None
+
+    def __init__(self):
+        self.__set_config()
+        self.__set_parser()
+        self.__parse_args()
+        self.__load_env_properties()
+
+    def get_path(self):
+        """Function returns path of result files."""
+        return self.path_to_results
+
+    def get_url(self):
+        """Function returns TMS url."""
+        return self.config.get(CONFIG_SECTION, CONFIG_URL)
+
+    def get_private_token(self):
+        """Function returns private token."""
+        return self.config.get(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN)
+
+    def get_project_id(self):
+        """Function returns project id."""
+        return self.config.get(CONFIG_SECTION, CONFIG_PROJECT_ID)
+
+    def get_configuration_id(self):
+        """Function returns configuration id."""
+        return self.config.get(CONFIG_SECTION, CONFIG_CONFIGURATION_ID)
+
+    def get_rabbitmq_url(self):
+        """Function returns rabbit mq url."""
+        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL)
+
+    def get_rabbitmq_user(self):
+        """Function returns rabbit mq user."""
+        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER)
+
+    def get_rabbitmq_password(self):
+        """Function returns rabbit mq user's password."""
+        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD)
+
+    def get_rabbitmq_exchange(self):
+        """Function returns rabbit mq exchange."""
+        return self.config.get(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE)
+
+    def get_minio_url(self):
+        """Function returns minio url."""
+        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL)
+
+    def get_minio_access_key(self):
+        """Function returns minio access key."""
+        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY)
+
+    def get_minio_secret_key(self):
+        """Function returns minio secret key."""
+        return self.config.get(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY)
+
+    def __set_config(self):
+        self.config = configparser.RawConfigParser()
+        self.path_to_config = os.path.join(os.path.dirname(__file__)[:os.path.dirname(__file__).rindex(os.sep)],
+                                           CONFIG_NAME)
+
+        self.config.read(self.path_to_config)
+
+    def __set_parser(self):
+        self.parser = argparse.ArgumentParser(description='Test IT importer', add_help=True)
+        self.parser.add_argument(
+            '-u',
+            '--url',
+            action="store",
+            default=None,
+            dest="set_url",
+            metavar="https://demo.testit.software",
+            help='Set location of the Test IT instance'
+        )
+        self.parser.add_argument(
+            '-pt',
+            '--privatetoken',
+            action="store",
+            dest="set_privatetoken",
+            metavar="T2lKd2pLZGI4WHRhaVZUejNl",
+            help='Set API secret key'
+        )
+        self.parser.add_argument(
+            '-pi',
+            '--projectid',
+            action="store",
+            dest="set_project",
+            metavar="5236eb3f-7c05-46f9-a609-dc0278896464",
+            help='Set project ID'
+        )
+        self.parser.add_argument(
+            '-ci',
+            '--configurationid',
+            action="store",
+            dest="set_configuration",
+            metavar="15dbb164-c1aa-4cbf-830c-8c01ae14f4fb",
+            help='Set configuration ID'
+        )
+        self.parser.add_argument(
+            '-ti',
+            '--testrunid',
+            action="store",
+            dest="set_testrun",
+            metavar="3802f329-190c-4617-8bb0-2c3696abeb8f",
+            help='Set test run ID'
+        )
+        self.parser.add_argument(
+            '-sh',
+            '--show',
+            action='store_true',
+            dest="show_settings",
+            help='Show the connection_config.ini file'
+        )
+        self.parser.add_argument(
+            '-rd',
+            '--resultsdir',
+            action="store",
+            dest="alluredir",
+            metavar="DIR",
+            default=None,
+            help='Import the Allure report in the specified directory if it exists'
+        )
+        self.parser.add_argument(
+            '-rh',
+            '--rabbitmqhost',
+            action="store",
+            dest="set_rabbitmqhost",
+            metavar="localhost:5672",
+            default=None,
+            help='Host of Rabbit MQ'
+        )
+        self.parser.add_argument(
+            '-ru',
+            '--rabbitmquser',
+            action="store",
+            dest="set_rabbitmquser",
+            metavar="user",
+            default=None,
+            help='User of Rabbit MQ'
+        )
+        self.parser.add_argument(
+            '-rp',
+            '--rabbitmqpassword',
+            action="store",
+            dest="set_rabbitmqpassword",
+            metavar="password",
+            default=None,
+            help='Password of Rabbit MQ'
+        )
+        self.parser.add_argument(
+            '-re',
+            '--rabbitmqexchange',
+            action="store",
+            dest="set_rabbitmqexchange",
+            metavar="exchange",
+            default=None,
+            help='Exchange of Rabbit MQ'
+        )
+        self.parser.add_argument(
+            '-mh',
+            '--miniohost',
+            action="store",
+            dest="set_miniohost",
+            metavar="localhost:9000",
+            default=None,
+            help='Host of Minio'
+        )
+        self.parser.add_argument(
+            '-mak',
+            '--minioaccesskey',
+            action="store",
+            dest="set_minioaccesskey",
+            metavar="accesskey",
+            default=None,
+            help='Access key of Minio'
+        )
+        self.parser.add_argument(
+            '-msk',
+            '--miniosecretkey',
+            action="store",
+            dest="set_miniosecretkey",
+            metavar="secretkey",
+            default=None,
+            help='Secret key of Minio'
+        )
+
+    def __load_env_properties(self):
+        if 'TMS_HOST' in os.environ.keys():
+            self.config.set(CONFIG_SECTION, CONFIG_URL, os.environ.get('TMS_HOST'))
+
+        if 'TMS_PRIVATE_TOKEN' in os.environ.keys():
+            self.config.set(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN, os.environ.get('TMS_PRIVATE_TOKEN'))
+
+        if 'TMS_PROJECT_ID' in os.environ.keys():
+            self.config.set(CONFIG_SECTION, CONFIG_PROJECT_ID, os.environ.get('TMS_PROJECT_ID'))
+
+        if 'TMS_CONFIGURATION_ID' in os.environ.keys():
+            self.config.set(CONFIG_SECTION, CONFIG_CONFIGURATION_ID, os.environ.get('TMS_CONFIGURATION_ID'))
+
+        if 'MINIO_API_HOST' in os.environ.keys():
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL, os.environ.get('MINIO_API_HOST'))
+
+        if 'MINIO_ACCESS_KEY' in os.environ.keys():
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY, os.environ.get('MINIO_ACCESS_KEY'))
+
+        if 'MINIO_SECRET_KEY' in os.environ.keys():
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY, os.environ.get('MINIO_SECRET_KEY'))
+
+        if 'RABBITMQ_HOST' in os.environ.keys():
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, os.environ.get('RABBITMQ_HOST'))
+
+        if 'RABBITMQ_USER' in os.environ.keys():
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER, os.environ.get('RABBITMQ_USER'))
+
+        if 'RABBITMQ_PASSWORD' in os.environ.keys():
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD, os.environ.get('RABBITMQ_PASSWORD'))
+
+        if 'RABBITMQ_EXCHANGE' in os.environ.keys():
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE, os.environ.get('RABBITMQ_EXCHANGE'))
+
+    def __parse_args(self):
+        args = self.parser.parse_args()
+        if args.set_url:
+            if not re.fullmatch(
+                    r"^(ht|f)tp(s?)\:\/\/[0-9a-zA-Z]([-.\w]*[0-9a-zA-Z])*(:(0-9)*)*(\/?)([a-zA-Z0-9\-\.\?\,\'\/\\\+&amp;%\$#_]*)?$",
+                    args.set_url):
+                print('The wrong URL!')
+                raise SystemExit
+
+            self.config.set(CONFIG_SECTION, CONFIG_URL,
+                            args.set_url if args.set_url[-1] != '/' else args.set_url[:-1])
+
+        if args.set_privatetoken:
+            self.config.set(CONFIG_SECTION, CONFIG_PRIVATE_TOKEN, args.set_privatetoken)
+
+        if args.set_project:
+            if not re.fullmatch(r"[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}",
+                                args.set_project):
+                print('The wrong project ID!')
+                raise SystemExit
+
+            self.config.set(CONFIG_SECTION, CONFIG_PROJECT_ID, args.set_project)
+
+        if args.set_configuration:
+            if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
+                                args.set_configuration):
+                print('The wrong configuration ID!')
+                raise SystemExit
+
+            self.config.set(CONFIG_SECTION, CONFIG_CONFIGURATION_ID, args.set_configuration)
+
+        if args.set_testrun:
+            if not re.fullmatch(r'[a-zA-Z\d]{8}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{4}-[a-zA-Z\d]{12}',
+                                args.set_testrun):
+                print('The wrong testrun ID!')
+                raise SystemExit
+
+            self.specified_testrun = args.set_testrun
+
+        if args.alluredir:
+            self.path_to_results = args.alluredir
+
+        if args.set_rabbitmqhost:
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_URL, args.set_rabbitmqhost)
+
+        if args.set_rabbitmquser:
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_USER, args.set_rabbitmquser)
+
+        if args.set_rabbitmqpassword:
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_PASSWORD, args.set_rabbitmqpassword)
+
+        if args.set_rabbitmqexchange:
+            self.config.set(RABBITMQ_CONFIG_SECTION, RABBITMQ_CONFIG_EXCHANGE, args.set_rabbitmqexchange)
+
+        if args.set_miniohost:
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_URL, args.set_miniohost)
+
+        if args.set_minioaccesskey:
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_ACCESS_KEY, args.set_minioaccesskey)
+
+        if args.set_miniosecretkey:
+            self.config.set(MINIO_CONFIG_SECTION, MINIO_CONFIG_SECRET_KEY, args.set_miniosecretkey)
+
+        if args.show_settings:
+            print(
+                f'url: {self.get_url()}\n'
+                f'privatetoken: {self.get_private_token()}\n'
+                f'projectID: {self.get_project_id()}\n'
+                f'configurationID: {self.get_configuration_id()}')
+
+        if args.set_url or args.set_privatetoken or args.set_project or args.set_configuration:
+            with open(self.path_to_config, "w", encoding='utf-8') as config_file:
+                self.config.write(config_file)
```

### Comparing `testit-importer-allure-1.3.0/src/converter.py` & `testit-importer-allure-1.3.1/src/converter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-from testit_api_client.models import (
-    AutoTestPostModel,
-    AutoTestPutModel,
-    AutoTestStepModel,
-    AvailableTestResultOutcome,
-    LinkPostModel,
-    LinkPutModel,
-    LinkType,
-    AutoTestResultsForTestRunModel,
-    AttachmentPutModelAutoTestStepResultsModel,
-    LabelPostModel)
-
-
-class Converter:
-    @classmethod
-    def test_result_to_autotest_post_model(
-            cls,
-            test_result: dict,
-            project_id: str):
-        return AutoTestPostModel(
-            test_result['external_id'],
-            project_id,
-            test_result['name'],
-            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
-            setup=cls.step_results_to_autotest_steps_model(test_result['setup']),
-            teardown=cls.step_results_to_autotest_steps_model(test_result['teardown']),
-            namespace=test_result['namespace'],
-            classname=test_result['classname'],
-            description=test_result['description'],
-            links=cls.links_to_links_post_model(test_result['links']),
-            labels=test_result['labels']
-        )
-
-    @classmethod
-    def test_result_to_autotest_put_model(
-            cls,
-            test_result: dict,
-            project_id: str):
-        return AutoTestPutModel(
-            test_result['external_id'],
-            project_id,
-            test_result['name'],
-            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
-            setup=cls.step_results_to_autotest_steps_model(test_result['setup']),
-            teardown=cls.step_results_to_autotest_steps_model(test_result['teardown']),
-            namespace=test_result['namespace'],
-            classname=test_result['classname'],
-            description=test_result['description'],
-            links=cls.links_to_links_put_model(test_result['links']),
-            labels=test_result['labels']
-        )
-
-    @classmethod
-    def test_result_to_testrun_result_post_model(
-            cls,
-            test_result: dict,
-            configuration_id: str):
-        return AutoTestResultsForTestRunModel(
-            configuration_id,
-            test_result['external_id'],
-            AvailableTestResultOutcome(test_result['outcome']),
-            step_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['step_results']),
-            setup_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['setup_results']),
-            teardown_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                test_result['teardown_results']),
-            traces=test_result['traces'],
-            attachments=test_result['attachments'],
-            parameters=test_result['parameters'],
-            links=cls.links_to_links_post_model(test_result['links']),
-            duration=round(test_result['duration']),
-            message=test_result['message'],
-            started_on=test_result.get('started_on', None),
-            completed_on=test_result.get('completed_on', None)
-        )
-
-    @staticmethod
-    def link_to_link_post_model(
-            url: str,
-            title: str,
-            url_type,
-            description: str):
-        if url_type:
-            if type(url_type) is str:
-                url_type = LinkType(value=url_type)
-            return LinkPostModel(
-                url,
-                title=title,
-                type=url_type,
-                description=description
-            )
-        else:
-            return LinkPostModel(
-                url,
-                title=title,
-                description=description
-            )
-
-    @staticmethod
-    def link_to_link_put_model(
-            url: str,
-            title: str,
-            url_type,
-            description: str):
-        if url_type:
-            if type(url_type) is str:
-                url_type = LinkType(value=url_type)
-            return LinkPutModel(
-                url,
-                title=title,
-                type=url_type,
-                description=description
-            )
-        else:
-            return LinkPutModel(
-                url,
-                title=title,
-                description=description
-            )
-
-    @classmethod
-    def links_to_links_post_model(cls, links: list):
-        post_model_links = []
-
-        for link in links:
-            post_model_links.append(cls.link_to_link_post_model(
-                link['url'],
-                link.get('title', None),
-                link.get('type', None),
-                link.get('description', None)
-            ))
-
-        return post_model_links
-
-    @classmethod
-    def links_to_links_put_model(cls, links: list):
-        put_model_links = []
-
-        for link in links:
-            put_model_links.append(cls.link_to_link_put_model(
-                link['url'],
-                link.get('title', None),
-                link.get('type', None),
-                link.get('description', None)
-            ))
-
-        return put_model_links
-
-    @classmethod
-    def step_results_to_autotest_steps_model(cls, steps: list):
-        autotest_model_steps = []
-
-        for step in steps:
-            autotest_model_steps.append(
-                cls.step_result_to_autotest_step_model(
-                    step['title'],
-                    cls.step_results_to_autotest_steps_model(
-                        step.get('steps', [])
-                    )
-                )
-            )
-
-        return autotest_model_steps
-
-    @staticmethod
-    def step_result_to_autotest_step_model(
-            title: str,
-            steps: list = None):
-        return AutoTestStepModel(
-            title=title,
-            steps=steps)
-
-    @classmethod
-    def step_results_to_attachment_put_model_autotest_step_results_model(cls, steps: list):
-        autotest_model_step_results = []
-
-        for step in steps:
-            autotest_model_step_results.append(
-                cls.step_result_to_attachment_put_model_autotest_step_results_model(
-                    step['title'],
-                    step['outcome'],
-                    step['duration'],
-                    step['parameters'],
-                    step['attachments'],
-                    cls.step_results_to_attachment_put_model_autotest_step_results_model(
-                        step.get('step_results', [])
-                    )
-                )
-            )
-
-        return autotest_model_step_results
-
-    @staticmethod
-    def step_result_to_attachment_put_model_autotest_step_results_model(
-            title: str,
-            outcome: str,
-            duration: str = None,
-            parameters: list = None,
-            attachments: list = None,
-            step_results: list = None
-    ):
-        return AttachmentPutModelAutoTestStepResultsModel(
-            title=title,
-            outcome=AvailableTestResultOutcome(outcome),
-            duration=duration,
-            parameters=parameters,
-            attachments=attachments,
-            step_results=step_results
-        )
-
-    @staticmethod
-    def label_to_label_post_model(label: str):
-        return LabelPostModel(label)
+from testit_api_client.models import (
+    AutoTestPostModel,
+    AutoTestPutModel,
+    AutoTestStepModel,
+    AvailableTestResultOutcome,
+    LinkPostModel,
+    LinkPutModel,
+    LinkType,
+    AutoTestResultsForTestRunModel,
+    AttachmentPutModelAutoTestStepResultsModel,
+    LabelPostModel)
+
+
+class Converter:
+    @classmethod
+    def test_result_to_autotest_post_model(
+            cls,
+            test_result: dict,
+            project_id: str):
+        return AutoTestPostModel(
+            test_result['external_id'],
+            project_id,
+            test_result['name'],
+            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
+            setup=cls.step_results_to_autotest_steps_model(test_result['setup']),
+            teardown=cls.step_results_to_autotest_steps_model(test_result['teardown']),
+            namespace=test_result['namespace'],
+            classname=test_result['classname'],
+            description=test_result['description'],
+            links=cls.links_to_links_post_model(test_result['links']),
+            labels=test_result['labels']
+        )
+
+    @classmethod
+    def test_result_to_autotest_put_model(
+            cls,
+            test_result: dict,
+            project_id: str):
+        return AutoTestPutModel(
+            test_result['external_id'],
+            project_id,
+            test_result['name'],
+            steps=cls.step_results_to_autotest_steps_model(test_result['steps']),
+            setup=cls.step_results_to_autotest_steps_model(test_result['setup']),
+            teardown=cls.step_results_to_autotest_steps_model(test_result['teardown']),
+            namespace=test_result['namespace'],
+            classname=test_result['classname'],
+            description=test_result['description'],
+            links=cls.links_to_links_put_model(test_result['links']),
+            labels=test_result['labels']
+        )
+
+    @classmethod
+    def test_result_to_testrun_result_post_model(
+            cls,
+            test_result: dict,
+            configuration_id: str):
+        return AutoTestResultsForTestRunModel(
+            configuration_id,
+            test_result['external_id'],
+            AvailableTestResultOutcome(test_result['outcome']),
+            step_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['step_results']),
+            setup_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['setup_results']),
+            teardown_results=cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                test_result['teardown_results']),
+            traces=test_result['traces'],
+            attachments=test_result['attachments'],
+            parameters=test_result['parameters'],
+            links=cls.links_to_links_post_model(test_result['links']),
+            duration=round(test_result['duration']),
+            message=test_result['message'],
+            started_on=test_result.get('started_on', None),
+            completed_on=test_result.get('completed_on', None)
+        )
+
+    @staticmethod
+    def link_to_link_post_model(
+            url: str,
+            title: str,
+            url_type,
+            description: str):
+        if url_type:
+            if type(url_type) is str:
+                url_type = LinkType(value=url_type)
+            return LinkPostModel(
+                url,
+                title=title,
+                type=url_type,
+                description=description
+            )
+        else:
+            return LinkPostModel(
+                url,
+                title=title,
+                description=description
+            )
+
+    @staticmethod
+    def link_to_link_put_model(
+            url: str,
+            title: str,
+            url_type,
+            description: str):
+        if url_type:
+            if type(url_type) is str:
+                url_type = LinkType(value=url_type)
+            return LinkPutModel(
+                url,
+                title=title,
+                type=url_type,
+                description=description
+            )
+        else:
+            return LinkPutModel(
+                url,
+                title=title,
+                description=description
+            )
+
+    @classmethod
+    def links_to_links_post_model(cls, links: list):
+        post_model_links = []
+
+        for link in links:
+            post_model_links.append(cls.link_to_link_post_model(
+                link['url'],
+                link.get('title', None),
+                link.get('type', None),
+                link.get('description', None)
+            ))
+
+        return post_model_links
+
+    @classmethod
+    def links_to_links_put_model(cls, links: list):
+        put_model_links = []
+
+        for link in links:
+            put_model_links.append(cls.link_to_link_put_model(
+                link['url'],
+                link.get('title', None),
+                link.get('type', None),
+                link.get('description', None)
+            ))
+
+        return put_model_links
+
+    @classmethod
+    def step_results_to_autotest_steps_model(cls, steps: list):
+        autotest_model_steps = []
+
+        for step in steps:
+            autotest_model_steps.append(
+                cls.step_result_to_autotest_step_model(
+                    step['title'],
+                    cls.step_results_to_autotest_steps_model(
+                        step.get('steps', [])
+                    )
+                )
+            )
+
+        return autotest_model_steps
+
+    @staticmethod
+    def step_result_to_autotest_step_model(
+            title: str,
+            steps: list = None):
+        return AutoTestStepModel(
+            title=title,
+            steps=steps)
+
+    @classmethod
+    def step_results_to_attachment_put_model_autotest_step_results_model(cls, steps: list):
+        autotest_model_step_results = []
+
+        for step in steps:
+            autotest_model_step_results.append(
+                cls.step_result_to_attachment_put_model_autotest_step_results_model(
+                    step['title'],
+                    step['outcome'],
+                    step['duration'],
+                    step['parameters'],
+                    step['attachments'],
+                    cls.step_results_to_attachment_put_model_autotest_step_results_model(
+                        step.get('step_results', [])
+                    )
+                )
+            )
+
+        return autotest_model_step_results
+
+    @staticmethod
+    def step_result_to_attachment_put_model_autotest_step_results_model(
+            title: str,
+            outcome: str,
+            duration: str = None,
+            parameters: list = None,
+            attachments: list = None,
+            step_results: list = None
+    ):
+        return AttachmentPutModelAutoTestStepResultsModel(
+            title=title,
+            outcome=AvailableTestResultOutcome(outcome),
+            duration=duration,
+            parameters=parameters,
+            attachments=attachments,
+            step_results=step_results
+        )
+
+    @staticmethod
+    def label_to_label_post_model(label: str):
+        return LabelPostModel(label)
```

### Comparing `testit-importer-allure-1.3.0/src/filereader.py` & `testit-importer-allure-1.3.1/src/filereader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-"""The module provides functionality for reading result files from file system"""
-import os
-from interface import implements
-
-from .filedto import FileDto
-from .reader import Reader
-
-
-class FileReader(implements(Reader)):
-    """Class representing a reader"""
-
-    def __init__(self, path_to_results: str):
-        self.__path_to_results = path_to_results
-
-    def get_all_files(self):
-        """Function returns all result files."""
-        files = []
-        if os.path.isdir(self.__path_to_results):
-            self.__path_to_results = os.path.abspath(self.__path_to_results)
-
-            if self.__path_to_results[-1] != '/':
-                self.__path_to_results += '/'
-
-            return os.listdir(self.__path_to_results)
-
-        if os.path.isfile(self.__path_to_results):
-            files.append(os.path.basename(self.__path_to_results))
-            self.__path_to_results = os.path.dirname(os.path.abspath(self.__path_to_results))
-
-        return files
-
-    def read_file(self, file_name: str):
-        """Function reads result file by name."""
-        return FileDto(file_name, open(f"{self.__path_to_results}{file_name}", encoding='UTF-8'))
-
-    def read_attachment(self, file_name: str):
-        """Function reads attachment by name."""
-        return open(f"{self.__path_to_results}{file_name}", 'rb')
-
-    def remove_attachment(self, file_name: str):
-        """Function removes attachment by name."""
-        return
+"""The module provides functionality for reading result files from file system"""
+import os
+from interface import implements
+
+from .filedto import FileDto
+from .reader import Reader
+
+
+class FileReader(implements(Reader)):
+    """Class representing a reader"""
+
+    def __init__(self, path_to_results: str):
+        self.__path_to_results = path_to_results
+
+    def get_all_files(self):
+        """Function returns all result files."""
+        files = []
+        if os.path.isdir(self.__path_to_results):
+            self.__path_to_results = os.path.abspath(self.__path_to_results)
+
+            if self.__path_to_results[-1] != '/':
+                self.__path_to_results += '/'
+
+            files = [f for f in os.listdir(self.__path_to_results) if
+                     os.path.isfile(os.path.join(self.__path_to_results, f))]
+
+            return files
+
+        if os.path.isfile(self.__path_to_results):
+            files.append(os.path.basename(self.__path_to_results))
+            self.__path_to_results = os.path.dirname(os.path.abspath(self.__path_to_results))
+
+        return files
+
+    def read_file(self, file_name: str):
+        """Function reads result file by name."""
+        return FileDto(file_name, open(f"{self.__path_to_results}{file_name}", encoding='UTF-8'))
+
+    def read_attachment(self, file_name: str):
+        """Function reads attachment by name."""
+        return open(f"{self.__path_to_results}{file_name}", 'rb')
+
+    def remove_attachment(self, file_name: str):
+        """Function removes attachment by name."""
+        return
```

### Comparing `testit-importer-allure-1.3.0/src/importer.py` & `testit-importer-allure-1.3.1/src/importer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-"""The module provides functionality for importing result to TMS"""
-import re
-import dataclasses
-from datetime import datetime
-from .apiclient import ApiClient
-from .configurator import Configurator
-from .parser import Parser
-from .converter import Converter
-
-
-@dataclasses.dataclass
-class Importer:
-    """Class representing an importer"""
-
-    def __init__(self, parser: Parser, api_client: ApiClient, config: Configurator):
-        self.__parser = parser
-        self.__api_client = api_client
-        self.__project_id = config.get_project_id()
-        self.__testrun_id = config.specified_testrun
-        self.__configuration_id = config.get_configuration_id()
-
-    def send_result(self):
-        """Function imports result to TMS."""
-        data_tests, data_fixtures = self.__parser.parse_results()
-
-        self.__set_test_run()
-
-        for history_id in data_tests:
-
-            test = data_tests[history_id]
-            prefix = '' if 'uuid' in test else '@'
-
-            test['external_id'] = history_id
-            test['labels'], test['namespace'], test['classname'], work_items_id = \
-                self.__get_data_from_labels(test['labels'])
-            test['attachments'] = self.__send_attachments(test['attachments']) if 'attachments' in test else []
-            test['setup'], test['setup_results'], test['teardown'], test['teardown_results'] = \
-                self.__form_setup_teardown(data_fixtures, test.get('uuid', None))
-            test['steps'], test['step_results'] = self.__form_steps(test.get('steps', None))
-            test['links'] = self.__form_links(test['links']) if 'links' in test else []
-            test['traces'] = test['statusDetails'].get('trace') if \
-                'statusDetails' in test and test['statusDetails'] else None
-            test['message'] = test['statusDetails']['message'] if \
-                'statusDetails' in test and test['statusDetails'] and 'message' in test['statusDetails'] else None
-            test['parameters'] = self.__form_parameters(test['parameters']) if 'parameters' in test else None
-            test['duration'] = (int(test[f'{prefix}stop']) - int(test[f'{prefix}start'])) if \
-                f'{prefix}stop' in test else 0
-            test['started_on'] = datetime.fromtimestamp(int(test[f'{prefix}start']) / 1000.0)
-            test['completed_on'] = datetime.fromtimestamp(int(test[f'{prefix}stop']) / 1000.0)
-            test['description'] = self.__get_description(test.get('description', None))
-
-            if f'{prefix}status' in test:
-                test['outcome'] = \
-                    test[f'{prefix}status'].title() if test[f'{prefix}status'] in ('passed', 'skipped') else 'Failed'
-            else:
-                test['outcome'] = 'Blocked'
-
-            autotest = self.__api_client.get_autotest(history_id, self.__project_id)
-
-            if not autotest:
-                autotest_id = self.__api_client.create_autotest(
-                    Converter.test_result_to_autotest_post_model(test, self.__project_id)
-                )
-            else:
-                autotest_id = autotest[0]['id']
-
-                if test['outcome'] == 'Passed':
-                    self.__api_client.update_autotest(
-                        Converter.test_result_to_autotest_put_model(test, self.__project_id)
-                    )
-                else:
-                    autotest[0]['links'] = test['links']
-
-                    for i in range(0, len(autotest[0]['labels'])):
-                        autotest[0]['labels'][i] = \
-                            Converter.label_to_label_post_model(autotest[0]['labels'][i]['name'])
-
-                    self.__api_client.update_autotest(
-                        Converter.test_result_to_autotest_put_model(autotest[0], self.__project_id)
-                    )
-
-            for work_item_id in work_items_id:
-                self.__api_client.link_autotest(autotest_id, work_item_id)
-
-            self.__api_client.send_test_result(
-                self.__testrun_id,
-                Converter.test_result_to_testrun_result_post_model(test, self.__configuration_id)
-            )
-
-    def __set_test_run(self):
-        if self.__testrun_id is None:
-            test_run_name = f'AllureRun {datetime.today().strftime("%d %b %Y %H:%M:%S")}'
-            self.__testrun_id = self.__api_client.create_test_run(self.__project_id, test_run_name)
-
-    def __send_attachments(self, attachments):
-        ids = []
-
-        if attachments:
-            if 'attachment' in attachments:
-                if type(attachments['attachment']) != list:
-                    attachments = [attachments['attachment']]
-                else:
-                    attachments = attachments['attachment']
-
-            prefix = '' if 'source' in attachments[0] else '@'
-
-            for attachment in attachments:
-
-                file = self.__parser.parse_attachment(f"{attachment[f'{prefix}source']}")
-
-                if file is None:
-                    continue
-
-                attachment_id = self.__api_client.upload_attachment(file)
-
-                if attachment_id:
-                    ids.append(attachment_id)
-
-                self.__parser.clean_attachment(f"{attachment[f'{prefix}source']}")
-
-        return ids
-
-    @staticmethod
-    def __get_description(allure_description):
-        if type(allure_description) == 'str':
-            return allure_description
-        elif type(allure_description) == 'dict':
-            return allure_description.get('#text', None)
-
-        return None
-
-    def __get_data_from_labels(self, allure_labels):
-        class_name = None
-        namespace = None
-        labels = []
-        work_items_id = []
-
-        if allure_labels:
-            allure_labels, prefix = self.__parse_xml(allure_labels, 'label', 'value')
-
-            for label in allure_labels:
-                if label[f'{prefix}name'] == 'testcase':
-                    work_items_id.append(label[f'{prefix}value'])
-                else:
-                    labels.append(
-                        Converter.label_to_label_post_model(
-                            f"{label[f'{prefix}name']}::{label[f'{prefix}value']}"))
-
-                if label[f'{prefix}name'] == 'package':
-                    packages = label[f'{prefix}value'].split('.')
-
-                    while packages and not packages[-1]:
-                        del packages[-1]
-
-                    if packages:
-                        namespace = packages[-1]
-                elif label[f'{prefix}name'] == 'parentSuite':
-                    namespace = label[f'{prefix}value']
-                elif label[f'{prefix}name'] in ('subSuite', 'suite'):
-                    class_name = label[f'{prefix}value']
-                elif label[f'{prefix}name'] == 'testClass':
-                    class_name = label[f'{prefix}value'].split('.')[-1]
-
-        return labels, namespace, class_name, work_items_id
-
-    @staticmethod
-    def __parse_xml(data, key, value):
-        if key in data:
-            if type(data[key]) != list:
-                data = [data[key]]
-            else:
-                data = data[key]
-
-        prefix = '' if data and value in data[0] else '@'
-
-        return data, prefix
-
-    @staticmethod
-    def __form_links(allure_links):
-        links = []
-
-        if allure_links:
-            for link in allure_links:
-                links.append({})
-
-                if 'url' in link and re.fullmatch(
-                        r'^(?:(?:(?:https?|ftp):)?\/\/)?(?:(?:[1-9]\d?|1\d\d|2[01]\d|22[0-3])(?:\.(?:1?\d{1,2}|2[0-4]\d|25[0-5])){2}(?:\.(?:[1-9]\d?|1\d\d|2[0-4]\d|25[0-4]))|(?:(?:[a-zA-Z0-9\u00a1-\uffff][a-zA-Z0-9\u00a1-\uffff_-]{0,62})?[a-zA-Z0-9\u00a1-\uffff]\.)+(?:[a-zA-Z\u00a1-\uffff]{2,}\.?))(?::\d{2,5})?(?:[/?#]\S*)?$',
-                        link['url']):
-                    links[-1]['url'] = link['url']
-                else:
-                    raise Exception('Some links have the wrong URL or no URL!')
-
-                if 'type' in link and link['type'] in (
-                        'Related', 'BlockedBy', 'Defect', 'Issue', 'Requirement', 'Repository'):
-                    links[-1]['type'] = link['type']
-
-                if 'name' in link:
-                    links[-1]['title'] = link['name']
-
-        return links
-
-    def __form_steps(self, steps):
-        adapt_steps = []
-        results_steps = []
-
-        if steps:
-            steps, prefix = self.__parse_xml(steps, 'step', 'status')
-
-            for step in steps:
-                if 'name' in step:
-                    if 'steps' in step:
-                        inner_steps, inner_results_steps = self.__form_steps(step['steps'])
-                    else:
-                        inner_steps = []
-                        inner_results_steps = []
-
-                    adapt_steps.append(
-                        {
-                            'title': step['name'],
-                            'steps': inner_steps
-                        }
-                    )
-
-                    attachments = self.__send_attachments(step['attachments']) if 'attachments' in step else []
-
-                    results_steps.append(
-                        {
-                            'title': step['name'],
-                            'step_results': inner_results_steps,
-                            'outcome': step[f'{prefix}status'].title() if step[f'{prefix}status'] in (
-                                'passed', 'skipped') else 'Failed',
-                            'duration': (int(step[f'{prefix}stop']) - int(
-                                step[f'{prefix}start'])) if f'{prefix}stop' in step else 0,
-                            'started_on': datetime.fromtimestamp(int(step[f'{prefix}start']) / 1000.0),
-                            'completed_on': datetime.fromtimestamp(
-                                int(step[f'{prefix}stop']) / 1000.0) if f'{prefix}stop' in step else None,
-                            "attachments": attachments,
-                            'parameters': self.__form_parameters(step['parameters']) if 'parameters' in step else None
-                        }
-                    )
-
-        return adapt_steps, results_steps
-
-    def __form_parameters(self, allure_parameters):
-        parameters = {}
-
-        if allure_parameters:
-            allure_parameters, prefix = self.__parse_xml(allure_parameters, 'parameter', 'value')
-
-            for parameter in allure_parameters:
-                parameters[parameter[f'{prefix}name']] = str(parameter[f'{prefix}value'])
-
-        return parameters
-
-    def __form_setup_teardown(self, data_before_after, test_uuid):
-        setup = []
-        teardown = []
-        results_setup = []
-        results_teardown = []
-
-        if test_uuid:
-            for uuid in data_before_after:
-                if 'children' in data_before_after[uuid]:
-                    for child in data_before_after[uuid]['children']:
-                        if child == test_uuid:
-                            steps, results_steps = self.__form_steps(data_before_after[uuid].get('befores'))
-                            setup += steps
-                            results_setup += results_steps
-                            steps, results_steps = self.__form_steps(data_before_after[uuid].get('afters'))
-                            teardown += steps
-                            results_teardown += results_steps
-
-        return setup, results_setup, teardown, results_teardown
+"""The module provides functionality for importing result to TMS"""
+import re
+import dataclasses
+from datetime import datetime
+from .apiclient import ApiClient
+from .configurator import Configurator
+from .parser import Parser
+from .converter import Converter
+
+
+@dataclasses.dataclass
+class Importer:
+    """Class representing an importer"""
+
+    def __init__(self, parser: Parser, api_client: ApiClient, config: Configurator):
+        self.__parser = parser
+        self.__api_client = api_client
+        self.__project_id = config.get_project_id()
+        self.__testrun_id = config.specified_testrun
+        self.__configuration_id = config.get_configuration_id()
+
+    def send_result(self):
+        """Function imports result to TMS."""
+        data_tests, data_fixtures = self.__parser.parse_results()
+
+        self.__set_test_run()
+
+        for history_id in data_tests:
+
+            test = data_tests[history_id]
+            prefix = '' if 'uuid' in test else '@'
+
+            test['external_id'] = history_id
+            test['labels'], test['namespace'], test['classname'], work_items_id = \
+                self.__get_data_from_labels(test['labels'])
+            test['attachments'] = self.__send_attachments(test['attachments']) if 'attachments' in test else []
+            test['setup'], test['setup_results'], test['teardown'], test['teardown_results'] = \
+                self.__form_setup_teardown(data_fixtures, test.get('uuid', None))
+            test['steps'], test['step_results'] = self.__form_steps(test.get('steps', None))
+            test['links'] = self.__form_links(test['links']) if 'links' in test else []
+            test['traces'] = test['statusDetails'].get('trace') if \
+                'statusDetails' in test and test['statusDetails'] else None
+            test['message'] = test['statusDetails']['message'] if \
+                'statusDetails' in test and test['statusDetails'] and 'message' in test['statusDetails'] else None
+            test['parameters'] = self.__form_parameters(test['parameters']) if 'parameters' in test else None
+            test['duration'] = (int(test[f'{prefix}stop']) - int(test[f'{prefix}start'])) if \
+                f'{prefix}stop' in test else 0
+            test['started_on'] = datetime.fromtimestamp(int(test[f'{prefix}start']) / 1000.0)
+            test['completed_on'] = datetime.fromtimestamp(int(test[f'{prefix}stop']) / 1000.0)
+            test['description'] = self.__get_description(test.get('description', None))
+
+            if f'{prefix}status' in test:
+                test['outcome'] = \
+                    test[f'{prefix}status'].title() if test[f'{prefix}status'] in ('passed', 'skipped') else 'Failed'
+            else:
+                test['outcome'] = 'Blocked'
+
+            autotest = self.__api_client.get_autotest(history_id, self.__project_id)
+
+            if not autotest:
+                autotest_id = self.__api_client.create_autotest(
+                    Converter.test_result_to_autotest_post_model(test, self.__project_id)
+                )
+            else:
+                autotest_id = autotest[0]['id']
+
+                if test['outcome'] == 'Passed':
+                    self.__api_client.update_autotest(
+                        Converter.test_result_to_autotest_put_model(test, self.__project_id)
+                    )
+                else:
+                    autotest[0]['links'] = test['links']
+
+                    for i in range(0, len(autotest[0]['labels'])):
+                        autotest[0]['labels'][i] = \
+                            Converter.label_to_label_post_model(autotest[0]['labels'][i]['name'])
+
+                    self.__api_client.update_autotest(
+                        Converter.test_result_to_autotest_put_model(autotest[0], self.__project_id)
+                    )
+
+            for work_item_id in work_items_id:
+                self.__api_client.link_autotest(autotest_id, work_item_id)
+
+            self.__api_client.send_test_result(
+                self.__testrun_id,
+                Converter.test_result_to_testrun_result_post_model(test, self.__configuration_id)
+            )
+
+    def __set_test_run(self):
+        if self.__testrun_id is None:
+            test_run_name = f'AllureRun {datetime.today().strftime("%d %b %Y %H:%M:%S")}'
+            self.__testrun_id = self.__api_client.create_test_run(self.__project_id, test_run_name)
+
+    def __send_attachments(self, attachments):
+        ids = []
+
+        if attachments:
+            if 'attachment' in attachments:
+                if type(attachments['attachment']) != list:
+                    attachments = [attachments['attachment']]
+                else:
+                    attachments = attachments['attachment']
+
+            prefix = '' if 'source' in attachments[0] else '@'
+
+            for attachment in attachments:
+
+                file = self.__parser.parse_attachment(f"{attachment[f'{prefix}source']}")
+
+                if file is None:
+                    continue
+
+                attachment_id = self.__api_client.upload_attachment(file)
+
+                if attachment_id:
+                    ids.append(attachment_id)
+
+                self.__parser.clean_attachment(f"{attachment[f'{prefix}source']}")
+
+        return ids
+
+    @staticmethod
+    def __get_description(allure_description):
+        if type(allure_description) == 'str':
+            return allure_description
+        elif type(allure_description) == 'dict':
+            return allure_description.get('#text', None)
+
+        return None
+
+    def __get_data_from_labels(self, allure_labels):
+        class_name = None
+        namespace = None
+        labels = []
+        work_items_id = []
+
+        if allure_labels:
+            allure_labels, prefix = self.__parse_xml(allure_labels, 'label', 'value')
+
+            for label in allure_labels:
+                if label[f'{prefix}name'] == 'testcase':
+                    work_items_id.append(label[f'{prefix}value'])
+                else:
+                    labels.append(
+                        Converter.label_to_label_post_model(
+                            f"{label[f'{prefix}name']}::{label[f'{prefix}value']}"))
+
+                if label[f'{prefix}name'] == 'package':
+                    packages = label[f'{prefix}value'].split('.')
+
+                    while packages and not packages[-1]:
+                        del packages[-1]
+
+                    if packages:
+                        namespace = packages[-1]
+                elif label[f'{prefix}name'] == 'parentSuite':
+                    namespace = label[f'{prefix}value']
+                elif label[f'{prefix}name'] in ('subSuite', 'suite'):
+                    class_name = label[f'{prefix}value']
+                elif label[f'{prefix}name'] == 'testClass':
+                    class_name = label[f'{prefix}value'].split('.')[-1]
+
+        return labels, namespace, class_name, work_items_id
+
+    @staticmethod
+    def __parse_xml(data, key, value):
+        if key in data:
+            if type(data[key]) != list:
+                data = [data[key]]
+            else:
+                data = data[key]
+
+        prefix = '' if data and value in data[0] else '@'
+
+        return data, prefix
+
+    @staticmethod
+    def __form_links(allure_links):
+        links = []
+
+        if allure_links:
+            for link in allure_links:
+                links.append({})
+
+                if 'url' in link and re.fullmatch(
+                        r'^(?:(?:(?:https?|ftp):)?\/\/)?(?:(?:[1-9]\d?|1\d\d|2[01]\d|22[0-3])(?:\.(?:1?\d{1,2}|2[0-4]\d|25[0-5])){2}(?:\.(?:[1-9]\d?|1\d\d|2[0-4]\d|25[0-4]))|(?:(?:[a-zA-Z0-9\u00a1-\uffff][a-zA-Z0-9\u00a1-\uffff_-]{0,62})?[a-zA-Z0-9\u00a1-\uffff]\.)+(?:[a-zA-Z\u00a1-\uffff]{2,}\.?))(?::\d{2,5})?(?:[/?#]\S*)?$',
+                        link['url']):
+                    links[-1]['url'] = link['url']
+                else:
+                    raise Exception('Some links have the wrong URL or no URL!')
+
+                if 'type' in link and link['type'] in (
+                        'Related', 'BlockedBy', 'Defect', 'Issue', 'Requirement', 'Repository'):
+                    links[-1]['type'] = link['type']
+
+                if 'name' in link:
+                    links[-1]['title'] = link['name']
+
+        return links
+
+    def __form_steps(self, steps):
+        adapt_steps = []
+        results_steps = []
+
+        if steps:
+            steps, prefix = self.__parse_xml(steps, 'step', 'status')
+
+            for step in steps:
+                if 'name' in step:
+                    if 'steps' in step:
+                        inner_steps, inner_results_steps = self.__form_steps(step['steps'])
+                    else:
+                        inner_steps = []
+                        inner_results_steps = []
+
+                    adapt_steps.append(
+                        {
+                            'title': step['name'],
+                            'steps': inner_steps
+                        }
+                    )
+
+                    attachments = self.__send_attachments(step['attachments']) if 'attachments' in step else []
+
+                    results_steps.append(
+                        {
+                            'title': step['name'],
+                            'step_results': inner_results_steps,
+                            'outcome': step[f'{prefix}status'].title() if step[f'{prefix}status'] in (
+                                'passed', 'skipped') else 'Failed',
+                            'duration': (int(step[f'{prefix}stop']) - int(
+                                step[f'{prefix}start'])) if f'{prefix}stop' in step else 0,
+                            'started_on': datetime.fromtimestamp(int(step[f'{prefix}start']) / 1000.0),
+                            'completed_on': datetime.fromtimestamp(
+                                int(step[f'{prefix}stop']) / 1000.0) if f'{prefix}stop' in step else None,
+                            "attachments": attachments,
+                            'parameters': self.__form_parameters(step['parameters']) if 'parameters' in step else None
+                        }
+                    )
+
+        return adapt_steps, results_steps
+
+    def __form_parameters(self, allure_parameters):
+        parameters = {}
+
+        if allure_parameters:
+            allure_parameters, prefix = self.__parse_xml(allure_parameters, 'parameter', 'value')
+
+            for parameter in allure_parameters:
+                parameters[parameter[f'{prefix}name']] = str(parameter[f'{prefix}value'])
+
+        return parameters
+
+    def __form_setup_teardown(self, data_before_after, test_uuid):
+        setup = []
+        teardown = []
+        results_setup = []
+        results_teardown = []
+
+        if test_uuid:
+            for uuid in data_before_after:
+                if 'children' in data_before_after[uuid]:
+                    for child in data_before_after[uuid]['children']:
+                        if child == test_uuid:
+                            steps, results_steps = self.__form_steps(data_before_after[uuid].get('befores'))
+                            setup += steps
+                            results_setup += results_steps
+                            steps, results_steps = self.__form_steps(data_before_after[uuid].get('afters'))
+                            teardown += steps
+                            results_teardown += results_steps
+
+        return setup, results_setup, teardown, results_teardown
```

### Comparing `testit-importer-allure-1.3.0/src/parser.py` & `testit-importer-allure-1.3.1/src/parser.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-"""The module provides functionality for parsing result files"""
-import os
-import json
-import hashlib
-import xmltodict
-from .filedto import FileDto
-from .reader import Reader
-
-
-class Parser:
-    """Class representing a parser"""
-
-    def __init__(self, reader: Reader):
-        self.__reader = reader
-        self.__data_tests = {}
-        self.__data_fixtures = {}
-
-    def parse_results(self):
-        """Function parses results"""
-        files = self.__reader.get_all_files()
-
-        for file in files:
-            self.__read(file)
-
-        return self.__data_tests, self.__data_fixtures
-
-    def parse_attachment(self, file_name: str):
-        """Function parses attachment"""
-        return self.__reader.read_attachment(file_name)
-
-    def clean_attachment(self, file_name: str):
-        """Function cleans after attachment"""
-        self.__reader.remove_attachment(file_name)
-
-    def __read(self, file_path: str):
-        file_name, file_extension = os.path.splitext(file_path)
-        file: FileDto = self.__reader.read_file(file_path)
-
-        if file_extension == '.json':
-            self.__read_json(file)
-        elif file_extension == '.xml' and file_name[-9:] == 'testsuite':
-            self.__read_xml(file)
-
-    def __read_json(self, file_dto: FileDto):
-        result_data = json.load(file_dto.file)
-
-        if 'result' in file_dto.name:
-            if result_data['historyId'] not in self.__data_tests \
-                    or result_data['start'] > self.__data_tests[result_data['historyId']]['start']:
-                self.__data_tests[result_data['historyId']] = result_data
-
-        elif 'container' in file_dto.name:
-            if 'children' in result_data:
-                self.__data_fixtures[result_data['uuid']] = result_data
-
-    def __read_xml(self, file_dto: FileDto):
-        testsuite = xmltodict.parse(file_dto.file.read())
-        testcases_data = testsuite['ns2:test-suite']['test-cases']['test-case']
-
-        if isinstance(testcases_data, list):
-            for testcase in testcases_data:
-                self.__read_xml_testcase(testcase)
-        else:
-            self.__read_xml_testcase(testcases_data)
-
-    def __read_xml_testcase(self, testcase: dict):
-        if testcase['title'] and testcase['name']:
-            md5 = hashlib.md5()
-            md5.update(testcase['title'].encode('utf-8'))
-            testcase_id = md5.hexdigest()
-
-            if testcase_id not in self.__data_tests \
-                    or testcase['@start'] > self.__data_tests[testcase_id]['@start']:
-                self.__data_tests[testcase_id] = testcase
+"""The module provides functionality for parsing result files"""
+import os
+import json
+import hashlib
+import xmltodict
+from .filedto import FileDto
+from .reader import Reader
+
+
+class Parser:
+    """Class representing a parser"""
+
+    def __init__(self, reader: Reader):
+        self.__reader = reader
+        self.__data_tests = {}
+        self.__data_fixtures = {}
+
+    def parse_results(self):
+        """Function parses results"""
+        files = self.__reader.get_all_files()
+
+        for file in files:
+            self.__read(file)
+
+        return self.__data_tests, self.__data_fixtures
+
+    def parse_attachment(self, file_name: str):
+        """Function parses attachment"""
+        return self.__reader.read_attachment(file_name)
+
+    def clean_attachment(self, file_name: str):
+        """Function cleans after attachment"""
+        self.__reader.remove_attachment(file_name)
+
+    def __read(self, file_path: str):
+        file_name, file_extension = os.path.splitext(file_path)
+        file: FileDto = self.__reader.read_file(file_path)
+
+        if file_extension == '.json':
+            self.__read_json(file)
+        elif file_extension == '.xml' and file_name[-9:] == 'testsuite':
+            self.__read_xml(file)
+
+    def __read_json(self, file_dto: FileDto):
+        result_data = json.load(file_dto.file)
+
+        if 'result' in file_dto.name:
+            if result_data['historyId'] not in self.__data_tests \
+                    or result_data['start'] > self.__data_tests[result_data['historyId']]['start']:
+                self.__data_tests[result_data['historyId']] = result_data
+
+        elif 'container' in file_dto.name:
+            if 'children' in result_data:
+                self.__data_fixtures[result_data['uuid']] = result_data
+
+    def __read_xml(self, file_dto: FileDto):
+        testsuite = xmltodict.parse(file_dto.file.read())
+        testcases_data = testsuite['ns2:test-suite']['test-cases']['test-case']
+
+        if isinstance(testcases_data, list):
+            for testcase in testcases_data:
+                self.__read_xml_testcase(testcase)
+        else:
+            self.__read_xml_testcase(testcases_data)
+
+    def __read_xml_testcase(self, testcase: dict):
+        if testcase['title'] and testcase['name']:
+            md5 = hashlib.md5()
+            md5.update(testcase['title'].encode('utf-8'))
+            testcase_id = md5.hexdigest()
+
+            if testcase_id not in self.__data_tests \
+                    or testcase['@start'] > self.__data_tests[testcase_id]['@start']:
+                self.__data_tests[testcase_id] = testcase
```

### Comparing `testit-importer-allure-1.3.0/src/rabbitmq.py` & `testit-importer-allure-1.3.1/src/rabbitmq.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-"""The module provides functionality for consuming rabbit MQ"""
-import dataclasses
-import pika
-
-
-@dataclasses.dataclass
-class RabbitMQ:
-    """Class representing a rabit mq client"""
-
-    def __init__(self, url: str, user: str, password: str, exchange: str):
-        self.__url = pika.URLParameters('amqp://' + user + ':' + password + '@' + url)
-        self.__exchange = exchange
-
-    def consume(self, callback_func):
-        """Function consumes query."""
-        connection = pika.BlockingConnection(self.__url)
-        channel = connection.channel()
-
-        result = channel.queue_declare(queue='', exclusive=True)
-        queue_name = result.method.queue
-        channel.queue_bind(exchange=self.__exchange, queue=queue_name, routing_key="key")
-
-        channel.basic_consume(queue=queue_name, on_message_callback=callback_func, auto_ack=True)
-        channel.start_consuming()
+"""The module provides functionality for consuming rabbit MQ"""
+import dataclasses
+import pika
+
+
+@dataclasses.dataclass
+class RabbitMQ:
+    """Class representing a rabit mq client"""
+
+    def __init__(self, url: str, user: str, password: str, exchange: str):
+        self.__url = pika.URLParameters('amqp://' + user + ':' + password + '@' + url)
+        self.__exchange = exchange
+
+    def consume(self, callback_func):
+        """Function consumes query."""
+        connection = pika.BlockingConnection(self.__url)
+        channel = connection.channel()
+
+        result = channel.queue_declare(queue='', exclusive=True)
+        queue_name = result.method.queue
+        channel.queue_bind(exchange=self.__exchange, queue=queue_name, routing_key="key")
+
+        channel.basic_consume(queue=queue_name, on_message_callback=callback_func, auto_ack=True)
+        channel.start_consuming()
```

### Comparing `testit-importer-allure-1.3.0/testit_importer_allure.egg-info/PKG-INFO` & `testit-importer-allure-1.3.1/testit_importer_allure.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,86 @@
-Metadata-Version: 2.1
-Name: testit-importer-allure
-Version: 1.3.0
-Summary: Allure report importer for Test IT
-Home-page: https://pypi.org/project/testit-importer-allure/
-Author: Integration team
-Author-email: integrations@testit.software
-License: Apache-2.0
-Description: # Test IT TMS importers
-        ![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
-        
-        # Allure report
-        
-        ## Getting Started
-        
-        ### Installation
-        ```
-        pip install testit-importer-allure
-        ```
-        
-        ## Usage
-        
-        ### API client
-        
-        To use importer you need to install `testit-api-client`:
-        ```
-        pip install testit-api-client
-        ```
-        
-        ### Configuration
-        
-        Use the command `testit --help` to view the configuration setup help:
-        ```
-        testit --url <url>
-        testit --privatetoken <token>
-        testit --projectid <id>
-        testit --configurationid <id>
-        ```
-        
-        And fill parameters with your configuration, where:  
-        `url` - location of the TMS instance  
-        `privatetoken` - API secret key  
-        
-        1. go to the https://{DOMAIN}/user-profile profile  
-        2. copy the API secret key
-        
-        `projectid` - id of project in TMS instance
-        
-        1. create a project
-        2. open DevTools -> network
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
-        4. GET-request project, Preview tab, copy id field  
-        
-        `configurationid` - id of configuration in TMS instance  
-        
-        1. create a project  
-        2. open DevTools -> network  
-        3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
-        4. GET-request configurations, Preview tab, copy id field 
-        
-        ### Importing
-        
-        Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
-        Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
-        **Important:** This command initiates the import.
-        
-        # Contributing
-        
-        You can help to develop the project. Any contributions are **greatly appreciated**.
-        
-        * If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
-        * Please make sure you check your spelling and grammar.
-        * Create individual PR for each suggestion.
-        * Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
-        
-        # License
-        
-        Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: testit-importer-allure
+Version: 1.3.1
+Summary: Allure report importer for Test IT
+Home-page: https://pypi.org/project/testit-importer-allure/
+Author: Integration team
+Author-email: integrations@testit.software
+License: Apache-2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# Test IT TMS importers
+![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
+
+# Allure report
+
+## Getting Started
+
+### Installation
+```
+pip install testit-importer-allure
+```
+
+## Usage
+
+### API client
+
+To use importer you need to install `testit-api-client`:
+```
+pip install testit-api-client
+```
+
+### Configuration
+
+Use the command `testit --help` to view the configuration setup help:
+```
+testit --url <url>
+testit --privatetoken <token>
+testit --projectid <id>
+testit --configurationid <id>
+```
+
+And fill parameters with your configuration, where:  
+`url` - location of the TMS instance  
+`privatetoken` - API secret key  
+
+1. go to the https://{DOMAIN}/user-profile profile  
+2. copy the API secret key
+
+`projectid` - id of project in TMS instance
+
+1. create a project
+2. open DevTools -> network
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests
+4. GET-request project, Preview tab, copy id field  
+
+`configurationid` - id of configuration in TMS instance  
+
+1. create a project  
+2. open DevTools -> network  
+3. go to the project https://{DOMAIN}/projects/{PROJECT_GLOBAL_ID}/tests  
+4. GET-request configurations, Preview tab, copy id field 
+
+### Importing
+
+Use the command `testit --resultsdir allure-results` to specify the directory with Allure report results and create new test run in TMS instance.  
+Or use the command `testit --resultsdir allure-results --testrunid <id>` to specify the directory with Allure report results and id of test run in TMS instance.
+**Important:** This command initiates the import.
+
+# Contributing
+
+You can help to develop the project. Any contributions are **greatly appreciated**.
+
+* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/testit-tms/importers/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
+* Please make sure you check your spelling and grammar.
+* Create individual PR for each suggestion.
+* Please also read through the [Code Of Conduct](https://github.com/testit-tms/importers/blob/master/CODE_OF_CONDUCT.md) before posting your first idea as well.
+
+# License
+
+Distributed under the Apache-2.0 License. See [LICENSE](https://github.com/testit-tms/importers/blob/master/LICENSE.md) for more information.
+
```

### Comparing `testit-importer-allure-1.3.0/testit_importer_allure.egg-info/SOURCES.txt` & `testit-importer-allure-1.3.1/testit_importer_allure.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-.gitignore
-.pylintrc
-Dockerfile
 README.md
-connection_config.ini
-debug.py
-requirements.txt
 setup.py
-.run/Debug.run.xml
 src/__init__.py
 src/__main__.py
 src/apiclient.py
 src/configurator.py
 src/converter.py
 src/filedto.py
 src/filereader.py
```

