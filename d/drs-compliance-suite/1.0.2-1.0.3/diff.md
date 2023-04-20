# Comparing `tmp/drs-compliance-suite-1.0.2.tar.gz` & `tmp/drs-compliance-suite-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drs-compliance-suite-1.0.2.tar", last modified: Sun Apr 16 23:50:12 2023, max compression
+gzip compressed data, was "drs-compliance-suite-1.0.3.tar", last modified: Thu Apr 20 20:38:12 2023, max compression
```

## Comparing `drs-compliance-suite-1.0.2.tar` & `drs-compliance-suite-1.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.160368 drs-compliance-suite-1.0.2/
--rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-suite-1.0.2/LICENSE
--rw-r--r--   0 ypuligun   (502) staff       (20)     7686 2023-04-16 23:50:12.159688 drs-compliance-suite-1.0.2/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     7275 2023-04-16 23:35:21.000000 drs-compliance-suite-1.0.2/README.md
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.139100 drs-compliance-suite-1.0.2/compliance_suite/
--rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/__init__.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/constants.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-16 22:43:53.000000 drs-compliance-suite-1.0.2/compliance_suite/helper.py
--rw-r--r--   0 ypuligun   (502) staff       (20)    17219 2023-04-16 23:25:54.000000 drs-compliance-suite-1.0.2/compliance_suite/report_runner.py
--rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-16 22:43:02.000000 drs-compliance-suite-1.0.2/compliance_suite/report_server.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.141767 drs-compliance-suite-1.0.2/compliance_suite/schemas/
--rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/service_info.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/service_type.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.149604 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/
--rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json
--rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/error.json
--rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/validate_drs_object_response.py
--rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-16 22:42:40.000000 drs-compliance-suite-1.0.2/compliance_suite/validate_response.py
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.150494 drs-compliance-suite-1.0.2/compliance_suite/web/
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.152285 drs-compliance-suite-1.0.2/compliance_suite/web/static/
--rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/web/static/style.css
--rw-r--r--   0 ypuligun   (502) staff       (20)    33141 2023-04-16 22:50:36.000000 drs-compliance-suite-1.0.2/compliance_suite/web/temp_report.json
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.153723 drs-compliance-suite-1.0.2/compliance_suite/web/templates/
--rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.2/compliance_suite/web/templates/index.html
-drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-16 23:50:12.158852 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/
--rw-r--r--   0 ypuligun   (502) staff       (20)     7686 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/PKG-INFO
--rw-r--r--   0 ypuligun   (502) staff       (20)     1074 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/SOURCES.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/dependency_links.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       71 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/entry_points.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/requires.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-16 23:50:12.000000 drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/top_level.txt
--rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-16 23:50:12.161981 drs-compliance-suite-1.0.2/setup.cfg
--rw-r--r--   0 ypuligun   (502) staff       (20)     1309 2023-04-16 23:49:54.000000 drs-compliance-suite-1.0.2/setup.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.104711 drs-compliance-suite-1.0.3/
+-rw-r--r--   0 ypuligun   (502) staff       (20)    11357 2022-07-08 15:27:41.000000 drs-compliance-suite-1.0.3/LICENSE
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7859 2023-04-20 20:38:12.104008 drs-compliance-suite-1.0.3/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7448 2023-04-20 20:38:03.000000 drs-compliance-suite-1.0.3/README.md
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.080674 drs-compliance-suite-1.0.3/compliance_suite/
+-rw-r--r--   0 ypuligun   (502) staff       (20)        0 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/__init__.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      448 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/constants.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     6314 2023-04-16 22:43:53.000000 drs-compliance-suite-1.0.3/compliance_suite/helper.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)    17176 2023-04-20 20:38:03.000000 drs-compliance-suite-1.0.3/compliance_suite/report_runner.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)      557 2023-04-16 22:43:02.000000 drs-compliance-suite-1.0.3/compliance_suite/report_server.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.083387 drs-compliance-suite-1.0.3/compliance_suite/schemas/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3333 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/service_info.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1264 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/service_type.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.093479 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1395 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/access_method.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      799 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/access_url.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1286 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/checksum.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1820 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/contents_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4766 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/drs_bundle.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4746 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/drs_object.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)      635 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/error.json
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2664 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/validate_drs_object_response.py
+-rw-r--r--   0 ypuligun   (502) staff       (20)     3563 2023-04-16 22:42:40.000000 drs-compliance-suite-1.0.3/compliance_suite/validate_response.py
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.094846 drs-compliance-suite-1.0.3/compliance_suite/web/
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.096457 drs-compliance-suite-1.0.3/compliance_suite/web/static/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     2441 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/web/static/style.css
+-rw-r--r--   0 ypuligun   (502) staff       (20)    41929 2023-04-20 20:16:11.000000 drs-compliance-suite-1.0.3/compliance_suite/web/temp_report.json
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.097509 drs-compliance-suite-1.0.3/compliance_suite/web/templates/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     4656 2023-04-12 18:08:46.000000 drs-compliance-suite-1.0.3/compliance_suite/web/templates/index.html
+drwxr-xr-x   0 ypuligun   (502) staff       (20)        0 2023-04-20 20:38:12.102927 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/
+-rw-r--r--   0 ypuligun   (502) staff       (20)     7859 2023-04-20 20:38:11.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/PKG-INFO
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1074 2023-04-20 20:38:12.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)        1 2023-04-20 20:38:11.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       77 2023-04-20 20:38:11.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/entry_points.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)      153 2023-04-20 20:38:11.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/requires.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       17 2023-04-20 20:38:11.000000 drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/top_level.txt
+-rw-r--r--   0 ypuligun   (502) staff       (20)       38 2023-04-20 20:38:12.106216 drs-compliance-suite-1.0.3/setup.cfg
+-rw-r--r--   0 ypuligun   (502) staff       (20)     1315 2023-04-20 20:38:03.000000 drs-compliance-suite-1.0.3/setup.py
```

### Comparing `drs-compliance-suite-1.0.2/LICENSE` & `drs-compliance-suite-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/PKG-INFO` & `drs-compliance-suite-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: drs-compliance-suite
-Version: 1.0.2
-Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
-Home-page: https://github.com/ga4gh/drs-compliance-suite
-Author: Yash Puligundla
-Author-email: yasasvini.puligundla@ga4gh.org
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # drs-compliance-suite
 Tests to verify the compliance of a DRS implementation with GA4GH Data Repository Service (DRS) specification. 
 This compliance suite currently supports the following DRS versions and will aim to support more versions of DRS in the future.
 * DRS 1.2.0
 
 ## Installations
 - [Python 3.x](https://www.python.org/downloads/) is required to run DRS Compliance Suite natively or using PyPI package.
@@ -38,35 +26,35 @@
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 2. Using PyPI Package
 
-Install the latest version of the `drs-compliance` PyPI package using pip3
+Install the latest version of the `drs-compliance-suite` PyPI package using pip3
 ```
-pip3 install drs-compliance --upgrade
+pip3 install drs-compliance-suite --upgrade
 ```
 Run the compliance suite
 ```
-drs-compliance --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
+drs-compliance-suite --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 3. Using Docker
 
 Pull the latest docker image from dockerhub. 
 ```
-docker pull ga4gh/drs-compliance-suite:1.0.2
+docker pull ga4gh/drs-compliance-suite:1.0.3
 ```
 Run the compliance suite using the docker image
 ```
-docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.2 --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
+docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.3: --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### Command Line Arguments
 | Command Line Argument | Description | Optional/Required | Default Value |
@@ -135,16 +123,21 @@
 
 Run the unittests with coverage
 ```
 pytest --cov=compliance_suite unittests/
 ```
 
 ## Changelog
+
+### v1.0.3
+* provide flexibility in providing different auth information for drs object and drs access endpoints
+* remove incorrect skip status setting
+
 ### v1.0.2
 * Reduce the docker image size by using python:3.11-slim-bullseye instead of python:3
 
 ### v1.0.1
 * Fixed a bug in the docker deployment of DRS Compliance Suite 
 * Update README documentation
 
 ### v1.0.0
-* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
+* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
```

### Comparing `drs-compliance-suite-1.0.2/README.md` & `drs-compliance-suite-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: drs-compliance-suite
+Version: 1.0.3
+Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
+Home-page: https://github.com/ga4gh/drs-compliance-suite
+Author: Yash Puligundla
+Author-email: yasasvini.puligundla@ga4gh.org
+License: MIT
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # drs-compliance-suite
 Tests to verify the compliance of a DRS implementation with GA4GH Data Repository Service (DRS) specification. 
 This compliance suite currently supports the following DRS versions and will aim to support more versions of DRS in the future.
 * DRS 1.2.0
 
 ## Installations
 - [Python 3.x](https://www.python.org/downloads/) is required to run DRS Compliance Suite natively or using PyPI package.
@@ -26,35 +38,35 @@
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 2. Using PyPI Package
 
-Install the latest version of the `drs-compliance` PyPI package using pip3
+Install the latest version of the `drs-compliance-suite` PyPI package using pip3
 ```
-pip3 install drs-compliance --upgrade
+pip3 install drs-compliance-suite --upgrade
 ```
 Run the compliance suite
 ```
-drs-compliance --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
+drs-compliance-suite --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 3. Using Docker
 
 Pull the latest docker image from dockerhub. 
 ```
-docker pull ga4gh/drs-compliance-suite:1.0.2
+docker pull ga4gh/drs-compliance-suite:1.0.3
 ```
 Run the compliance suite using the docker image
 ```
-docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.2 --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
+docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.3: --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### Command Line Arguments
 | Command Line Argument | Description | Optional/Required | Default Value |
@@ -123,16 +135,21 @@
 
 Run the unittests with coverage
 ```
 pytest --cov=compliance_suite unittests/
 ```
 
 ## Changelog
+
+### v1.0.3
+* provide flexibility in providing different auth information for drs object and drs access endpoints
+* remove incorrect skip status setting
+
 ### v1.0.2
 * Reduce the docker image size by using python:3.11-slim-bullseye instead of python:3
 
 ### v1.0.1
 * Fixed a bug in the docker deployment of DRS Compliance Suite 
 * Update README documentation
 
 ### v1.0.0
-* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
+* DRS Compliance Suite for [Data Repository Service v1.2.0](https://ga4gh.github.io/data-repository-service-schemas/preview/release/drs-1.2.0/docs/)
```

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/helper.py` & `drs-compliance-suite-1.0.3/compliance_suite/helper.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/report_runner.py` & `drs-compliance-suite-1.0.3/compliance_suite/report_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def report_runner(server_base_url, platform_name, platform_description, drs_version, config_file):
     """
     Returns a Report Object which is generated by running compliance tests on various endpoints of a DRS server.
     """
     # Read input DRS objects from config folder
     # TODO: Add lower and upper limits to input DRS objects
-    config_service_info, input_drs_objects = get_config_json(config_file)
+    config_service_info, config_drs_object_info, config_drs_object_access = get_config_json(config_file)
 
     # TODO: config json objects must contain auth_token and auth_type for service_info and for each of the drs_objects
     # get authentication information from respective config file based on type of authentication
 
     # Create a compliance report object
     report_object = Report()
     report_object.set_testbed_name(TESTBED_NAME)
@@ -64,15 +64,15 @@
 
 
     ### PHASE: /objects/{object_id}
     drs_object_phase = report_object.add_phase()
     drs_object_phase.set_phase_name("drs object info")
     drs_object_phase.set_phase_description("run all the tests for drs object info endpoint")
 
-    for this_drs_object in input_drs_objects:
+    for this_drs_object in config_drs_object_info:
 
         # TODO: Add code to figure out what the expected_status_code
         #  and expected_content_type are for each drs_object_id.
         test_drs_object_info(
             drs_object_phase,
             server_base_url,
             auth_type = this_drs_object["auth_type"],
@@ -90,15 +90,15 @@
     drs_object_phase.set_end_time_now()
 
     # PHASE: /objects/{object_id}/access/{access_id}
     drs_access_phase = report_object.add_phase()
     drs_access_phase.set_phase_name("drs object access")
     drs_access_phase.set_phase_description("run all the tests for drs access endpoint")
 
-    for this_drs_object in input_drs_objects:
+    for this_drs_object in config_drs_object_access:
         for this_access_id in drs_objects_access_id_map[this_drs_object["drs_id"]]:
             test_drs_object_access(
                 drs_access_phase,
                 server_base_url,
                 auth_type = this_drs_object["auth_type"],
                 auth_token = this_drs_object["auth_token"],
                 drs_object_id = this_drs_object["drs_id"],
@@ -117,16 +117,17 @@
     """
     Returns the auth details for service-info endpoint and input DRS objects from the config file.
     """
     try:
         with open(os.path.join(config_file), "r") as f:
             config = json.load(f)
             config_service_info = config["service_info"]
-            config_input_drs_objects = config["drs_objects"]
-            return config_service_info, config_input_drs_objects
+            config_drs_object_info = config["drs_object_info"]
+            config_drs_object_access = config["drs_object_access"]
+            return config_service_info, config_drs_object_info, config_drs_object_access
     except Exception as e:
         raise Exception(f"Failed loading JSON config file: {config_file}",e)
 
 def test_service_info(
         service_info_phase,
         server_base_url,
         auth_type,
@@ -190,18 +191,14 @@
         expected_content_type = expected_content_type,
         schema_dir = schema_dir,
         schema_file = schema_file)
 
     skip_access_methods_test_cases = False
     skip_message = ""
 
-    if status_code_pass != Status.PASS:
-        skip_access_methods_test_cases = True
-        skip_message = "Skipping this test case as response status code is not as expected"
-
     if is_bundle:
 
         # Response with expand parameter set to true
         response = send_request(
             server_base_url,
             DRS_OBJECT_INFO_URL + drs_object_id,
             auth_type,
```

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/report_server.py` & `drs-compliance-suite-1.0.3/compliance_suite/report_server.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/service_info.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/service_info.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/service_type.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/service_type.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/access_method.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/access_method.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/access_url.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/access_url.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/checksum.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/checksum.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/contents_object.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/contents_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/drs_bundle.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/drs_bundle.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/drs_object.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/drs_object.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/schemas/v1.2.0/error.json` & `drs-compliance-suite-1.0.3/compliance_suite/schemas/v1.2.0/error.json`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/validate_drs_object_response.py` & `drs-compliance-suite-1.0.3/compliance_suite/validate_drs_object_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/validate_response.py` & `drs-compliance-suite-1.0.3/compliance_suite/validate_response.py`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/web/static/style.css` & `drs-compliance-suite-1.0.3/compliance_suite/web/static/style.css`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/compliance_suite/web/templates/index.html` & `drs-compliance-suite-1.0.3/compliance_suite/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/PKG-INFO` & `drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drs-compliance-suite
-Version: 1.0.2
+Version: 1.0.3
 Summary: A compliance utility reporting system for GA4GH DRS server implementations. Supports GA4GH DRS versions - 1.2.0
 Home-page: https://github.com/ga4gh/drs-compliance-suite
 Author: Yash Puligundla
 Author-email: yasasvini.puligundla@ga4gh.org
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -38,35 +38,35 @@
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 2. Using PyPI Package
 
-Install the latest version of the `drs-compliance` PyPI package using pip3
+Install the latest version of the `drs-compliance-suite` PyPI package using pip3
 ```
-pip3 install drs-compliance --upgrade
+pip3 install drs-compliance-suite --upgrade
 ```
 Run the compliance suite
 ```
-drs-compliance --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
+drs-compliance-suite --server_base_url "http://localhost:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_basic.json" --serve --serve_port 56565
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### 3. Using Docker
 
 Pull the latest docker image from dockerhub. 
 ```
-docker pull ga4gh/drs-compliance-suite:1.0.2
+docker pull ga4gh/drs-compliance-suite:1.0.3
 ```
 Run the compliance suite using the docker image
 ```
-docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.2 --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
+docker run -d --name drs-compliance-suite -v $(PWD)/output/:/usr/src/app/output/ -p 57568:57568 ga4gh/drs-compliance-suite:1.0.3: --server_base_url "http://host.docker.internal:8085/ga4gh/drs/v1" --platform_name "ga4gh starter kit drs" --platform_description "GA4GH reference implementation of DRS specification" --report_path "./output/test-report.json" --drs_version "1.2.0" --config_file "compliance_suite/config/config_samples/config_none.json" --serve --serve_port 57568
 ```
 Note: This specific command is an example of running the compliance suite on a local deployment of DRS that is running on port 8085. \
 When running the compliance suite, it's important to configure the command line arguments according to the specific DRS implementation you're testing.
 Please refer to the [Command Line Arguments](#command-line-arguments) section for details on each of these arguments.
 
 ### Command Line Arguments
 | Command Line Argument | Description | Optional/Required | Default Value |
@@ -135,14 +135,19 @@
 
 Run the unittests with coverage
 ```
 pytest --cov=compliance_suite unittests/
 ```
 
 ## Changelog
+
+### v1.0.3
+* provide flexibility in providing different auth information for drs object and drs access endpoints
+* remove incorrect skip status setting
+
 ### v1.0.2
 * Reduce the docker image size by using python:3.11-slim-bullseye instead of python:3
 
 ### v1.0.1
 * Fixed a bug in the docker deployment of DRS Compliance Suite 
 * Update README documentation
```

### Comparing `drs-compliance-suite-1.0.2/drs_compliance_suite.egg-info/SOURCES.txt` & `drs-compliance-suite-1.0.3/drs_compliance_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drs-compliance-suite-1.0.2/setup.py` & `drs-compliance-suite-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from supported_drs_versions import SUPPORTED_DRS_VERSIONS
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="drs-compliance-suite",
-    version="1.0.2",
+    version="1.0.3",
     author="Yash Puligundla",
     author_email="yasasvini.puligundla@ga4gh.org",
     packages=["compliance_suite"],
     package_data={'compliance_suite': ['config/*', 'schemas/*', 'schemas/v1.2.0/*', 'web/*', 'web/static/*', 'web/templates/*']},
     description="A compliance utility reporting system for GA4GH DRS server implementations. "
                 "Supports GA4GH DRS versions - " + ",".join(SUPPORTED_DRS_VERSIONS),
     long_description=long_description,
@@ -24,11 +24,11 @@
                       'Flask==2.2.0',
                       'Flask-HTTPAuth==4.7.0',
                       'pytest==7.1.2',
                       'pytest-cov==3.0.0',
                       'ga4gh-testbed-lib==0.2.0'],
     entry_points='''
         [console_scripts]
-        drs-compliance=compliance_suite.report_runner:main
+        drs-compliance-suite=compliance_suite.report_runner:main
     '''
 
 )
```

