# Comparing `tmp/tarvis-btb-0.9.0.tar.gz` & `tmp/tarvis-btb-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-btb-0.9.0.tar", last modified: Mon Apr 17 16:56:59 2023, max compression
+gzip compressed data, was "tarvis-btb-0.9.1.tar", last modified: Thu Apr 20 20:29:56 2023, max compression
```

## Comparing `tarvis-btb-0.9.0.tar` & `tarvis-btb-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:56:59.176821 tarvis-btb-0.9.0/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/tarvis/btb/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/tarvis/btb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24291 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/tarvis/btb/basictradingbot.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/tarvis/btb/btbs.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/tarvis/btb/exchangeaccount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/tarvis_btb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      397 2023-04-17 16:56:59.000000 tarvis-btb-0.9.0/tarvis_btb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-17 16:56:59.000000 tarvis-btb-0.9.0/tarvis_btb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:56:59.000000 tarvis-btb-0.9.0/tarvis_btb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 16:56:59.000000 tarvis-btb-0.9.0/tarvis_btb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-17 16:56:59.000000 tarvis-btb-0.9.0/tarvis_btb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:56:59.180821 tarvis-btb-0.9.0/test/
--rw-r--r--   0 root         (0) root         (0)     3152 2023-04-17 16:56:47.000000 tarvis-btb-0.9.0/test/test_all.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:29:56.081651 tarvis-btb-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-20 20:29:56.077651 tarvis-btb-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 20:29:56.081651 tarvis-btb-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:29:56.077651 tarvis-btb-0.9.1/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:29:56.077651 tarvis-btb-0.9.1/tarvis/btb/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/tarvis/btb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24425 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/tarvis/btb/basictradingbot.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/tarvis/btb/btbs.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/tarvis/btb/exchangeaccount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:29:56.077651 tarvis-btb-0.9.1/tarvis_btb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-04-20 20:29:56.000000 tarvis-btb-0.9.1/tarvis_btb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-20 20:29:56.000000 tarvis-btb-0.9.1/tarvis_btb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 20:29:56.000000 tarvis-btb-0.9.1/tarvis_btb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-20 20:29:56.000000 tarvis-btb-0.9.1/tarvis_btb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-20 20:29:56.000000 tarvis-btb-0.9.1/tarvis_btb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 20:29:56.077651 tarvis-btb-0.9.1/test/
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-20 20:29:47.000000 tarvis-btb-0.9.1/test/test_all.py
```

### Comparing `tarvis-btb-0.9.0/LICENSE.txt` & `tarvis-btb-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.0/setup.py` & `tarvis-btb-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-btb",
-    version="0.9.0",
+    version="0.9.1",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Basic Trading Bot Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-btb-0.9.0/tarvis/btb/basictradingbot.py` & `tarvis-btb-0.9.1/tarvis/btb/basictradingbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,22 +201,23 @@
                     elif order.order_type == OrderType.LIMIT:
                         direction_vector += order_vector
                     elif order.order_type == OrderType.STOP_LOSS_MARKET:
                         stop_loss_orders.append(order)
                         stop_loss_vector += order_vector
 
                 if cancel_order:
+                    # noinspection PyProtectedMember
                     self._logger.info(
                         "Cancelling order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order.side.name,
-                            "order_type": order.order_type,
-                            "order_quantity": order._quantity,  # noqa
-                            "order_amount": order._amount,  # noqa
+                            "order_type": order.order_type.name,
+                            "order_quantity": str(order._quantity),
+                            "order_amount": str(order._amount),
                         },
                     )
                     exchange.cancel_order(order)
 
         opposing_position = base_asset_position + flatten_vector
         match indicator.direction:
             case MarketPosition.LONG:
@@ -234,15 +235,15 @@
             else:
                 flatten_order_side = OrderSide.BUY
             self._logger.info(
                 "Placing flattening order.",
                 extra={
                     **log_extra_iteration,
                     "order_side": flatten_order_side.name,
-                    "order_quantity": flatten_quantity,
+                    "order_quantity": str(flatten_quantity),
                 },
             )
             exchange.place_order(
                 trading_policy,
                 base_asset,
                 quote_asset,
                 flatten_order_side,
@@ -355,17 +356,17 @@
                         order_quantity
                     )
                     self._logger.info(
                         "Placing directional order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order_side.name,
-                            "order_quantity": order_quantity,
-                            "order_price": order_price,
-                            "order_amount": order_quantity * order_price,
+                            "order_quantity": str(order_quantity),
+                            "order_price": str(order_price),
+                            "order_amount": str(order_quantity * order_price),
                         },
                     )
                     exchange.place_order(
                         trading_policy,
                         base_asset,
                         quote_asset,
                         order_side,
@@ -406,22 +407,23 @@
 
                 stop_loss_completed = (not stop_loss_excessive) and (
                     stop_loss_quantity < minimum_order_quantity
                 )
 
                 if stop_loss_excessive:
                     order = stop_loss_orders.pop()
+                    # noinspection PyProtectedMember
                     self._logger.info(
                         "Cancelling excessive stop-loss order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order.side.name,
-                            "order_type": order.order_type,
-                            "order_quantity": order._quantity,  # noqa
-                            "order_amount": order._amount,  # noqa
+                            "order_type": order.order_type.name,
+                            "order_quantity": str(order._quantity),
+                            "order_amount": str(order._amount),
                         },
                     )
                     exchange.cancel_order(order)
 
                 elif stop_loss_quantity >= minimum_order_quantity:
                     stop_loss_price = quote_price * stop_loss_price_ratio
                     stop_loss_price = trading_policy.align_price(stop_loss_price)
@@ -429,16 +431,16 @@
                         stop_loss_quantity
                     )
                     self._logger.info(
                         "Placing stop loss order.",
                         extra={
                             **log_extra_iteration,
                             "order_side": order_side_opposing.name,
-                            "order_quantity": stop_loss_quantity,
-                            "order_price": stop_loss_price,
+                            "order_quantity": str(stop_loss_quantity),
+                            "order_price": str(stop_loss_price),
                         },
                     )
                     exchange.place_order(
                         trading_policy,
                         base_asset,
                         quote_asset,
                         order_side_opposing,
```

### Comparing `tarvis-btb-0.9.0/tarvis/btb/btbs.py` & `tarvis-btb-0.9.1/tarvis/btb/btbs.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.0/tarvis/btb/exchangeaccount.py` & `tarvis-btb-0.9.1/tarvis/btb/exchangeaccount.py`

 * *Files identical despite different names*

### Comparing `tarvis-btb-0.9.0/test/test_all.py` & `tarvis-btb-0.9.1/test/test_all.py`

 * *Files identical despite different names*

