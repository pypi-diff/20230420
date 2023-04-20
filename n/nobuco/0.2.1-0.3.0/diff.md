# Comparing `tmp/nobuco-0.2.1.tar.gz` & `tmp/nobuco-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.2.1.tar", last modified: Wed Apr 19 08:39:45 2023, max compression
+gzip compressed data, was "nobuco-0.3.0.tar", last modified: Thu Apr 20 12:10:50 2023, max compression
```

## Comparing `nobuco-0.2.1.tar` & `nobuco-0.3.0.tar`

### file list

```diff
@@ -1,87 +1,94 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.2.1/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.2.1/MANIFEST.in
--rw-rw-r--   0 alex      (1000) alex      (1000)    18223 2023-04-19 08:39:45.501697 nobuco-0.2.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    16389 2023-04-19 08:38:31.000000 nobuco-0.2.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.493697 nobuco-0.2.1/docs/
--rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.2.1/docs/channel_ordering.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.2.1/docs/channel_ordering_forced.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.2.1/docs/control_if.png
--rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.2.1/docs/converter_inside_converter1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.2.1/docs/converter_inside_converter1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.2.1/docs/converter_inside_converter2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.2.1/docs/converter_inside_converter2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.2.1/docs/essentials1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.2.1/docs/essentials1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.2.1/docs/essentials2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.2.1/docs/essentials2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.2.1/docs/essentials3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.2.1/docs/essentials3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.2.1/docs/inplace1.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.2.1/docs/inplace1.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.2.1/docs/inplace2.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.2.1/docs/inplace2.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.2.1/docs/inplace3.html
--rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.2.1/docs/inplace3.svg
--rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.2.1/docs/inplace_empty.png
--rw-rw-r--   0 alex      (1000) alex      (1000)   926558 2023-04-16 10:49:50.000000 nobuco-0.2.1/docs/nobuco.png
--rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.2.1/docs/tutorial.png
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      461 2023-04-18 17:44:04.000000 nobuco-0.2.1/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      798 2023-03-07 13:07:06.000000 nobuco-0.2.1/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13145 2023-04-19 08:35:20.000000 nobuco-0.2.1/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.2.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.2.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2455 2023-04-18 11:52:51.000000 nobuco-0.2.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.2.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.2.1/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.2.1/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.2.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3106 2023-04-18 10:12:58.000000 nobuco-0.2.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.2.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1275 2023-04-18 18:43:04.000000 nobuco-0.2.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.2.1/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.2.1/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.2.1/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.2.1/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.2.1/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.2.1/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.2.1/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6822 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.2.1/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.2.1/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.2.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.2.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.2.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.2.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.501697 nobuco-0.2.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.2.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.2.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.2.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-19 08:39:45.497697 nobuco-0.2.1/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    18223 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2055 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-19 08:39:45.000000 nobuco-0.2.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-19 08:39:27.000000 nobuco-0.2.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-19 08:39:45.501697 nobuco-0.2.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-03-02 20:53:15.000000 nobuco-0.3.0/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       14 2023-04-15 10:44:29.000000 nobuco-0.3.0/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21658 2023-04-20 12:10:50.847216 nobuco-0.3.0/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    19824 2023-04-20 12:08:50.000000 nobuco-0.3.0/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/docs/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    64876 2023-03-25 20:16:55.000000 nobuco-0.3.0/docs/channel_ordering.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    63145 2023-03-25 20:46:53.000000 nobuco-0.3.0/docs/channel_ordering_forced.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    67966 2023-04-18 11:28:12.000000 nobuco-0.3.0/docs/control_if.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2110 2023-04-05 14:55:45.000000 nobuco-0.3.0/docs/converter_inside_converter1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26497 2023-04-05 19:25:33.000000 nobuco-0.3.0/docs/converter_inside_converter1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-04-05 14:56:10.000000 nobuco-0.3.0/docs/converter_inside_converter2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30325 2023-04-05 19:25:54.000000 nobuco-0.3.0/docs/converter_inside_converter2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1061 2023-04-20 11:04:43.000000 nobuco-0.3.0/docs/dynamic_shape1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    29177 2023-04-20 10:58:19.000000 nobuco-0.3.0/docs/dynamic_shape1.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13716 2023-04-20 10:56:49.000000 nobuco-0.3.0/docs/dynamic_shape1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2299 2023-04-20 11:06:54.000000 nobuco-0.3.0/docs/dynamic_shape2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    65071 2023-04-20 11:08:28.000000 nobuco-0.3.0/docs/dynamic_shape2.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    31893 2023-04-20 11:07:03.000000 nobuco-0.3.0/docs/dynamic_shape2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3070 2023-04-06 09:06:34.000000 nobuco-0.3.0/docs/essentials1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    35615 2023-04-06 09:06:58.000000 nobuco-0.3.0/docs/essentials1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2811 2023-04-05 14:47:00.000000 nobuco-0.3.0/docs/essentials2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    32971 2023-04-05 19:22:33.000000 nobuco-0.3.0/docs/essentials2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2281 2023-04-05 14:48:33.000000 nobuco-0.3.0/docs/essentials3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    28090 2023-04-05 19:22:46.000000 nobuco-0.3.0/docs/essentials3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1559 2023-04-05 14:51:28.000000 nobuco-0.3.0/docs/inplace1.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    18606 2023-04-05 19:23:57.000000 nobuco-0.3.0/docs/inplace1.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1050 2023-04-05 14:52:17.000000 nobuco-0.3.0/docs/inplace2.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11981 2023-04-05 19:24:22.000000 nobuco-0.3.0/docs/inplace2.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1195 2023-04-05 14:52:18.000000 nobuco-0.3.0/docs/inplace3.html
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14409 2023-04-05 19:25:18.000000 nobuco-0.3.0/docs/inplace3.svg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6859 2023-03-24 11:40:17.000000 nobuco-0.3.0/docs/inplace_empty.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)   863504 2023-04-19 06:48:26.000000 nobuco-0.3.0/docs/nobuco.png
+-rw-rw-r--   0 alex      (1000) alex      (1000)    82036 2023-03-03 12:08:40.000000 nobuco-0.3.0/docs/tutorial.png
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      526 2023-04-20 09:21:24.000000 nobuco-0.3.0/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      818 2023-04-19 23:06:10.000000 nobuco-0.3.0/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13153 2023-04-19 22:56:45.000000 nobuco-0.3.0/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-11-11 15:28:31.000000 nobuco-0.3.0/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-18 11:13:00.000000 nobuco-0.3.0/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-19 23:06:10.000000 nobuco-0.3.0/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-18 18:43:24.000000 nobuco-0.3.0/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-03-08 10:20:55.000000 nobuco-0.3.0/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3497 2023-03-07 10:32:51.000000 nobuco-0.3.0/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 10:29:29.000000 nobuco-0.3.0/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-20 11:44:40.000000 nobuco-0.3.0/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13309 2023-04-18 18:06:08.000000 nobuco-0.3.0/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-20 10:41:07.000000 nobuco-0.3.0/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-12-06 13:02:40.000000 nobuco-0.3.0/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-03-08 10:21:14.000000 nobuco-0.3.0/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4886 2023-04-18 10:06:25.000000 nobuco-0.3.0/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2022-12-06 13:05:18.000000 nobuco-0.3.0/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-18 10:06:25.000000 nobuco-0.3.0/nobuco/layers/weight.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1202 2023-04-20 09:37:25.000000 nobuco-0.3.0/nobuco/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-18 09:00:20.000000 nobuco-0.3.0/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4398 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4675 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9840 2023-04-18 17:59:47.000000 nobuco-0.3.0/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6816 2023-04-19 23:20:41.000000 nobuco-0.3.0/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3071 2023-04-19 08:28:44.000000 nobuco-0.3.0/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2568 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10232 2023-04-18 11:44:33.000000 nobuco-0.3.0/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-10-12 09:47:48.000000 nobuco-0.3.0/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-03-10 22:09:16.000000 nobuco-0.3.0/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9670 2023-04-18 11:49:04.000000 nobuco-0.3.0/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-18 18:22:15.000000 nobuco-0.3.0/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.847216 nobuco-0.3.0/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-02-28 17:54:05.000000 nobuco-0.3.0/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1943 2023-04-18 10:12:57.000000 nobuco-0.3.0/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3167 2023-04-18 10:12:58.000000 nobuco-0.3.0/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-04-20 12:10:50.843216 nobuco-0.3.0/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21658 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2218 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-04-20 12:10:50.000000 nobuco-0.3.0/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-04-20 11:19:12.000000 nobuco-0.3.0/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-04-20 12:10:50.847216 nobuco-0.3.0/setup.cfg
```

### Comparing `nobuco-0.2.1/LICENSE` & `nobuco-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/PKG-INFO` & `nobuco-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,10 @@
-Metadata-Version: 2.1
-Name: nobuco
-Version: 0.2.1
-Summary: Pytorch to Tensorflow conversion made somewhat easy
-Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Alexander Lutsenko
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
-Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
-Keywords: pytorch,tensorflow,keras,converter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
 <img src="docs/nobuco.png">
+<sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
@@ -57,17 +22,19 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
-  - Control flows
-  - Dynamic shapes
+  - [Control flows](#control-flows)
+  - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [More nice things](#more-nice-things)
+  - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -107,15 +74,17 @@
 Aaaand done! That's all it takes to... wait, what's that?
 
 <img src="docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
-Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
+Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
+A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
+The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
@@ -228,14 +197,15 @@
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
+
 @nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
@@ -357,34 +327,108 @@
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
 @nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
-def converterControlIf(self, x):
+def converter_ControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
     kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
     
     conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
     conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="30%">
+<img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
-:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
+What if we wanted out module to accept images of arbitrary height and width?
+Can we have that? Let's try:
+
+```python
+class DynamicShape(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
+
+    def forward(self, x):
+        x = self.conv(x)
+
+        # Produces static shape
+        b, c, h, w = x.shape
+
+        x = x[:, :, h//3:, w//3:]
+        return x
+
+
+input = torch.normal(0, 1, size=(1, 3, 128, 128))
+pytorch_module = DynamicShape().eval()
+
+keras_model = nobuco.pytorch_to_keras(
+    pytorch_module,
+    args=[input],
+    input_shapes={input: (None, 3, None, None)}, # Annotate dynamic axes with None
+    inputs_channel_order=ChannelOrder.TENSORFLOW,
+    outputs_channel_order=ChannelOrder.TENSORFLOW,
+)
+```
+
+Something's not right. We don't see shape extraction ops in the debug output or the graph:
+
+<img src="docs/dynamic_shape1.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape1.png" width="15%">
+</p>
+
+That's not surprising, actually. 
+In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
+`nobuco.shape` solves this problem.
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+
+```python
+# Allows for dynamic shape
+b, c, h, w = nobuco.shape(x)
+```
+
+<img src="docs/dynamic_shape2.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape2.png" width="30%">
+</p>
+
+Also, take a moment to appreciate how elegant the solution is. 
+`nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
+No special treatment required!
+
+```python
+@traceable
+def shape(x: Tensor):
+    return tuple(torch.tensor(d, dtype=torch.int32) for d in x.shape)
+
+
+@converter(shape, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_shape(x: Tensor):
+    def func(x):
+        shape = tf.unstack(tf.shape(x))
+        if get_channel_order(x) == ChannelOrder.TENSORFLOW:
+            shape = permute_keras2pytorch(shape)
+        return tuple(shape)
+    return func
+```
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
@@ -446,10 +490,48 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## More nice things
+
+### Nobuco knowledge base
+
+Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
+Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
+These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
+and there's a utility function to help you find what you need:
+
+
+```python
+node = torch.Tensor.repeat
+# node = F.relu_
+# node = nn.Conv2d
+
+location_link, source_code = nobuco.locate_converter(node)
+print('Converter location:')
+print(location_link)
+print('Converter source code:')
+print(source_code)
+```
+
+```console
+Converter location:
+File "/home/user/anaconda3/envs/nb/lib/python3.9/site-packages/nobuco/node_converters/tensor_manipulation.py", line 141
+
+Converter source code:
+@converter(torch.Tensor.repeat, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_repeat(self, *sizes):
+    def func(self, *sizes):
+        if get_channel_order(self) == ChannelOrder.TENSORFLOW:
+            sizes = permute_pytorch2keras(sizes)
+        return tf.tile(self, sizes)
+    return func
+```
+
+---
+
 ### Acknowledgements
 
 Slice assign converter is based on [Zaccharie Ramzi's tf-slice-assign script](https://github.com/zaccharieramzi/tf-slice-assign).
```

### Comparing `nobuco-0.2.1/README.md` & `nobuco-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,46 @@
+Metadata-Version: 2.1
+Name: nobuco
+Version: 0.3.0
+Summary: Pytorch to Tensorflow conversion made somewhat easy
+Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Alexander Lutsenko
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
+Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
+Keywords: pytorch,tensorflow,keras,converter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
 <img src="docs/nobuco.png">
+<sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
@@ -21,17 +58,19 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
-  - Control flows
-  - Dynamic shapes
+  - [Control flows](#control-flows)
+  - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [More nice things](#more-nice-things)
+  - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -71,15 +110,17 @@
 Aaaand done! That's all it takes to... wait, what's that?
 
 <img src="docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
-Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
+Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
+A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
+The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
@@ -192,14 +233,15 @@
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
+
 @nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
@@ -321,34 +363,108 @@
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
 @nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
-def converterControlIf(self, x):
+def converter_ControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
     kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
     
     conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
     conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="30%">
+<img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
-:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
+What if we wanted out module to accept images of arbitrary height and width?
+Can we have that? Let's try:
+
+```python
+class DynamicShape(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
+
+    def forward(self, x):
+        x = self.conv(x)
+
+        # Produces static shape
+        b, c, h, w = x.shape
+
+        x = x[:, :, h//3:, w//3:]
+        return x
+
+
+input = torch.normal(0, 1, size=(1, 3, 128, 128))
+pytorch_module = DynamicShape().eval()
+
+keras_model = nobuco.pytorch_to_keras(
+    pytorch_module,
+    args=[input],
+    input_shapes={input: (None, 3, None, None)}, # Annotate dynamic axes with None
+    inputs_channel_order=ChannelOrder.TENSORFLOW,
+    outputs_channel_order=ChannelOrder.TENSORFLOW,
+)
+```
+
+Something's not right. We don't see shape extraction ops in the debug output or the graph:
+
+<img src="docs/dynamic_shape1.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape1.png" width="15%">
+</p>
+
+That's not surprising, actually. 
+In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
+`nobuco.shape` solves this problem.
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+
+```python
+# Allows for dynamic shape
+b, c, h, w = nobuco.shape(x)
+```
+
+<img src="docs/dynamic_shape2.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape2.png" width="30%">
+</p>
+
+Also, take a moment to appreciate how elegant the solution is. 
+`nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
+No special treatment required!
+
+```python
+@traceable
+def shape(x: Tensor):
+    return tuple(torch.tensor(d, dtype=torch.int32) for d in x.shape)
+
+
+@converter(shape, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_shape(x: Tensor):
+    def func(x):
+        shape = tf.unstack(tf.shape(x))
+        if get_channel_order(x) == ChannelOrder.TENSORFLOW:
+            shape = permute_keras2pytorch(shape)
+        return tuple(shape)
+    return func
+```
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
@@ -410,10 +526,48 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## More nice things
+
+### Nobuco knowledge base
+
+Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
+Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
+These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
+and there's a utility function to help you find what you need:
+
+
+```python
+node = torch.Tensor.repeat
+# node = F.relu_
+# node = nn.Conv2d
+
+location_link, source_code = nobuco.locate_converter(node)
+print('Converter location:')
+print(location_link)
+print('Converter source code:')
+print(source_code)
+```
+
+```console
+Converter location:
+File "/home/user/anaconda3/envs/nb/lib/python3.9/site-packages/nobuco/node_converters/tensor_manipulation.py", line 141
+
+Converter source code:
+@converter(torch.Tensor.repeat, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_repeat(self, *sizes):
+    def func(self, *sizes):
+        if get_channel_order(self) == ChannelOrder.TENSORFLOW:
+            sizes = permute_pytorch2keras(sizes)
+        return tf.tile(self, sizes)
+    return func
+```
+
+---
+
 ### Acknowledgements
 
 Slice assign converter is based on [Zaccharie Ramzi's tf-slice-assign script](https://github.com/zaccharieramzi/tf-slice-assign).
```

### Comparing `nobuco-0.2.1/docs/channel_ordering.png` & `nobuco-0.3.0/docs/channel_ordering.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/channel_ordering_forced.png` & `nobuco-0.3.0/docs/channel_ordering_forced.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/control_if.png` & `nobuco-0.3.0/docs/control_if.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/converter_inside_converter1.html` & `nobuco-0.3.0/docs/converter_inside_converter1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/converter_inside_converter1.svg` & `nobuco-0.3.0/docs/converter_inside_converter1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/converter_inside_converter2.html` & `nobuco-0.3.0/docs/converter_inside_converter2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/converter_inside_converter2.svg` & `nobuco-0.3.0/docs/converter_inside_converter2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials1.html` & `nobuco-0.3.0/docs/essentials1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials1.svg` & `nobuco-0.3.0/docs/essentials1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials2.html` & `nobuco-0.3.0/docs/essentials2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials2.svg` & `nobuco-0.3.0/docs/essentials2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials3.html` & `nobuco-0.3.0/docs/essentials3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/essentials3.svg` & `nobuco-0.3.0/docs/essentials3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace1.html` & `nobuco-0.3.0/docs/inplace1.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace1.svg` & `nobuco-0.3.0/docs/inplace1.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace2.html` & `nobuco-0.3.0/docs/inplace2.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace2.svg` & `nobuco-0.3.0/docs/inplace2.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace3.html` & `nobuco-0.3.0/docs/inplace3.html`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace3.svg` & `nobuco-0.3.0/docs/inplace3.svg`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/inplace_empty.png` & `nobuco-0.3.0/docs/inplace_empty.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/docs/tutorial.png` & `nobuco-0.3.0/docs/tutorial.png`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/commons.py` & `nobuco-0.3.0/nobuco/commons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 import tensorflow as tf
 from tensorflow.python.keras.engine.keras_tensor import KerasTensor
 from tensorflow.python.ops.resource_variable_ops import ResourceVariable
 
+CONVERTER_DICT = {}
 
 CONVERTED_OP_DICT = {}
 
 
 TF_TENSOR_CLASSES = (
     tf.Tensor,
     tf.Variable,
```

### Comparing `nobuco-0.2.1/nobuco/convert.py` & `nobuco-0.3.0/nobuco/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 def convert_node(node: PytorchNode, node_converter: Pytorch2KerasNodeConverter) -> Callable:
     input_args = node.input_args
     if node.instance is not None:
         input_args = (node.instance, *input_args)
 
     # clone the inputs to be on the safe side
     input_args, input_kwargs = clone_torch_tensors_recursively((input_args, node.input_kwargs))
-    layer = node_converter(*input_args, **input_kwargs)
+    layer = node_converter.convert(*input_args, **input_kwargs)
     return layer
 
 
 def convert_container(
         node: PytorchNode,
         children: Collection[PytorchNodeHierarchy],
         children_converted_nodes: Collection[KerasConvertedNode],
```

### Comparing `nobuco-0.2.1/nobuco/converters/channel_ordering.py` & `nobuco-0.3.0/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/converters/node_converter.py` & `nobuco-0.3.0/nobuco/converters/node_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,43 @@
 from typing import Callable
 
 from nobuco.converters.validation import validate_diff_default
-from nobuco.commons import ChannelOrderingStrategy
+from nobuco.commons import ChannelOrderingStrategy, CONVERTER_DICT
 from nobuco.layers.channel_order import ChangeOrderingLayer
 from nobuco.trace.trace import Tracer
 
-CONVERTER_DICT = {}
-
 
 class Pytorch2KerasNodeConverter:
-    def __call__(self, *args, **kwargs):
-        keras_op = self.convert(*args, **kwargs)
-        return keras_op
-
-    def convert(self, *args, **kwargs):
-        raise NotImplementedError()
-
-    def validate(self, keras_op, pytorch_op, input_tensors_pt, args_pt, kwargs_pt, is_training=False):
-        raise NotImplementedError()
-
-
-class Pytorch2KerasLambdaConverter(Pytorch2KerasNodeConverter):
-    def __init__(self, convert_func, validate_func, reusable):
+    def __init__(self, convert_func, validate_func, channel_ordering_strategy, autocast, reusable):
         self.convert_func = convert_func
         self.validate_func = validate_func
+        self.channel_ordering_strategy = channel_ordering_strategy
+        self.autocast = autocast
         self.reusable = reusable
 
     def convert(self, *args, **kwargs):
-        return self.convert_func(*args, **kwargs)
+        converter_result_func = self.convert_func(*args, **kwargs)
+        return ChangeOrderingLayer(converter_result_func, self.channel_ordering_strategy, self.autocast)
 
     def validate(self, keras_op, pytorch_op, input_tensors_pt, args_pt, kwargs_pt, is_training=False):
         raise self.validate_func(keras_op, pytorch_op, input_tensors_pt, args_pt, kwargs_pt, is_training=False)
 
 
 def converter(*ops,
               validate_func=validate_diff_default,
               channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER,
               autocast: bool = False,
               reusable = True,
-              converter_dict=None,
               ):
-    if converter_dict is None:
-        converter_dict = CONVERTER_DICT
-
-    def channel_ordering_decorator(converter_func, channel_ordering_strategy):
-        def decorator(*args, **kwargs):
-            converter_result_func = converter_func(*args, **kwargs)
-            return ChangeOrderingLayer(converter_result_func, channel_ordering_strategy, autocast)
-        return decorator
-
-    def inner(convert_func: Callable) -> Callable:
-        convert_func = channel_ordering_decorator(convert_func, channel_ordering_strategy)
-        node_converter = Pytorch2KerasLambdaConverter(convert_func, validate_func, reusable)
+    def inner(convert_func: Callable) -> Pytorch2KerasNodeConverter:
+        node_converter = Pytorch2KerasNodeConverter(convert_func, validate_func, channel_ordering_strategy, autocast, reusable)
         for op in ops:
             op = Tracer.op_unwrap(op)
-            converter_dict[op] = node_converter
+            CONVERTER_DICT[op] = node_converter
         return node_converter
-
     return inner
 
 
-def converter_unregister(op, converter_dict=None):
-    if converter_dict is None:
-        converter_dict = CONVERTER_DICT
-
+def converter_unregister(op):
     op = Tracer.op_unwrap(op)
-    if op in converter_dict:
-        del converter_dict[op]
+    if op in CONVERTER_DICT:
+        del CONVERTER_DICT[op]
```

### Comparing `nobuco-0.2.1/nobuco/converters/tensor.py` & `nobuco-0.3.0/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/converters/type_cast.py` & `nobuco-0.3.0/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/converters/validation.py` & `nobuco-0.3.0/nobuco/converters/validation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/entity/pytorch.py` & `nobuco-0.3.0/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/funcs.py` & `nobuco-0.3.0/nobuco/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch
+from torch import Tensor
 
 import tensorflow as tf
 from nobuco.converters.tensor import permute_pytorch2keras, permute_keras2pytorch
 
 from nobuco.converters.channel_ordering import get_channel_order
 
 from nobuco.commons import ChannelOrderingStrategy, ChannelOrder
@@ -27,19 +28,19 @@
 
 @converter(force_pytorch_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_force_pytorch_order(inputs):
     return lambda inputs: inputs
 
 
 @traceable
-def shape(x):
+def shape(x: Tensor):
     return tuple(torch.tensor(d, dtype=torch.int32) for d in x.shape)
 
 
 @converter(shape, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_shape(x):
+def converter_shape(x: Tensor):
     def func(x):
         shape = tf.unstack(tf.shape(x))
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             shape = permute_keras2pytorch(shape)
         return tuple(shape)
     return func
```

### Comparing `nobuco-0.2.1/nobuco/layers/channel_order.py` & `nobuco-0.3.0/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/layers/container.py` & `nobuco-0.3.0/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/layers/weight.py` & `nobuco-0.3.0/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/activation.py` & `nobuco-0.3.0/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/boolean.py` & `nobuco-0.3.0/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/boolean_mask.py` & `nobuco-0.3.0/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/comparison.py` & `nobuco-0.3.0/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/convolution.py` & `nobuco-0.3.0/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/dropout.py` & `nobuco-0.3.0/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/interpolation.py` & `nobuco-0.3.0/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/linear.py` & `nobuco-0.3.0/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/math.py` & `nobuco-0.3.0/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/misc.py` & `nobuco-0.3.0/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/normalization.py` & `nobuco-0.3.0/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/padding.py` & `nobuco-0.3.0/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/pooling.py` & `nobuco-0.3.0/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/recurrent.py` & `nobuco-0.3.0/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/slice.py` & `nobuco-0.3.0/nobuco/node_converters/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     sliced_tensor_updated = tf.transpose(
         sliced_tensor_reshaped,
         perm=inverse_scatter_nd_perm,
     )
     return sliced_tensor_updated
 
 
-@converter(None, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
+@converter(channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def getitem_indexed(self, *slices):
     slices = _flatten(slices)
     slices = torch.broadcast_tensors(*slices)
     slices_combined = torch.stack(slices, dim=-1).numpy()
 
     def func(self, *slices):
         return tf.gather_nd(self, slices_combined)
```

### Comparing `nobuco-0.2.1/nobuco/node_converters/tensor_cast.py` & `nobuco-0.3.0/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/tensor_creation.py` & `nobuco-0.3.0/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.3.0/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/trace/tensor_storage.py` & `nobuco-0.3.0/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/trace/trace.py` & `nobuco-0.3.0/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/util.py` & `nobuco-0.3.0/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/vis/console_stylizer.py` & `nobuco-0.3.0/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco/vis/html_stylizer.py` & `nobuco-0.3.0/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.2.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.3.0/nobuco.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.2.1
+Version: 0.3.0
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="docs/nobuco.png">
+<sup><a href="https://www.behance.net/diliajl">diliajl</a></sup>
 </p>
 
 **No** **Bu**llshit **Co**nverter is a tool that helps you translate pytorch models into tensorflow graphs without losing your mind.
 
 - Supports a wide range of architectures
   - [x] Control flow ops (If, While)
   - [x] Recurrent layers (LSTM, GRU)
@@ -57,17 +58,19 @@
 ```
 
 ## Table of Contents
 - [Essentials](#essentials)
 - [Channel order wizardry](#channel-order-wizardry)
 - [In-place operations](#in-place-operations)
 - [Going dynamic](#going-dynamic)
-  - Control flows
-  - Dynamic shapes
+  - [Control flows](#control-flows)
+  - [Dynamic shapes](#dynamic-shapes)
 - [So we put a converter inside your converter](#so-we-put-a-converter-inside-your-converter)
+- [More nice things](#more-nice-things)
+  - [Nobuco knowledge base](#nobuco-knowledge-base)
 
 <!-- tocstop -->
 
 ## Essentials
 
 Suppose we want to convert a pytorch module similar to this one:
 
@@ -107,15 +110,17 @@
 Aaaand done! That's all it takes to... wait, what's that?
 
 <img src="docs/essentials1.svg" width="100%">
 
 Nobuco says it doesn't know how to handle hard sigmoid.
 Apparently, it's our job to provide a node converter for either `F.hardsigmoid` or the enclosing `Hardsigmoid` module (or the entire `MyModule`, but that makes little sense). Here, we'll go for the former.
 
-Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. A node converter is just a `Callable` that takes in the same arguments as the corresponding node and outputs an equivalent node in tensorflow. The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
+Conversion is done directly. No layers upon layers of abstraction, no obscure intermediate representation. 
+A node converter is just a `Callable` that takes in the same arguments as the corresponding node in pytorch and outputs an equivalent node in tensorflow. 
+The converted node preserves the original node's signature, but pytorch tensors replaced with tensorflow counterparts (be that `tf.Tensor`, `KerasTensor`, `tf.Variable`, or `ResourceVariable`).
 
 This should do the trick:
 
 ````python
 @nobuco.converter(F.hardsigmoid, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def hardsigmoid(input: torch.Tensor, inplace: bool = False):
     return lambda input, inplace=False: tf.keras.activations.hard_sigmoid(input)
@@ -228,14 +233,15 @@
 In case you are curious, the implementation is trivial:
 
 ```python
 @nobuco.traceable
 def force_tensorflow_order(inputs):
     return inputs
 
+
 @nobuco.converter(force_tensorflow_order, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
 def converter_force_tensorflow_order(inputs):
     return lambda inputs: inputs
 ```
 
 `force_pytorch_order` is defined analogously.
 
@@ -357,34 +363,108 @@
             x = self.conv_shared(x)
             x = x - 1
         x = self.conv_shared(x)
         return x
 
 
 @nobuco.converter(ControlIf, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_TENSORFLOW_ORDER)
-def converterControlIf(self, x):
+def converter_ControlIf(self, x):
     order = ChannelOrder.TENSORFLOW
     kwargs = {'inputs_channel_order': order, 'outputs_channel_order': order, 'return_outputs_pt': True}
     
     conv_pre, out_pre = nobuco.pytorch_to_keras(self.conv_pre, [x], **kwargs)
     conv_true, out_true = nobuco.pytorch_to_keras(self.conv_true, [out_pre], **kwargs)
     conv_false, out_false = nobuco.pytorch_to_keras(self.conv_false, [out_pre], **kwargs)
     conv_shared, _ = nobuco.pytorch_to_keras(self.conv_shared, [out_true], **kwargs)
     layer = ControlIfKeras(conv_pre, conv_true, conv_false, conv_shared)
     return layer
 ```
 
 <p align="center">
-<img src="docs/control_if.png" width="30%">
+<img src="docs/control_if.png" width="25%">
 </p>
 
 See [examples](/examples) for other ways to convert control flow ops.
 
 ### Dynamic shapes
-:construction: See [examples/dynamic_shape](https://github.com/AlexanderLutsenko/nobuco/blob/master/examples/dynamic_shape.py) :construction:
+
+What if we wanted out module to accept images of arbitrary height and width?
+Can we have that? Let's try:
+
+```python
+class DynamicShape(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv = nn.Conv2d(3, 16, kernel_size=(1, 1))
+
+    def forward(self, x):
+        x = self.conv(x)
+
+        # Produces static shape
+        b, c, h, w = x.shape
+
+        x = x[:, :, h//3:, w//3:]
+        return x
+
+
+input = torch.normal(0, 1, size=(1, 3, 128, 128))
+pytorch_module = DynamicShape().eval()
+
+keras_model = nobuco.pytorch_to_keras(
+    pytorch_module,
+    args=[input],
+    input_shapes={input: (None, 3, None, None)}, # Annotate dynamic axes with None
+    inputs_channel_order=ChannelOrder.TENSORFLOW,
+    outputs_channel_order=ChannelOrder.TENSORFLOW,
+)
+```
+
+Something's not right. We don't see shape extraction ops in the debug output or the graph:
+
+<img src="docs/dynamic_shape1.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape1.png" width="15%">
+</p>
+
+That's not surprising, actually. 
+In pytorch, tensor shape is a tuple of regular integers, not tensors, so it's quite difficult to track them.
+`nobuco.shape` solves this problem.
+This function returns tensors, much like [`tf.shape`](https://www.tensorflow.org/api_docs/python/tf/shape) does:
+
+```python
+# Allows for dynamic shape
+b, c, h, w = nobuco.shape(x)
+```
+
+<img src="docs/dynamic_shape2.svg" width="100%">
+
+<p align="center">
+<img src="docs/dynamic_shape2.png" width="30%">
+</p>
+
+Also, take a moment to appreciate how elegant the solution is. 
+`nobuco.shape` is a one-liner that simply replaces each integer in shape tuple with a scalar tensor.
+No special treatment required!
+
+```python
+@traceable
+def shape(x: Tensor):
+    return tuple(torch.tensor(d, dtype=torch.int32) for d in x.shape)
+
+
+@converter(shape, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_shape(x: Tensor):
+    def func(x):
+        shape = tf.unstack(tf.shape(x))
+        if get_channel_order(x) == ChannelOrder.TENSORFLOW:
+            shape = permute_keras2pytorch(shape)
+        return tuple(shape)
+    return func
+```
 
 ## So we put a converter inside your converter
 
 One of the operations currently not supported is mask assign.
 There's no particular reason why, I just haven't done it yet (and your contribution is highly welcome!) 
 For now, let's use it as an excuse to explain the concept of nested converters.
 Like I said, for this module, conversion will fail:
@@ -446,10 +526,48 @@
     tf_rep.export_graph(model_path)
     model = tf.keras.models.load_model(model_path)
     return keras.layers.Lambda(lambda x, mask: model(input=x, mask=mask))
 ```
 
 <img src="docs/converter_inside_converter2.svg" width="100%">
 
+## More nice things
+
+### Nobuco knowledge base
+
+Don't want to convert anything but looking for a tensorflow equivalent of a certain pytorch node (operation or module)?
+Nobuco already implements quite a few node converters, most written in concise and (hopefully) understandable way.
+These are located in [nobuco/node_converters](https://github.com/AlexanderLutsenko/nobuco/tree/master/nobuco/node_converters),
+and there's a utility function to help you find what you need:
+
+
+```python
+node = torch.Tensor.repeat
+# node = F.relu_
+# node = nn.Conv2d
+
+location_link, source_code = nobuco.locate_converter(node)
+print('Converter location:')
+print(location_link)
+print('Converter source code:')
+print(source_code)
+```
+
+```console
+Converter location:
+File "/home/user/anaconda3/envs/nb/lib/python3.9/site-packages/nobuco/node_converters/tensor_manipulation.py", line 141
+
+Converter source code:
+@converter(torch.Tensor.repeat, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_repeat(self, *sizes):
+    def func(self, *sizes):
+        if get_channel_order(self) == ChannelOrder.TENSORFLOW:
+            sizes = permute_pytorch2keras(sizes)
+        return tf.tile(self, sizes)
+    return func
+```
+
+---
+
 ### Acknowledgements
 
 Slice assign converter is based on [Zaccharie Ramzi's tf-slice-assign script](https://github.com/zaccharieramzi/tf-slice-assign).
```

### Comparing `nobuco-0.2.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.3.0/nobuco.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 docs/channel_ordering.png
 docs/channel_ordering_forced.png
 docs/control_if.png
 docs/converter_inside_converter1.html
 docs/converter_inside_converter1.svg
 docs/converter_inside_converter2.html
 docs/converter_inside_converter2.svg
+docs/dynamic_shape1.html
+docs/dynamic_shape1.png
+docs/dynamic_shape1.svg
+docs/dynamic_shape2.html
+docs/dynamic_shape2.png
+docs/dynamic_shape2.svg
 docs/essentials1.html
 docs/essentials1.svg
 docs/essentials2.html
 docs/essentials2.svg
 docs/essentials3.html
 docs/essentials3.svg
 docs/inplace1.html
@@ -24,14 +30,15 @@
 docs/inplace_empty.png
 docs/nobuco.png
 docs/tutorial.png
 nobuco/__init__.py
 nobuco/commons.py
 nobuco/convert.py
 nobuco/funcs.py
+nobuco/locate.py
 nobuco/util.py
 nobuco.egg-info/PKG-INFO
 nobuco.egg-info/SOURCES.txt
 nobuco.egg-info/dependency_links.txt
 nobuco.egg-info/requires.txt
 nobuco.egg-info/top_level.txt
 nobuco/converters/__init__.py
```

### Comparing `nobuco-0.2.1/pyproject.toml` & `nobuco-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.2.1"
+version = "0.3.0"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

