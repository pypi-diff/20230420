# Comparing `tmp/pss_pywaapi-1.0.2.tar.gz` & `tmp/pss_pywaapi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pss_pywaapi-1.0.2.tar", last modified: Tue Dec 20 16:28:44 2022, max compression
+gzip compressed data, was "pss_pywaapi-1.0.3.tar", last modified: Thu Apr 20 16:44:56 2023, max compression
```

## Comparing `pss_pywaapi-1.0.2.tar` & `pss_pywaapi-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-20 16:28:44.153838 pss_pywaapi-1.0.2/
--rw-rw-rw-   0        0        0     1060 2022-12-19 15:53:17.000000 pss_pywaapi-1.0.2/LICENCE
--rw-rw-rw-   0        0        0       25 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      852 2022-12-20 16:28:44.153838 pss_pywaapi-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      402 2022-12-19 15:53:09.000000 pss_pywaapi-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-20 16:28:44.139826 pss_pywaapi-1.0.2/pss_helpers/
--rw-rw-rw-   0        0        0      564 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.2/pss_helpers/AudioFileReader.py
--rw-rw-rw-   0        0        0     1017 2021-05-06 09:13:45.000000 pss_pywaapi-1.0.2/pss_helpers/Files.py
--rw-rw-rw-   0        0        0      131 2022-08-17 16:52:14.000000 pss_pywaapi-1.0.2/pss_helpers/__init__.py
--rw-rw-rw-   0        0        0     1686 2022-04-20 21:31:46.000000 pss_pywaapi-1.0.2/pss_helpers/gui.py
--rw-rw-rw-   0        0        0     1669 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.2/pss_helpers/soundbank_helper.py
--rw-rw-rw-   0        0        0     1425 2022-08-17 16:54:42.000000 pss_pywaapi-1.0.2/pss_helpers/wwise_settings.py
-drwxrwxrwx   0        0        0        0 2022-12-20 16:28:44.150836 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/
--rw-rw-rw-   0        0        0      852 2022-12-20 16:28:44.000000 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2022-12-20 16:28:44.000000 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-20 16:28:44.000000 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-12-20 16:28:44.000000 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2022-12-20 16:28:44.000000 pss_pywaapi-1.0.2/pss_pywaapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    49428 2022-12-20 16:27:35.000000 pss_pywaapi-1.0.2/pss_pywaapi.py
--rw-rw-rw-   0        0        0       42 2022-12-20 16:28:44.154838 pss_pywaapi-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2022-12-20 16:28:11.000000 pss_pywaapi-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:44:56.396661 pss_pywaapi-1.0.3/
+-rw-rw-rw-   0        0        0     1060 2022-12-19 15:53:17.000000 pss_pywaapi-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0       25 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      852 2023-04-20 16:44:56.396661 pss_pywaapi-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2022-12-19 15:53:09.000000 pss_pywaapi-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 16:44:56.383650 pss_pywaapi-1.0.3/pss_helpers/
+-rw-rw-rw-   0        0        0      564 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.3/pss_helpers/AudioFileReader.py
+-rw-rw-rw-   0        0        0     1017 2021-05-06 09:13:45.000000 pss_pywaapi-1.0.3/pss_helpers/Files.py
+-rw-rw-rw-   0        0        0      131 2022-08-17 16:52:14.000000 pss_pywaapi-1.0.3/pss_helpers/__init__.py
+-rw-rw-rw-   0        0        0     1686 2022-04-20 21:31:46.000000 pss_pywaapi-1.0.3/pss_helpers/gui.py
+-rw-rw-rw-   0        0        0     1669 2021-02-17 11:13:35.000000 pss_pywaapi-1.0.3/pss_helpers/soundbank_helper.py
+-rw-rw-rw-   0        0        0     2184 2023-04-20 16:25:09.000000 pss_pywaapi-1.0.3/pss_helpers/wwise_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:44:56.393658 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-04-20 16:44:51.000000 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-04-20 16:44:51.000000 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:44:51.000000 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-20 16:44:51.000000 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-20 16:44:51.000000 pss_pywaapi-1.0.3/pss_pywaapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    50112 2023-04-20 16:28:47.000000 pss_pywaapi-1.0.3/pss_pywaapi.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:44:56.397661 pss_pywaapi-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-04-20 16:43:49.000000 pss_pywaapi-1.0.3/setup.py
```

### Comparing `pss_pywaapi-1.0.2/LICENCE` & `pss_pywaapi-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pss_pywaapi-1.0.2/PKG-INFO` & `pss_pywaapi-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pss_pywaapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper package for interfacing with Wwise using waapi.
 Home-page: https://github.com/simongumbleton/pss_pywaapi
 Author: Simon Gumbleton
 Author-email: simongumbleton@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pss_pywaapi-1.0.2/pss_helpers/AudioFileReader.py` & `pss_pywaapi-1.0.3/pss_helpers/AudioFileReader.py`

 * *Files identical despite different names*

### Comparing `pss_pywaapi-1.0.2/pss_helpers/Files.py` & `pss_pywaapi-1.0.3/pss_helpers/Files.py`

 * *Files identical despite different names*

### Comparing `pss_pywaapi-1.0.2/pss_helpers/gui.py` & `pss_pywaapi-1.0.3/pss_helpers/gui.py`

 * *Files identical despite different names*

### Comparing `pss_pywaapi-1.0.2/pss_helpers/soundbank_helper.py` & `pss_pywaapi-1.0.3/pss_helpers/soundbank_helper.py`

 * *Files identical despite different names*

### Comparing `pss_pywaapi-1.0.2/pss_pywaapi.egg-info/PKG-INFO` & `pss_pywaapi-1.0.3/pss_pywaapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pss-pywaapi
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper package for interfacing with Wwise using waapi.
 Home-page: https://github.com/simongumbleton/pss_pywaapi
 Author: Simon Gumbleton
 Author-email: simongumbleton@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pss_pywaapi-1.0.2/pss_pywaapi.py` & `pss_pywaapi-1.0.3/pss_pywaapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,30 @@
     "PostEvent":41
 }
 
 def getWwiseUserSetting_WAMPport():
     """Get the WAMP port saved in the user setting file for the authoring tool"""
     return wwise_settings.get_wamp_port()
 
+def getWwiseUserSettingByName(Name=""):
+    """ Get a named setting from the various .wsettings files wwise generates
+    :param Name: Name of the setting to retrieve
+    :return: Dictionary of Key Value pairs relating to the requested setting, or None if not found
+    e.g. <DefaultOutputBus Name="SFX" ID="{DA827D60-6AFF-47BB-AB1B-BD786FCFD3E6}"/>
+    or
+    <Property Name="Waapi\WampPort" Type="int32" Value="8095"/>
+    """
+    if not Name:
+        return None
+    DirsToCheck = []
+    DirsToCheck.append(wwise_settings.get_wwise_datadir())
+    DirsToCheck.append(getPathToWwiseProjectFolder())
+    return wwise_settings.get_wwise_usersetting(Name,DirsToCheck)
+
+
 def getWwiseVersion():
     """Get the Wwise Version struct"""
     result = client.call("ak.wwise.core.getInfo")
     if result:
         return result["version"]
     else:
         return False
```

### Comparing `pss_pywaapi-1.0.2/setup.py` & `pss_pywaapi-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.md') as f:
         README = f.read()
     return README
 
 
 setup(
     name="pss_pywaapi",
-    version="1.0.2",
+    version="1.0.3",
     description="Helper package for interfacing with Wwise using waapi.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/simongumbleton/pss_pywaapi",
     author="Simon Gumbleton",
     author_email="simongumbleton@gmail.com",
     license="MIT",
```

