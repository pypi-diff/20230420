# Comparing `tmp/os_ios_app_automation-1.15.tar.gz` & `tmp/os_ios_app_automation-1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/os_ios_app_automation-1.15.tar", last modified: Sun Feb 27 09:25:54 2022, max compression
+gzip compressed data, was "os_ios_app_automation-1.16.tar", last modified: Thu Apr 20 07:47:54 2023, max compression
```

## Comparing `os_ios_app_automation-1.15.tar` & `os_ios_app_automation-1.16.tar`

### file list

```diff
@@ -1,9 +1,17 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-02-27 09:25:54.000000 os_ios_app_automation-1.15/
--rw-r--r--   0 home       (501) staff       (20)      835 2022-02-27 09:25:54.000000 os_ios_app_automation-1.15/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     1741 2022-02-27 09:25:53.000000 os_ios_app_automation-1.15/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-02-27 09:25:54.000000 os_ios_app_automation-1.15/os_ios_app_automation/
-drwxr-xr-x   0 home       (501) staff       (20)        0 2022-02-27 09:25:54.000000 os_ios_app_automation-1.15/os_ios_app_automation/bp/
--rw-r--r--   0 home       (501) staff       (20)    11705 2022-02-27 09:22:03.000000 os_ios_app_automation-1.15/os_ios_app_automation/bp/_xcode_manipulation_mapper.py
--rw-r--r--   0 home       (501) staff       (20)      596 2021-12-23 08:36:05.000000 os_ios_app_automation-1.15/os_ios_app_automation/bp/_res.py
--rw-r--r--   0 home       (501) staff       (20)      737 2021-01-25 14:15:58.000000 os_ios_app_automation-1.15/os_ios_app_automation/app_automation.py
--rw-r--r--   0 home       (501) staff       (20)       43 2019-07-11 10:53:04.000000 os_ios_app_automation-1.15/setup.cfg
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-04-20 07:47:54.617621 os_ios_app_automation-1.16/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1065 2019-06-20 10:31:16.000000 os_ios_app_automation-1.16/LICENSE.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      822 2023-04-20 07:47:54.617668 os_ios_app_automation-1.16/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     9134 2021-02-07 14:17:24.000000 os_ios_app_automation-1.16/README.md
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-04-20 07:47:54.616390 os_ios_app_automation-1.16/os_ios_app_automation/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      737 2021-01-25 14:15:58.000000 os_ios_app_automation-1.16/os_ios_app_automation/app_automation.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-04-20 07:47:54.617310 os_ios_app_automation-1.16/os_ios_app_automation/bp/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      596 2021-12-23 08:36:05.000000 os_ios_app_automation-1.16/os_ios_app_automation/bp/_res.py
+-rw-r--r--   0 ozshabbat   (501) staff       (20)    11880 2023-04-20 07:47:12.000000 os_ios_app_automation-1.16/os_ios_app_automation/bp/_xcode_manipulation_mapper.py
+drwxr-xr-x   0 ozshabbat   (501) staff       (20)        0 2023-04-20 07:47:54.616957 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      822 2023-04-20 07:47:54.000000 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/PKG-INFO
+-rw-r--r--   0 ozshabbat   (501) staff       (20)      392 2023-04-20 07:47:54.000000 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)        1 2023-04-20 07:47:54.000000 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       58 2023-04-20 07:47:54.000000 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/requires.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       22 2023-04-20 07:47:54.000000 os_ios_app_automation-1.16/os_ios_app_automation.egg-info/top_level.txt
+-rw-r--r--   0 ozshabbat   (501) staff       (20)       38 2023-04-20 07:47:54.617815 os_ios_app_automation-1.16/setup.cfg
+-rw-r--r--   0 ozshabbat   (501) staff       (20)     1741 2023-04-20 07:47:23.000000 os_ios_app_automation-1.16/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `os_ios_app_automation-1.15/PKG-INFO` & `os_ios_app_automation-1.16/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: os_ios_app_automation
-Version: 1.15
+Version: 1.16
 Summary: Will prepare an iOS app by properties defined by a xml file
 Home-page: https://github.com/osfunapps/os-ios-app-automation-py
 Author: Oz Shabat
 Author-email: support@os-apps.com
 License: MIT
-Description: UNKNOWN
 Keywords: python,osfunapps,osapps,files,xml,tools,utils,xcode,ios,automation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE.txt
```

### Comparing `os_ios_app_automation-1.15/setup.py` & `os_ios_app_automation-1.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
     name='os_ios_app_automation',  # How you named your package folder (MyLib)
     packages=['os_ios_app_automation',
               'os_ios_app_automation.bp'],  # Choose the same as "name"
-    version='1.15',  # Start with a small number and increase it with every change you make
+    version='1.16',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='Will prepare an iOS app by properties defined by a xml file',  # Give a short description about your library
     author='Oz Shabat',  # Type in your name
     author_email='support@os-apps.com',  # Type in your E-Mail
     url='https://github.com/osfunapps/os-ios-app-automation-py',  # Provide either the link to your github or to your website
     keywords=['python', 'osfunapps', 'osapps', 'files', 'xml', 'tools', 'utils', 'xcode','ios','automation'],  # Keywords that define your package best
     install_requires=['os_file_handler', 'os_xml_handler', 'os-tools', 'os-xml-automation'],
```

### Comparing `os_ios_app_automation-1.15/os_ios_app_automation/bp/_xcode_manipulation_mapper.py` & `os_ios_app_automation-1.16/os_ios_app_automation/bp/_xcode_manipulation_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,20 @@
 # operate the next step
 def run_next_step_cycle(project, root_node, xml_path, place_holder_map, curr_step):
     next_step_node = xh.get_child_nodes(root_node, f'{shared_res.NODE_STEP}_{str(curr_step)}')
 
     # if the next step exists, start running on all of the direct children
     if next_step_node:
         print_line()
-        print(f'Starting step: {str(curr_step)}')
         next_step_node = next_step_node[0]
+        next_step_str = f'Starting step {str(curr_step)}'
+        step_name = xh.get_node_att(next_step_node, "name")
+        if step_name is not None:
+          next_step_str += f': {step_name}'
+        print(next_step_str)
         for curr_step_child_node in xh.get_all_direct_child_nodes(next_step_node):
             curr_step_tag = curr_step_child_node.tag
 
             # if link
             if curr_step_tag == res.NODE_LINK:
                 do_link_tag(project, xml_path, place_holder_map, curr_step_child_node)
```

### Comparing `os_ios_app_automation-1.15/os_ios_app_automation/bp/_res.py` & `os_ios_app_automation-1.16/os_ios_app_automation/bp/_res.py`

 * *Files identical despite different names*

### Comparing `os_ios_app_automation-1.15/os_ios_app_automation/app_automation.py` & `os_ios_app_automation-1.16/os_ios_app_automation/app_automation.py`

 * *Files identical despite different names*

