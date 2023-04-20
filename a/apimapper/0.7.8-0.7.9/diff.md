# Comparing `tmp/apimapper-0.7.8.tar.gz` & `tmp/apimapper-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apimapper-0.7.8.tar", last modified: Wed Feb  5 13:02:19 2020, max compression
+gzip compressed data, was "apimapper-0.7.9.tar", last modified: Thu Apr 20 11:52:01 2023, max compression
```

## Comparing `apimapper-0.7.8.tar` & `apimapper-0.7.9.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxr-x   0 saranb    (1000) saranb    (1000)        0 2020-02-05 13:02:19.000000 apimapper-0.7.8/
--rw-r--r--   0 saranb    (1000) saranb    (1000)      934 2020-02-05 13:01:02.000000 apimapper-0.7.8/setup.py
--rw-rw-r--   0 saranb    (1000) saranb    (1000)     2832 2020-02-03 14:07:41.000000 apimapper-0.7.8/README.md
-drwxrwxr-x   0 saranb    (1000) saranb    (1000)        0 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper/
--rw-r--r--   0 saranb    (1000) saranb    (1000)     3576 2019-11-21 16:24:50.000000 apimapper-0.7.8/apimapper/apimapper.py
-drwxrwxr-x   0 saranb    (1000) saranb    (1000)        0 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper/config/
--rw-r--r--   0 saranb    (1000) saranb    (1000)      296 2019-07-29 11:10:58.000000 apimapper-0.7.8/apimapper/config/config.py
--rw-r--r--   0 saranb    (1000) saranb    (1000)        0 2019-03-19 16:41:05.000000 apimapper-0.7.8/apimapper/config/__init__.py
--rw-r--r--   0 saranb    (1000) saranb    (1000)     4516 2019-03-19 16:41:03.000000 apimapper-0.7.8/apimapper/config/demo.py
--rw-r--r--   0 saranb    (1000) saranb    (1000)      131 2019-03-25 10:43:15.000000 apimapper-0.7.8/apimapper/__init__.py
--rw-r--r--   0 saranb    (1000) saranb    (1000)     3713 2020-02-05 12:06:26.000000 apimapper-0.7.8/apimapper/responsemapper.py
--rw-rw-r--   0 saranb    (1000) saranb    (1000)     3988 2020-02-05 13:02:19.000000 apimapper-0.7.8/PKG-INFO
-drwxrwxr-x   0 saranb    (1000) saranb    (1000)        0 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/
--rw-r--r--   0 saranb    (1000) saranb    (1000)     3988 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/PKG-INFO
--rw-r--r--   0 saranb    (1000) saranb    (1000)        1 2019-03-19 16:22:35.000000 apimapper-0.7.8/apimapper.egg-info/not-zip-safe
--rw-r--r--   0 saranb    (1000) saranb    (1000)       10 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/top_level.txt
--rw-r--r--   0 saranb    (1000) saranb    (1000)      368 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/SOURCES.txt
--rw-r--r--   0 saranb    (1000) saranb    (1000)        1 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/dependency_links.txt
--rw-r--r--   0 saranb    (1000) saranb    (1000)       18 2020-02-05 13:02:19.000000 apimapper-0.7.8/apimapper.egg-info/requires.txt
--rw-rw-r--   0 saranb    (1000) saranb    (1000)       38 2020-02-05 13:02:19.000000 apimapper-0.7.8/setup.cfg
+drwxrwxr-x   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 11:52:01.179477 apimapper-0.7.9/
+-rw-r--r--   0 gythaogg  (1000) gythaogg  (1000)     1066 2019-06-26 09:07:16.000000 apimapper-0.7.9/LICENSE
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)     3347 2023-04-20 11:52:01.179477 apimapper-0.7.9/PKG-INFO
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)     2816 2023-04-20 11:43:50.000000 apimapper-0.7.9/README.md
+drwxrwxr-x   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 11:52:01.179477 apimapper-0.7.9/apimapper/
+-rw-r--r--   0 gythaogg  (1000) gythaogg  (1000)      131 2019-06-26 09:07:16.000000 apimapper-0.7.9/apimapper/__init__.py
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)     3668 2023-04-20 10:42:50.000000 apimapper-0.7.9/apimapper/apimapper.py
+drwxrwxr-x   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 11:52:01.179477 apimapper-0.7.9/apimapper/config/
+-rw-r--r--   0 gythaogg  (1000) gythaogg  (1000)        0 2019-06-26 09:07:16.000000 apimapper-0.7.9/apimapper/config/__init__.py
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)      296 2020-02-03 08:38:50.000000 apimapper-0.7.9/apimapper/config/config.py
+-rw-r--r--   0 gythaogg  (1000) gythaogg  (1000)     4516 2019-06-26 09:07:16.000000 apimapper-0.7.9/apimapper/config/demo.py
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)     3830 2023-04-20 10:43:39.000000 apimapper-0.7.9/apimapper/responsemapper.py
+drwxrwxr-x   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 11:52:01.179477 apimapper-0.7.9/apimapper/tests/
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 08:53:41.000000 apimapper-0.7.9/apimapper/tests/__init__.py
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)      790 2023-04-20 10:41:41.000000 apimapper-0.7.9/apimapper/tests/test_apimapper.py
+drwxrwxr-x   0 gythaogg  (1000) gythaogg  (1000)        0 2023-04-20 11:52:01.179477 apimapper-0.7.9/apimapper.egg-info/
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)     3347 2023-04-20 11:52:01.000000 apimapper-0.7.9/apimapper.egg-info/PKG-INFO
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)      438 2023-04-20 11:52:01.000000 apimapper-0.7.9/apimapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)        1 2023-04-20 11:52:01.000000 apimapper-0.7.9/apimapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)        1 2023-04-20 08:59:46.000000 apimapper-0.7.9/apimapper.egg-info/not-zip-safe
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)       18 2023-04-20 11:52:01.000000 apimapper-0.7.9/apimapper.egg-info/requires.txt
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)       10 2023-04-20 11:52:01.000000 apimapper-0.7.9/apimapper.egg-info/top_level.txt
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)       38 2023-04-20 11:52:01.183477 apimapper-0.7.9/setup.cfg
+-rw-rw-r--   0 gythaogg  (1000) gythaogg  (1000)      936 2023-04-20 11:50:23.000000 apimapper-0.7.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apimapper-0.7.8/setup.py` & `apimapper-0.7.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # read the contents of your README file
 from os import path
 
 from setuptools import find_packages, setup
 
-with open('README.md', 'r') as f:
+with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
-    name='apimapper',
-    version='0.7.8',
-    description='API Mapper',
+    name="apimapper",
+    version="0.7.9",
+    description="API Mapper",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Scientific/Engineering :: Information Analysis',
+        "Development Status :: 3 - Alpha",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
+        "Topic :: Scientific/Engineering :: Information Analysis",
     ],
-    keywords='API Mapper',
-    url='https://github.com/acdh-oeaw/apimapper',
-    author='Saranya Balasubramanian, Ksenia Zaytseva',
-    author_email='saranya.balasubramanian@oeaw.ac.at',
-    license='MIT',
+    keywords="API Mapper",
+    url="https://github.com/acdh-oeaw/apimapper",
+    author="Saranya Balasubramanian, Ksenia Zaytseva",
+    author_email="saranya.balasubramanian@oeaw.ac.at",
+    license="MIT",
     packages=find_packages(),
     install_requires=[
-        'markdown',
-        'requests',
+        "markdown",
+        "requests",
     ],
     include_package_data=True,
-    zip_safe=False)
+    zip_safe=False,
+)
```

### Comparing `apimapper-0.7.8/README.md` & `apimapper-0.7.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Install package
 * from PyPi:
     pip install apimapper
 * from source:
     pip install -e .
 
 ## Unit Testing
-   tests> python -m pytest
+   >pytest
 
 ## Usage
 
 * See https://github.com/acdh-oeaw/apimapper/blob/develop/demo/APIMapper%20Demo.ipynb
 * Multiple APIs (GND and VIAF) mapped to a common JSON schema
 
 VIAF only returns VIAF ID - which is contructed into a url using a "rule"
```

### Comparing `apimapper-0.7.8/apimapper/apimapper.py` & `apimapper-0.7.9/apimapper/apimapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class APIMapper:
     def __init__(self, source, mapping=None, timeout: float = 0.1):
         # URL, result, mapping, filter
         self.source = source
         self.mapping = ResponseMapper(mapping)
         self.timeout = timeout
         if not self.source or not self.source.get(URL):
-            raise ValueError('Bad source, no URL')
+            raise ValueError("Bad source, no URL")
 
         return
 
     def add_payload(self, payload_dict):
         if not self.source.get(PAYLOAD):
             self.source[PAYLOAD] = {}
 
@@ -29,80 +29,87 @@
         return
 
     def set_payload(self, payload_dict):
         self.source[PAYLOAD] = payload_dict
         return
 
     def add_query(self, query):
-        '''
-        Adds query string to the payload, 
+        """
+        Adds query string to the payload,
         sandwiched by wildcards as applicable
-        '''
+        """
         full_query = query
         if self.source.get(QUERY_PREFIX_WILDCARD, False):
-            full_query = '*{}'.format(full_query)
+            full_query = "*{}".format(full_query)
         else:
             pass
         if self.source.get(QUERY_SUFFIX_WILDCARD, False):
-            full_query = '{}*'.format(full_query)
+            full_query = "{}*".format(full_query)
         else:
             pass
 
         self.add_payload({self.source.get(QUERY_FIELD): full_query})
 
         return
 
     def fetch_results(self, query=None):
-        '''
+        """
         requests the url with the payload as specified in the source
         maps the response to the schema as specified in the source
         returns mapped_schema
-        '''
+        """
         self.add_query(query)
 
         def get_response_content():
-            '''
-            analyses "original_response" - handles error codes and exceptions 
+            """
+            analyses "original_response" - handles error codes and exceptions
             and returns json decoded response from the result field if specified in the source
             or the complete response
-            '''
-            if re.search(r'^2\d\d$', str(original_response.status_code)):
+            """
+            if re.search(r"^2\d\d$", str(original_response.status_code)):
                 try:
                     return json.loads(original_response.content)
 
                 except Exception as e:  # super bad!
                     logging.warning(
-                        'Cannot read API response, got %s. Error: %s',
-                        original_response.content, repr(e))
+                        "Cannot read API response, got %s. Error: %s",
+                        original_response.content,
+                        repr(e),
+                    )
                     # Keep calm and carry on
             else:
                 # bad status code in response
-                logging.warning('Bad request, got %s\nContents:\n%s',
-                                original_response.status_code,
-                                original_response.content)
+                logging.warning(
+                    "Bad request, got %s\nContents:\n%s",
+                    original_response.status_code,
+                    original_response.content,
+                )
 
             return {}
 
         # set accept property in header
         if not HEADER in self.source:
-            self.source[HEADER] = {'accept': 'application/json'}
+            self.source[HEADER] = {"accept": "application/json"}
         else:
-            self.source[HEADER]['accept'] = 'application/json'
+            self.source[HEADER]["accept"] = "application/json"
 
         try:
             original_response = requests.get(
                 self.source.get(URL),
                 params=self.source.get(PAYLOAD),
                 headers=self.source.get(HEADER),
-                timeout=self.source.get(TIMEOUT, self.timeout))
+                timeout=self.source.get(TIMEOUT, self.timeout),
+            )
 
-        except (requests.exceptions.ConnectionError,
-                requests.exceptions.Timeout) as ce:
+        except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as ce:
             # Keep calm and carry on
-            logging.warning('Connection error while trying to access %s:\n %s',
-                            self.source.get('URL'), repr(ce))
+            logging.warning(
+                "Connection error while trying to access %s:\n %s",
+                self.source.get("URL"),
+                repr(ce),
+            )
             return {}
 
         response_content = get_response_content()
         logging.debug(response_content)
         mapped_response = self.mapping.get_mapped_response(response_content)
         return mapped_response
```

### Comparing `apimapper-0.7.8/apimapper/config/demo.py` & `apimapper-0.7.9/apimapper/config/demo.py`

 * *Files identical despite different names*

### Comparing `apimapper-0.7.8/apimapper/responsemapper.py` & `apimapper-0.7.9/apimapper/responsemapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 import logging
-from collections import Iterable
+
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
 from copy import deepcopy
 
 from .config.config import *
 
 logger = logging.getLogger(__name__)
 
 
 class ResponseMapper:
     def __init__(self, mapping=None):
         self.mapping = mapping
         return
 
     def _is_relevant_result(self, res_item):
-        '''
+        """
         called for every item in the response (res_item)
         returns True if the response matches the "filter" condition specified in the configurationq
 
-        '''
+        """
         for filter_field, filter_value in self.mapping.get(FILTER, {}).items():
             if res_item.get(filter_field) != filter_value:
                 return False
             else:
                 pass
         return True
 
     def _map_item_rules(self, res_item):
         # Rule based mapping
         mapped_schema = {}
         for to_key, rule_data in self.mapping.get(RULES, {}).items():
-            logger.debug('Mapping rule: %s <- %s', to_key, rule_data)
+            logger.debug("Mapping rule: %s <- %s", to_key, rule_data)
             rule = rule_data.get(RULE)
             fields = rule_data.get(FIELDS, {})
             eval_params = {}
 
             # obtain values from response to evauate the "mapping rule"
             for k, v in fields.items():
                 eval_params[k] = self._deep_search(res_item, v)
                 # res_item.get(v, '')
-
-            # logging.debug('%s: %s', k, rule.format(**eval_params))
+                logging.debug("%s: %s", k, rule.format(**eval_params))
 
             try:
                 mapped_schema[to_key] = eval(rule.format(**eval_params))
-                logging.debug('%s: %s', to_key, mapped_schema[to_key])
+                logging.debug("%s: %s", to_key, mapped_schema[to_key])
             except Exception as e:
                 # Bad rule: keep calm and carry on
-                mapped_schema[to_key] = ''
+                mapped_schema[to_key] = ""
                 logging.warning(
-                    'Encountered bad rule (%s) for input "%s"\n %s', rule_data,
-                    eval_params, repr(e))
+                    'Encountered bad rule (%s) for input "%s"\n %s',
+                    rule_data,
+                    eval_params,
+                    repr(e),
+                )
 
         return mapped_schema
 
     def _map_item_direct(self, res_item):
         # Direct field based mapping
         mapped_schema = {}
         for to_key, from_key in self.mapping.get(DIRECT, {}).items():
             mapped_schema[to_key] = self._deep_search(res_item, from_key)
         return mapped_schema
 
     @staticmethod
     def _deep_search(res_item, from_key_path):
-        '''
+        """
         maps the parmeter empedded within JSON fields
-        '''
+        """
 
-        if not isinstance(from_key_path, str) and isinstance(
-                from_key_path, Iterable):
+        if not isinstance(from_key_path, str) and isinstance(from_key_path, Iterable):
             deep_search = deepcopy(res_item)
             for from_key_item in from_key_path:
                 deep_search = deep_search.get(from_key_item)
 
             return deep_search
 
         return res_item.get(from_key_path)
@@ -83,29 +89,29 @@
             direct_map = self._map_item_direct(res_item)
             rule_map = self._map_item_rules(res_item)
             return {**direct_map, **rule_map}
 
         return {}
 
     def get_mapped_response(self, original_response):
-        '''
+        """
         map original response to fields specified in config
-        '''
+        """
         if not self.mapping:
-            logging.warning('No mapping found. Returning as-is.')
+            logging.warning("No mapping found. Returning as-is.")
             return original_response
 
         mapped_response = []
         if self.mapping.get(RESULT):
-            original_response = original_response.get(
-                self.mapping.get(RESULT), [])
+            original_response = original_response.get(self.mapping.get(RESULT), [])
 
         try:
             for res_item in original_response:  # what
                 mapped_item = self._map_item(res_item)
-                if len(mapped_item): mapped_response.append(mapped_item)
+                if len(mapped_item):
+                    mapped_response.append(mapped_item)
 
             return mapped_response
         except TypeError as te:
-            logging.warning('Encountered TypeError: %s', repr(te))
+            logging.warning("Encountered TypeError: %s", repr(te))
 
         return []
```

### Comparing `apimapper-0.7.8/PKG-INFO` & `apimapper-0.7.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: apimapper
-Version: 0.7.8
+Version: 0.7.9
 Summary: API Mapper
 Home-page: https://github.com/acdh-oeaw/apimapper
 Author: Saranya Balasubramanian, Ksenia Zaytseva
 Author-email: saranya.balasubramanian@oeaw.ac.at
 License: MIT
-Description: # API Wrapper
-        
-        ## Install package
-        * from PyPi:
-            pip install apimapper
-        * from source:
-            pip install -e .
-        
-        ## Unit Testing
-           tests> python -m pytest
-        
-        ## Usage
-        
-        * See https://github.com/acdh-oeaw/apimapper/blob/develop/demo/APIMapper%20Demo.ipynb
-        * Multiple APIs (GND and VIAF) mapped to a common JSON schema
-        
-        VIAF only returns VIAF ID - which is contructed into a url using a "rule"
-        ```
-        from apimapper import APIMapper
-        from apimapper import config
-        
-        GND_PERSON_MAP = {config.DIRECT: {'uri': 'id',
-                              'label': 'label'}}
-        
-        VIAF_PERSON_MAP = {config.RESULT: 'result',
-                           config.FILTER: {'nametype': 'personal'},
-                           config.DIRECT: {'label': 'displayForm'},
-                           config.RULES: {'uri': {config.RULE: '"http://www.viaf.org/viaf/{p1}"',
-                                                  config.FIELDS: {'p1': 'viafid'}}}}
-        
-        GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
-                             config.QUERY_FIELD: 'q',
-                             config.PAYLOAD: {'format':'json:suggest',
-                                              'filter': 'type:Person'}}
-        
-        VIAF_PERSON_SOURCE =  {config.URL: 'http://www.viaf.org/viaf/AutoSuggest',
-                               config.QUERY_FIELD: 'query'}
-        
-        
-        gnd = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
-        viaf = APIMapper(VIAF_PERSON_SOURCE, VIAF_PERSON_MAP)
-        apis = [gnd, viaf]
-        results = []
-        for api in apis:
-            res = api.fetch_results('Pratchett')
-            results.extend(res)
-        
-        print(results)
-        ```
-        
-        * Using mapping rules
-        
-        Splitting the GND label field into meaningful subparts
-        ```
-        from apimapper import APIMapper
-        from apimapper import config
-        
-        GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
-                             config.QUERY_FIELD: 'q',
-                             config.PAYLOAD: {'format':'json:suggest',
-                                              'filter': 'type:Person'}}
-        
-        GND_PERSON_MAP = {config.DIRECT: {'label': 'label',
-                                          'uri': 'id'},
-                  config.RULES: {'source': {config.RULE: '"GND"'},
-                                 'label_name': {config.RULE: '"{p1}".split("|")[0].strip()',
-                                                        config.FIELDS: {'p1': 'label'}},
-                                         'label_year': {config.RULE: '"{p1}".split("|")[1].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else ""',
-                                                    config.FIELDS: {'p1': 'label'}},
-                                             'label_profession': {config.RULE: '"{p1}".split("|")[2].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else "{p1}".split("|")[1].strip()',
-                                                                  config.FIELDS: {'p1': 'label'}}}}
-        
-        api = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
-        res = api.fetch_results('Rosalind Franklin')
-        ```
-        
-        * More example usage in apimapper/demo
-        
 Keywords: API Mapper
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# API Wrapper
+
+## Install package
+* from PyPi:
+    pip install apimapper
+* from source:
+    pip install -e .
+
+## Unit Testing
+   >pytest
+
+## Usage
+
+* See https://github.com/acdh-oeaw/apimapper/blob/develop/demo/APIMapper%20Demo.ipynb
+* Multiple APIs (GND and VIAF) mapped to a common JSON schema
+
+VIAF only returns VIAF ID - which is contructed into a url using a "rule"
+```
+from apimapper import APIMapper
+from apimapper import config
+
+GND_PERSON_MAP = {config.DIRECT: {'uri': 'id',
+                      'label': 'label'}}
+
+VIAF_PERSON_MAP = {config.RESULT: 'result',
+                   config.FILTER: {'nametype': 'personal'},
+                   config.DIRECT: {'label': 'displayForm'},
+                   config.RULES: {'uri': {config.RULE: '"http://www.viaf.org/viaf/{p1}"',
+                                          config.FIELDS: {'p1': 'viafid'}}}}
+
+GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
+                     config.QUERY_FIELD: 'q',
+                     config.PAYLOAD: {'format':'json:suggest',
+                                      'filter': 'type:Person'}}
+
+VIAF_PERSON_SOURCE =  {config.URL: 'http://www.viaf.org/viaf/AutoSuggest',
+                       config.QUERY_FIELD: 'query'}
+
+
+gnd = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
+viaf = APIMapper(VIAF_PERSON_SOURCE, VIAF_PERSON_MAP)
+apis = [gnd, viaf]
+results = []
+for api in apis:
+    res = api.fetch_results('Pratchett')
+    results.extend(res)
+
+print(results)
+```
+
+* Using mapping rules
+
+Splitting the GND label field into meaningful subparts
+```
+from apimapper import APIMapper
+from apimapper import config
+
+GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
+                     config.QUERY_FIELD: 'q',
+                     config.PAYLOAD: {'format':'json:suggest',
+                                      'filter': 'type:Person'}}
+
+GND_PERSON_MAP = {config.DIRECT: {'label': 'label',
+                                  'uri': 'id'},
+          config.RULES: {'source': {config.RULE: '"GND"'},
+                         'label_name': {config.RULE: '"{p1}".split("|")[0].strip()',
+                                                config.FIELDS: {'p1': 'label'}},
+                                 'label_year': {config.RULE: '"{p1}".split("|")[1].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else ""',
+                                            config.FIELDS: {'p1': 'label'}},
+                                     'label_profession': {config.RULE: '"{p1}".split("|")[2].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else "{p1}".split("|")[1].strip()',
+                                                          config.FIELDS: {'p1': 'label'}}}}
+
+api = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
+res = api.fetch_results('Rosalind Franklin')
+```
+
+* More example usage in apimapper/demo
```

### Comparing `apimapper-0.7.8/apimapper.egg-info/PKG-INFO` & `apimapper-0.7.9/apimapper.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: apimapper
-Version: 0.7.8
+Version: 0.7.9
 Summary: API Mapper
 Home-page: https://github.com/acdh-oeaw/apimapper
 Author: Saranya Balasubramanian, Ksenia Zaytseva
 Author-email: saranya.balasubramanian@oeaw.ac.at
 License: MIT
-Description: # API Wrapper
-        
-        ## Install package
-        * from PyPi:
-            pip install apimapper
-        * from source:
-            pip install -e .
-        
-        ## Unit Testing
-           tests> python -m pytest
-        
-        ## Usage
-        
-        * See https://github.com/acdh-oeaw/apimapper/blob/develop/demo/APIMapper%20Demo.ipynb
-        * Multiple APIs (GND and VIAF) mapped to a common JSON schema
-        
-        VIAF only returns VIAF ID - which is contructed into a url using a "rule"
-        ```
-        from apimapper import APIMapper
-        from apimapper import config
-        
-        GND_PERSON_MAP = {config.DIRECT: {'uri': 'id',
-                              'label': 'label'}}
-        
-        VIAF_PERSON_MAP = {config.RESULT: 'result',
-                           config.FILTER: {'nametype': 'personal'},
-                           config.DIRECT: {'label': 'displayForm'},
-                           config.RULES: {'uri': {config.RULE: '"http://www.viaf.org/viaf/{p1}"',
-                                                  config.FIELDS: {'p1': 'viafid'}}}}
-        
-        GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
-                             config.QUERY_FIELD: 'q',
-                             config.PAYLOAD: {'format':'json:suggest',
-                                              'filter': 'type:Person'}}
-        
-        VIAF_PERSON_SOURCE =  {config.URL: 'http://www.viaf.org/viaf/AutoSuggest',
-                               config.QUERY_FIELD: 'query'}
-        
-        
-        gnd = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
-        viaf = APIMapper(VIAF_PERSON_SOURCE, VIAF_PERSON_MAP)
-        apis = [gnd, viaf]
-        results = []
-        for api in apis:
-            res = api.fetch_results('Pratchett')
-            results.extend(res)
-        
-        print(results)
-        ```
-        
-        * Using mapping rules
-        
-        Splitting the GND label field into meaningful subparts
-        ```
-        from apimapper import APIMapper
-        from apimapper import config
-        
-        GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
-                             config.QUERY_FIELD: 'q',
-                             config.PAYLOAD: {'format':'json:suggest',
-                                              'filter': 'type:Person'}}
-        
-        GND_PERSON_MAP = {config.DIRECT: {'label': 'label',
-                                          'uri': 'id'},
-                  config.RULES: {'source': {config.RULE: '"GND"'},
-                                 'label_name': {config.RULE: '"{p1}".split("|")[0].strip()',
-                                                        config.FIELDS: {'p1': 'label'}},
-                                         'label_year': {config.RULE: '"{p1}".split("|")[1].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else ""',
-                                                    config.FIELDS: {'p1': 'label'}},
-                                             'label_profession': {config.RULE: '"{p1}".split("|")[2].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else "{p1}".split("|")[1].strip()',
-                                                                  config.FIELDS: {'p1': 'label'}}}}
-        
-        api = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
-        res = api.fetch_results('Rosalind Franklin')
-        ```
-        
-        * More example usage in apimapper/demo
-        
 Keywords: API Mapper
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# API Wrapper
+
+## Install package
+* from PyPi:
+    pip install apimapper
+* from source:
+    pip install -e .
+
+## Unit Testing
+   >pytest
+
+## Usage
+
+* See https://github.com/acdh-oeaw/apimapper/blob/develop/demo/APIMapper%20Demo.ipynb
+* Multiple APIs (GND and VIAF) mapped to a common JSON schema
+
+VIAF only returns VIAF ID - which is contructed into a url using a "rule"
+```
+from apimapper import APIMapper
+from apimapper import config
+
+GND_PERSON_MAP = {config.DIRECT: {'uri': 'id',
+                      'label': 'label'}}
+
+VIAF_PERSON_MAP = {config.RESULT: 'result',
+                   config.FILTER: {'nametype': 'personal'},
+                   config.DIRECT: {'label': 'displayForm'},
+                   config.RULES: {'uri': {config.RULE: '"http://www.viaf.org/viaf/{p1}"',
+                                          config.FIELDS: {'p1': 'viafid'}}}}
+
+GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
+                     config.QUERY_FIELD: 'q',
+                     config.PAYLOAD: {'format':'json:suggest',
+                                      'filter': 'type:Person'}}
+
+VIAF_PERSON_SOURCE =  {config.URL: 'http://www.viaf.org/viaf/AutoSuggest',
+                       config.QUERY_FIELD: 'query'}
+
+
+gnd = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
+viaf = APIMapper(VIAF_PERSON_SOURCE, VIAF_PERSON_MAP)
+apis = [gnd, viaf]
+results = []
+for api in apis:
+    res = api.fetch_results('Pratchett')
+    results.extend(res)
+
+print(results)
+```
+
+* Using mapping rules
+
+Splitting the GND label field into meaningful subparts
+```
+from apimapper import APIMapper
+from apimapper import config
+
+GND_PERSON_SOURCE = {config.URL: 'https://lobid.org/gnd/search',
+                     config.QUERY_FIELD: 'q',
+                     config.PAYLOAD: {'format':'json:suggest',
+                                      'filter': 'type:Person'}}
+
+GND_PERSON_MAP = {config.DIRECT: {'label': 'label',
+                                  'uri': 'id'},
+          config.RULES: {'source': {config.RULE: '"GND"'},
+                         'label_name': {config.RULE: '"{p1}".split("|")[0].strip()',
+                                                config.FIELDS: {'p1': 'label'}},
+                                 'label_year': {config.RULE: '"{p1}".split("|")[1].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else ""',
+                                            config.FIELDS: {'p1': 'label'}},
+                                     'label_profession': {config.RULE: '"{p1}".split("|")[2].strip() if "{p1}".split("|")[1].strip()[0].isnumeric() else "{p1}".split("|")[1].strip()',
+                                                          config.FIELDS: {'p1': 'label'}}}}
+
+api = APIMapper(GND_PERSON_SOURCE, GND_PERSON_MAP)
+res = api.fetch_results('Rosalind Franklin')
+```
+
+* More example usage in apimapper/demo
```

