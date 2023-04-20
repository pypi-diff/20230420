# Comparing `tmp/zscaler_api_talkers-4.0.0.tar.gz` & `tmp/zscaler_api_talkers-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_api_talkers-4.0.0.tar", last modified: Wed Apr  5 17:10:56 2023, max compression
+gzip compressed data, was "zscaler_api_talkers-4.0.1.tar", last modified: Thu Apr 20 16:54:51 2023, max compression
```

## Comparing `zscaler_api_talkers-4.0.0.tar` & `zscaler_api_talkers-4.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.886240 zscaler_api_talkers-4.0.0/
--rw-r--r--   0 spereira   (501) staff       (20)     1071 2022-04-21 16:27:44.000000 zscaler_api_talkers-4.0.0/LICENSE.txt
--rw-r--r--   0 spereira   (501) staff       (20)     2941 2023-04-05 17:10:56.885924 zscaler_api_talkers-4.0.0/PKG-INFO
--rw-r--r--   0 spereira   (501) staff       (20)     2593 2023-04-04 21:03:06.000000 zscaler_api_talkers-4.0.0/README.md
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.878069 zscaler_api_talkers-4.0.0/models/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.0/models/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)    14364 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.0/models/models.py
--rw-r--r--   0 spereira   (501) staff       (20)       84 2022-04-21 20:33:36.000000 zscaler_api_talkers-4.0.0/pyproject.toml
--rw-r--r--   0 spereira   (501) staff       (20)       38 2023-04-05 17:10:56.886323 zscaler_api_talkers-4.0.0/setup.cfg
--rw-r--r--   0 spereira   (501) staff       (20)      568 2023-04-04 21:10:18.000000 zscaler_api_talkers-4.0.0/setup.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.879243 zscaler_api_talkers-4.0.0/zcc_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.0/zcc_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     4747 2023-04-05 17:08:58.000000 zscaler_api_talkers-4.0.0/zcc_talker/zcc_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.880945 zscaler_api_talkers-4.0.0/zia_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 02:12:49.000000 zscaler_api_talkers-4.0.0/zia_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)    14177 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.0/zia_talker/zia_portaltalker.py
--rw-r--r--   0 spereira   (501) staff       (20)    66881 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.0/zia_talker/zia_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.883106 zscaler_api_talkers-4.0.0/zpa_talker/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.0/zpa_talker/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     2369 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.0/zpa_talker/zpa_portaltalker.py
--rw-r--r--   0 spereira   (501) staff       (20)    20237 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.0/zpa_talker/zpa_talker.py
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.885100 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/
--rw-r--r--   0 spereira   (501) staff       (20)     2941 2023-04-05 17:10:56.000000 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/PKG-INFO
--rw-r--r--   0 spereira   (501) staff       (20)      559 2023-04-05 17:10:56.000000 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/SOURCES.txt
--rw-r--r--   0 spereira   (501) staff       (20)        1 2023-04-05 17:10:56.000000 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/dependency_links.txt
--rw-r--r--   0 spereira   (501) staff       (20)       25 2023-04-05 17:10:56.000000 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/requires.txt
--rw-r--r--   0 spereira   (501) staff       (20)       56 2023-04-05 17:10:56.000000 zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/top_level.txt
-drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-05 17:10:56.885589 zscaler_api_talkers-4.0.0/zscaler_helpers/
--rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.0/zscaler_helpers/__init__.py
--rw-r--r--   0 spereira   (501) staff       (20)     7203 2023-04-04 18:41:17.000000 zscaler_api_talkers-4.0.0/zscaler_helpers/http_calls.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.044587 zscaler_api_talkers-4.0.1/
+-rw-r--r--   0 spereira   (501) staff       (20)     1071 2022-04-21 16:27:44.000000 zscaler_api_talkers-4.0.1/LICENSE.txt
+-rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-20 16:54:51.044207 zscaler_api_talkers-4.0.1/PKG-INFO
+-rw-r--r--   0 spereira   (501) staff       (20)     2683 2023-04-19 16:20:53.000000 zscaler_api_talkers-4.0.1/README.md
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.033077 zscaler_api_talkers-4.0.1/models/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/models/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)    14364 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/models/models.py
+-rw-r--r--   0 spereira   (501) staff       (20)       84 2022-04-21 20:33:36.000000 zscaler_api_talkers-4.0.1/pyproject.toml
+-rw-r--r--   0 spereira   (501) staff       (20)       38 2023-04-20 16:54:51.044690 zscaler_api_talkers-4.0.1/setup.cfg
+-rw-r--r--   0 spereira   (501) staff       (20)      568 2023-04-07 21:48:18.000000 zscaler_api_talkers-4.0.1/setup.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.034284 zscaler_api_talkers-4.0.1/zcc_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zcc_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     4747 2023-04-05 17:08:58.000000 zscaler_api_talkers-4.0.1/zcc_talker/zcc_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.037046 zscaler_api_talkers-4.0.1/zia_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 02:12:49.000000 zscaler_api_talkers-4.0.1/zia_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)    15297 2023-04-20 16:51:44.000000 zscaler_api_talkers-4.0.1/zia_talker/zia_portaltalker.py
+-rw-r--r--   0 spereira   (501) staff       (20)    66881 2023-04-14 15:49:45.000000 zscaler_api_talkers-4.0.1/zia_talker/zia_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.040067 zscaler_api_talkers-4.0.1/zpa_talker/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zpa_talker/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     2369 2023-04-05 17:08:09.000000 zscaler_api_talkers-4.0.1/zpa_talker/zpa_portaltalker.py
+-rw-r--r--   0 spereira   (501) staff       (20)    20237 2023-04-19 16:14:30.000000 zscaler_api_talkers-4.0.1/zpa_talker/zpa_talker.py
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.042693 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/
+-rw-r--r--   0 spereira   (501) staff       (20)     3031 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/PKG-INFO
+-rw-r--r--   0 spereira   (501) staff       (20)      559 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/SOURCES.txt
+-rw-r--r--   0 spereira   (501) staff       (20)        1 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/dependency_links.txt
+-rw-r--r--   0 spereira   (501) staff       (20)       25 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/requires.txt
+-rw-r--r--   0 spereira   (501) staff       (20)       56 2023-04-20 16:54:50.000000 zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/top_level.txt
+drwxr-xr-x   0 spereira   (501) staff       (20)        0 2023-04-20 16:54:51.043375 zscaler_api_talkers-4.0.1/zscaler_helpers/
+-rw-r--r--   0 spereira   (501) staff       (20)        0 2022-12-14 01:53:08.000000 zscaler_api_talkers-4.0.1/zscaler_helpers/__init__.py
+-rw-r--r--   0 spereira   (501) staff       (20)     7203 2023-04-19 03:45:34.000000 zscaler_api_talkers-4.0.1/zscaler_helpers/http_calls.py
```

### Comparing `zscaler_api_talkers-4.0.0/LICENSE.txt` & `zscaler_api_talkers-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/PKG-INFO` & `zscaler_api_talkers-4.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler_api_talkers
-Version: 4.0.0
+Version: 4.0.1
 Summary: Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC
 Home-page: https://github.com/sergitopereira/zscaler_api_talkers.git
 Author: Sergio Pereira
 Author-email: sergitopereira@hotmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -49,22 +49,22 @@
   source .zs_api_talkers/bin/activate
   # Windows
   .\.zs_api_talkers\Scripts\activate
 * Install Zscales API talkers
    pip install zscaler-api-talkers  
 ```
 
-# ZIA Talker
+# Zscaler Secure Internet and SaaS Access SDK (zia_talker)
 
 ## Usage zia_talker
 ``` python
 from zia_talker.zia_talker import ZiaTalker
-a=ZiaTalker('<Zscaler Cloud Name>')
-a.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
-a.list_url_categorie.url_categories()
+zia=ZiaTalker('<Zscaler Cloud Name>')
+zia.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
+zia.list_urlcategories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 ## Usage zia_talker with OAUTH2.0
 ``` python
@@ -73,25 +73,25 @@
 a.list_url_categorie.url_categories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 
-# ZPA Talker
+# Zscaler Secure Private Access SDK (zpa_talker)
 
 ## Usage zpa_talker
 ``` python
 from zpa_talker.zpa_talker import ZpaTalker
 a=ZpaTalker('customerID')
 a.authenticate(client_id='clientID',client_secret='clientSecret')
 # To view all methods available
 print(dir(a))
 ```
-# ZCC talker
+# Zscaler Client Connector SDK  (zcc_talker)
 
 ## Usage zcc_talker
 ``` python
 from zcc_talker.zcc_talker import ZccTalker
 a=ZccTalker('<Zscaler Cloud Name>')    
 a.authenticate(clientid='clientID',secretkey='clientSecret')
 a.list_devices('companyID')
@@ -107,13 +107,13 @@
 # Bugs and enhancements
 
 Feel free to open an issues using [Gihub Issues](https://github.com/sergitopereira/zscaler_api_talkers)
 
 
 # Author
 
-Sergio Augusto Pereira Alarcon
+Sergio Pereira 
 
 Zscaler Professional Services
```

### Comparing `zscaler_api_talkers-4.0.0/README.md` & `zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: zscaler-api-talkers
+Version: 4.0.1
+Summary: Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC
+Home-page: https://github.com/sergitopereira/zscaler_api_talkers.git
+Author: Sergio Pereira
+Author-email: sergitopereira@hotmail.com
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Unofficial Zscaler API talkers
 
 ### ZIA API Talker
 Python client to leverage  [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
 ### ZPA API Talker
 Python client to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
@@ -38,22 +49,22 @@
   source .zs_api_talkers/bin/activate
   # Windows
   .\.zs_api_talkers\Scripts\activate
 * Install Zscales API talkers
    pip install zscaler-api-talkers  
 ```
 
-# ZIA Talker
+# Zscaler Secure Internet and SaaS Access SDK (zia_talker)
 
 ## Usage zia_talker
 ``` python
 from zia_talker.zia_talker import ZiaTalker
-a=ZiaTalker('<Zscaler Cloud Name>')
-a.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
-a.list_url_categorie.url_categories()
+zia=ZiaTalker('<Zscaler Cloud Name>')
+zia.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
+zia.list_urlcategories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 ## Usage zia_talker with OAUTH2.0
 ``` python
@@ -62,25 +73,25 @@
 a.list_url_categorie.url_categories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 
-# ZPA Talker
+# Zscaler Secure Private Access SDK (zpa_talker)
 
 ## Usage zpa_talker
 ``` python
 from zpa_talker.zpa_talker import ZpaTalker
 a=ZpaTalker('customerID')
 a.authenticate(client_id='clientID',client_secret='clientSecret')
 # To view all methods available
 print(dir(a))
 ```
-# ZCC talker
+# Zscaler Client Connector SDK  (zcc_talker)
 
 ## Usage zcc_talker
 ``` python
 from zcc_talker.zcc_talker import ZccTalker
 a=ZccTalker('<Zscaler Cloud Name>')    
 a.authenticate(clientid='clientID',secretkey='clientSecret')
 a.list_devices('companyID')
@@ -96,13 +107,13 @@
 # Bugs and enhancements
 
 Feel free to open an issues using [Gihub Issues](https://github.com/sergitopereira/zscaler_api_talkers)
 
 
 # Author
 
-Sergio Augusto Pereira Alarcon
+Sergio Pereira 
 
 Zscaler Professional Services
```

### Comparing `zscaler_api_talkers-4.0.0/models/models.py` & `zscaler_api_talkers-4.0.1/models/models.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/setup.py` & `zscaler_api_talkers-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zscaler_api_talkers',
-    version='4.0.0',
+    version='4.0.1',
     author='Sergio Pereira',
     author_email='sergitopereira@hotmail.com',
     packages=find_packages(),
     url='https://github.com/sergitopereira/zscaler_api_talkers.git',
     license='LICENSE.txt',
     description='Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC',
     long_description_content_type="text/markdown",
```

### Comparing `zscaler_api_talkers-4.0.0/zcc_talker/zcc_talker.py` & `zscaler_api_talkers-4.0.1/zcc_talker/zcc_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/zia_talker/zia_portaltalker.py` & `zscaler_api_talkers-4.0.1/zia_talker/zia_portaltalker.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,8 +327,34 @@
         :return: json
         """
         url = f'/apiKeys'
         response = self.hp_http.get_call(url=url, headers=self.headers,
                                          cookies={'JSESSIONID': self.jsessionid,
                                                   'ZS_SESSION_CODE': self.zs_session_code,
                                                   })
-        return response.json()
+        return response.json()
+
+    def delete_group(self, groupid):
+        """
+        Method to delete a group given group id
+        :param groupid: type int. Group id
+        :return: HTTP response
+        """
+        url = f'/groups/{groupid}'
+        response = self.hp_http.delete_call(url=url, headers=self.headers,
+                                         cookies={'JSESSIONID': self.jsessionid,
+                                                  'ZS_SESSION_CODE': self.zs_session_code,
+                                                  })
+        return response
+
+    def delete_department(self, departmentid):
+        """
+        Method to delete a group given department
+        :param departmentid: type int. Departmentid id
+        :return: HTTP response
+        """
+        url = f'/departments/{departmentid}'
+        response = self.hp_http.delete_call(url=url, headers=self.headers,
+                                         cookies={'JSESSIONID': self.jsessionid,
+                                                  'ZS_SESSION_CODE': self.zs_session_code,
+                                                  })
+        return response
```

### Comparing `zscaler_api_talkers-4.0.0/zia_talker/zia_talker.py` & `zscaler_api_talkers-4.0.1/zia_talker/zia_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/zpa_talker/zpa_portaltalker.py` & `zscaler_api_talkers-4.0.1/zpa_talker/zpa_portaltalker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/zpa_talker/zpa_talker.py` & `zscaler_api_talkers-4.0.1/zpa_talker/zpa_talker.py`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/PKG-INFO` & `zscaler_api_talkers-4.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: zscaler-api-talkers
-Version: 4.0.0
-Summary: Unofficial Zscaler API python SDK for ZIA, ZPA and ZCC
-Home-page: https://github.com/sergitopereira/zscaler_api_talkers.git
-Author: Sergio Pereira
-Author-email: sergitopereira@hotmail.com
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Unofficial Zscaler API talkers
 
 ### ZIA API Talker
 Python client to leverage  [Zscaler Internet Access API](https://help.zscaler.com/zia/api)
 
 ### ZPA API Talker
 Python client to leverage [Zscaler Private Access API](https://help.zscaler.com/zpa/api-reference)
@@ -49,22 +38,22 @@
   source .zs_api_talkers/bin/activate
   # Windows
   .\.zs_api_talkers\Scripts\activate
 * Install Zscales API talkers
    pip install zscaler-api-talkers  
 ```
 
-# ZIA Talker
+# Zscaler Secure Internet and SaaS Access SDK (zia_talker)
 
 ## Usage zia_talker
 ``` python
 from zia_talker.zia_talker import ZiaTalker
-a=ZiaTalker('<Zscaler Cloud Name>')
-a.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
-a.list_url_categorie.url_categories()
+zia=ZiaTalker('<Zscaler Cloud Name>')
+zia.authenticate(apikey='API_KEY', username='USERNAME', password='PASSWORD')
+zia.list_urlcategories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 ## Usage zia_talker with OAUTH2.0
 ``` python
@@ -73,25 +62,25 @@
 a.list_url_categorie.url_categories()
 a.list_users()
 # To view all methods available
 print(dir(a))
 ```
 
 
-# ZPA Talker
+# Zscaler Secure Private Access SDK (zpa_talker)
 
 ## Usage zpa_talker
 ``` python
 from zpa_talker.zpa_talker import ZpaTalker
 a=ZpaTalker('customerID')
 a.authenticate(client_id='clientID',client_secret='clientSecret')
 # To view all methods available
 print(dir(a))
 ```
-# ZCC talker
+# Zscaler Client Connector SDK  (zcc_talker)
 
 ## Usage zcc_talker
 ``` python
 from zcc_talker.zcc_talker import ZccTalker
 a=ZccTalker('<Zscaler Cloud Name>')    
 a.authenticate(clientid='clientID',secretkey='clientSecret')
 a.list_devices('companyID')
@@ -107,13 +96,13 @@
 # Bugs and enhancements
 
 Feel free to open an issues using [Gihub Issues](https://github.com/sergitopereira/zscaler_api_talkers)
 
 
 # Author
 
-Sergio Augusto Pereira Alarcon
+Sergio Pereira 
 
 Zscaler Professional Services
```

### Comparing `zscaler_api_talkers-4.0.0/zscaler_api_talkers.egg-info/SOURCES.txt` & `zscaler_api_talkers-4.0.1/zscaler_api_talkers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zscaler_api_talkers-4.0.0/zscaler_helpers/http_calls.py` & `zscaler_api_talkers-4.0.1/zscaler_helpers/http_calls.py`

 * *Files identical despite different names*

