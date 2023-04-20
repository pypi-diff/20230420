# Comparing `tmp/python-blockbee-checkout-1.0.0.tar.gz` & `tmp/python-blockbee-checkout-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-blockbee-checkout-1.0.0.tar", last modified: Tue Jan 31 09:40:46 2023, max compression
+gzip compressed data, was "python-blockbee-checkout-1.0.1.tar", last modified: Thu Apr 20 14:22:35 2023, max compression
```

## Comparing `python-blockbee-checkout-1.0.0.tar` & `python-blockbee-checkout-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:40:46.718266 python-blockbee-checkout-1.0.0/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-30 18:34:25.000000 python-blockbee-checkout-1.0.0/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3366 2023-01-31 09:40:46.718158 python-blockbee-checkout-1.0.0/PKG-INFO
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-01-31 09:40:46.717985 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3366 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)      302 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-01-31 09:40:46.718303 python-blockbee-checkout-1.0.0/setup.cfg
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1037 2023-01-30 18:10:08.000000 python-blockbee-checkout-1.0.0/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.008952 python-blockbee-checkout-1.0.1/
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.007983 python-blockbee-checkout-1.0.1/BlockBee/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2570 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/BlockBee/BlockBeeCheckout.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       52 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/BlockBee/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-30 18:34:25.000000 python-blockbee-checkout-1.0.1/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3453 2023-04-20 14:22:35.008853 python-blockbee-checkout-1.0.1/PKG-INFO
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.008688 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3453 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      352 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-04-20 14:22:35.008988 python-blockbee-checkout-1.0.1/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1037 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/setup.py
```

### Comparing `python-blockbee-checkout-1.0.0/LICENSE` & `python-blockbee-checkout-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-blockbee-checkout-1.0.0/PKG-INFO` & `python-blockbee-checkout-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee-checkout
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Library for BlockBee Checkout
 Home-page: https://github.com/blockbee-io/python-blockbee-checkout
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,23 +41,23 @@
 [on GitHub](https://github.com/blockbee-io/python-blockbee-checkout)
 
 ## Usage
 
 ### Importing in your project file
 
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 ```
 
 ### Generate a Payment Checkout page
 
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 
-bb = BlockBeeCheckout.Helper(api_key, params, bb_params)
+bb = BlockBeeCheckoutHelper(api_key, params, bb_params)
 
 payment_page = bb.payment_request(redirect_url, value)
 ```
 
 Where:
 
 * ``api_key`` is the API Key provided by our [Dashboard](https://dash.blockbee.io/).
@@ -67,17 +67,17 @@
 * ``value`` amount in currency set in Payment Settings you want to receive from the user.
 
 ### Getting notified when the user completes the Payment
 > When receiving payments, you have the option to receive them in either the ``notify_url`` or the ``redirect_url``, but adding the ``redirect_url``  is required (refer to our documentation at https://docs.blockbee.io/#operation/paymentipn).
 
 ### Requesting Deposit
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 
-bb = BlockBeeCheckout.Helper(api_key, params, bb_params)
+bb = BlockBeeCheckoutHelper(api_key, params, bb_params)
 
 deposit_page = bb.deposit_request(notify_url)
 ```
 * ``api_key`` is the API Key provided by our [Dashboard](https://dash.blockbee.io/).
 * ``params`` is any parameter you wish to send to identify the payment, such as `{'order_id': 1234}`.
 * ``bb_params`` parameters that will be passed to BlockBee _(check which extra parameters are available here: https://docs.blockbee.io/#operation/deposit).
 * ``notify_url`` URL in your platform, where the IPN will be sent notifying that a deposit was done. Parameters are available here: https://docs.blockbee.io/#operation/depositipn.
@@ -91,7 +91,10 @@
 Contact us @ https://blockbee.io/contacts/
 
 
 ### Changelog
 
 #### 1.0.0
 * Initial Release
+
+#### 1.0.1
+* Minor bugfixes
```

### Comparing `python-blockbee-checkout-1.0.0/python_blockbee_checkout.egg-info/PKG-INFO` & `python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee-checkout
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Library for BlockBee Checkout
 Home-page: https://github.com/blockbee-io/python-blockbee-checkout
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,23 +41,23 @@
 [on GitHub](https://github.com/blockbee-io/python-blockbee-checkout)
 
 ## Usage
 
 ### Importing in your project file
 
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 ```
 
 ### Generate a Payment Checkout page
 
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 
-bb = BlockBeeCheckout.Helper(api_key, params, bb_params)
+bb = BlockBeeCheckoutHelper(api_key, params, bb_params)
 
 payment_page = bb.payment_request(redirect_url, value)
 ```
 
 Where:
 
 * ``api_key`` is the API Key provided by our [Dashboard](https://dash.blockbee.io/).
@@ -67,17 +67,17 @@
 * ``value`` amount in currency set in Payment Settings you want to receive from the user.
 
 ### Getting notified when the user completes the Payment
 > When receiving payments, you have the option to receive them in either the ``notify_url`` or the ``redirect_url``, but adding the ``redirect_url``  is required (refer to our documentation at https://docs.blockbee.io/#operation/paymentipn).
 
 ### Requesting Deposit
 ```python
-import BlockBeeCheckout
+from BlockBee import BlockBeeCheckoutHelper
 
-bb = BlockBeeCheckout.Helper(api_key, params, bb_params)
+bb = BlockBeeCheckoutHelper(api_key, params, bb_params)
 
 deposit_page = bb.deposit_request(notify_url)
 ```
 * ``api_key`` is the API Key provided by our [Dashboard](https://dash.blockbee.io/).
 * ``params`` is any parameter you wish to send to identify the payment, such as `{'order_id': 1234}`.
 * ``bb_params`` parameters that will be passed to BlockBee _(check which extra parameters are available here: https://docs.blockbee.io/#operation/deposit).
 * ``notify_url`` URL in your platform, where the IPN will be sent notifying that a deposit was done. Parameters are available here: https://docs.blockbee.io/#operation/depositipn.
@@ -91,7 +91,10 @@
 Contact us @ https://blockbee.io/contacts/
 
 
 ### Changelog
 
 #### 1.0.0
 * Initial Release
+
+#### 1.0.1
+* Minor bugfixes
```

### Comparing `python-blockbee-checkout-1.0.0/setup.py` & `python-blockbee-checkout-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 
     name='python-blockbee-checkout',
 
-    version='1.0.0',
+    version='1.0.1',
 
     packages=find_packages(),
 
     author="BlockBee",
 
     author_email="info@blockbee.io",
     install_requires=[
```

