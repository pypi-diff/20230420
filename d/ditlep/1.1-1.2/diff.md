# Comparing `tmp/ditlep-1.1.tar.gz` & `tmp/ditlep-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditlep-1.1.tar", last modified: Thu Apr 20 11:13:27 2023, max compression
+gzip compressed data, was "ditlep-1.2.tar", last modified: Thu Apr 20 11:18:57 2023, max compression
```

## Comparing `ditlep-1.1.tar` & `ditlep-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.313608 ditlep-1.1/
--rw-rw-rw-   0        0        0      272 2023-04-20 11:13:27.312608 ditlep-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-03-06 00:34:56.000000 ditlep-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.200609 ditlep-1.1/ditlep/
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.261608 ditlep-1.1/ditlep/fetcher/
--rw-rw-rw-   0        0        0      950 2023-03-05 02:27:57.000000 ditlep-1.1/ditlep/fetcher/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-20 11:02:29.000000 ditlep-1.1/ditlep/fetcher/alliance_chests.py
--rw-rw-rw-   0        0        0     1651 2023-03-05 02:35:13.000000 ditlep-1.1/ditlep/fetcher/base.py
--rw-rw-rw-   0        0        0      475 2023-02-27 19:28:09.000000 ditlep-1.1/ditlep/fetcher/breed_calculator.py
--rw-rw-rw-   0        0        0     3032 2023-03-05 02:45:18.000000 ditlep-1.1/ditlep/fetcher/dragon_search.py
--rw-rw-rw-   0        0        0      404 2023-02-27 19:28:09.000000 ditlep-1.1/ditlep/fetcher/dragon_tv.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.291604 ditlep-1.1/ditlep/fetcher/islands/
--rw-rw-rw-   0        0        0      524 2023-02-27 02:17:37.000000 ditlep-1.1/ditlep/fetcher/islands/__init__.py
--rw-rw-rw-   0        0        0      344 2023-02-27 19:28:48.000000 ditlep-1.1/ditlep/fetcher/islands/base.py
--rw-rw-rw-   0        0        0      337 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/fog_islands.py
--rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/grid_islands.py
--rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/heroic_races.py
--rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/maze_islands.py
--rw-rw-rw-   0        0        0      346 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/puzzle_islands.py
--rw-rw-rw-   0        0        0      346 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/runner_islands.py
--rw-rw-rw-   0        0        0      343 2023-02-27 19:28:37.000000 ditlep-1.1/ditlep/fetcher/islands/tower_islands.py
--rw-rw-rw-   0        0        0      867 2023-04-20 11:03:31.000000 ditlep-1.1/ditlep/fetcher/items_search.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.302605 ditlep-1.1/ditlep/fetcher/quests/
--rw-rw-rw-   0        0        0      157 2023-02-27 02:15:33.000000 ditlep-1.1/ditlep/fetcher/quests/__init__.py
--rw-rw-rw-   0        0        0      257 2023-02-27 19:28:09.000000 ditlep-1.1/ditlep/fetcher/quests/permanents.py
--rw-rw-rw-   0        0        0      245 2023-02-27 19:28:09.000000 ditlep-1.1/ditlep/fetcher/quests/temporary.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.309604 ditlep-1.1/ditlep/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:13:24.000000 ditlep-1.1/ditlep/utils/__init__.py
--rw-rw-rw-   0        0        0      748 2023-03-05 02:47:52.000000 ditlep-1.1/ditlep/utils/decrypt_data.py
-drwxrwxrwx   0        0        0        0 2023-04-20 11:13:27.239608 ditlep-1.1/ditlep.egg-info/
--rw-rw-rw-   0        0        0      272 2023-04-20 11:13:26.000000 ditlep-1.1/ditlep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      879 2023-04-20 11:13:27.000000 ditlep-1.1/ditlep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 11:13:26.000000 ditlep-1.1/ditlep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      260 2023-04-20 11:13:26.000000 ditlep-1.1/ditlep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 11:13:26.000000 ditlep-1.1/ditlep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 11:13:27.314621 ditlep-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-20 11:03:47.000000 ditlep-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:57.069048 ditlep-1.2/
+-rw-rw-rw-   0        0        0      272 2023-04-20 11:18:57.068046 ditlep-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-03-06 00:34:56.000000 ditlep-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:56.930046 ditlep-1.2/ditlep/
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:56.995051 ditlep-1.2/ditlep/fetcher/
+-rw-rw-rw-   0        0        0      952 2023-04-20 11:18:05.000000 ditlep-1.2/ditlep/fetcher/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-20 11:02:29.000000 ditlep-1.2/ditlep/fetcher/alliance_chests.py
+-rw-rw-rw-   0        0        0     1651 2023-03-05 02:35:13.000000 ditlep-1.2/ditlep/fetcher/base.py
+-rw-rw-rw-   0        0        0      475 2023-02-27 19:28:09.000000 ditlep-1.2/ditlep/fetcher/breed_calculator.py
+-rw-rw-rw-   0        0        0     3032 2023-03-05 02:45:18.000000 ditlep-1.2/ditlep/fetcher/dragon_search.py
+-rw-rw-rw-   0        0        0      404 2023-02-27 19:28:09.000000 ditlep-1.2/ditlep/fetcher/dragon_tv.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:57.048050 ditlep-1.2/ditlep/fetcher/islands/
+-rw-rw-rw-   0        0        0      524 2023-02-27 02:17:37.000000 ditlep-1.2/ditlep/fetcher/islands/__init__.py
+-rw-rw-rw-   0        0        0      344 2023-02-27 19:28:48.000000 ditlep-1.2/ditlep/fetcher/islands/base.py
+-rw-rw-rw-   0        0        0      337 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/fog_islands.py
+-rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/grid_islands.py
+-rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/heroic_races.py
+-rw-rw-rw-   0        0        0      340 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/maze_islands.py
+-rw-rw-rw-   0        0        0      346 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/puzzle_islands.py
+-rw-rw-rw-   0        0        0      346 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/runner_islands.py
+-rw-rw-rw-   0        0        0      343 2023-02-27 19:28:37.000000 ditlep-1.2/ditlep/fetcher/islands/tower_islands.py
+-rw-rw-rw-   0        0        0      867 2023-04-20 11:03:31.000000 ditlep-1.2/ditlep/fetcher/items_search.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:57.059054 ditlep-1.2/ditlep/fetcher/quests/
+-rw-rw-rw-   0        0        0      157 2023-02-27 02:15:33.000000 ditlep-1.2/ditlep/fetcher/quests/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-02-27 19:28:09.000000 ditlep-1.2/ditlep/fetcher/quests/permanents.py
+-rw-rw-rw-   0        0        0      245 2023-02-27 19:28:09.000000 ditlep-1.2/ditlep/fetcher/quests/temporary.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:57.065047 ditlep-1.2/ditlep/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-20 11:13:24.000000 ditlep-1.2/ditlep/utils/__init__.py
+-rw-rw-rw-   0        0        0      748 2023-03-05 02:47:52.000000 ditlep-1.2/ditlep/utils/decrypt_data.py
+drwxrwxrwx   0        0        0        0 2023-04-20 11:18:56.970048 ditlep-1.2/ditlep.egg-info/
+-rw-rw-rw-   0        0        0      272 2023-04-20 11:18:56.000000 ditlep-1.2/ditlep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      879 2023-04-20 11:18:56.000000 ditlep-1.2/ditlep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 11:18:56.000000 ditlep-1.2/ditlep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      260 2023-04-20 11:18:56.000000 ditlep-1.2/ditlep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 11:18:56.000000 ditlep-1.2/ditlep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 11:18:57.069048 ditlep-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-04-20 11:17:45.000000 ditlep-1.2/setup.py
```

### Comparing `ditlep-1.1/ditlep/fetcher/__init__.py` & `ditlep-1.2/ditlep/fetcher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .alliance_chests import AllianceChestFetcher
+from .alliance_chests import AllianceChestsFetcher
 from .breed_calculator import BreedCalculatorFetcher
 from .dragon_search import DragonSearchFetcher, DragonSearchAsyncFetcher
 from .dragon_tv import DragonTvFetcher
 from .islands import (
     FogIslandsFetcher,
     GridIslandsFetcher,
     HeroicRacesFetcher,
@@ -11,15 +11,15 @@
     RunnerIslandsFetcher,
     TowerIslandsFetcher
 )
 from .items_search import ItemsSearchFetcher
 from .quests import TemporaryQuestsFetcher, PermanentQuestsFetcher
 
 __all__ = [
-    AllianceChestFetcher,
+    AllianceChestsFetcher,
     BreedCalculatorFetcher,
     DragonSearchFetcher,
     DragonSearchAsyncFetcher,
     DragonTvFetcher,
     FogIslandsFetcher,
     GridIslandsFetcher,
     HeroicRacesFetcher,
```

### Comparing `ditlep-1.1/ditlep/fetcher/base.py` & `ditlep-1.2/ditlep/fetcher/base.py`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/ditlep/fetcher/dragon_search.py` & `ditlep-1.2/ditlep/fetcher/dragon_search.py`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/ditlep/fetcher/islands/__init__.py` & `ditlep-1.2/ditlep/fetcher/islands/__init__.py`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/ditlep/fetcher/items_search.py` & `ditlep-1.2/ditlep/fetcher/items_search.py`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/ditlep/utils/decrypt_data.py` & `ditlep-1.2/ditlep/utils/decrypt_data.py`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/ditlep.egg-info/SOURCES.txt` & `ditlep-1.2/ditlep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ditlep-1.1/setup.py` & `ditlep-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="ditlep",
-    version="1.1",
+    version="1.2",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="dragoncity dcutils tools",
     description=f"Fetcher/scraper of https://ditlep.com",
```

