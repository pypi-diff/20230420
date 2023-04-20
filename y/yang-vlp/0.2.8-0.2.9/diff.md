# Comparing `tmp/yang-vlp-0.2.8.tar.gz` & `tmp/yang-vlp-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp\dist\.tmp-58akbb83\yang-vlp-0.2.8.tar", last modified: Thu Mar 23 04:47:50 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-6kr17y0d\yang-vlp-0.2.9.tar", last modified: Thu Apr 20 06:28:34 2023, max compression
```

## Comparing `yang-vlp-0.2.8.tar` & `yang-vlp-0.2.9.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.892709 yang-vlp-0.2.8/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      257 2022-11-23 04:06:33.000000 yang-vlp-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2537 2023-03-23 04:47:50.891714 yang-vlp-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-03-21 10:49:54.000000 yang-vlp-0.2.8/README.md
--rw-rw-rw-   0        0        0      636 2023-03-23 04:47:02.000000 yang-vlp-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-23 04:47:50.892709 yang-vlp-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      931 2023-03-23 04:47:06.000000 yang-vlp-0.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.635695 yang-vlp-0.2.8/vlppy/
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.660020 yang-vlp-0.2.8/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.8/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.8/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      248 2022-11-23 04:08:29.000000 yang-vlp-0.2.8/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.675032 yang-vlp-0.2.8/vlppy/demo/
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.8/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.704068 yang-vlp-0.2.8/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.8/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.8/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.8/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0      834 2023-01-09 06:54:09.000000 yang-vlp-0.2.8/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2158 2022-11-22 13:14:33.000000 yang-vlp-0.2.8/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     3303 2022-11-22 13:06:18.000000 yang-vlp-0.2.8/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.723051 yang-vlp-0.2.8/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.8/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1230 2022-11-08 07:30:23.000000 yang-vlp-0.2.8/vlppy/error/error.py
--rw-rw-rw-   0        0        0      111 2023-03-23 04:46:42.000000 yang-vlp-0.2.8/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.730039 yang-vlp-0.2.8/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.8/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5287 2023-03-22 12:59:54.000000 yang-vlp-0.2.8/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.748519 yang-vlp-0.2.8/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.8/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.803948 yang-vlp-0.2.8/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.8/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.8/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.8/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.8/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.8/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     5613 2022-11-24 09:07:29.000000 yang-vlp-0.2.8/vlppy/model/led.py
--rw-rw-rw-   0        0        0    16688 2022-12-21 06:14:59.000000 yang-vlp-0.2.8/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    16636 2022-12-21 06:14:30.000000 yang-vlp-0.2.8/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.825888 yang-vlp-0.2.8/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.8/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.840851 yang-vlp-0.2.8/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.8/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.8/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2898 2023-03-16 02:13:44.000000 yang-vlp-0.2.8/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.8/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.861802 yang-vlp-0.2.8/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.8/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0     9002 2022-11-24 09:00:42.000000 yang-vlp-0.2.8/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3662 2022-12-21 06:18:17.000000 yang-vlp-0.2.8/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.872769 yang-vlp-0.2.8/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.8/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     2619 2023-03-23 04:45:19.000000 yang-vlp-0.2.8/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-03-23 04:47:50.889717 yang-vlp-0.2.8/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2537 2023-03-23 04:47:50.000000 yang-vlp-0.2.8/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1211 2023-03-23 04:47:50.000000 yang-vlp-0.2.8/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 04:47:50.000000 yang-vlp-0.2.8/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-23 04:47:50.000000 yang-vlp-0.2.8/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-23 04:47:50.000000 yang-vlp-0.2.8/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:34.024581 yang-vlp-0.2.9/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2640 2023-04-20 06:28:34.023589 yang-vlp-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2023-04-20 06:27:54.000000 yang-vlp-0.2.9/README.md
+-rw-rw-rw-   0        0        0      636 2023-04-20 05:23:09.000000 yang-vlp-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 06:28:34.025579 yang-vlp-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      931 2023-04-20 05:22:36.000000 yang-vlp-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.806106 yang-vlp-0.2.9/vlppy/
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.809096 yang-vlp-0.2.9/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.9/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.9/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.9/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.826053 yang-vlp-0.2.9/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.9/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.9/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.841014 yang-vlp-0.2.9/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.9/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.9/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.9/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0      993 2023-04-19 03:13:01.000000 yang-vlp-0.2.9/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.9/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     3303 2022-11-22 13:06:18.000000 yang-vlp-0.2.9/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.846998 yang-vlp-0.2.9/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.9/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.9/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      109 2023-04-20 05:22:10.000000 yang-vlp-0.2.9/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.859960 yang-vlp-0.2.9/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.9/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.9/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.878071 yang-vlp-0.2.9/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.9/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.907993 yang-vlp-0.2.9/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.9/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.9/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.9/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.9/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.9/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6142 2023-04-20 06:10:04.000000 yang-vlp-0.2.9/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    17076 2023-04-20 06:11:29.000000 yang-vlp-0.2.9/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    16974 2023-04-20 06:11:55.000000 yang-vlp-0.2.9/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.921959 yang-vlp-0.2.9/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.9/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.927939 yang-vlp-0.2.9/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.9/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.9/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.9/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.9/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.945890 yang-vlp-0.2.9/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.9/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.9/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3662 2022-12-21 06:18:17.000000 yang-vlp-0.2.9/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.961853 yang-vlp-0.2.9/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.9/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.9/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:33.974824 yang-vlp-0.2.9/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.9/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.9/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-04-20 06:28:34.015617 yang-vlp-0.2.9/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2640 2023-04-20 06:28:33.000000 yang-vlp-0.2.9/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-20 06:28:33.000000 yang-vlp-0.2.9/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 06:28:33.000000 yang-vlp-0.2.9/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-20 06:28:33.000000 yang-vlp-0.2.9/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 06:28:33.000000 yang-vlp-0.2.9/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.8/LICENSE` & `yang-vlp-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/PKG-INFO` & `yang-vlp-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,40 +25,43 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://gitee.com/yangwuju/yang_vlp
 Project-URL: Bug Tracker, https://gitee.com/yangwuju/yang_vlp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 @start date:  2022-08-26
 
 @auther:  yang wu ju
 
 @url: https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room： 房间、墙壁参数
-- model/led:  led位置、发射的信号
-- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号
+- model/led:  led位置、发射的信号(None、DC、AC、AIM)
+- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter:  滤波器设计（包括fir,iir）
 - signal/plot: 绘制波形图
 - demo/vlp_model: 可见光定位模型
 - demo/demo_main: test demo
 - io/io: 数据保存与加载
 - setting/json_setting: 加载json配置文件
 - error/error: VLP常见异常
 - vis/vis: 可视化绘图
+- tools/decorator:VLP可能用到的装饰器
 
-@Download
+@download
 
 ```
 py -m pip install yang-vlp
 ```
 
 @updata log
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
+
+优化部分代码；
```

### Comparing `yang-vlp-0.2.8/README.md` & `yang-vlp-0.2.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 @auther:  yang wu ju
 
 @url: https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room： 房间、墙壁参数
-- model/led:  led位置、发射的信号
-- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号
+- model/led:  led位置、发射的信号(None、DC、AC、AIM)
+- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter:  滤波器设计（包括fir,iir）
 - signal/plot: 绘制波形图
 - demo/vlp_model: 可见光定位模型
 - demo/demo_main: test demo
 - io/io: 数据保存与加载
 - setting/json_setting: 加载json配置文件
 - error/error: VLP常见异常
 - vis/vis: 可视化绘图
+- tools/decorator:VLP可能用到的装饰器
 
-@Download
+@download
 
 ```
 py -m pip install yang-vlp
 ```
 
 @updata log
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
+
+优化部分代码；
```

### Comparing `yang-vlp-0.2.8/pyproject.toml` & `yang-vlp-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `yang-vlp-0.2.8/setup.py` & `yang-vlp-0.2.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.8',  #版本号
+    version = '0.2.9',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `yang-vlp-0.2.8/vlppy/LICENSE.txt` & `yang-vlp-0.2.9/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.9/vlppy/demo/demo_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from ..signal import filter,plot
-np.set_printoptions(suppress=True)  #不以科学计数法显示
-
-Fs = 1200 # 采样频率,单位为Hz
-N = 1024  # 采样点数
-t = np.arange(N) * 1/Fs  # 产生一个以采样时间为间隔的时间序列
-
-# 产生一个信号
-f1 = 3000
-f2 = 4000
-f3 = 5000
-Amp = 10
-U1 = Amp * np.cos(2 * np.pi * f1 * t)
-U2 = Amp * np.cos(2 * np.pi * f2 * t)
-U3 = Amp * np.cos(2 * np.pi * f3 * t)
-
-U = U1 + U2 + U3
-
-# 显示信号的波形
-plot.signal_wave(t,U1,U2,U3,U)
-plot.signal_fft_wave(t,U1,U2,U3,U)
-
-# 滤波器设计
-Fc = f1 # 滤波频率
-buff = filter.ButterFilter(Fc,Fs,[300,400],[2,40])
-buff.show_wave(N)
-
-
-# 滤波
-Ulf = buff.filter(U)
-
-# 滤波信号波形
-plot.signal_wave(t,Ulf)
-plot.signal_fft_wave(t,Ulf)
 
+def main():
+    print("This is a demo about filter!")
+    Fs = 1200 # 采样频率,单位为Hz
+    N = 1024  # 采样点数
+    t = np.arange(N) * 1/Fs  # 产生一个以采样时间为间隔的时间序列
+
+    # 产生多个子信号
+    f1 = 3000
+    f2 = 4000
+    f3 = 5000
+    Amp = 10
+    U1 = Amp * np.cos(2 * np.pi * f1 * t)
+    U2 = Amp * np.cos(2 * np.pi * f2 * t)
+    U3 = Amp * np.cos(2 * np.pi * f3 * t)
+
+    # 信号 = 子信号叠加
+    U = U1 + U2 + U3 
+
+    # 显示信号的波形
+    plot.signal_wave(t,U1,U2,U3,U)
+    plot.signal_fft_wave(t,U1,U2,U3,U)
+
+    # 滤波器设计
+    Fc = f1 # 滤波频率
+    buff = filter.ButterFilter(Fc,Fs,[300,400],[2,40]) 
+    buff.show_wave(N)
+
+    # 滤波
+    Ulf = buff.filter(U)
+
+    # 滤波信号波形
+    plot.signal_wave(t,Ulf)
+    plot.signal_fft_wave(t,Ulf)
 
+if __name__ == '__main__':
+    main()
```

### Comparing `yang-vlp-0.2.8/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.9/vlppy/demo/vlp_model.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/error/error.py` & `yang-vlp-0.2.9/vlppy/error/error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,53 @@
 import typing
 
 class VLPError(Exception):
     pass
 
 class VLPTypeError(VLPError):
+    """数据类型异常:
+    """
     def __init__(self, value, *typeargv:type):
+        """数据需为指定的类型
+        """
         self._value = value
         self._type = [str(i).split("\'")[1] for i in list(typeargv)]
     
     def __str__(self):
         s = str(type(self._value)).split("\'")[1]
-        return repr(f"the value must be of type {self._type}, but this value is of type {s}.")
+        return repr(f"The value must be of type {self._type}, but this value is of type {s}.")
 
 class VLPSequenceLenError(VLPError):
+    """序列长度异常
+    """
     def __init__(self,value:typing.Sequence,length:int):
+        """序列需固定的长度
+        """
         self._value = value
         self._len = length
     def __str__(self) -> str:
-        return repr(f"the length of the Sequence has to be {self._len}, but this Sequence has length {len(self._value)}.")
-
+        return repr(f"The length of the Sequence has to be {self._len}, but this Sequence has length {len(self._value)}.")
 
 class VLPValueError(VLPError):
+    """数据取值异常
+    """
     def __init__(self,value,*argv):
+        """数据应指定的取值
+        """
         self._value = value
         self._argv = list(argv)
     def __str__(self) -> str:
         return repr(f"The value {self._value} is not in {self._argv}.")
- 
 
 class VLPValueRangeError(VLPError):
+    """数据取值范围异常
+    """
     def __init__(self,value,low,hignt):
+        """数据应在指定的范围内,可能不包括端点处的取值
+        """
         self._value = value
         self._range = (low,hignt)
     def __str__(self) -> str:
         return repr(f"The value {self._value} must be in the range {self._range}.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yang-vlp-0.2.8/vlppy/io/io.py` & `yang-vlp-0.2.9/vlppy/io/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import scipy.io as scio
 import pandas as pd
 import numpy as np
 
 
 class IO:
-
+    """数据保存和读写
+    """
     def save_excel(self, fp:str, *data, header=False,index=False):
         """保存为.excel
         加载:pd.read_excel(fp,sheet_name=Sheet1)  
         header: 是否包含标题
         index: 是否包含索引号（第一列行号）
         """
         dataset = []
@@ -52,83 +53,84 @@
         return pd.read_csv(fp).to_numpy()
 
     def svae_txt(self, fp:str, data:dict):
         """保存为.txt
         加载:np.loadtxt(fp) 
         """
         data = pd.DataFrame(data)
-        np.savetxt(fp,data)
+        np.savetxt(fp, data)
    
     # 读取txt 存储的数据
-    def load_txt(self,fp:str,sep=None,start_row=0,end_row=-1,start_column=0,end_column=-1):
+    def load_txt(self, fp:str, sep=None, start_row=0, end_row=-1, start_column=0, end_column=-1):
         return pd.read_csv(fp," ")
 
     def save_mat(self, fp:str, mdict:dict={}):
         """保存为.mat文件
         加载: scipy.io.loadmat(fp)
         """
-        scio.savemat(fp,mdict)
+        scio.savemat(fp, mdict)
 
-    def load_mat(self,fp:str, keys:dict={}, default=None):
+    def load_mat(self, fp:str, keys:dict={}, default=None):
         """加载.mat文件
         """
         mdict = scio.loadmat(fp)
         output = []
         for key in keys:
-            output.append(mdict.get(key,default))
+            output.append(mdict.get(key, default))
         return output
 
-    def user_save_npz_2d(self,fp:str,train_p=None,train_x=None,train_y=None,test_p=None,test_x=None,test_y=None):
+    def user_save_npz_2d(self, fp:str, train_p=None, train_x=None, train_y=None, test_p=None, test_x=None, test_y=None):
         """用户保存numpy数据2D
         加载: user_load_npz_2d(fp)
         """
         # 数据保存.npz
         np.savez(fp,train_p=train_p,train_x=train_x,train_y=train_y,
                                 test_p=test_p,test_x=test_x,test_y=test_y)
 
-    def user_load_npz_2d(self,fp:str):
+    def user_load_npz_2d(self, fp:str):
         """用户加载numpy数据2D
         """
         with np.load(fp) as f:
             train_p,train_x,train_y = f['train_p'],f['train_x'],f['train_y']
             test_p,test_x,test_y = f['test_p'],f['test_x'],f['test_y']
         return (train_p,train_x,train_y), (test_p,test_x,test_y)
 
-    def user_save_npz_3d(self,fp:str,train_p=None,train_x=None,train_y=None,train_z=None,test_p=None,test_x=None,test_y=None,test_z=None):
+    def user_save_npz_3d(self, fp:str, train_p=None, train_x=None, train_y=None, train_z=None, test_p=None, test_x=None, test_y=None, test_z=None):
         """用户保存numpy数据3D
         加载: user_load_npz_3d(fp)
         """
         # 数据保存.npz
         np.savez(fp, train_p=train_p, train_x=train_x, train_y=train_y, train_z=train_z,
                             test_p=test_p, test_x=test_x, test_y=test_y, test_z=test_z)
 
-    def user_load_npz_3d(self,fp:str):
+    def user_load_npz_3d(self, fp:str):
         """用户加载numpy数据3D
         """
-        with np.load(fp,allow_pickle=True) as f:
+        with np.load(fp) as f:
             train_p, train_x, train_y, train_z = f['train_p'], f['train_x'], f['train_y'], f['train_z']
             test_p, test_x, test_y, test_z = f['test_p'], f['test_x'], f['test_y'], f['test_z']
         return (train_p,train_x,train_y,train_z), (test_p,test_x,test_y,test_z)
 
     def dataset_save_npz(self, fp:str, train_inputs=None, train_outputs=None, test_inputs=None, test_outputs=None):
         """保存数据集
         加载: dataset_load_npz(fp)
         """
         np.savez(fp, train_inputs=train_inputs, train_outputs=train_outputs, 
                         test_inputs=test_inputs, test_outputs=test_outputs)
 
     def dataset_load_npz(self, fp:str):
         """加载数据集
         """
-        with np.load(fp,allow_pickle=True) as f:
+        with np.load(fp, allow_pickle=True) as f:
             train_inputs, train_outputs = f['train_inputs'], f['train_outputs'] 
             test_inputs, test_outputs = f['test_inputs'], f['test_outputs']
         return (train_inputs, train_outputs), (test_inputs, test_outputs)
     
-    def data_sort(sfp:str,dfp:str="",column=3):
+
+    def data_sort(self, sfp:str, dfp: str="", column=0):
         """excel、csv数据排序(将excel中数据按某一列数据进行排序)
         Params
             sfp: 源地址
             dfp: 目标地址
             column: 第几列
         Return
             无
```

### Comparing `yang-vlp-0.2.8/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/model/led.py` & `yang-vlp-0.2.9/vlppy/model/led.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import numpy as np
 from typing import Union
 from ..error import VLPSequenceLenError,VLPValueError
+from numbers import Number
 
 class LED:
+    """发光二极管
+    """
     def __init__(self,
-                theta=30,
+                theta:Number=30,
                 pos:tuple=(0,0,0),
+                Nv:tuple=(0,0,-1),
                 signal:str="None",
                 *args,
                 **kwargs) -> None:
         """
         theta: LED半功率点半角 (单位: 度)
         pos: LED参考位置 (注意:self.pos设置的是参考位置,self.pos获取的是相对位置)
+        Nv: LED法向量
         signal: LED发射信号类型
         *args和**kwargs:
             signal="None":无发射信号,无需传参数: 默认led.signal=0
             signal="DC":发射直流功率,传参详见函数: DC_Power(Pt);
             signal="AC":发射交流信号(电压信号或电流信号),传参详见函数: AC_Signal(DCbias, Amp, freq, t, signal_func);
             signal="AIM":强度调制功率信号,传参详见函数: AIM_Signal(Pt, m, freq, t, signal_func)
         """
         self.theta = theta
         self.pos = pos #参考位置
+        self.Nv = Nv
         self.send_signal(signal,*args,**kwargs) 
         self.origin = (0,0,0)
 
     def DC_Signal(self, Pt, *args, **kwargs):
         """直流信号
         Params
             Pt: 直流功率
@@ -75,15 +81,15 @@
         if signal_func not in ('sin', 'cos', np.sin, np.cos):
             raise VLPValueError(signal_func, 'sin', 'cos', np.sin, np.cos)
         if isinstance(signal_func, str):
             signal_func = np.sin if signal_func == 'sin' else np.cos
         return Pt*(1 + m*signal_func(2 * np.pi * (t * freq + np.random.random())))
 
     def send_signal(self, signal:str, *args, **kwargs):
-        """设置LED发射信号
+        """设置内置的LED发射信号
         Params
             signal: LED信号类型
             *args和**kwargs:
                 signal="None":无发射信号,无需传参: 默认led.signal=0;
                 signal="DC":发射直流功率,传参详见函数: DC_Power(Pt);
                 signal="AC":发射交流信号(电压信号或电流信号),传参详见函数: AC_Signal(DCbias, Amp, freq, t, signal_func);
                 signal="AIM":强度调制功率信号,传参详见函数: AIM_Signal(Pt, m, freq, t, signal_func)
@@ -101,21 +107,21 @@
         elif signal == 'AIM': # 强度调制
             self.signal = self.AIM_Signal(*args,**kwargs)
         else:   # 无发射信号
             self.signal = 0
 
     @property
     def signal(self):
-        """LED发射的信号
+        """获取LED发射的信号
         """
         return self._signal
 
     @signal.setter
     def signal(self, s):
-        """LED发射的信号
+        """注册LED发射的信号
         """
         self._signal = s
 
     @property
     def origin(self) -> tuple:
         """获取原点
         """
@@ -138,26 +144,40 @@
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
         if not len(pos) == 3:
             raise VLPSequenceLenError(pos,3)
         self._pos = tuple(pos)
- 
+        
+    @property
+    def Nv(self):  
+        """获取LED单位法向量  
+        """  
+        return self._Nv/np.linalg.norm(self._Nv)
+
+    @Nv.setter
+    def Nv(self, n): 
+        """设置LED法向量 
+        """
+        if not len(n) == 3:
+            raise VLPSequenceLenError(n, 3)
+        self._Nv = n
+
     @property
     def theta(self):  
         """获取半功率点半角 (单位: 度)  
         """  
         return self._theta
 
     @theta.setter
-    def theta(self,t): 
+    def theta(self, t): 
         """设置半功率点半角 (单位: 度)  
         """
         self._theta = t
 
     @property
     def m(self):
         """获取朗伯发射级数 
         """
-        theta_rad = self.theta * np.pi/180
+        theta_rad = np.radians(self.theta) # 角度制转弧度制
         return -np.log(2)/np.log(np.cos(theta_rad))
```

### Comparing `yang-vlp-0.2.8/vlppy/model/pd.py` & `yang-vlp-0.2.9/vlppy/model/pd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import numpy as np
+from numbers import Number
 from .led import LED
 from .room import Room
-from ..error import VLPSequenceLenError
+from ..error import VLPSequenceLenError,VLPValueRangeError
 
 class PD:
+    """光电探测器
+    """
     def __init__(self,
-                n=1.5,
-                fov=60,
-                Ar=1e-4,
-                Ts=1,
+                n:Number=1.5,
+                fov:Number=60,
+                Ar:Number=1e-4,
+                Ts:Number=1,
                 pos:tuple=(0,0,0),
-                alpha=0, 
-                beta=0,
+                alpha:Number=0, 
+                beta:Number=0,
                 *args,
                 **kwargs) -> None:
         """ 
         n: 透镜的折射率
-        fov: 接收视场角 (单位: 度)
+        fov: 接收视场角 (单位: 度) [0,90]
         Ar: PD检测器的接收面积(单位:平方米)
         Ts: 光学滤波器的增益
         pos: PD参考位置(注意:self._pos为参考位置,self.pos为相对位置) 
-        alpha: PD方位角(单位: 度)
-        beta: PD倾斜角(单位: 度)
+        alpha: PD方位角(单位: 度) [0,360]
+        beta: PD倾斜角(单位: 度) [-90,90]
         """
         self.n = n
         self.fov = fov
         self.Ar = Ar
         self.Ts = Ts
 
         self.pos = pos
@@ -43,28 +46,31 @@
             alpha:倾斜PD方位角(单位:度) 
             center_tp_pos: 测试点位置 
         Return
             (xr,yr,zr): 倾斜PD位置
             (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
         """
         # 倾斜PD的方位角和倾斜角
-        alpha_rad = alpha*np.pi/180 # 角度制转弧度制
+        alpha_rad = np.radians(alpha) # 角度制转弧度制
         beta_rad = l/r   # PD倾斜角
-
-        assert 0 <= beta_rad <= np.pi/2 # 限定
+        beta = np.degrees(beta_rad) # 弧度制转角度制
+        
+        if not 0 <= beta <= 90: # 限定
+            raise VLPValueRangeError(beta, 0, 90)
+        
         [x0, y0, z0] = np.array(center_tp_pos, dtype=np.float) #测试点位置
 
         L = r * np.tan(beta_rad/2) * (1 + np.cos(beta_rad)) # 倾斜PD到顶部中心的水平距离
         H = r * np.tan(beta_rad/2) * np.sin(beta_rad)  # 倾斜PD到顶部中心的垂直距离
+
         # 倾斜PD位置
         xr = x0 + L * np.cos(alpha_rad) 
         yr = y0 + L * np.sin(alpha_rad) 
         zr = z0 - H
 
-        beta = np.degrees(beta_rad) # 弧度制转角度制
         return (xr,yr,zr), (alpha,beta) 
 
     @staticmethod
     def tilt_pd_frame(l, alpha, beta, center_tp_pos:tuple):
         """PD支架:倾斜PD和中心参考点位置关系
         Params
             l: 倾斜PD到中心水平PD(参考点)的长度(单位:米)
@@ -73,37 +79,34 @@
             center_tp_pos: 水平中心测试点位置
         Return
             (xr,yr,zr): 倾斜PD位置
             (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
         """
         [x0, y0, z0] = np.array(center_tp_pos, dtype=np.float)  #水平中心测试点位置
         # 倾斜PD的方位角和倾斜角,角度制转弧度制
-        alpha_rad = alpha*np.pi/180
-        beta_rad = beta*np.pi/180
+        alpha_rad, beta_rad = np.radians([alpha, beta])
 
         xr = x0 + l * np.cos(alpha_rad) * np.cos(beta_rad) 
         yr = y0 + l * np.sin(alpha_rad) * np.cos(beta_rad)
         zr = z0 + l * np.sin(beta_rad)
+
         return (xr,yr,zr), (alpha,beta) 
 
     def recv_led_radiation_intensity(self, led:LED):
         """计算LED辐射强度(LOS链路):
         Parameters
             led: LED实例化
         Return 
             LOS链路LED辐射强度
         """
-        pd_pos = np.array(self.pos, dtype=np.float) # PD相对位置
-        led_pos = np.array(led.pos, dtype=np.float) # LED相对位置
-        
-        [xr, yr, zr] = pd_pos  # PD位置坐标矩阵
-        [xt, yt, zt] = led_pos # led位置
-
-        d = np.sqrt((xt-xr)**2 + (yt-yr)**2 + (zt-zr)**2) # LED灯到PD接收器的距离 (l,w,h) 
-        cos_led_t_angle_rad_rad = np.abs(zt - zr) / d # LED发射角的余弦值 (l,w,h)  
+        led_pos = np.stack(led.pos, axis=-1)  # (3,..) -> (..,3)
+        pd_pos = np.stack(self.pos, axis=-1)  # (3,l,w,h) -> (.l,w,h,3)
+        Vt_r = pd_pos - led_pos               # LED到PD的方向向量 (l,w,h，3)
+        d = np.linalg.norm(Vt_r,axis=-1)      # LED到PD的方向向量的模 (l,w,h)
+        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l,w,h)
 
         R0 = ((led.m + 1)  / (2 * np.pi)) * cos_led_t_angle_rad_rad**led.m  # 辐射强度模型 (l,w,h)
 
         # 如果LED发送的是直流信号
         if led.is_dc:
             return R0 * led.send_signal  # LED辐射强度 (l,w,h)
 
@@ -120,118 +123,117 @@
     def recv_los_led_signal(self, led:LED):
         """计算PD接收LED信号(LOS链路):
         Parameters
             led: LED实例化
         Return 
             LOS链路中PD探测器接收LED信号
         """
-        pd_pos = np.array(self.pos,dtype=np.float) # PD相对位置
-        led_pos = np.array(led.pos,dtype=np.float) # LED相对位置
-        
-        [xr, yr, zr] = pd_pos  # PD位置坐标矩阵
-        [xt, yt, zt] = led_pos # led位置
+        # 坐标shape转换,使其可以进行矩阵乘法运算
+        pd_pos = np.stack(self.pos, axis=-1)  # (3,l,w,h) -> (l,w,h,3)
 
-        # PD方位角和倾斜角,角度制转弧度制
-        alpha_rad = self.alpha*np.pi/180
-        beta_rad = self.beta*np.pi/180
+        # LED发射端
+        Vt_r = pd_pos - led.pos                     # LED到PD的方向向量 (l,w,h，3)
+        d = np.linalg.norm(Vt_r,axis=-1)            # 求模:LED到PD的方向向量的模 (l,w,h)
+        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l,w,h)
+
+        # PD接收端
+        Vr_t = -Vt_r # PD到LED的方向向量 (l,w,h，3)
+        cos_pd_r_angle_rad = np.sum(Vr_t*self.Nv, axis=-1) / d     # PD接收角的余弦值 (l,w,h) 
 
-        d = np.sqrt((xt-xr)**2 + (yt-yr)**2 + (zt-zr)**2) # LED灯到PD接收器的距离 (l,w,h) 
-        cos_led_t_angle_rad_rad = np.abs(zt - zr) / d # LED发射角的余弦值 (l,w,h)
-        h = (xt-xr) * np.cos(alpha_rad) * np.sin(beta_rad) + \
-            (yt-yr) * np.sin(alpha_rad) * np.sin(beta_rad) + \
-            (zt-zr) * np.cos(beta_rad) # PD到LED方向向量在PD接收面法向量上的投影 (l,w,h) 
-        cos_pd_r_angle_rad = h / d # PD接收器入射角的余弦值 (l,w,h)   
-          
+        # PD入射角
         pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角的大小(弧度制) (l,w,h)
-        pd_r_angle = np.degrees(pd_r_angle_rad) # 弧度制转为角度制 (l,w,h)
-  
+        pd_r_angle = np.degrees(pd_r_angle_rad)        # 弧度制转为角度制 (l,w,h)
+
+        # 计算信道增益
         H0 = (((led.m + 1) * self.Ar) / (2 * np.pi * d**2)) * cos_led_t_angle_rad_rad**led.m * cos_pd_r_angle_rad * self.Ts * self.G_Con # 信道增益 (l,w,h)
         H0 = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), H0, 0)  # 视场内信道增益 (l,w,h) <=> np.place(H0,(phi>=0)&(phi<=pd.fov),0)
 
         # 以下是为了兼容交直流信号
         """
         H0 = H0.flatten() #打平 (l,w) -> (l*w,)
         return np.array([np.convolve(h,led.send_signal) for h in H0])  #卷积 (l*w,npt)
               <=> np.array([h * led.send_signal for h in H0])          #相乘 (l*w,npt) 
         """
         H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l,w,h) -> (l,w,h,1)  <=> H0.reshape(l,w,h,1) <=> H0[...,np.newaxis]
         recv_signal = H0 * led.signal # PD接收信号 [广播机制 (l,w,h,1) * (npt) -> (l,w,h,npt) * (l,w,h,npt) = (l,w,h,npt)]
         return np.squeeze(recv_signal) # (l,w,h,npt).如果npt==1,则返回形状为(l,w,h)
-
-    
+      
     def recv_nlos_led_signal(self, led:LED, room:Room):
         """计算PD接收LED一次反射信号(NLOS链路):
         Params
             led: LED实例化
             room: Room实例化
         Return 
             NLOS链路中PD探测器接收LED一次反射信号
         """
-        pd_pos = np.array(self.pos,dtype=np.float) # PD相对位置
-        led_pos = np.array(led.pos,dtype=np.float) # LED相对位置
-        
-        # 
-        [xr, yr, zr] = pd_pos  # PD位置坐标矩阵[测试点位于空间区域内:(l,w,h), 测试点位于一个平面区域:(l,w)]
-        [xt, yt, zt] = led_pos # led位置
-        
+        pd_pos = np.asarray(self.pos)
         # 对PD坐标张量扩充两个维度,以便使用广播
-        xr = xr[..., np.newaxis, np.newaxis]  # (l,w,h,1,1) 
-        yr = yr[..., np.newaxis, np.newaxis]  # (l,w,h,1,1)
-        zr = zr[..., np.newaxis, np.newaxis]  # (l,w,h,1,1)
+        pd_pos = pd_pos[..., np.newaxis, np.newaxis]  # (l,w,h,1,1) 
+
+        # 坐标shape转换,使其可以进行矩阵乘法运算
+        pd_pos = np.stack(pd_pos, axis=-1)  # (3,l,w,h,1,1) -> (l,w,h,1,1,3)
 
         H0 = 0  #反射（LOS）链路信道增益
         # 遍历每一面反射墙壁参数:((l1,w1),(l1,w1),(l1,w1)), ((l1,w1),(l1,w1))
         for i, ((xw, yw, zw), (w_alpha, w_beta)) in enumerate(room.get_reflect_wall_args()):
+            # 坐标shape转换,使其可以进行矩阵乘法运算
+            wall_pos = np.stack([xw, yw, zw], axis=-1)  # (3,l1,w1) -> (l1,w1,3)
+
             # 墙壁反射单元的方向角和倾斜角,角度制转弧度制
-            w_alpha_rad = w_alpha*np.pi/180
-            w_beta_rad = w_beta*np.pi/180
+            w_alpha_rad , w_beta_rad = np.radians([w_alpha, w_beta])
+
+            # 墙壁反射单元法向量
+            Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
+            Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
+            Nz = np.cos(w_beta_rad)
+            Nw = np.stack([Nx,Ny,Nz], axis=-1)  # 墙壁法向量 (l1,w1,3)
+            Nw = Nw/np.linalg.norm(Nw)  # 墙壁单位法向量 (l1,w1,3)
 
             # LED -> 墙壁反射单元
-            d1 = np.sqrt((xt-xw)**2 + (yt-yw)**2 + (zt-zw)**2)  # LED灯到墙壁反射单元的距离 (l1,w1)
-            cos_led_t_angle_rad = np.abs(zt - zw) / d1 # LED发射角的余弦值 (l1,w1)
-            h1 = (xt-xw) * np.cos(w_alpha_rad) * np.sin(w_beta_rad) + \
-                 (yt-yw) * np.sin(w_alpha_rad) * np.sin(w_beta_rad) + \
-                 (zt-zw) * np.cos(w_beta_rad)  # 墙壁反射单元到LED方向向量在墙壁反射单元法向量上的投影 (l1,w1)
-            cos_wall_r_angle_rad = h1 / d1 # 墙壁反射单元入射角 (l1,w1)
-            
-            # 墙壁反射单元 -> PD
-            d2 = np.sqrt((xw-xr)**2 + (yw-yr)**2 + (zw-zr)**2)  # 墙壁反射单元到PD之间的距离 (l,w,h,l1,w1)
-            h2 = (xr-xw) * np.cos(w_alpha_rad) * np.sin(w_beta_rad) + \
-                 (yr-yw) * np.sin(w_alpha_rad) * np.sin(w_beta_rad) + \
-                 (zr-zw) * np.cos(w_beta_rad)  # 墙壁反射面到PD方向向量在墙壁反射单元法向量上的投影  (l,w,h,l1,w1)
-
-            # 1.限定d2(除数)不为0 (去掉墙壁反射单元和参考点重合)  2.限定cos_wall_t_angle_rad不小于0 
-            h2 = np.where((d2>0) & (h2>0), h2, 0) # 限定cos_wall_t_angle_rad不小于0，并使得d2中为0的元素（反射点与测试点重合）对应位置上h2元素为0
-            d2 = np.where((d2>0), d2, 1)  # 使得d2中为0的元素等于一个不为0的数,且h2为0,从而cos_wall_t_angle_rad为0
-            cos_wall_t_angle_rad = h2 / d2    # 墙壁反射单元发射角  (l,w,h,l1,w1)
-
-            # PD的方向角和倾斜角,角度制转弧度制
-            alpha_rad = self.alpha*np.pi/180
-            beta_rad = self.beta*np.pi/180
-            h = (xw-xr) * np.cos(alpha_rad) * np.sin(beta_rad) + \
-                (yw-yr) * np.sin(alpha_rad) * np.sin(beta_rad) + \
-                (zw-zr) * np.cos(beta_rad) # PD到墙壁反射单元方向向量在PD接收面法向量上的投影 (l,w,h,l1,w1)
+            # 发射端
+            Vt_w = wall_pos - led.pos  # LED灯到墙壁反射单元的方向向量 (l1,w1,3)
+            d1 = np.linalg.norm(Vt_w, axis=-1) # 求模:LED灯到墙壁反射单元的距离 (l1,w1)
+
+            mark1 = np.all(Vt_w==0, axis=-1) # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l,w,h,l1,w1)
+            d1 = np.where(mark1, 1, d1)      # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1,w1)
+
+            cos_led_t_angle_rad = np.sum(Vt_w*led.Nv, axis=-1) / d1  # LED发射角的余弦值 (l1,w1)
+
+            # 接收端
+            Vw_t = -Vt_w  # 墙壁反射单元到LED灯的方向向量 (l1,w1,3)
+            cos_wall_r_angle_rad = np.sum(Vw_t*Nw, axis=-1) / d1 # 墙壁反射单元入射角 (l1,w1)
 
-            h = np.where((d2>0) & (h>0), h, 0) # 限定cos_pd_r_angle不小于0，并使得d2中为0的元素（反射点与测试点重合）对应位置上h元素为0    
-            cos_pd_r_angle_rad = h / d2 # PD接收角的余弦值   (l,w,h,l1,w1)
+            # 墙壁反射单元 -> PD
+            # 发射端
+            Vw_r = pd_pos - wall_pos # 墙壁反射单元到PD的方向向量   (l,w,h,l1,w1,3)
+            d2 = np.linalg.norm(Vw_r, axis=-1) # 求模:墙壁反射单元到PD之间的距离 (l,w,h,l1,w1)
+
+            mark2 = np.all(Vw_r==0, axis=-1) # 异常点处理:判断墙壁反射单元和参考点是否重合(方向向量是否为零向量) (l,w,h,l1,w1)
+            d2 = np.where(mark2, 1, d2)      # 异常点处理:为使cos_wall_t_angle_rad分母不为0,让墙壁反射单元和参考点重合时的距离不为0
+
+            cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2 # 墙壁反射单元发射角  (l,w,h,l1,w1)
+            cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射入射条件
+
+            # 接收端
+            Vr_w = -Vw_r  # PD到墙壁反射单元的方向向量   (l,w,h,l1,w1,3)
+            cos_pd_r_angle_rad = np.sum(Vr_w*self.Nv, axis=-1) / d2 # PD接收角的余弦值   (l,w,h,l1,w1)
+            cos_pd_r_angle_rad = np.where(cos_pd_r_angle_rad>0, cos_pd_r_angle_rad, 0) # 满足墙壁反射发射条件
 
+            # PD入射角
             pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角(弧度制) (l,w,h,l1,w1)
             pd_r_angle = np.degrees(pd_r_angle_rad) # 弧度制转为角度制 (l,w,h,l1,w1)
 
             rho = room.rho[i]   #墙壁反射率
             Aw = room.Aw[i]     #墙壁反射单元面积
 
-            # 反射(NLOS)链路信道增益 (l,w,h,l1,w1)
+            # 反射(NLOS)子链路信道增益 (l,w,h,l1,w1)
             Hw = (((led.m + 1) * self.Ar) / (2 * np.pi**2 * d1**2 * d2**2)) * rho * Aw * cos_led_t_angle_rad**led.m * cos_wall_r_angle_rad * cos_wall_t_angle_rad *  cos_pd_r_angle_rad * self.Ts * self.G_Con  # 信道增益 
             Hw = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), Hw, 0)  # 视场内信道增益 (l,w,h,l1,w1)
 
-            pd_pos_shape = Hw.shape[:-2] # pd坐标矩阵形状【测试点位于空间区域内:(l,w,h), 测试点位于一个平面区域:(l,w)】
-            l1, w1 = Hw.shape[-2:]    # 墙壁反射单元坐标形状 (l1,w1)
-            Hw = Hw.reshape(*pd_pos_shape, l1*w1)  # 重塑形状 (l,w,h,l1*w1)
-            Hw = np.sum(Hw, axis=-1)     # 墙壁反射面增益 (l,w,h)
+            Hw = np.sum(np.sum(Hw, axis=-1), axis=-1)   # 反射(NLOS)链路信道增益 (l,w,h)
             H0 += Hw  # 墙壁反射(NLOS)链路信道增益(l,w,h)
         
         H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l,w,h) -> (l,w,h,1)  <=> H0.reshape(l,w,h,1) <=> H0[...,np.newaxis]
         recv_signal = H0 * led.signal # PD接收信号[广播机制 (l,w,h,1) * (npt) -> (l,w,h,npt) * (l,w,h,npt) = (l,w,h,npt)]
         return np.squeeze(recv_signal)
     
     def recv_led_signal(self, led:LED, room:Room):
@@ -242,15 +244,15 @@
         Return 
             LOS+NLOS链路中PD探测器接收LED信号
         """
         recv_los_signal = self.recv_los_led_signal(led=led)  # PD接收直射链路信号
         recv_nlos_signal = self.recv_nlos_led_signal(led=led, room=room) # PD接收一次反射链路信号
         return recv_los_signal + recv_nlos_signal
 
-    def shot_noise(self,P,R=0.4,Ibg=5,I2=0.562,B=100,*argv,**kwargv):
+    def shot_noise(self, P, R=0.4, Ibg=5, I2=0.562, B=100, *argv, **kwargv):
         """获取PD散粒噪声功率
         Params
             P: PD接收功率(W)
             R: PD响应度(A/W)
             Ibg: 暗电流(uA)
             I2: 噪声带宽系数
             B: 噪声带宽(MHz)
@@ -258,15 +260,15 @@
             PD散粒噪声功率
         """
         q = 1.6e-19  # 电子电荷量(C)
         # Ibg *= 1e-6  # 单位换算 （1 A = 1e6 uA）
         # B *= 1e6  
         return 2*q*R*P + 2*q*Ibg*I2*B
     
-    def thermal_noise(self,Tk=300,G=10,eta=112,B=100,I2=0.562,I3=0.0868,gamma=1.5,gm=30,*argv,**kwargv):
+    def thermal_noise(self, Tk=300, G=10, eta=112, B=100, I2=0.562, I3=0.0868, gamma=1.5, gm=30, *argv, **kwargv):
         """获取PD热噪声功率
         Params
             Tk: 热力学温度:Tk = T + 273.15°C(K)
             G: 开环电压增益
             eta: PD每单位面积上固定电容(pF/cm2)
             B: 噪声带宽(MHz)
             I2: 噪声带宽系数 
@@ -279,120 +281,139 @@
         k = 1.38e-23  # 玻尔兹曼常数
         eta *= 1e-8 # 单位换算（1pF/cm2 = 1e-8F/m2）
         B *= 1e6
         gm *= 1e-3
         return 8*np.pi*k*Tk/G*eta*self.Ar*I2*B**2 + \
             16*np.pi**2*k*Tk*gamma/gm*eta**2*self.Ar**2*I3*B**3
 
-    def recv_noise_signal(self, *argv,**kwargv):
+    def recv_noise_signal(self, *argv, **kwargv):
         """接收噪声信号功率
         """
         return self.shot_noise(*argv, **kwargv) + self.thermal_noise(*argv, **kwargv)
 
     @property
     def origin(self) -> tuple:
         """设置原点位置
         """
         return self._origin
 
     @origin.setter
-    def origin(self,o):
+    def origin(self, o):
         """获取原点位置
         """
         if not len(o) == 3:
             raise VLPSequenceLenError(o,3)
         self._origin = tuple(o) 
 
     @property
     def pos(self) -> tuple:
         """获取相对位置(参考位置相对与原点的相对位置)
         """
         return tuple(i+j for i,j in zip(self._pos,self.origin))
     
     @pos.setter
-    def pos(self,pos:tuple):
+    def pos(self, pos:tuple):
         """设置参考位置
         """
         if not len(pos) == 3:
             raise VLPSequenceLenError(pos,3)
         self._pos = tuple(pos)
-    
+
+    @property
+    def Nv(self):  
+        """获取PD单位法向量  
+        """  
+        # PD方位角和倾斜角,角度制转弧度制
+        alpha_rad, beta_rad = np.radians([self.alpha, self.beta])
+        
+        Nx = np.cos(alpha_rad) * np.sin(beta_rad)
+        Ny = np.sin(alpha_rad) * np.sin(beta_rad)
+        Nz = np.cos(beta_rad)
+        N = (Nx,Ny,Nz)
+
+        return  N/np.linalg.norm(N) # 单位化
+
     @property
     def alpha(self):
         """获取PD方位角(单位: 度)
         """
         return self._alpha
     
     @alpha.setter
-    def alpha(self,alpha):
+    def alpha(self, alpha):
         """设置PD方位角(单位: 度)
         """
+        if not 0 <= alpha <= 360:
+            raise VLPValueRangeError(alpha,0,360)
         self._alpha = alpha 
 
     @property
     def beta(self):
         """获取PD倾斜角(单位: 度)
         """
         return self._beta
     
     @beta.setter
-    def beta(self,beta):
+    def beta(self, beta):
         """设置PD倾斜角(单位: 度)
         """
+        if not -90 <= beta <= 90:
+            raise VLPValueRangeError(beta,-90,90)
         self._beta = beta 
 
     @property
     def fov(self):
         """获取接收视场角 (单位: 度)
         """    
         return self._fov
 
     @fov.setter
-    def fov(self,fov): 
+    def fov(self, fov): 
         """设置接收视场角 (单位: 度)
         """
-        assert 0 <= fov <= 90
+        if not 0 <= fov <= 90:
+            raise VLPValueRangeError(fov,0,90)
         self._fov = fov
 
     @property
     def Ar(self):   
         """获取PD检测器的接收面积(单位:平方米)
         """ 
         return self._Ar
 
     @Ar.setter
-    def Ar(self,a): 
+    def Ar(self, a): 
         """设置PD检测器的接收面积(单位:平方米)
         """
         self._Ar = a
 
     @property
     def Ts(self):   
         """获取光学滤波器的增益 
         """ 
         return self._Ts
 
     @Ts.setter
-    def Ts(self,ts): 
+    def Ts(self, ts): 
         """设置光学滤波器的增益 
         """
         self._Ts = ts
 
     @property
     def n(self): 
         """获取透镜的折射率
         """   
         return self._n
 
     @n.setter
-    def n(self,n): 
+    def n(self, n): 
         """设置透镜的折射率
         """
         self._n = n
 
     @property
     def G_Con(self):
         """获取聚光器增益
         """
-        fov_rad = self.fov * np.pi/180
+        fov_rad = np.radians(self.fov)
         return self.n**2 / np.sin(fov_rad)**2
```

### Comparing `yang-vlp-0.2.8/vlppy/model/room.py` & `yang-vlp-0.2.9/vlppy/model/room.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
 import numpy as np
 import pandas as pd
 from typing import Sequence,Union
 from numbers import Number
-from ..error import VLPTypeError, VLPSequenceLenError, VLPValueError
-
+from ..error import VLPTypeError, VLPSequenceLenError, VLPValueError,VLPValueRangeError
 
 class Room:
+    """房间
+    坐标系的建立:取房间前侧左下墙角为原点, 前侧左下墙角到右下墙角为x轴方向,\
+        前侧左下墙角到后侧左下墙角为y轴方向, 前侧左下墙角到前侧左上墙角为z轴方向
+    """
     def __init__(self, 
                 length:Number, 
                 width:Number, 
                 height:Number, 
                 tp_gap:Union[Number,Sequence]=0.1,
                 tp_height:Union[Number,Sequence]=0,
                 reflect_wall:Sequence=[], 
@@ -36,18 +39,16 @@
         self.tp_height = tp_height  # 测试区域距离地面的高度
 
         # 在考虑墙壁有反射的情况下，使用以下参数
         self.reflect_wall = reflect_wall  #存储反射墙壁序列号的集合
         self.wall_gap = wall_gap #墙壁划分网格的间隔
         self.rho = rho #墙壁反射率
         
-        self.rp_height = [0, height]   # 前后左右墙反射单元距离地面高度范围
+        self.rp_height = [0, height]   # 前后左右反射墙壁高度范围
 
-        # 原点位置(取房间前侧左下墙角为原点,前侧左下墙角到右下墙角为x轴方向,
-        # 前侧左下墙角到后侧左下墙角为y轴方向,前侧左下墙角到前侧左上墙角为z轴方向)
         self.origin = (0,0,0) #原点位置
         self.wall_args_path = f"wall_args.xlsx" # 默认墙壁参数地址
 
     def _get_reflect_wall_grid(self, gap, wall):
         """得到反射墙壁反射面的网格矩阵
         Params
             gap: 墙壁划分网格的间隔
@@ -78,18 +79,18 @@
         Xw, Yw, Zw = np.squeeze(Xw), np.squeeze(Yw), np.squeeze(Zw) # 去除维数为1的维度
         return (Xw, Yw, Zw)
 
     def _get_reflect_wall_angle(self, grid_shape):
         """获取反射墙壁反射单元(法向量)的方位角和倾斜角
         Return 
             alpha: 方位角(单位:度) (min,max) = (0°,360°)
-            beta: 倾斜角(单位:度)  (min,max) = (-180°,180°)
+            beta: 倾斜角(单位:度)  (min,max) = (-90°,90°)
         """
         alpha = np.random.uniform(low=0, high=360, size=grid_shape)
-        beta = np.random.uniform(low=-180, high=180, size=grid_shape)
+        beta = np.random.uniform(low=-90, high=90, size=grid_shape)
         return alpha, beta
 
     def _save_reflect_wall_args(self, fp:str, reflect_pos:tuple, angle):
         """保存反射墙壁参数(方位角和倾斜角)到excell
         Params 
             fp: 保存路径
             reflect_pos: 墙壁反射单元所在位置
@@ -128,20 +129,20 @@
         xw,yw,zw,alpha,beta = np.split(wall_args,indices_or_sections=5,axis=-1)
         # 加载npz文件
         # with np.load(fp) as f:
         #     xw,yw,zw,alpha,beta = f['xw'],f['yw'],f['zw'],f['alpha'],f['beta']
         return (xw, yw, zw), (alpha, beta)
 
     def set_regular_wall(self):
-        """设置为规制墙壁
+        """设置为规制墙壁 (更新墙壁参数)
         """
-        # 如果前后左右墙反射单元距离地面高度不为0,则无需考虑地面反射
+        # 如果前后左右墙反射单元距离地面最小高度不为0,则无需考虑地面反射
         if self.rp_height[0] > 0 and 0 in self.reflect_wall:
             self.reflect_wall.remove(0)
-        # 如果前后左右墙反射单元与天花板距离不为0,则无需考虑天花板反射
+        # 如果前后左右墙反射单元与天花板最小距离不为0,则无需考虑天花板反射
         if self.rp_height[1] < self.height and 5 in self.reflect_wall:
             self.reflect_wall.remove(5)
 
         for wall in self.reflect_wall:
             (Xw, Yw, Zw) = self._get_reflect_wall_grid(self.wall_gap, wall) #得到反射面的网格矩阵
             grid_shape = Xw.shape # 获取矩阵形状
             fpath = self.wall_args_path.format(wall) #默认路径
@@ -152,19 +153,19 @@
         """获取墙壁参数
         params
             无
         Return
             [((Xw, Yw, Zw), (alpha, beta)),...]: 
                     反射墙壁网格坐标矩阵和反射单元方向角和倾斜角(列表元素个数等于反射墙壁的个数)
         """
-        # 如果前后左右墙反射单元距离地面高度不为0,则无需考虑地面反射
+        # 如果前后左右墙反射单元距离地面最小高度不为0,则无需考虑地面反射
         if self.rp_height[0] > 0 and 0 in self.reflect_wall:
             self.reflect_wall.remove(0)
             self.Aw.remove(self.reflect_wall.index(0))
-        # 如果前后左右墙反射单元与天花板距离不为0,则无需考虑天花板反射
+        # 如果前后左右墙反射单元与天花板最小距离不为0,则无需考虑天花板反射
         if self.rp_height[1] < self.height and 5 in self.reflect_wall:
             self.reflect_wall.remove(5)
             self.Aw.remove(self.reflect_wall.index(5))
 
         reflect_wall_args = []  # 反射墙壁网格坐标矩阵和反射单元方向角和倾斜角
         for wall in self.reflect_wall:
             (Xw, Yw, Zw) = self._get_reflect_wall_grid(self.wall_gap, wall) #得到反射面的网格矩阵
@@ -243,15 +244,15 @@
     @property
     def origin(self) -> tuple:
         """获取原点
         """
         return self._origin
 
     @origin.setter
-    def origin(self,o):
+    def origin(self, o):
         """设置原点
         """
         if not len(o) == 3:
             raise VLPSequenceLenError(o,3)
         self._origin = tuple(o)
 
     @property
@@ -284,18 +285,19 @@
     def tp_gap(self, gap:Union[Number, Sequence]):
         """设置测试区域划分网格的间隔
         """
         if not isinstance(gap,(Number ,Sequence)): #类型
             raise VLPTypeError(gap, Number, Sequence)
 
         # 测试点平面划分网格的间隔限制
-        gap = np.array(gap)
-        assert gap.size in (1,3)
+        gap = np.asarray(gap)
+        if not gap.size in (1,3):
+            raise VLPValueError(gap.size,1,3)
         if not np.all((gap>0) & (gap<self.size)):
-            raise Exception("The gap setting is not reasonable!")
+            raise VLPValueRangeError(gap, 0, self.size) # The gap setting is not reasonable!
         if gap.size == 1:
             gap = np.full(shape=(3), fill_value=gap) # 填充
         self._tp_gap = gap
 
     @property
     def tp_grid_pos(self) -> tuple:
         """获取测试点位置的网格矩阵(所有测试点的相对位置)
@@ -318,19 +320,20 @@
     
     @wall_gap.setter
     def wall_gap(self, gap:Union[Number, Sequence]):
         """设置墙壁划分网格的间隔
         """
         if not isinstance(gap,(Number, Sequence)): #类型
             raise VLPTypeError(gap, Number, Sequence)
-        gap = np.array(gap)
-        assert gap.size in (1,3)
-        # 测试点平面划分网格的间隔限制
+        gap = np.asarray(gap)
+        if not gap.size in (1,3):
+            raise VLPValueError(gap.size,1,3)
+        # 墙壁划分反射单元网格的间隔限制
         if not np.all((gap>0) & (gap<self.size)):
-            raise Exception("The gap setting is not reasonable!")
+            raise VLPValueRangeError(gap, 0, self.size) # The gap setting is not reasonable!
         if gap.size == 1:
             gap = np.full(shape=(3), fill_value=gap)
         self._wall_gap = gap 
 
     @property
     def reflect_wall(self) -> list:
         """获取存储反射墙壁序列号的列表
@@ -352,16 +355,17 @@
     
     @rho.setter
     def rho(self, n:Union[Number, Sequence]):
         """设置墙壁反射率
         """
         if not isinstance(n, (Number, Sequence)): #类型
             raise VLPTypeError(n, Number, Sequence)
-        n = np.array(n)
-        assert n.size == 1 or n.size == self.reflect_wall.size #断言：实际反射墙壁个数与反射面折射率个数需相等
+        n = np.asarray(n)
+        if not n.size in (1, self.reflect_wall.size): # 实际反射墙壁个数与反射面折射率个数需相等或全部相同
+            raise VLPValueError(n.size, 1, self.reflect_wall.size)
         if n.size == 1:
             n = np.full(shape=(self.reflect_wall.size), fill_value=n) # 填充
         self._rho = n
 
     @property
     def Aw(self):
         """获取墙壁反射单元面积
@@ -384,15 +388,16 @@
         return self._rp_height
     
     def rp_height(self, h:Sequence):
         """设置前后左右墙反射面距离地面高度范围
         """
         if not isinstance(h, Sequence):
             raise VLPTypeError(h, Sequence)
-        assert len(h) == 2
+        if not len(h) == 2:
+            raise VLPSequenceLenError(h,2)
         assert 0 <= h[0] <= h[1] <= self.height # 对取h的反射面距离地面高度限制
         self._rp_height = h
 
     @property
     def wall_args_path(self):
         """获取墙壁参数保存地址
         """
```

### Comparing `yang-vlp-0.2.8/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.9/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/setting/json_setting.py` & `yang-vlp-0.2.9/vlppy/setting/json_setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     if getattr(sys, 'frozen', False):
         _abspath = os.path.dirname(os.path.abspath(sys.executable))
     elif __file__:
         _abspath = os.path.dirname(os.path.abspath(__file__)) # current file dir
     _file_name = "settings.json"
     
     # INIT SETTINGS
-    def __init__(self,settings_path:str=...):
+    def __init__(self, settings_path:str=...):
         """set file path
         settings_path: .json file path or directory(include settings.json)
                         default: settings.json file in the directory where the current file resides
         """
         super(Settings, self).__init__()
         # set file path
         self.set_settings_path(settings_path)
@@ -24,15 +24,15 @@
         # DICTIONARY WITH SETTINGS
         # Just to have objects references
         self.items = {}
 
         # DESERIALIZE
         self.deserialize() # 从文件中加载json数据,转为dict型数据,赋值给self.items
 
-    def set_settings_path(self,settings_path:str=...):
+    def set_settings_path(self, settings_path:str=...):
         """set file path
         settings_path: settings.json file path or directory
         """
         settings_path = settings_path if settings_path != Ellipsis else self._abspath
         settings_path = os.path.abspath(os.path.normpath(settings_path)) #规范路径中'//'为'/'
 
         if settings_path.endswith(".json"):
@@ -43,35 +43,35 @@
         if not os.path.exists(self._settings_path):
             sys.exit(f"WARNING: \".json\" file not found! check in the path \"{self._settings_path}\"")
     
     def get_settings_path(self) -> str: 
         return self._settings_path
 
     # 去除json中注释 "//"、"/**/"
-    def _parse_json(self,json_raw):
+    def _parse_json(self, json_raw):
         """Remove json comments "//", "/* */"
         json_raw: raw json
         """
         try:
             json_str1 = re.sub(re.compile('(//[\\s\\S]*?\n)'),'',json_raw)
             json_str2 = re.sub(re.compile('(/\*[\\s\\S]*?\*/)'),'',json_str1)
             return json.loads(json_str2)
         except:
             raise Exception("Remove json comments error!")
 
     # 序列化:将字典型数据转为json，并保存到文件
-    def serialize(self,filepath=...):
+    def serialize(self, filepath=...):
         if filepath is Ellipsis:
             filepath = self._settings_path
         # WRITE JSON FILE
         with open(filepath, "w", encoding='utf-8') as fd:
             json.dump(self.items, fd, indent=4)
 
     # 反序列化:从文件中加载json数据，并转为dict型数据
-    def deserialize(self,filepath=...):
+    def deserialize(self, filepath=...):
         if filepath is Ellipsis:
             filepath = self._settings_path
         # READ JSON FILE
         with open(filepath, "r", encoding='utf-8') as fd:
             self.items = self._parse_json(fd.read())
```

### Comparing `yang-vlp-0.2.8/vlppy/setting/settings.json` & `yang-vlp-0.2.9/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/signal/filter.py` & `yang-vlp-0.2.9/vlppy/signal/filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typing
 from scipy import signal
 import numpy as np
 import matplotlib.pyplot as plt
+from ..error import VLPValueError
+
 
 class BandFilter:
-    def __init__(self,n,fs,fm,w=2,*args,**kwargs) -> None:
+    def __init__(self, n, fs, fm, w=2, *args, **kwargs) -> None:
         """理想带通滤波器
         n: 采样点数
         fs: 采样频率
         fm: 滤波器频率
         w: 通带到中心的距离 阻带为距离 w+Fd(频率间隔)
         """
         self.N = n # 采样点数
@@ -17,47 +19,51 @@
         self.t = np.arange(n) / fs # 时间序列
         self.fftfreq = np.fft.fftfreq(n,1/fs)  # 频率序列
         self.fm = fm  # 滤波频率
         self.W = w  # 通带宽度
         self.window_fft = self._window(w) # 窗函数
         self.window = np.fft.ifft(self.window_fft) # 窗函数的逆fft
 
-    def _window(self,w):
+    def _window(self, w):
         """
         # 窗函数(fft) lim:通带宽度
         """
         condition = (np.abs(self.fftfreq)>self.fm-w)&(np.abs(self.fftfreq)<self.fm+w)
         return np.where(condition,1,0)
 
     # 滤波
-    def filter(self,signal):
+    def filter(self, signal):
         fft_signal = np.fft.fft(signal)
         fft_signal_filter = fft_signal * self.window_fft
         signal_filter = np.fft.ifft(fft_signal_filter)
         return signal_filter,fft_signal_filter
 
 class BaseFilter:
-    def __init__(self,fc,fs,D:list=[100,200],G:list=[2,35],btype='bandpass',analog=False,*args,**kwargs) -> None:
+    def __init__(self, fc, fs, D:list=[100,200], G:list=[2,35], btype='bandpass', analog=False, *args, **kwargs) -> None:
         """滤波器基类
         fc: 截止频率
         fs: 采样频率
         D:  [通带到中心的距离(单边通带宽度),阻带到中心的距离(单边阻带宽度)]
         G: 通带增益,阻带衰减
+        btype: 滤波器类型,可选['lowpass', 'highpass', 'bandpass', 'bandstop']
         analog: 为True是模拟滤波器,为False是数字滤波器
         """
+        if not btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
+
         self.Fc = fc # 滤波频率
         self.Fs = fs
         Pd,Sd = D[0],D[1]
         self.Wp = np.array([fc-Pd,fc+Pd])/(fs/2) # 通带频率 
         self.Ws = np.array([fc-Sd,fc+Sd])/(fs/2) # 阻带频率
         self.gp,self.gs = G[0],G[1]
         self.btype = btype
         self.analog = analog
 
-    def show_wave(self,N,whole=False,savepath=...,showfig=True):
+    def show_wave(self, N, whole=False, savepath=..., showfig=True):
         """显示幅频响应波形、相频响应波形
         N: 采样点数
         whole: 单边还是全部
         """
         if self.analog:
             w,h = signal.freqs(self.b,self.a)
         else:
@@ -75,111 +81,121 @@
         ax[1].set_ylabel('Pha:du')
         ax[1].set_title('f-Arc') # 相频响应波形
         if savepath != ...:
             plt.savefig(savepath)
         if showfig:
             plt.show()
 
-    def filter(self,x,lfilter=False):
+    def filter(self, x, lfilter=False):
         """滤波
         x: 滤波信号
         lfilter: 为True使用lfilter滤波;为False使用filtfilt滤波
                  lfilter 滤波后的波形有偏移,filtfilt滤波后的没有偏移
         """
         return signal.lfilter(self.b,self.a,x) if lfilter else signal.filtfilt(self.b,self.a,x)
 
 class ButterFilter(BaseFilter):
-    def __init__(self,fc,fs,D:list=[100,200],G:list=[2,35],btype='bandpass',analog=False,*args,**kwargs) -> None:
+    def __init__(self, fc, fs, D:list=[100,200], G:list=[2,35], btype='bandpass', analog=False, *args, **kwargs) -> None:
         """巴特沃斯带通滤波器
         fc: 截止频率
         fs: 采样频率
         D: [通带到中心的距离(单边通带宽度),阻带到中心的距离(单边阻带宽度)]
         G: 通带增益,阻带衰减
+        btype: 滤波器类型,可选['lowpass', 'highpass', 'bandpass', 'bandstop']
         analog: 为True是模拟滤波器,为False是数字滤波器
         """
+        if not btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
+        
         super(ButterFilter,self).__init__(fc,fs,D,G,btype,analog,*args,**kwargs)
         n, Wn = signal.buttord(self.Wp, self.Ws, self.gp, self.gs,analog=self.analog) # 返回巴特沃斯滤波器最小阶n和截止频率Wn
         self.b, self.a = signal.butter(n, Wn, btype='bandpass', analog=self.analog) # 返回归一化截止频率Wn的n阶巴特沃斯滤波器的传递函数系数
 
 class ChebyFilter(BaseFilter):
-    def __init__(self,fc,fs,D:list=[100,200],G:list=[2,35],btype='bandpass',analog=False,cheby=1,*args,**kwargs):
+    def __init__(self, fc, fs, D:list=[100,200], G:list=[2,35], btype='bandpass', analog=False, cheby=1, *args, **kwargs):
         """切比雪夫滤波器
         Params
             fc: 截止频率
             fs: 采样率
             D: [通带到中心的距离(单边通带宽度),阻带到中心的距离(单边阻带宽度)]
             G: 通带增益,阻带衰减
             btype: 滤波器类型,可选['lowpass', 'highpass', 'bandpass', 'bandstop']
             analog: 为True是模拟滤波器,为False是数字滤波器
             cheby: 为1时,为切比雪夫I型滤波器;为2时,为切比雪夫II型滤波器
         """
-        assert btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']
-        assert cheby in [1,2]
+        if not btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
+        if not cheby in [1,2]:
+            raise VLPValueError(cheby, 1, 2)
+
         super(ChebyFilter,self).__init__(fc,fs,D,G,btype,analog,*args,**kwargs)
         if cheby == 1:
             ripple = self.gp
             filter_ord = signal.cheb1ord
             filter_func = signal.cheby1
         else:
             ripple = self.gs
             filter_ord = signal.cheb2ord
             filter_func = signal.cheby2
 
         n, Wn = filter_ord(self.Wp, self.Ws, self.gp, self.gs,analog=analog) # 返回滤波器最小阶n和截止频率Wn
         self.b, self.a = filter_func(n, ripple, Wn, btype=self.btype, analog=analog)
 
 class EllipFilter(BaseFilter):
-    def __init__(self,fc,fs,D:list=[100,200],G:list=[2,35],btype='bandpass',analog=False,*args,**kwargs) -> None:
+    def __init__(self, fc, fs, D:list=[100,200], G:list=[2,35], btype='bandpass', analog=False, *args, **kwargs) -> None:
         """椭圆滤波器
         fc: 截止频率
         fs: 采样频率
         D: [通带到中心的距离(单边通带宽度),阻带到中心的距离(单边阻带宽度)]
         G: 通带增益,阻带衰减
         btype: 滤波器类型,可选['lowpass', 'highpass', 'bandpass', 'bandstop']
         analog: 为True是模拟滤波器,为False是数字滤波器
         """
-        assert btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']
+        if not btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
         super(EllipFilter,self).__init__(fc,fs,D,G,btype,analog,*args,**kwargs)
 
         n, Wn = signal.ellipord(self.Wp, self.Ws, self.gp, self.gs,analog=self.analog) # 返回巴特沃斯滤波器最小阶n和截止频率Wn
         rp,rs = self.gp,self.gs
         self.b, self.a = signal.ellip(n, rp, rs, Wn, btype=self.btype,analog=self.analog) # 返回归一化截止频率Wn的n阶巴特沃斯滤波器的传递函数系数
 
 class BesselFilter(BaseFilter):
-    def __init__(self,fc,fs,n,Wn:typing.Union[int,list],btype='bandpass',analog=False,*args,**kwargs) -> None:
+    def __init__(self, fc, fs, n, Wn:typing.Union[int,list], btype='bandpass', analog=False, *args, **kwargs) -> None:
         """贝塞尔滤波器
         fc: 截止频率
         fs: 采样频率
         n: 滤波器阶数
         wn: 单边通带宽度
         btype:滤波器类型,可选['lowpass', 'highpass', 'bandpass', 'bandstop']
         analog:为True是模拟滤波器,为False是数字滤波器
         """
-        assert btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']
+        if not btype in ['lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
         super(BesselFilter,self).__init__(fc,fs,btype=btype,analog=analog,*args,**kwargs)
         if np.array(Wn).size == 2:
             Wn = np.array([fc-Wn[0],fc+Wn[1]]) / (fs/2)
         else:
             Wn = Wn if btype in ['lowpass', 'highpass'] else np.array([fc-Wn,fc+Wn]) / (fs/2)
         self.b, self.a = signal.bessel(n, Wn, btype=self.btype,analog=self.analog) # 返回归一化截止频率Wn的n阶巴特沃斯滤波器的传递函数系数
 
 class FIR_Filter(BaseFilter):
-    def __init__(self,fc,fs,n,Wp,window='hamming',btype='bandpass',*args,**kwargs) -> None:
+    def __init__(self, fc, fs, n, Wp, window='hamming', btype='bandpass', *args, **kwargs) -> None:
         """Fir滤波器
         Params
             fc:截止频率
             fs:采样率
             n:滤波器阶数(越大越好)
             Wp:单边通带宽度
             window:窗函数,可选["barthann","bartlett","blackman","blackmanharris","bohman","boxcar","chebwin","cosine",
                         "dpss","exponential","flattop""gaussian","general_cosine","general_gaussian","general_hamming",
                         "hamming","hann","hanning","kaiser","nuttall","parzen","taylor","triang","tukey"]
             btype:滤波器类型,可选[True, False,'lowpass', 'highpass', 'bandpass', 'bandstop']
         """
-        assert btype in [True, False, 'lowpass', 'highpass','bandpass', 'bandstop']
+        if not btype in [True, False, 'lowpass', 'highpass', 'bandpass', 'bandstop']:
+            raise VLPValueError(btype, 'lowpass', 'highpass', 'bandpass', 'bandstop')
         super(FIR_Filter,self).__init__(fc,fs,btype=btype,analog=False,*args,**kwargs)
         if np.array(Wp).size == 2:
             Wp = np.array([fc-Wp[0],fc+Wp[1]])/(fs/2)
         else:
             Wp = np.array([fc-Wp,fc+Wp])/(fs/2) if btype in ['bandpass', 'bandstop'] else Wp/ (fs/2) 
         # window = signal.windows.boxcar(n)
         # window = signal.get_window('boxcar',n)
```

### Comparing `yang-vlp-0.2.8/vlppy/signal/plot.py` & `yang-vlp-0.2.9/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.8/vlppy/vis/vis.py` & `yang-vlp-0.2.9/vlppy/vis/vis.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,73 +14,92 @@
     assert len(pred) == len(true) 
     pred = np.asarray(pred)
     # (n,2) or (n,3) -> (2,n) or (3,n)
     if pred.shape[-1] in (2,3):
         pred = np.transpose(pred)
         true = np.transpose(true)
     if pred.shape[0] == 2:
-        plt.plot(*pred,'ro')
-        plt.plot(*true,'b*')
+        plt.scatter(*pred, c='none',facecolors='none',edgecolors='r',linewidths=1)
+        plt.scatter(*true, c='k',marker='+',linewidths=1)
     elif pred.shape[0] == 3:
         ax = plt.axes(projection='3d')
-        ax.scatter3D(*pred, c='r',marker="o")
-        ax.scatter3D(*true, c='b',marker="*")
-    else:
-        plt.plot(pred,'ro')
-        plt.plot(true,'b*')
+        ax.scatter3D(*pred, c='none',facecolors='none',edgecolors='r',linewidths=1)
+        ax.scatter3D(*true, c='k',marker='+',linewidths=1)
+    else: 
+        plt.scatter(pred, c='none',linewidths=1, facecolors='none',edgecolors='r')
+        plt.scatter(true, c='k', marker='+',linewidths=1)
     plt.title(title)
-    plt.legend(['pred','true'])
+    plt.legend(['Predicted position','Actual position'])
     if savepath != ...:
         plt.savefig(savepath)
     if showfig:
         plt.show()
 
-
 def draw_history(history,title="history",savepath=...,showfig=True):
     """绘制网络模型训练过程参数变换图
     Params
         history: 历史值
         title: 标题
         savepath: 保存路径
         showfig: 是否显示图例
     """
     data = pd.DataFrame(history)
     data.plot(figsize=(8,5))
     plt.grid(True)
     plt.title(title)
-    plt.xlabel("iter")
+    plt.xlabel("Iter")
+    if savepath != ...:
+        plt.savefig(savepath)
+    if showfig:
+        plt.show()
+
+def draw_error_hist(error,bins=10,rwidth=0.6,title="",savepath=...,showfig=True):
+    """绘制误差分布直方图
+    """
+    # 解决中文乱码
+    plt.rcParams["font.sans-serif"]=["SimHei"] #设置字体
+    plt.rcParams["axes.unicode_minus"]=False #该语句解决图像中的“-”负号的乱码问题
+    fre_tuple = plt.hist(error, bins=bins, rwidth=rwidth, align='left')
+    # 绘制统计文本
+    [plt.text(y, x, f'{int(x)}', ha='center', va= 'bottom', fontsize=10) for x,y in zip(*fre_tuple[:2])]
+    plt.title(title)
+    plt.xlabel("Position error")
+    plt.ylabel("The number of position error")
+
     if savepath != ...:
         plt.savefig(savepath)
     if showfig:
         plt.show()
+    return fre_tuple
 
 def cdfplot(error,title="",savepath=...,showfig=True):
-    """绘制误差积累分布图CDF
+    """绘制经验误差积累分布图CDF
     Params 
         error: 误差数组
         title: 标题
         savepath: 保存路径
         showfig: 是否显示图例
     """
-    x = np.array(error)
+    assert len(error) > 1
+    x = np.asarray(error,dtype=np.float)
     x = x[~np.isnan(x)]     #去除nan
     x = np.sort(x)          #排序
     n = len(x)              
     y = np.arange(1,n+1)/n  #返回1/n步进到1
     notdup = [x[i]-x[i-1]>0 for i in range(1,len(x))]  #返回梯度布尔值
     notdup.append(True) 
-    xx = x[notdup]             #去除重复元素
-    yy = np.array([0,*y[notdup]])  #在第一位置上插入一个0
-    m = np.repeat(np.arange(1,len(xx)+1),2)  #在第0轴上复制元素
-    xCDF = np.array([-np.inf,*xx[m-1],np.inf]) #前后延申
+    xx = x[notdup]          #去除重复元素
+    yy = np.insert(y[notdup],0,0) #在第一位置上插入一个0
+    m = np.repeat(np.arange(len(xx)),2)  #在第0轴上复制元素
+    xCDF = np.array([-np.inf,*xx[m],np.inf]) #前后延申
     yCDF = np.array([0,0,*yy[m]]) #在第一位置上插入两个0
-
+    
     plt.plot(xCDF,yCDF)  #绘图
     plt.title(title)
-    plt.xlabel("position error")
+    plt.xlabel("Position error")
     plt.ylabel("CDF")
 
     if savepath != ...:
         plt.savefig(savepath)
     if showfig:
         plt.show()
     return xCDF,yCDF
```

### Comparing `yang-vlp-0.2.8/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.9/yang_vlp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,40 +25,43 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://gitee.com/yangwuju/yang_vlp
 Project-URL: Bug Tracker, https://gitee.com/yangwuju/yang_vlp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 @start date:  2022-08-26
 
 @auther:  yang wu ju
 
 @url: https://gitee.com/yangwuju/yang_vlp
 
 @file:
 
 - model/room： 房间、墙壁参数
-- model/led:  led位置、发射的信号
-- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号
+- model/led:  led位置、发射的信号(None、DC、AC、AIM)
+- model/pd:  pd 各种参数、LOS链路和NLOS链路接收LED信号、噪声
 - signal/filter:  滤波器设计（包括fir,iir）
 - signal/plot: 绘制波形图
 - demo/vlp_model: 可见光定位模型
 - demo/demo_main: test demo
 - io/io: 数据保存与加载
 - setting/json_setting: 加载json配置文件
 - error/error: VLP常见异常
 - vis/vis: 可视化绘图
+- tools/decorator:VLP可能用到的装饰器
 
-@Download
+@download
 
 ```
 py -m pip install yang-vlp
 ```
 
 @updata log
 
 将测试平面更新为测试空间区域，可以实现3d定位仿真;
+
+优化部分代码；
```

### Comparing `yang-vlp-0.2.8/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.9/yang_vlp.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.py
 vlppy/LICENSE.txt
 vlppy/__init__.py
 vlppy/info.py
 vlppy/.vscode/settings.json
+vlppy/demo/README.md
 vlppy/demo/__init__.py
 vlppy/demo/demo_filter.py
 vlppy/demo/demo_main.py
 vlppy/demo/vlp_model.py
 vlppy/demo/__pycache__/__init__.cpython-39.pyc
 vlppy/demo/__pycache__/demo_main.cpython-39.pyc
 vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
@@ -31,14 +32,16 @@
 vlppy/setting/json_setting.py
 vlppy/setting/settings.json
 vlppy/setting/__pycache__/__init__.cpython-39.pyc
 vlppy/setting/__pycache__/json_setting.cpython-39.pyc
 vlppy/signal/__init__.py
 vlppy/signal/filter.py
 vlppy/signal/plot.py
+vlppy/tools/__init__.py
+vlppy/tools/decorator.py
 vlppy/vis/__init__.py
 vlppy/vis/vis.py
 yang_vlp.egg-info/PKG-INFO
 yang_vlp.egg-info/SOURCES.txt
 yang_vlp.egg-info/dependency_links.txt
 yang_vlp.egg-info/requires.txt
 yang_vlp.egg-info/top_level.txt
```

