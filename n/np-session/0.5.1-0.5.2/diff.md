# Comparing `tmp/np-session-0.5.1.tar.gz` & `tmp/np-session-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.5.1.tar", last modified: Tue Apr 11 20:30:52 2023, max compression
+gzip compressed data, was "np-session-0.5.2.tar", last modified: Thu Apr 20 17:28:18 2023, max compression
```

## Comparing `np-session-0.5.1.tar` & `np-session-0.5.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2113 2023-04-11 20:30:41.750465 np-session-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.1/README.md
--rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.1/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.1/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     7972 2023-04-11 20:30:10.239218 np-session-0.5.1/src/np_session/components/info.py
--rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.1/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.1/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.1/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.1/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.1/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.1/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.1/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.1/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.1/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.1/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.1/src/np_session/databases/sql_alchemy.py
--rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.1/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.1/src/np_session/jobs/find_missing_files.py
--rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.1/src/np_session/jobs/generate_session_summaries.py
--rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.1/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.1/src/np_session/jobs/probes.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.1/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.1/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0    25576 2023-03-29 21:44:41.257200 np-session-0.5.1/src/np_session/session.py
--rw-r--r--   0        0        0     8288 2023-03-17 05:14:59.167647 np-session-0.5.1/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.1/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.1/tests/test_platform_json.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2113 2023-04-20 17:28:10.838237 np-session-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.2/README.md
+-rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.2/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.2/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     7972 2023-04-13 01:45:59.657072 np-session-0.5.2/src/np_session/components/info.py
+-rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.2/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.2/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.2/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.2/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.2/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.2/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.2/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.2/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.2/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.2/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.2/src/np_session/databases/sql_alchemy.py
+-rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.2/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.2/src/np_session/jobs/find_missing_files.py
+-rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.2/src/np_session/jobs/generate_session_summaries.py
+-rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.2/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.2/src/np_session/jobs/probes.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.2/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.2/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0    25576 2023-03-29 21:44:41.257200 np-session-0.5.2/src/np_session/session.py
+-rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.2/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.2/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.2/tests/test_platform_json.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.2/PKG-INFO
```

### Comparing `np-session-0.5.1/pyproject.toml` & `np-session-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.5.1"
+version = "0.5.2"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-session-0.5.1/README.md` & `np-session-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/components/info.py` & `np-session-0.5.2/src/np_session/components/info.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/components/lims_manifests.py` & `np-session-0.5.2/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/components/paths.py` & `np-session-0.5.2/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/components/platform_json.py` & `np-session-0.5.2/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/components/settings_xml.py` & `np-session-0.5.2/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/data_getters.py` & `np-session-0.5.2/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/firebase_state.py` & `np-session-0.5.2/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/lims2.py` & `np-session-0.5.2/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/mtrain.py` & `np-session-0.5.2/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/redis_state.py` & `np-session-0.5.2/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/databases/sql_alchemy.py` & `np-session-0.5.2/src/np_session/databases/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/jobs/lims_upload.py` & `np-session-0.5.2/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/jobs/probes.py` & `np-session-0.5.2/src/np_session/jobs/probes.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/jobs/sessions.json` & `np-session-0.5.2/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/jobs/sync_states.py` & `np-session-0.5.2/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/session.py` & `np-session-0.5.2/src/np_session/session.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/src/np_session/utils.py` & `np-session-0.5.2/src/np_session/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 RE_FOLDER = re.compile("[0-9]{8,}_[0-9]{6}_[0-9]{8}")
 RE_PROBES = re.compile("(?<=_probe)_?(([A-F]+)|([0-5]))")
 
 REPLACED_COMP_ID: dict[str, tuple[datetime.date, str]] = {
     "NP.0-Acq": (datetime.date(2022, 10, 18), "W10DT05515"),
     "NP.1-Acq": (datetime.date(2022, 10, 27), "W10DT05501"),
     "NP.2-Acq": (datetime.date(2022, 7, 14), "W10DT05517"),
-    "NP.0-Stim": (datetime.date(2023, 2, 7), "W10DT713938"),
-    "NP.1-Stim": (datetime.date(2023, 1, 19), "W10DT713942"),
+    "NP.0-Stim": (datetime.date(2023, 2, 7), "W10DTSM112721"),
+    "NP.1-Stim": (datetime.date(2023, 1, 19), "W10DTSM118294"),
+    "NP.2-Stim": (datetime.date(2023, 3, 15), "W10DTSM118295"),
 }
 
 
 def old_hostname(comp_id: str, date: datetime.date) -> str | None:
     """Return the hostname for a computer that was replaced, if `date` predates the switchover.
 
     For a date before the hostname changed:
```

### Comparing `np-session-0.5.1/tests/test_platform_json.py` & `np-session-0.5.2/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.1/PKG-INFO` & `np-session-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

