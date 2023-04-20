# Comparing `tmp/aliyun-python-sdk-cas-2020.4.7.tar.gz` & `tmp/aliyun-python-sdk-cas-2020.6.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cas-2020.4.7.tar", last modified: Wed Apr 15 07:27:47 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cas-2020.6.23.tar", last modified: Tue Jun 23 11:21:38 2020, max compression
```

## Comparing `aliyun-python-sdk-cas-2020.4.7.tar` & `aliyun-python-sdk-cas-2020.6.23.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/
--rw-rw-r--   0 admin      (531) admin      (531)        1 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/dependency_links.txt
--rw-rw-r--   0 admin      (531) admin      (531)       31 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/requires.txt
--rw-rw-r--   0 admin      (531) admin      (531)      641 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/SOURCES.txt
--rw-rw-r--   0 admin      (531) admin      (531)       13 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/top_level.txt
--rw-rw-r--   0 admin      (531) admin      (531)     1540 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/PKG-INFO
--rw-rw-r--   0 admin      (531) admin      (531)       38 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/setup.cfg
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/
--rw-rw-r--   0 admin      (531) admin      (531)       26 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     3229 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/endpoint.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/__init__.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     2062 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/CreateCertificateRequestRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1440 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/DeleteCertificateRequestRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1278 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/DescribePackageStateRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1440 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/DescribeCertificateStateRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2452 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/setup.py
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/MANIFEST.in
--rw-rw-r--   0 admin      (531) admin      (531)      527 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/README.rst
--rw-rw-r--   0 admin      (531) admin      (531)     1540 2020-04-15 07:27:47.000000 aliyun-python-sdk-cas-2020.4.7/PKG-INFO
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/
+-rw-rw-r--   0 admin      (531) admin      (531)        1 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       31 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/requires.txt
+-rw-rw-r--   0 admin      (531) admin      (531)      641 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin      (531) admin      (531)       13 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/top_level.txt
+-rw-rw-r--   0 admin      (531) admin      (531)     1541 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/PKG-INFO
+-rw-rw-r--   0 admin      (531) admin      (531)       38 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/setup.cfg
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/
+-rw-rw-r--   0 admin      (531) admin      (531)       26 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     3229 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/endpoint.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/__init__.py
+drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/__init__.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2240 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/CreateCertificateRequestRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1440 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/DeleteCertificateRequestRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1456 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/DescribePackageStateRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     1440 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/DescribeCertificateStateRequest.py
+-rw-rw-r--   0 admin      (531) admin      (531)     2452 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/setup.py
+-rw-rw-r--   0 admin      (531) admin      (531)        0 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/MANIFEST.in
+-rw-rw-r--   0 admin      (531) admin      (531)      527 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/README.rst
+-rw-rw-r--   0 admin      (531) admin      (531)     1541 2020-06-23 11:21:38.000000 aliyun-python-sdk-cas-2020.6.23/PKG-INFO
```

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/SOURCES.txt` & `aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyun_python_sdk_cas.egg-info/PKG-INFO` & `aliyun-python-sdk-cas-2020.6.23/aliyun_python_sdk_cas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cas
-Version: 2020.4.7
+Version: 2020.6.23
 Summary: The cas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cas
```

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/endpoint.py` & `aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/CreateCertificateRequestRequest.py` & `aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/CreateCertificateRequestRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,36 +27,42 @@
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
+	def get_ProductCode(self):
+		return self.get_query_params().get('ProductCode')
+
+	def set_ProductCode(self,ProductCode):
+		self.add_query_param('ProductCode',ProductCode)
+
 	def get_ValidateType(self):
 		return self.get_query_params().get('ValidateType')
 
 	def set_ValidateType(self,ValidateType):
 		self.add_query_param('ValidateType',ValidateType)
 
+	def get_Email(self):
+		return self.get_query_params().get('Email')
+
+	def set_Email(self,Email):
+		self.add_query_param('Email',Email)
+
 	def get_Phone(self):
 		return self.get_query_params().get('Phone')
 
 	def set_Phone(self,Phone):
 		self.add_query_param('Phone',Phone)
 
 	def get_Domain(self):
 		return self.get_query_params().get('Domain')
 
 	def set_Domain(self,Domain):
 		self.add_query_param('Domain',Domain)
 
-	def get_Email(self):
-		return self.get_query_params().get('Email')
-
-	def set_Email(self,Email):
-		self.add_query_param('Email',Email)
-
 	def get_Username(self):
 		return self.get_query_params().get('Username')
 
 	def set_Username(self,Username):
 		self.add_query_param('Username',Username)
```

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/DeleteCertificateRequestRequest.py` & `aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/DeleteCertificateRequestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/aliyunsdkcas/request/v20200407/DescribeCertificateStateRequest.py` & `aliyun-python-sdk-cas-2020.6.23/aliyunsdkcas/request/v20200407/DescribeCertificateStateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/setup.py` & `aliyun-python-sdk-cas-2020.6.23/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/README.rst` & `aliyun-python-sdk-cas-2020.6.23/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cas-2020.4.7/PKG-INFO` & `aliyun-python-sdk-cas-2020.6.23/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cas
-Version: 2020.4.7
+Version: 2020.6.23
 Summary: The cas module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cas
```

