# Comparing `tmp/osin-1.9.1.tar.gz` & `tmp/osin-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osin-1.9.1.tar", max compression
+gzip compressed data, was "osin-1.9.2.tar", max compression
```

## Comparing `osin-1.9.1.tar` & `osin-1.9.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1064 2022-12-13 23:27:28.877276 osin-1.9.1/LICENSE
--rw-r--r--   0        0        0     1367 2022-12-13 23:27:28.877276 osin-1.9.1/README.md
--rw-r--r--   0        0        0       93 2022-12-13 23:27:28.877276 osin-1.9.1/osin/__init__.py
--rw-r--r--   0        0        0     1705 2022-12-13 23:27:28.877276 osin-1.9.1/osin/__main__.py
--rw-r--r--   0        0        0        0 2022-12-13 23:27:28.877276 osin-1.9.1/osin/apis/__init__.py
--rw-r--r--   0        0        0     2050 2022-12-13 23:27:28.877276 osin-1.9.1/osin/apis/local_osin.py
--rw-r--r--   0        0        0    11582 2022-12-13 23:27:28.877276 osin-1.9.1/osin/apis/osin.py
--rw-r--r--   0        0        0     1815 2022-12-13 23:27:28.877276 osin-1.9.1/osin/apis/remote_exp.py
--rw-r--r--   0        0        0     6226 2022-12-13 23:27:28.877276 osin-1.9.1/osin/apis/remote_osin.py
--rw-r--r--   0        0        0      865 2022-12-13 23:27:28.877276 osin-1.9.1/osin/app.py
--rw-r--r--   0        0        0      243 2022-12-13 23:27:28.877276 osin-1.9.1/osin/config.py
--rw-r--r--   0        0        0        0 2022-12-13 23:27:28.877276 osin-1.9.1/osin/controllers/__init__.py
--rw-r--r--   0        0        0     4636 2022-12-13 23:27:28.877276 osin-1.9.1/osin/controllers/exp.py
--rw-r--r--   0        0        0    10281 2022-12-13 23:27:28.877276 osin-1.9.1/osin/controllers/report.py
--rw-r--r--   0        0        0      195 2022-12-13 23:27:28.877276 osin-1.9.1/osin/controllers/views.py
--rw-r--r--   0        0        0       41 2022-12-13 23:27:28.877276 osin-1.9.1/osin/formats/__init__.py
--rw-r--r--   0        0        0     9776 2022-12-13 23:27:28.877276 osin-1.9.1/osin/formats/hdf5.py
--rw-r--r--   0        0        0        0 2022-12-13 23:27:28.877276 osin-1.9.1/osin/integrations/__init__.py
--rw-r--r--   0        0        0     2658 2022-12-13 23:27:28.877276 osin-1.9.1/osin/integrations/ream.py
--rw-r--r--   0        0        0     2798 2022-12-13 23:27:28.877276 osin-1.9.1/osin/misc.py
--rw-r--r--   0        0        0      459 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/__init__.py
--rw-r--r--   0        0        0      904 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/base.py
--rw-r--r--   0        0        0     2711 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/exp.py
--rw-r--r--   0        0        0     1073 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/exp_data.py
--rw-r--r--   0        0        0        0 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/migration/__init__.py
--rw-r--r--   0        0        0      795 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/migration/v_1_6_2_1_7_0.backup
--rw-r--r--   0        0        0      536 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report/__init__.py
--rw-r--r--   0        0        0     5450 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report/auto_table.py
--rw-r--r--   0        0        0     3238 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report/base_report.py
--rw-r--r--   0        0        0     1802 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report/dbmodel.py
--rw-r--r--   0        0        0    15138 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report/index_schema.py
--rw-r--r--   0        0        0     6765 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/report.py.backup
--rw-r--r--   0        0        0      411 2022-12-13 23:27:28.877276 osin-1.9.1/osin/models/views.py
--rw-r--r--   0        0        0     1119 2022-12-13 23:27:28.877276 osin-1.9.1/osin/params_helper.py
--rw-r--r--   0        0        0     2348 2022-12-13 23:27:28.877276 osin-1.9.1/osin/repository.py
--rw-r--r--   0        0        0      294 2022-12-13 23:27:28.881276 osin-1.9.1/osin/types/__init__.py
--rw-r--r--   0        0        0     2204 2022-12-13 23:27:28.881276 osin-1.9.1/osin/types/param_schema.py
--rw-r--r--   0        0        0     3845 2022-12-13 23:27:28.881276 osin-1.9.1/osin/types/primitive_type.py
--rw-r--r--   0        0        0     1983 2022-12-13 23:27:28.881276 osin-1.9.1/osin/types/pyobject.py
--rw-r--r--   0        0        0     3953 2022-12-13 23:27:28.881276 osin-1.9.1/osin/types/pyobject_type.py
--rw-r--r--   0        0        0      562 2022-12-13 23:27:28.881276 osin-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 osin-1.9.1/setup.py
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 osin-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-26 08:13:34.023654 osin-1.9.2/LICENSE
+-rw-r--r--   0        0        0     1367 2022-12-26 08:13:34.023654 osin-1.9.2/README.md
+-rw-r--r--   0        0        0       93 2022-12-26 08:13:34.023654 osin-1.9.2/osin/__init__.py
+-rw-r--r--   0        0        0     1705 2022-12-26 08:13:34.023654 osin-1.9.2/osin/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-26 08:13:34.023654 osin-1.9.2/osin/apis/__init__.py
+-rw-r--r--   0        0        0     2050 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/local_osin.py
+-rw-r--r--   0        0        0    11582 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/osin.py
+-rw-r--r--   0        0        0     1815 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/remote_exp.py
+-rw-r--r--   0        0        0     6226 2022-12-26 08:13:34.027654 osin-1.9.2/osin/apis/remote_osin.py
+-rw-r--r--   0        0        0      865 2022-12-26 08:13:34.027654 osin-1.9.2/osin/app.py
+-rw-r--r--   0        0        0      243 2022-12-26 08:13:34.027654 osin-1.9.2/osin/config.py
+-rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/__init__.py
+-rw-r--r--   0        0        0     4636 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/exp.py
+-rw-r--r--   0        0        0    10281 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/report.py
+-rw-r--r--   0        0        0      195 2022-12-26 08:13:34.027654 osin-1.9.2/osin/controllers/views.py
+-rw-r--r--   0        0        0       41 2022-12-26 08:13:34.027654 osin-1.9.2/osin/formats/__init__.py
+-rw-r--r--   0        0        0     9776 2022-12-26 08:13:34.027654 osin-1.9.2/osin/formats/hdf5.py
+-rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/integrations/__init__.py
+-rw-r--r--   0        0        0     2658 2022-12-26 08:13:34.027654 osin-1.9.2/osin/integrations/ream.py
+-rw-r--r--   0        0        0     2798 2022-12-26 08:13:34.027654 osin-1.9.2/osin/misc.py
+-rw-r--r--   0        0        0      459 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/__init__.py
+-rw-r--r--   0        0        0      904 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/base.py
+-rw-r--r--   0        0        0     2711 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/exp.py
+-rw-r--r--   0        0        0     1073 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/exp_data.py
+-rw-r--r--   0        0        0        0 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/migration/__init__.py
+-rw-r--r--   0        0        0      795 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/migration/v_1_6_2_1_7_0.backup
+-rw-r--r--   0        0        0      536 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/__init__.py
+-rw-r--r--   0        0        0     5450 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/auto_table.py
+-rw-r--r--   0        0        0     3238 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/base_report.py
+-rw-r--r--   0        0        0     1802 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/dbmodel.py
+-rw-r--r--   0        0        0    15138 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report/index_schema.py
+-rw-r--r--   0        0        0     6765 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/report.py.backup
+-rw-r--r--   0        0        0      411 2022-12-26 08:13:34.027654 osin-1.9.2/osin/models/views.py
+-rw-r--r--   0        0        0     1119 2022-12-26 08:13:34.027654 osin-1.9.2/osin/params_helper.py
+-rw-r--r--   0        0        0     2348 2022-12-26 08:13:34.027654 osin-1.9.2/osin/repository.py
+-rw-r--r--   0        0        0      294 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/__init__.py
+-rw-r--r--   0        0        0     2204 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/param_schema.py
+-rw-r--r--   0        0        0     3845 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/primitive_type.py
+-rw-r--r--   0        0        0     1983 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/pyobject.py
+-rw-r--r--   0        0        0     3953 2022-12-26 08:13:34.027654 osin-1.9.2/osin/types/pyobject_type.py
+-rw-r--r--   0        0        0      562 2022-12-26 08:13:34.027654 osin-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 osin-1.9.2/setup.py
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 osin-1.9.2/PKG-INFO
```

### Comparing `osin-1.9.1/LICENSE` & `osin-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/README.md` & `osin-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/__main__.py` & `osin-1.9.2/osin/__main__.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/apis/local_osin.py` & `osin-1.9.2/osin/apis/local_osin.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/apis/osin.py` & `osin-1.9.2/osin/apis/osin.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/apis/remote_exp.py` & `osin-1.9.2/osin/apis/remote_exp.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/apis/remote_osin.py` & `osin-1.9.2/osin/apis/remote_osin.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/app.py` & `osin-1.9.2/osin/app.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/controllers/exp.py` & `osin-1.9.2/osin/controllers/exp.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/controllers/report.py` & `osin-1.9.2/osin/controllers/report.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/formats/hdf5.py` & `osin-1.9.2/osin/formats/hdf5.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/integrations/ream.py` & `osin-1.9.2/osin/integrations/ream.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/misc.py` & `osin-1.9.2/osin/misc.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/base.py` & `osin-1.9.2/osin/models/base.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/exp.py` & `osin-1.9.2/osin/models/exp.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/exp_data.py` & `osin-1.9.2/osin/models/exp_data.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/migration/v_1_6_2_1_7_0.backup` & `osin-1.9.2/osin/models/migration/v_1_6_2_1_7_0.backup`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report/__init__.py` & `osin-1.9.2/osin/models/report/__init__.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report/auto_table.py` & `osin-1.9.2/osin/models/report/auto_table.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report/base_report.py` & `osin-1.9.2/osin/models/report/base_report.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report/dbmodel.py` & `osin-1.9.2/osin/models/report/dbmodel.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report/index_schema.py` & `osin-1.9.2/osin/models/report/index_schema.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/models/report.py.backup` & `osin-1.9.2/osin/models/report.py.backup`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/params_helper.py` & `osin-1.9.2/osin/params_helper.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/repository.py` & `osin-1.9.2/osin/repository.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/types/param_schema.py` & `osin-1.9.2/osin/types/param_schema.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/types/primitive_type.py` & `osin-1.9.2/osin/types/primitive_type.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/types/pyobject.py` & `osin-1.9.2/osin/types/pyobject.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/osin/types/pyobject_type.py` & `osin-1.9.2/osin/types/pyobject_type.py`

 * *Files identical despite different names*

### Comparing `osin-1.9.1/pyproject.toml` & `osin-1.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osin"
-version = "1.9.1"
+version = "1.9.2"
 description = "Research and Experiments"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -13,16 +13,16 @@
 tornado = "^6.2"
 gena = "^1.6.4"
 loguru = "^0.6.0"
 orjson = "^3.8.2"
 h5py = "^3.7.0"
 psutil = "^5.9.2"
 python-slugify = "^6.1.2"
-t2-yada = "^1.0.4"
-ream2 = "^1.5.4"
+t2-yada = "^1.0.5"
+ream2 = "^1.6.2"
 
 [tool.poetry.dev-dependencies]
 black = "^22.10.0"
 pytest = "^7.1.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `osin-1.9.1/setup.py` & `osin-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
  'gena>=1.6.4,<2.0.0',
  'h5py>=3.7.0,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'orjson>=3.8.2,<4.0.0',
  'peewee>=3.15.2,<4.0.0',
  'psutil>=5.9.2,<6.0.0',
  'python-slugify>=6.1.2,<7.0.0',
- 'ream2>=1.5.4,<2.0.0',
- 't2-yada>=1.0.4,<2.0.0',
+ 'ream2>=1.6.2,<2.0.0',
+ 't2-yada>=1.0.5,<2.0.0',
  'tornado>=6.2,<7.0']
 
 setup_kwargs = {
     'name': 'osin',
-    'version': '1.9.1',
+    'version': '1.9.2',
     'description': 'Research and Experiments',
     'long_description': "# osin &middot; [![PyPI](https://img.shields.io/pypi/v/osin)](https://pypi.org/project/osin)\n\nThere are existing systems (e.g., neptune.ai, sacred) helping you organize, log data of your experiments. However, typically, the tasks of running the experiments are your responsible to bear. If you update your code and need to re-run your experiments, you may want to delete previous runs, which would be painful to have to do manually many times.\n\nWe rethink the experimenting process. Why don't we start with specifying the designed report (e.g., charts) and how to run/query to get the numbers to fill the report? This would free ones from manually starting/running the experiments and managing the experiment data. `osin` is a tool that helps you to achieve that goal.\n\nNote: this tool is expected to use locally or inside VPN network as it doesn't provide any protection against attackers.\n\n## Quick start\n\nStart the application:\n\n```bash\nDBFILE=%PATH_TO_DBFILE% python -m osin.main\n```\n\nOr start the services manually:\n\n```bash\nexport DBFILE=%PATH_TO_DBFILE%\npython -m osin.worker # start worker to run jobs\npython -m osin.server # start the server so clients can send job result\nstreamlit run osin/ui/dashboard.py # start a dashboard to view/create reports\n```\n\nYou will start by designing the output that your experiments will produce. For example:\n\n```yaml\n\n```\n",
     'author': 'Binh Vu',
     'author_email': 'binh@toan2.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `osin-1.9.1/PKG-INFO` & `osin-1.9.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osin
-Version: 1.9.1
+Version: 1.9.2
 Summary: Research and Experiments
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Requires-Dist: gena (>=1.6.4,<2.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: orjson (>=3.8.2,<4.0.0)
 Requires-Dist: peewee (>=3.15.2,<4.0.0)
 Requires-Dist: psutil (>=5.9.2,<6.0.0)
 Requires-Dist: python-slugify (>=6.1.2,<7.0.0)
-Requires-Dist: ream2 (>=1.5.4,<2.0.0)
-Requires-Dist: t2-yada (>=1.0.4,<2.0.0)
+Requires-Dist: ream2 (>=1.6.2,<2.0.0)
+Requires-Dist: t2-yada (>=1.0.5,<2.0.0)
 Requires-Dist: tornado (>=6.2,<7.0)
 Description-Content-Type: text/markdown
 
 # osin &middot; [![PyPI](https://img.shields.io/pypi/v/osin)](https://pypi.org/project/osin)
 
 There are existing systems (e.g., neptune.ai, sacred) helping you organize, log data of your experiments. However, typically, the tasks of running the experiments are your responsible to bear. If you update your code and need to re-run your experiments, you may want to delete previous runs, which would be painful to have to do manually many times.
```

