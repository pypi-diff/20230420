# Comparing `tmp/toggler-0.1.2.tar.gz` & `tmp/toggler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggler-0.1.2.tar", last modified: Fri Mar 24 16:03:19 2023, max compression
+gzip compressed data, was "toggler-0.2.0.tar", last modified: Thu Apr 20 05:32:34 2023, max compression
```

## Comparing `toggler-0.1.2.tar` & `toggler-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.827178 toggler-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-24 16:03:10.000000 toggler-0.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-24 16:03:10.000000 toggler-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-24 16:03:10.000000 toggler-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-24 16:03:10.000000 toggler-0.1.2/.python-black
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-24 16:03:19.831178 toggler-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-24 16:03:10.000000 toggler-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 16:03:10.000000 toggler-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-24 16:03:19.831178 toggler-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-24 16:03:10.000000 toggler-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:10.000000 toggler-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-24 16:03:10.000000 toggler-0.1.2/tests/data/cfg_1.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-24 16:03:10.000000 toggler-0.1.2/tests/test_toggler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/toggler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:10.000000 toggler-0.1.2/toggler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-24 16:03:10.000000 toggler-0.1.2/toggler/env.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-24 16:03:10.000000 toggler-0.1.2/toggler/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-24 16:03:10.000000 toggler-0.1.2/toggler/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-03-24 16:03:10.000000 toggler-0.1.2/toggler/toggler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 16:03:19.831178 toggler-0.1.2/toggler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-24 16:03:19.000000 toggler-0.1.2/toggler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-24 16:03:19.000000 toggler-0.1.2/toggler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 16:03:19.000000 toggler-0.1.2/toggler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 16:03:19.000000 toggler-0.1.2/toggler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-24 16:03:19.000000 toggler-0.1.2/toggler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-24 16:03:10.000000 toggler-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.001540 toggler-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-20 05:32:25.000000 toggler-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-20 05:32:25.000000 toggler-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-20 05:32:25.000000 toggler-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 05:32:25.000000 toggler-0.2.0/.python-black
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 05:32:34.005540 toggler-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-20 05:32:25.000000 toggler-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 05:32:25.000000 toggler-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 05:32:34.005540 toggler-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-20 05:32:25.000000 toggler-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/data/cfg_1.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/test_config_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-20 05:32:25.000000 toggler-0.2.0/tests/test_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/services/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/toggler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 05:32:25.000000 toggler-0.2.0/toggler/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 05:32:34.005540 toggler-0.2.0/toggler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 05:32:33.000000 toggler-0.2.0/toggler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-20 05:32:25.000000 toggler-0.2.0/tox.ini
```

### Comparing `toggler-0.1.2/.github/workflows/main.yml` & `toggler-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `toggler-0.1.2/.pre-commit-config.yaml` & `toggler-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `toggler-0.1.2/PKG-INFO` & `toggler-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggler
-Version: 0.1.2
+Version: 0.2.0
 Summary: Feature Flags Manager
 Home-page: https://github.com/versada/toggler
 Author: Versada (Andrius Laukavičius)
 Author-email: andrius.laukavicius@versada.eu
 License: LGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `toggler-0.1.2/README.md` & `toggler-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `toggler-0.1.2/setup.py` & `toggler-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `toggler-0.1.2/tests/test_toggler.py` & `toggler-0.2.0/tests/test_feature.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,136 @@
 """Test class for feature toggling functionality."""
 import pathlib
 from datetime import date
 
 from toggler.toggler import Toggler
-from toggler.env import toggle_feature, modified_environ, ENV_KEY_CFG, ENV_KEY_MODE
+from toggler.services.env import (
+    toggle_feature,
+    modified_environ,
+    ENV_KEY_CFG,
+    ENV_KEY_MODE,
+)
 
 CFG_STREAM_1 = """---
-prod:
-  feature2:
-    active: true
-stage:
-  feature1:
-    active: true
-    ref: r123
-    deadline: 2022-01-01
-  feature2:
-    active: true
-  feature3:
-    active: false
+feature1:
+  modes: [prod, stage]
+  date: 2023-01-01
+  days_to_expire: 10
+  ref: r123
+feature2:
+  modes: [stage]
+  date: 2023-01-01
+feature3:
+  modes: [other]
+  date: 2023-01-01
+"""
+CFG_STREAM_2 = """---
+feature1:
+  date: 2023-02-02
+feature2:
+  modes: [prod]
+  ref: r222
+feature4:
+  modes: [stage]
+  date: 2023-01-01
 """
 
 path_cfg_1 = path = pathlib.Path(__file__).parent / "data/cfg_1.yml"
 
 
 def test_01_prod_mode():
     # GIVEN
     # WHEN
-    tog = Toggler("prod", path=path_cfg_1)
+    tog = Toggler("prod", paths=[path_cfg_1])
     # THEN
-    assert len(tog.features_cfg) == 2
-    assert len(tog.mode_features) == 1
-    assert tog.is_active("feature1") is None
-    assert tog.is_active("feature2") is True
-    assert tog.is_active("feature3") is None
+    assert len(tog.cfg) == 3
+    assert tog.is_active("feature1") is True
+    assert tog.is_active("feature2") is False
+    assert tog.is_active("feature3") is False
+    assert tog.is_active("feature4") is None
     expired_features = tog.check_deadlines()
     assert len(expired_features) == 1
     assert expired_features[0].name == "feature1"
 
 
 def test_02_stage_mode():
     # GIVEN
     # WHEN
-    tog = Toggler("stage", stream=CFG_STREAM_1)
+    tog = Toggler("stage", streams=[CFG_STREAM_1])
     # THEN
-    assert len(tog.features_cfg) == 2
-    assert len(tog.mode_features) == 3
+    assert len(tog.cfg) == 3
     assert tog.is_active("feature1") is True
     assert tog.is_active("feature2") is True
     assert tog.is_active("feature3") is False
-    assert tog.mode_features["feature1"].ref == "r123"
-    assert tog.mode_features["feature2"].ref is None
-    assert tog.mode_features["feature1"].deadline == date(2022, 1, 1)
-    assert tog.mode_features["feature2"].deadline is None
+    # WHEN
+    feature1 = tog.cfg.get("feature1")
+    # THEN
+    assert feature1 is not None
+    assert feature1.ref == "r123"
+    assert feature1.deadline == date(2023, 1, 11)
+    # WHEN
+    feature2 = tog.cfg.get("feature2")
+    assert feature2 is not None
+    assert feature2.ref is None
+    assert feature2.deadline is None
+    # assert tog.mode_features["feature1"].ref == "r123"
+    # assert tog.mode_features["feature2"].ref is None
+    # 2023-01-01 + 10 days
+    # assert tog.mode_features["feature1"].deadline == date(2023, 1, 11)
+    # assert tog.mode_features["feature2"].deadline is None
     expired_features = tog.check_deadlines()
     assert len(expired_features) == 1
     assert expired_features[0].name == "feature1"
 
 
 def test_03_forced_feature_via_env_prod():
     # GIVEN
     envs = {ENV_KEY_CFG: str(path_cfg_1), ENV_KEY_MODE: "prod"}
     with modified_environ(**envs):
         tog = Toggler()
     # WHEN
-    with toggle_feature("feature1", True):
+    with toggle_feature("feature3", True):
         # THEN
-        assert tog.is_active("feature1") is True
-    assert tog.is_active("feature1") is None
+        assert tog.is_active("feature3") is True
+    assert tog.is_active("feature3") is False
+    # WHEN
+    with toggle_feature("feature4", True):
+        # THEN
+        assert tog.is_active("feature4") is True
+    assert tog.is_active("feature4") is None
 
 
 def test_04_forced_feature_via_env_stage():
     # GIVEN
-    tog = Toggler("stage", stream=CFG_STREAM_1)
+    tog = Toggler("stage", streams=[CFG_STREAM_1])
     # WHEN
     with toggle_feature("feature1", False):
         # THEN
         assert tog.is_active("feature1") is False
     assert tog.is_active("feature1") is True
     # GIVEN
     # WHEN
     with toggle_feature("feature3", True):
         # THEN
         assert tog.is_active("feature3") is True
     assert tog.is_active("feature3") is False
 
 
 def test_05_feature_not_exists():
-    tog = Toggler("stage", stream=CFG_STREAM_1)
+    tog = Toggler("stage", streams=[CFG_STREAM_1])
     assert tog.is_active("ff1122312312312") is None
+
+
+def test_06_feature_prod_multiple_configs():
+    tog = Toggler("prod", streams=[CFG_STREAM_1, CFG_STREAM_2])
+    assert tog.is_active("feature1") is True
+    assert tog.is_active("feature2") is True
+    assert tog.is_active("feature3") is False
+    assert tog.is_active("feature4") is False
+
+
+def test_07_feature_stage_multiple_configs():
+    tog = Toggler("stage", streams=[CFG_STREAM_1, CFG_STREAM_2])
+    assert tog.is_active("feature1") is True
+    assert tog.is_active("feature2") is False
+    assert tog.is_active("feature3") is False
+    assert tog.is_active("feature4") is True
```

### Comparing `toggler-0.1.2/toggler/env.py` & `toggler-0.2.0/toggler/services/env.py`

 * *Files identical despite different names*

### Comparing `toggler-0.1.2/toggler.egg-info/PKG-INFO` & `toggler-0.2.0/toggler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toggler
-Version: 0.1.2
+Version: 0.2.0
 Summary: Feature Flags Manager
 Home-page: https://github.com/versada/toggler
 Author: Versada (Andrius Laukavičius)
 Author-email: andrius.laukavicius@versada.eu
 License: LGPLv3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

