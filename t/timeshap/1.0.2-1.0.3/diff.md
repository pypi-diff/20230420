# Comparing `tmp/timeshap-1.0.2.tar.gz` & `tmp/timeshap-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/timeshap/timeshap/dist/tmph9clzjnb/timeshap-1.0.2.tar", last modified: Wed Aug 10 11:14:09 2022, max compression
+gzip compressed data, was "/home/runner/work/timeshap/timeshap/dist/.tmp-pao2qoel/timeshap-1.0.3.tar", last modified: Thu Apr 20 16:09:31 2023, max compression
```

## Comparing `timeshap-1.0.2.tar` & `timeshap-1.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11434 2022-08-10 11:13:59.000000 timeshap-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-08-10 11:13:59.000000 timeshap-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-08-10 11:14:09.000000 timeshap-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9683 2022-08-10 11:13:59.000000 timeshap-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-10 11:13:59.000000 timeshap-1.0.2/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-08-10 11:13:59.000000 timeshap-1.0.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-10 11:14:09.000000 timeshap-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-08-10 11:13:59.000000 timeshap-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/explainer/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11612 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/cell_level.py
--rw-r--r--   0 runner    (1001) docker     (121)    14719 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/event_level.py
--rw-r--r--   0 runner    (1001) docker     (121)    15389 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/feature_level.py
--rw-r--r--   0 runner    (1001) docker     (121)    11803 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/global_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/explainer/kernel/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40695 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/kernel/timeshap_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    12221 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/local_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)    16403 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/explainer/pruning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6157 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/cell_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/event_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     6838 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/feature_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/global_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/local_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/pruning.py
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/plot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     6447 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/utils/timeshap_legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)    16473 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap/wrappers/
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/wrappers/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/wrappers/tf_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8338 2022-08-10 11:13:59.000000 timeshap-1.0.2/src/timeshap/wrappers/torch_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 11:14:08.000000 timeshap-1.0.2/src/timeshap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-10 11:14:09.000000 timeshap-1.0.2/src/timeshap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11434 2023-04-20 16:09:16.000000 timeshap-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-20 16:09:16.000000 timeshap-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-20 16:09:30.000000 timeshap-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-04-20 16:09:16.000000 timeshap-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 16:09:16.000000 timeshap-1.0.3/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-20 16:09:16.000000 timeshap-1.0.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:09:30.000000 timeshap-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-20 16:09:16.000000 timeshap-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/explainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/cell_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/event_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15941 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/feature_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/global_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/explainer/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40695 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/kernel/timeshap_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/local_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16406 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/explainer/pruning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/cell_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/event_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/feature_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/global_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/local_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/utils/timeshap_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/wrappers/base_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/wrappers/tf_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-04-20 16:09:16.000000 timeshap-1.0.3/src/timeshap/wrappers/torch_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 16:09:30.000000 timeshap-1.0.3/src/timeshap.egg-info/top_level.txt
```

### Comparing `timeshap-1.0.2/LICENSE` & `timeshap-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/MANIFEST.in` & `timeshap-1.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/PKG-INFO` & `timeshap-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: timeshap
-Version: 1.0.2
+Version: 1.0.3
 Summary: KernelSHAP adaptation for recurrent models.
 Home-page: https://github.com/feedzai/timeshap
 Author: Feedzai
 Keywords: explainability,TimeShap
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TimeSHAP
 TimeSHAP is a model-agnostic, recurrent explainer that builds upon KernelSHAP and 
 extends it to the sequential domain.
 TimeSHAP computes event/timestamp- feature-, and cell-level attributions.
```

### Comparing `timeshap-1.0.2/README.md` & `timeshap-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/setup.py` & `timeshap-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     package_dir={'': 'src'},
     packages=find_packages('src', exclude=['tests', 'tests.*']),
     package_data={
         '': ['*.yaml, *.yml'],
     },
     include_package_data=True,
 
-    python_requires='>=3.6.*',
+    python_requires='>=3.6',
 
     install_requires=requirements,
 
     zip_safe=False,
 
     test_suite='tests',
     tests_require=requirements_test,
```

### Comparing `timeshap-1.0.2/src/timeshap/__init__.py` & `timeshap-1.0.3/src/timeshap/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/explainer/__init__.py` & `timeshap-1.0.3/src/timeshap/explainer/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/explainer/cell_level.py` & `timeshap-1.0.3/src/timeshap/explainer/cell_level.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/explainer/event_level.py` & `timeshap-1.0.3/src/timeshap/explainer/event_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,35 +255,44 @@
     verify_event_dict(event_dict)
     file_path = event_dict.get('path')
     make_predictions = True
     event_data = None
 
     tolerances_to_calc = get_tolerances_to_test(pruning_data, event_dict)
 
-    if file_path is not None and os.path.exists(file_path) and not append_to_files:
+    if file_path is not None and os.path.exists(file_path):
         event_data = pd.read_csv(file_path)
         make_predictions = False
 
-        # TODO resume explanations
-        # conditions = []
-        # necessary_entities = set(np.unique(data[entity_col].values))
-        # event_data = pd.read_csv(file_path)
-        # present_entities = set(np.unique(event_data[entity_col].values))
-        # if necessary_entities.issubset(present_entities):
-        #     conditions.append(True)
-        #     event_data = event_data[event_data[entity_col].isin(necessary_entities)]
-        #
-        # necessary_tols = set(tolerances_to_calc)
-        # loaded_csv = pd.read_csv(file_path)
-        # present_tols = set(np.unique(loaded_csv['Tolerance'].values))
-        # if necessary_tols.issubset(present_tols):
-        #     conditions.append(True)
-        #     event_data = event_data[event_data['Tolerance'].isin(necessary_tols)]
-        #
-        # make_predictions = ~np.array(conditions).all()
+        present_tols = set(np.unique(event_data['Tolerance'].values))
+        required_tols = [x for x in tolerances_to_calc if x not in present_tols]
+        if len(required_tols) == 0:
+            pass
+        elif len(required_tols) == 1 and -1 in tolerances_to_calc:
+            # Assuming all sequences are already explained
+            make_predictions = True
+        else:
+            raise NotImplementedError
+            # TODO resume explanations
+            # conditions = []
+            # necessary_entities = set(np.unique(data[entity_col].values))
+            # event_data = pd.read_csv(file_path)
+            # present_entities = set(np.unique(event_data[entity_col].values))
+            # if necessary_entities.issubset(present_entities):
+            #     conditions.append(True)
+            #     event_data = event_data[event_data[entity_col].isin(necessary_entities)]
+            #
+            # necessary_tols = set(tolerances_to_calc)
+            # loaded_csv = pd.read_csv(file_path)
+            # present_tols = set(np.unique(loaded_csv['Tolerance'].values))
+            # if necessary_tols.issubset(present_tols):
+            #     conditions.append(True)
+            #     event_data = event_data[event_data['Tolerance'].isin(necessary_tols)]
+            #
+            # make_predictions = ~np.array(conditions).all()
 
     if make_predictions:
         random_seeds = list(np.unique(event_dict.get('rs')))
         nsamples = list(np.unique(event_dict.get('nsamples')))
         names = ["Random Seed", "NSamples", "Event", "Shapley Value", "t (event index)", "Entity", 'Tolerance']
 
         if file_path is not None:
@@ -305,20 +314,22 @@
         ret_event_data = []
         for rs in random_seeds:
             for ns in nsamples:
                 for sequence in data:
                     if entity_col is not None:
                         entity = sequence[0, 0, entity_col_index]
                     if model_features:
-                        sequence = sequence[:, :, model_features]
+                        sequence = sequence[:, :, model_features_index]
                     sequence = sequence.astype(np.float64)
                     event_data = None
                     prev_pruning_idx = None
                     for tol in tolerances_to_calc:
-                        if pruning_data is None:
+                        if tol == -1:
+                            pruning_idx = 0
+                        elif pruning_data is None:
                             #we need to perform the pruning on the fly
                             coal_prun_idx, _ = temp_coalition_pruning(f, sequence, baseline, tol)
                             pruning_idx = data.shape[1] + coal_prun_idx
                         else:
                             instance = pruning_data[pruning_data["Entity"] == entity]
                             pruning_idx = instance[instance['Tolerance'] == tol]['Pruning idx'].iloc[0]
                             pruning_idx = sequence.shape[1] + pruning_idx
```

### Comparing `timeshap-1.0.2/src/timeshap/explainer/feature_level.py` & `timeshap-1.0.3/src/timeshap/explainer/feature_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,35 +270,45 @@
     verify_feature_dict(feat_dict)
     file_path = feat_dict.get('path')
     make_predictions = True
     feat_data = None
 
     tolerances_to_calc = get_tolerances_to_test(pruning_data, feat_dict)
 
-    if file_path is not None and os.path.exists(file_path) and not append_to_files:
+    if file_path is not None and os.path.exists(file_path):
         feat_data = pd.read_csv(file_path)
         make_predictions = False
 
-        # TODO resume explanations
-        # conditions = []
-        # necessary_entities = set(np.unique(data[entity_col].values))
-        # feat_data = pd.read_csv(file_path)
-        # present_entities = set(np.unique(feat_data[entity_col].values))
-        # if necessary_entities.issubset(present_entities):
-        #     conditions.append(True)
-        #     feat_data = feat_data[feat_data[entity_col].isin(necessary_entities)]
-        #
-        # necessary_tols = set(tolerances_to_calc)
-        # loaded_csv = pd.read_csv(file_path)
-        # present_tols = set(np.unique(loaded_csv['Tolerance'].values))
-        # if necessary_tols.issubset(present_tols):
-        #     conditions.append(True)
-        #     feat_data = feat_data[loaded_csv['Tolerance'].isin(necessary_tols)]
-        #
-        # make_predictions = ~np.array(conditions).all()
+        present_tols = set(np.unique(feat_data['Tolerance'].values))
+        required_tols = [x for x in tolerances_to_calc if x not in present_tols]
+        if len(required_tols) == 0:
+            pass
+        elif len(required_tols) == 1 and -1 in tolerances_to_calc:
+            # Assuming all sequences are already explained
+            make_predictions = True
+        else:
+            raise NotImplementedError
+
+            # TODO resume explanations
+            # conditions = []
+            # necessary_entities = set(np.unique(data[entity_col].values))
+            # feat_data = pd.read_csv(file_path)
+            # present_entities = set(np.unique(feat_data[entity_col].values))
+            # if necessary_entities.issubset(present_entities):
+            #     conditions.append(True)
+            #     feat_data = feat_data[feat_data[entity_col].isin(necessary_entities)]
+            #
+            # necessary_tols = set(tolerances_to_calc)
+            # loaded_csv = pd.read_csv(file_path)
+            # present_tols = set(np.unique(loaded_csv['Tolerance'].values))
+            # if necessary_tols.issubset(present_tols):
+            #     conditions.append(True)
+            #     feat_data = feat_data[loaded_csv['Tolerance'].isin(necessary_tols)]
+            #
+            # make_predictions = ~np.array(conditions).all()
 
     if make_predictions:
         random_seeds = list(np.unique(feat_dict.get('rs')))
         nsamples = list(np.unique(feat_dict.get('nsamples')))
         names = ["Random Seed", "NSamples", "Feature",  "Shapley Value", "Entity", 'Tolerance']
 
         if file_path is not None:
@@ -320,20 +330,22 @@
         ret_feat_data = []
         for rs in random_seeds:
             for ns in nsamples:
                 for sequence in data:
                     if entity_col is not None:
                         entity = sequence[0, 0, entity_col_index]
                     if model_features:
-                        sequence = sequence[:, :, model_features]
+                        sequence = sequence[:, :, model_features_index]
                     sequence = sequence.astype(np.float64)
                     feat_data = None
                     prev_pruning_idx = None
                     for tol in tolerances_to_calc:
-                        if pruning_data is None:
+                        if tol == -1:
+                            pruning_idx = 0
+                        elif pruning_data is None:
                             #we need to perform the pruning on the fly
                             coal_prun_idx, _ = temp_coalition_pruning(f, sequence, baseline, tol)
                             pruning_idx = data.shape[1] + coal_prun_idx
                         else:
                             instance = pruning_data[pruning_data["Entity"] == entity]
                             pruning_idx = instance[instance['Tolerance'] == tol]['Pruning idx'].iloc[0]
                             pruning_idx = sequence.shape[1] + pruning_idx
```

### Comparing `timeshap-1.0.2/src/timeshap/explainer/global_methods.py` & `timeshap-1.0.3/src/timeshap/explainer/global_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,22 +87,25 @@
     """
     validate_input(f, data, baseline, model_features, schema, entity_col, time_col)
 
     if isinstance(data, np.ndarray):
         if len(data.shape) == 2:
             assert entity_col is not None, "Entity column must be provided when using 2D numpy arrays as data"
 
-    verify_pruning_dict(pruning_dict)
+    if pruning_dict is not None:
+        verify_pruning_dict(pruning_dict)
+
+        if pruning_dict.get("path"):
+            if os.path.exists(pruning_dict.get("path")) and not append_to_files:
+                print(
+                    "The defined path for pruning data already exists and the append option is turned off. TimeSHAP will only read from this file and will not create new explanation data")
+        else:
+            print("No path to persist pruning data provided.")
     verify_event_dict(event_dict)
     verify_feature_dict(feature_dict)
-    if pruning_dict.get("path"):
-        if os.path.exists(pruning_dict.get("path")) and not append_to_files:
-            print("The defined path for pruning data already exists and the append option is turned off. TimeSHAP will only read from this file and will not create new explanation data")
-    else:
-        print("No path to persist pruning data provided.")
 
     if event_dict.get("path"):
         if os.path.exists(event_dict.get("path")) and not append_to_files:
             print("The defined path for event explanations already exists and the append option is turned off. TimeSHAP will only read from this file and will not create new explanation data")
     else:
         print("No path to persist event explanations provided.")
 
@@ -195,16 +198,22 @@
         schema, entity_col, time_col, append_to_files, verbose)
 
     model_features_index, entity_col_index, time_col_index = convert_to_indexes(model_features, schema, entity_col, time_col)
     data = convert_data_to_3d(data, entity_col_index, time_col_index)
     if len(data) > max_instances:
         selected_sequences = np.random.choice(np.arange(len(data)), max_instances, False)
         data = [data[idx] for idx in selected_sequences]
-    print("Calculating pruning algorithm")
-    prun_indexes = prune_all(f, data, pruning_dict, baseline, model_features_index, schema, entity_col_index, time_col_index, append_to_files, verbose)
+
+    if pruning_dict is None:
+        prun_indexes = None
+    else:
+        print("Calculating pruning algorithm")
+        prun_indexes = prune_all(f, data, pruning_dict, baseline,
+                                 model_features_index, schema, entity_col_index,
+                                 time_col_index, append_to_files, verbose)
 
     print("Calculating event data")
     event_data = event_explain_all(f, data, event_dict, prun_indexes, baseline, model_features_index, schema, entity_col_index, time_col_index, append_to_files, verbose)
 
     print("Calculating feat data")
     feat_data = feat_explain_all(f, data, feature_dict, prun_indexes, baseline, model_features_index, schema, entity_col_index, time_col_index, append_to_files, verbose)
```

### Comparing `timeshap-1.0.2/src/timeshap/explainer/kernel/__init__.py` & `timeshap-1.0.3/src/timeshap/explainer/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/explainer/kernel/timeshap_kernel.py` & `timeshap-1.0.3/src/timeshap/explainer/kernel/timeshap_kernel.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/explainer/local_methods.py` & `timeshap-1.0.3/src/timeshap/explainer/local_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,19 @@
             assert time_col in data_cols, "When providing time feature, these should be on the given DataFrame"
     else:
         assert len(data.shape) == 3, "Provided data must be an numpy array with 3 dimensions"
         assert data.shape[0] == 1, "For local report, provided data must contain one instance only"
 
     assert baseline is None or isinstance(baseline, (pd.DataFrame, np.ndarray)), "Baseline must be a pd.DataFrame or np.ndarrays"
 
-    assert pruning_dict.get("tol") is not None, "Prunning dict must have tolerance attribute"
-    assert isinstance(pruning_dict.get("tol"), (int, float)), "Provided tolerance must be a int or float"
-    if isinstance(pruning_dict.get("tol"), int):
-        assert pruning_dict.get("tol") == 0, "Provided tolerance must be a float or 0"
+    assert pruning_dict is None or pruning_dict.get("tol") is not None, "Prunning dict must have tolerance attribute"
+    if pruning_dict is not None:
+        assert isinstance(pruning_dict.get("tol"), (int, float)), "Provided tolerance must be a int or float"
+        if isinstance(pruning_dict.get("tol"), int):
+            assert pruning_dict.get("tol") == 0, "Provided tolerance must be a float or 0"
 
     check_dict(event_dict, 'rs', int, "Provided random seed must be a int")
     check_dict(event_dict, 'nsamples', int, "Provided nsamples must be a int")
     check_dict(feature_dict, 'rs', int, "Provided random seed must be a int")
     check_dict(feature_dict, 'nsamples', int, "Provided nsamples must be a int")
     check_dict(feature_dict, 'top_feats', int, "Provided top_feats must be a int")
     check_dict(feature_dict, 'plot_features', dict, "Provided plot_features must be a dict, mapping model features, to plot features")
@@ -201,16 +202,21 @@
             data = data.sort_values(time_col)
         if model_features is not None:
             data = data[model_features]
         else:
             data = data.values
         data = np.expand_dims(data.to_numpy().copy(), axis=0).astype(float)
 
-    coal_plot_data, coal_prun_idx = local_pruning(f, data, pruning_dict, baseline, entity_uuid, entity_col, verbose)
-    pruning_idx = data.shape[1] + coal_prun_idx
+    if pruning_dict is None:
+        print("No pruning dict passed. Skipping pruning procedures")
+        pruning_idx = 0
+        coal_plot_data = None
+    else:
+        coal_plot_data, coal_prun_idx = local_pruning(f, data, pruning_dict, baseline, entity_uuid, entity_col, verbose)
+        pruning_idx = data.shape[1] + coal_prun_idx
 
     event_data = local_event(f, data, event_dict, entity_uuid, entity_col, baseline, pruning_idx)
 
     feature_data = local_feat(f, data, feature_dict, entity_uuid, entity_col, baseline, pruning_idx)
 
     if cell_dict:
         cell_data = local_cell_level(f, data, cell_dict, event_data, feature_data, entity_uuid, entity_col, baseline, pruning_idx)
@@ -231,14 +237,16 @@
                  entity_col: str = None,
                  entity_uuid: str = None,
                  time_col: str = None,
                  verbose=False,
                  ):
     """Calculates local report and plots it.
 
+     `None` on the pruning_dict argument makes TimeSHAP skip the pruning step.
+
     Parameters
     ----------
     f: Callable[[np.ndarray], np.ndarray]
         Point of entry for model being explained.
         This method receives a 3-D np.ndarray (#samples, #seq_len, #features).
         This method returns a 2-D np.ndarray (#samples, 1).
```

### Comparing `timeshap-1.0.2/src/timeshap/explainer/pruning.py` & `timeshap-1.0.3/src/timeshap/explainer/pruning.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,19 +363,19 @@
     if schema is None and isinstance(data, pd.DataFrame):
         schema = list(data.columns)
     verify_pruning_dict(pruning_dict)
     file_path = pruning_dict.get('path')
     tolerances = list(np.unique(pruning_dict.get('tol')))
     make_predictions = True
     prun_data = None
-    if file_path is not None and os.path.exists(file_path) and not append_to_files:
+    if file_path is not None and os.path.exists(file_path):
         prun_data = pd.read_csv(file_path)
         make_predictions = False
 
-        # TODO resume explanations
+        # TODO resume explanations for missing entities
         # necessary_entities = set(np.unique(data[entity_col].values))
         # loaded_csv = pd.read_csv(file_path)
         # present_entities = set(np.unique(loaded_csv[entity_col].values))
         # if necessary_entities.issubset(present_entities):
         #     make_predictions = False
         #     prun_data = loaded_csv[loaded_csv[entity_col].isin(necessary_entities)]
 
@@ -398,15 +398,15 @@
         model_features_index, entity_col_index, time_col_index = convert_to_indexes(model_features, schema, entity_col, time_col)
         data = convert_data_to_3d(data, entity_col_index, time_col_index)
 
         for sequence in data:
             if entity_col is not None:
                 entity = sequence[0, 0, entity_col_index]
             if model_features:
-                sequence = sequence[:, :, model_features]
+                sequence = sequence[:, :, model_features_index]
             sequence = sequence.astype(np.float64)
             local_pruning_data = temp_coalition_pruning(f, sequence, baseline, None, ret_plot_data=True, verbose=verbose)
 
             if entity_col is not None:
                 local_pruning_data["Entity"] = entity
 
             ret_prun_data.append(local_pruning_data.values)
```

### Comparing `timeshap-1.0.2/src/timeshap/plot/__init__.py` & `timeshap-1.0.3/src/timeshap/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/plot/cell_level.py` & `timeshap-1.0.3/src/timeshap/plot/cell_level.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/plot/event_level.py` & `timeshap-1.0.3/src/timeshap/plot/event_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     plot_parameters: dict
         Dict containing optional plot parameters
             'height': height of the plot, default 150
             'width': width of the plot, default 360
             'axis_lims': plot Y domain, default [-0.3, 0.9]
             't_limit': number of events to plot, default -20
     """
-    def plot(event_data: pd.DataFrame, plot_parameters: dict):
+    def plot(event_data: pd.DataFrame, plot_parameters: dict = None):
         event_data = copy.deepcopy(event_data)
         event_data = event_data[event_data['t (event index)'] < 1]
         event_data = event_data[['Shapley Value', 't (event index)']]
 
         event_data['type'] = 'Shapley Value'
 
         avg_df = event_data.groupby('t (event index)').mean()['Shapley Value']
@@ -136,8 +136,8 @@
         ).properties(
             width=width,
             height=height,
         )
 
         return global_event
 
-    return multi_plot_wrapper(event_data, plot, (plot_parameters))
+    return multi_plot_wrapper(event_data, plot, ((plot_parameters),))
```

### Comparing `timeshap-1.0.2/src/timeshap/plot/feature_level.py` & `timeshap-1.0.3/src/timeshap/plot/feature_level.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/plot/global_report.py` & `timeshap-1.0.3/src/timeshap/plot/global_report.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,31 +43,35 @@
 
     event_data: pd.DataFrame
         Global event explanations to plot
 
     feat_data: pd.DataFrame
         Global feature explanations to plot
     """
-
-    if prun_indexes is None:
-        assert pruning_dict.get('path', False), "No data or path to data provided to calculate pruning statistics"
+    if pruning_dict is None:
+        if pruning_dict is not None:
+            assert pruning_dict.get('path', False), "No data or path to data provided to calculate pruning statistics"
     if event_data is None:
         assert event_dict.get('path', False), "No data or path to data provided to plot event explanations"
     if feat_data is None:
         assert feature_dict.get('path', False), "No data or path to data provided to plot feature explanations"
 
     if prun_indexes is None:
-        prun_indexes = pd.read_csv(pruning_dict.get('path'))
+        if pruning_dict is not None and pruning_dict.get('path'):
+            prun_indexes = pd.read_csv(pruning_dict.get('path'))
     if event_data is None:
         event_data = pd.read_csv(event_dict.get('path'))
     if feat_data is None:
         feat_data = pd.read_csv(feature_dict.get('path'))
 
-    print("Calculating pruning indexes")
-    pruning_stats = pruning_statistics(prun_indexes, pruning_dict.get('tol'))
+    if pruning_dict is None:
+        pruning_stats = None
+    else:
+        print("Calculating pruning indexes")
+        pruning_stats = pruning_statistics(prun_indexes, pruning_dict.get('tol'))
 
     plot_tols, plot_rs, plot_nsamples = find_parameters_to_plot(event_dict, feature_dict, event_data, feat_data)
 
     final_plot = alt.vconcat()
     for tolerance in plot_tols:
         for rs in plot_rs:
             for nsamples in plot_nsamples:
@@ -76,13 +80,13 @@
                 event_global_plot = plot_global_event(plot_event_data)
 
                 plot_feat_data = filter_dataset(feat_data, tolerance, rs, nsamples)
                 feat_global_plot = plot_global_feat(plot_feat_data, **feature_dict)
 
                 horizontal_plot = alt.hconcat(event_global_plot, feat_global_plot, center=True)
 
-                horizontal_plot.properties(
+                horizontal_plot = horizontal_plot.properties(
                     title=f"Parameters: NSamples={nsamples} | Random Seed={rs} | Pruning Tol= {tolerance}"
                 )
                 final_plot &= horizontal_plot
 
     return pruning_stats, final_plot
```

### Comparing `timeshap-1.0.2/src/timeshap/plot/local_report.py` & `timeshap-1.0.3/src/timeshap/plot/local_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,41 +49,51 @@
 
     feat_data: pd.DataFrame
         Feature explanations to plot
 
     cell_data: pd.DataFrame
         Cell explanations to plot
     """
-    if coal_plot_data is None:
-        assert pruning_dict.get('path', False), "No data or path to data provided to calculate pruning statistics"
+    if pruning_dict is None:
+        if pruning_dict is not None:
+            assert pruning_dict.get('path', False), "No data or path to data provided to calculate pruning statistics"
     if event_data is None:
         assert event_dict.get('path', False), "No data or path to data provided to plot event explanations"
     if feat_data is None:
         assert feature_dict.get('path', False), "No data or path to data provided to plot feature explanations"
     if cell_data is None and cell_dict is not None:
         assert cell_dict.get('path', False), "No data or path to data provided to plot feature explanations"
 
     if coal_plot_data is None:
-        coal_plot_data = pd.read_csv(pruning_dict.get('path'))
+        if pruning_dict is not None and pruning_dict.get('path'):
+            coal_plot_data = pd.read_csv(pruning_dict.get('path'))
     if event_data is None:
         event_data = pd.read_csv(event_dict.get('path'))
     if feat_data is None:
         feat_data = pd.read_csv(feature_dict.get('path'))
     if cell_data is None and cell_dict is not None:
         cell_data = pd.read_csv(cell_dict.get('path'))
 
-    coal_prun_idx = prune_given_data(coal_plot_data, pruning_dict.get('tol'))
-    plot_lim = max(abs(coal_prun_idx)+10, 40)
-    pruning_plot = plot_temp_coalition_pruning(coal_plot_data, coal_prun_idx, plot_lim)
+    if coal_plot_data is not None:
+        coal_prun_idx = prune_given_data(coal_plot_data, pruning_dict.get('tol'))
+        plot_lim = max(abs(coal_prun_idx)+10, 40)
+        pruning_plot = plot_temp_coalition_pruning(coal_plot_data, coal_prun_idx, plot_lim)
 
     event_plot = plot_event_heatmap(event_data)
 
     feature_plot = plot_feat_barplot(feat_data, feature_dict.get('top_feats'), feature_dict.get('plot_features'))
 
     if cell_dict:
         feat_names = list(feat_data['Feature'].values)[:-1]  # exclude pruned events
         cell_plot = plot_cell_level(cell_data, feat_names, feature_dict.get('plot_features'))
-        plot_report = (pruning_plot | event_plot | feature_plot | cell_plot).resolve_scale(color='independent')
+        if coal_plot_data is not None:
+            plot_report = (pruning_plot | event_plot | feature_plot | cell_plot).resolve_scale(color='independent')
+        else:
+            plot_report = (event_plot | feature_plot | cell_plot).resolve_scale(color='independent')
+
     else:
-        plot_report = (pruning_plot | event_plot | feature_plot).resolve_scale(color='independent')
+        if coal_plot_data is not None:
+            plot_report = (pruning_plot | event_plot | feature_plot).resolve_scale( color='independent')
+        else:
+            plot_report = (event_plot | feature_plot).resolve_scale( color='independent')
 
     return plot_report
```

### Comparing `timeshap-1.0.2/src/timeshap/plot/pruning.py` & `timeshap-1.0.3/src/timeshap/plot/pruning.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         Whether to remove negative importances of the background instances
     """
 
     def solve_negatives_method(df):
         negative_values = copy.deepcopy(df[df['Shapley Value'] < 0])
         for idx, row in negative_values.iterrows():
             corresponding_row = df[np.logical_and(df['t (event index)'] == row['t (event index)'], ~(df['Coalition'] == row['Coalition']))]
-            df.at[corresponding_row.index, 'Shapley Value'] = corresponding_row['Shapley Value'].values[0] + row['Shapley Value']
+            df.at[corresponding_row.index[0], 'Shapley Value'] = corresponding_row['Shapley Value'].values[0] + row['Shapley Value']
             df.at[idx, 'Shapley Value'] = 0
         return df
 
     df = df[df['t (event index)'] >= -plot_limit]
     if solve_negatives:
         df = solve_negatives_method(df)
```

### Comparing `timeshap-1.0.2/src/timeshap/plot/utils.py` & `timeshap-1.0.3/src/timeshap/plot/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     multi_plot = True if len(data_nsamples) > 1 or len(data_rs) > 1 or len(data_tol) > 1 else False
     final_plot = alt.vconcat()
 
     for tolerance in data_tol:
         for rs in data_rs:
             for nsamples in data_nsamples:
                 filtered_data = filter_dataset(explanation_data, tolerance, rs, nsamples)
-                param_plot = method(filtered_data, {}) if parameters is None else method(filtered_data, *parameters)
+                param_plot = method(filtered_data) if parameters is None else method(filtered_data, *parameters)
 
                 if multi_plot:
-                    param_plot.properties(
+                    param_plot = param_plot.properties(
                         title=f"Parameters: NSamples={nsamples} | Random Seed={rs} | Pruning Tol= {tolerance}"
                     )
                 final_plot &= param_plot
 
     return final_plot
```

### Comparing `timeshap-1.0.2/src/timeshap/utils/__init__.py` & `timeshap-1.0.3/src/timeshap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/utils/compatibility.py` & `timeshap-1.0.3/src/timeshap/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/utils/timeshap_legacy.py` & `timeshap-1.0.3/src/timeshap/utils/timeshap_legacy.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/utils/utils.py` & `timeshap-1.0.3/src/timeshap/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,22 +116,27 @@
 
     Returns
     -------
     List[np.ndarray]
         List of sequences
     """
     if pruning_data is None:
-        if explanation_dict.get('tol', False):
+        if explanation_dict.get('tol', True):
             print("No pruning data provided and no pruning tolerances provided. No pruning will take place")
             tolerances_to_calc = [-1.0]
         else:
             tolerances_to_calc = explanation_dict.get('tol')
             print(f"No pruning data provided. TimeSHAP will calculate pruning on-the fly using provided tolerances: {list(tolerances_to_calc)} ")
     else:
-        tolerances_to_calc = np.unique(pruning_data['Tolerance'].values)
+        tolerance_values = pruning_data['Tolerance'].values
+        if 'No Pruning' in tolerance_values:
+            index = np.where(tolerance_values == 'No Pruning')
+            tolerance_values = np.delete(tolerance_values, index)
+            tolerance_values = np.append(tolerance_values, -1)
+        tolerances_to_calc = np.unique(tolerance_values)
         tolerances_to_calc = tolerances_to_calc[~(tolerances_to_calc == -1)]
         input_tols = list(np.unique(explanation_dict.get('tol', tolerances_to_calc)))
         if input_tols is not None:
             assert np.array([x in tolerances_to_calc for x in input_tols]).all(), "Inputed tolerances are not present on the provided pruning data"
             tolerances_to_calc = input_tols
 
     return tolerances_to_calc
```

### Comparing `timeshap-1.0.2/src/timeshap/wrappers/__init__.py` & `timeshap-1.0.3/src/timeshap/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/wrappers/base_wrapper.py` & `timeshap-1.0.3/src/timeshap/wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/wrappers/tf_wrappers.py` & `timeshap-1.0.3/src/timeshap/wrappers/tf_wrappers.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap/wrappers/torch_wrappers.py` & `timeshap-1.0.3/src/timeshap/wrappers/torch_wrappers.py`

 * *Files identical despite different names*

### Comparing `timeshap-1.0.2/src/timeshap.egg-info/PKG-INFO` & `timeshap-1.0.3/src/timeshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: timeshap
-Version: 1.0.2
+Version: 1.0.3
 Summary: KernelSHAP adaptation for recurrent models.
 Home-page: https://github.com/feedzai/timeshap
 Author: Feedzai
 Keywords: explainability,TimeShap
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TimeSHAP
 TimeSHAP is a model-agnostic, recurrent explainer that builds upon KernelSHAP and 
 extends it to the sequential domain.
 TimeSHAP computes event/timestamp- feature-, and cell-level attributions.
```

### Comparing `timeshap-1.0.2/src/timeshap.egg-info/SOURCES.txt` & `timeshap-1.0.3/src/timeshap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

