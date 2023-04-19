# Comparing `tmp/Izmon-1.1.1.tar.gz` & `tmp/Izmon-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Izmon-1.1.1.tar", last modified: Sat Apr 15 08:28:32 2023, max compression
+gzip compressed data, was "Izmon-1.1.2.tar", last modified: Wed Apr 19 22:09:53 2023, max compression
```

## Comparing `Izmon-1.1.1.tar` & `Izmon-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,49 @@
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.361338 Izmon-1.1.1/
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.268688 Izmon-1.1.1/Izmon/
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.283595 Izmon-1.1.1/Izmon/Class/
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.293218 Izmon-1.1.1/Izmon/Class/Basic/
--rwxrwxrwx   0 yohei      (504) staff       (20)      738 2023-03-27 00:35:52.000000 Izmon-1.1.1/Izmon/Class/Basic/Common_Function.py
--rwxrwxrwx   0 yohei      (504) staff       (20)      859 2023-04-14 12:09:48.000000 Izmon-1.1.1/Izmon/Class/Basic/Common_Variable.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     8906 2023-04-14 12:19:57.000000 Izmon-1.1.1/Izmon/Class/Basic/Settings.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       14 2023-03-06 02:43:12.000000 Izmon-1.1.1/Izmon/Class/Basic/__init__.py
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.326196 Izmon-1.1.1/Izmon/Class/Battle/
--rwxrwxrwx   0 yohei      (504) staff       (20)     3733 2023-03-10 00:50:08.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     2696 2023-03-27 01:57:28.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Caluculate.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     2638 2023-03-05 23:44:30.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Other.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     2628 2023-03-06 04:02:18.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Set.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:30.000000 Izmon-1.1.1/Izmon/Class/Battle/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     1355 2023-03-06 10:15:46.000000 Izmon-1.1.1/Izmon/Class/Dictionary.py
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.336728 Izmon-1.1.1/Izmon/Class/Events/
--rwxrwxrwx   0 yohei      (504) staff       (20)      313 2023-03-05 08:36:34.000000 Izmon-1.1.1/Izmon/Class/Events/Events_Latest.py
--rwxrwxrwx   0 yohei      (504) staff       (20)        0 2023-03-01 05:47:34.000000 Izmon-1.1.1/Izmon/Class/Events/Events_Passed.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:42.000000 Izmon-1.1.1/Izmon/Class/Events/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     4778 2023-04-12 11:12:48.000000 Izmon-1.1.1/Izmon/Class/Gym.py
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.347166 Izmon-1.1.1/Izmon/Class/Save_Code/
--rwxrwxrwx   0 yohei      (504) staff       (20)     1601 2023-03-27 03:08:20.000000 Izmon-1.1.1/Izmon/Class/Save_Code/Decode.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     1177 2023-03-09 04:41:52.000000 Izmon-1.1.1/Izmon/Class/Save_Code/Encode.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:43:56.000000 Izmon-1.1.1/Izmon/Class/Save_Code/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     2153 2023-03-27 03:13:26.000000 Izmon-1.1.1/Izmon/Class/Set.py
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.354548 Izmon-1.1.1/Izmon/Class/Start_End/
--rwxrwxrwx   0 yohei      (504) staff       (20)     2135 2023-04-14 12:27:14.000000 Izmon-1.1.1/Izmon/Class/Start_End/End.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     5275 2023-04-14 12:25:52.000000 Izmon-1.1.1/Izmon/Class/Start_End/Start.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:44:10.000000 Izmon-1.1.1/Izmon/Class/Start_End/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 09:47:24.000000 Izmon-1.1.1/Izmon/Class/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)      281 2023-03-30 01:10:43.000000 Izmon-1.1.1/Izmon/Class/setup.py
--rwxrwxrwx   0 yohei      (504) staff       (20)     1513 2023-04-14 12:01:37.000000 Izmon-1.1.1/Izmon/Main.py
--rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 10:08:06.000000 Izmon-1.1.1/Izmon/__init__.py
--rwxrwxrwx   0 yohei      (504) staff       (20)      280 2023-04-14 11:24:09.000000 Izmon-1.1.1/Izmon/setup.py
-drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.273651 Izmon-1.1.1/Izmon.egg-info/
--rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/PKG-INFO
--rw-r--r--   0 yohei      (504) staff       (20)      899 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/SOURCES.txt
--rw-r--r--   0 yohei      (504) staff       (20)        1 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/dependency_links.txt
--rw-r--r--   0 yohei      (504) staff       (20)        6 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/top_level.txt
--rwxrwxrwx   0 yohei      (504) staff       (20)      634 2023-03-02 11:44:52.000000 Izmon-1.1.1/LICENSE.txt
--rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-15 08:28:32.360697 Izmon-1.1.1/PKG-INFO
--rwxrwxrwx   0 yohei      (504) staff       (20)      492 2023-03-06 05:47:12.000000 Izmon-1.1.1/README.md
--rw-r--r--   0 yohei      (504) staff       (20)       38 2023-04-15 08:28:32.361567 Izmon-1.1.1/setup.cfg
--rwxrwxrwx   0 yohei      (504) staff       (20)      877 2023-04-14 11:23:57.000000 Izmon-1.1.1/setup.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.949731 Izmon-1.1.2/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.944558 Izmon-1.1.2/Izmon/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.946008 Izmon-1.1.2/Izmon/Class/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.946902 Izmon-1.1.2/Izmon/Class/Basic/
+-rwxrwxrwx   0 yohei      (504) staff       (20)      738 2023-03-27 00:35:52.000000 Izmon-1.1.2/Izmon/Class/Basic/Common_Function.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      859 2023-04-14 12:09:48.000000 Izmon-1.1.2/Izmon/Class/Basic/Common_Variable.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     8906 2023-04-19 21:39:48.000000 Izmon-1.1.2/Izmon/Class/Basic/Settings.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       14 2023-03-06 02:43:12.000000 Izmon-1.1.2/Izmon/Class/Basic/__init__.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.947519 Izmon-1.1.2/Izmon/Class/Battle/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     3733 2023-03-10 00:50:08.000000 Izmon-1.1.2/Izmon/Class/Battle/Battle.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2696 2023-03-27 01:57:28.000000 Izmon-1.1.2/Izmon/Class/Battle/Battle_Caluculate.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2638 2023-03-05 23:44:30.000000 Izmon-1.1.2/Izmon/Class/Battle/Battle_Other.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2628 2023-03-06 04:02:18.000000 Izmon-1.1.2/Izmon/Class/Battle/Battle_Set.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:30.000000 Izmon-1.1.2/Izmon/Class/Battle/__init__.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.948359 Izmon-1.1.2/Izmon/Class/CloudSave/
+-rw-r--r--   0 yohei      (504) staff       (20)     1014 2023-04-14 12:08:37.000000 Izmon-1.1.2/Izmon/Class/CloudSave/Common.py
+-rw-r--r--   0 yohei      (504) staff       (20)     1069 2023-04-14 12:22:10.000000 Izmon-1.1.2/Izmon/Class/CloudSave/Download.py
+-rw-r--r--   0 yohei      (504) staff       (20)     1267 2023-04-14 11:39:51.000000 Izmon-1.1.2/Izmon/Class/CloudSave/Upload.py
+-rw-r--r--   0 yohei      (504) staff       (20)       18 2023-04-19 21:43:44.000000 Izmon-1.1.2/Izmon/Class/CloudSave/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1355 2023-03-06 10:15:46.000000 Izmon-1.1.2/Izmon/Class/Dictionary.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.948753 Izmon-1.1.2/Izmon/Class/Events/
+-rwxrwxrwx   0 yohei      (504) staff       (20)      313 2023-03-05 08:36:34.000000 Izmon-1.1.2/Izmon/Class/Events/Events_Latest.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)        0 2023-03-01 05:47:34.000000 Izmon-1.1.2/Izmon/Class/Events/Events_Passed.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:42.000000 Izmon-1.1.2/Izmon/Class/Events/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     4778 2023-04-12 11:12:48.000000 Izmon-1.1.2/Izmon/Class/Gym.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.949122 Izmon-1.1.2/Izmon/Class/Save_Code/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1601 2023-03-27 03:08:20.000000 Izmon-1.1.2/Izmon/Class/Save_Code/Decode.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1177 2023-03-09 04:41:52.000000 Izmon-1.1.2/Izmon/Class/Save_Code/Encode.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:43:56.000000 Izmon-1.1.2/Izmon/Class/Save_Code/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2153 2023-03-27 03:13:26.000000 Izmon-1.1.2/Izmon/Class/Set.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.949472 Izmon-1.1.2/Izmon/Class/Start_End/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2135 2023-04-14 12:27:14.000000 Izmon-1.1.2/Izmon/Class/Start_End/End.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     5275 2023-04-14 12:25:52.000000 Izmon-1.1.2/Izmon/Class/Start_End/Start.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:44:10.000000 Izmon-1.1.2/Izmon/Class/Start_End/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 09:47:24.000000 Izmon-1.1.2/Izmon/Class/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      281 2023-03-30 01:10:43.000000 Izmon-1.1.2/Izmon/Class/setup.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1512 2023-04-19 21:42:53.000000 Izmon-1.1.2/Izmon/Main.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 10:08:06.000000 Izmon-1.1.2/Izmon/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      280 2023-04-19 21:39:45.000000 Izmon-1.1.2/Izmon/setup.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-19 22:09:53.945048 Izmon-1.1.2/Izmon.egg-info/
+-rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-19 22:09:53.000000 Izmon-1.1.2/Izmon.egg-info/PKG-INFO
+-rw-r--r--   0 yohei      (504) staff       (20)     1031 2023-04-19 22:09:53.000000 Izmon-1.1.2/Izmon.egg-info/SOURCES.txt
+-rw-r--r--   0 yohei      (504) staff       (20)        1 2023-04-19 22:09:53.000000 Izmon-1.1.2/Izmon.egg-info/dependency_links.txt
+-rw-r--r--   0 yohei      (504) staff       (20)        6 2023-04-19 22:09:53.000000 Izmon-1.1.2/Izmon.egg-info/top_level.txt
+-rwxrwxrwx   0 yohei      (504) staff       (20)      634 2023-03-02 11:44:52.000000 Izmon-1.1.2/LICENSE.txt
+-rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-19 22:09:53.949623 Izmon-1.1.2/PKG-INFO
+-rwxrwxrwx   0 yohei      (504) staff       (20)      492 2023-03-06 05:47:12.000000 Izmon-1.1.2/README.md
+-rw-r--r--   0 yohei      (504) staff       (20)       38 2023-04-19 22:09:53.949764 Izmon-1.1.2/setup.cfg
+-rwxrwxrwx   0 yohei      (504) staff       (20)      877 2023-04-19 21:39:44.000000 Izmon-1.1.2/setup.py
```

### Comparing `Izmon-1.1.1/Izmon/Class/Basic/Common_Function.py` & `Izmon-1.1.2/Izmon/Class/Basic/Common_Function.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Basic/Common_Variable.py` & `Izmon-1.1.2/Izmon/Class/Basic/Common_Variable.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Basic/Settings.py` & `Izmon-1.1.2/Izmon/Class/Basic/Settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	・PARTY_NUM
 	・LEVELUP_NUM (桁数)
 	・CODE_FELLOW_LEN
 	以上の 4 定数の " いずれか " を変更する際はコード と メジャーバージョンの変更が必要
 	'''
 
 	#バージョン
-	VERSION = '1.1.1'
+	VERSION = '1.1.2'
 	
 	#イズモンの数
 	IZ_NUM = 80
 
 	#イズモン設定一覧
 	IZUMON_SETTING = [[1 , "サーファー", 0, 162, 80, 115, 153, 111, 0.4, 0], [2 , "キョーリュー", 0, 166, 154, 115, 120, 120, 0.2, 0],
 					[3 , "ササントラ", 1, 167, 125, 110, 145, 110, 0.2, 0], [4 , "トラパルト", 2, 163, 140, 95, 120, 95, 0.2, 0],
```

### Comparing `Izmon-1.1.1/Izmon/Class/Battle/Battle.py` & `Izmon-1.1.2/Izmon/Class/Battle/Battle.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Battle/Battle_Caluculate.py` & `Izmon-1.1.2/Izmon/Class/Battle/Battle_Caluculate.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Battle/Battle_Other.py` & `Izmon-1.1.2/Izmon/Class/Battle/Battle_Other.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Battle/Battle_Set.py` & `Izmon-1.1.2/Izmon/Class/Battle/Battle_Set.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Dictionary.py` & `Izmon-1.1.2/Izmon/Class/Dictionary.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Gym.py` & `Izmon-1.1.2/Izmon/Class/Gym.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Save_Code/Decode.py` & `Izmon-1.1.2/Izmon/Class/Save_Code/Decode.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Save_Code/Encode.py` & `Izmon-1.1.2/Izmon/Class/Save_Code/Encode.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Set.py` & `Izmon-1.1.2/Izmon/Class/Set.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Start_End/End.py` & `Izmon-1.1.2/Izmon/Class/Start_End/End.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Class/Start_End/Start.py` & `Izmon-1.1.2/Izmon/Class/Start_End/Start.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/Izmon/Main.py` & `Izmon-1.1.2/Izmon/Main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 def main():
-	from Class.Basic.Common_Function import Common_Function as co_f
-	from Class.Gym import Gym
-	from Class.Dictionary import Dictionary as dic
-	from Class.Events.Events_Latest import Events_Latest as ev
-	from Class.Start_End.Start import Start
-	from Class.Start_End.End import End
-	from Class.Set import Set
-	from Class.Battle.Battle_Set import Battle_Set as bat_s
-	from Class.Battle.Battle import Battle as ba
-	# from Izmon.Class.Basic.Common_Function import Common_Function as co_f
-	# from Izmon.Class.Gym import Gym
-	# from Izmon.Class.Dictionary import Dictionary as dic
-	# from Izmon.Class.Events.Events_Latest import Events_Latest as ev
-	# from Izmon.Class.Start_End.Start import Start
-	# from Izmon.Class.Start_End.End import End
-	# from Izmon.Class.Set import Set
-	# from Izmon.Class.Battle.Battle_Set import Battle_Set as bat_s
-	# from Izmon.Class.Battle.Battle import Battle as ba
+	# from Class.Basic.Common_Function import Common_Function as co_f
+	# from Class.Gym import Gym
+	# from Class.Dictionary import Dictionary as dic
+	# from Class.Events.Events_Latest import Events_Latest as ev
+	# from Class.Start_End.Start import Start
+	# from Class.Start_End.End import End
+	# from Class.Set import Set
+	# from Class.Battle.Battle_Set import Battle_Set as bat_s
+	# from Class.Battle.Battle import Battle as ba
+	from Izmon.Class.Basic.Common_Function import Common_Function as co_f
+	from Izmon.Class.Gym import Gym
+	from Izmon.Class.Dictionary import Dictionary as dic
+	from Izmon.Class.Events.Events_Latest import Events_Latest as ev
+	from Izmon.Class.Start_End.Start import Start
+	from Izmon.Class.Start_End.End import End
+	from Izmon.Class.Set import Set
+	from Izmon.Class.Battle.Battle_Set import Battle_Set as bat_s
+	from Izmon.Class.Battle.Battle import Battle as ba
 	gym = Gym(); start = Start(); end = End(); set = Set()
 	start.set_up()
 	while True:
 		action = co_f.typing("どうしますか? 0:バトルする 1:ジムに行く 2:イズモン辞典 3:イベント 4:設定 5:やめる", 1, 6)
 		if action == 0:
 			enemy = bat_s.select_ene()
 			ba.battle(enemy, 0)
 		elif action == 1:
 			gym.gym_main()
 		elif action == 2:
-			dic.dic(0)
+			dic.dic()
 		elif action == 3:
 			ev.events()
 		elif action == 4:
 			set.main()
 		elif action ==5:
 			action = co_f.typing("本当にやめますか? 0:やめる 1:続ける", 1, 2)
 			if action == 0:
```

### Comparing `Izmon-1.1.1/Izmon.egg-info/PKG-INFO` & `Izmon-1.1.2/Izmon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Izmon
-Version: 1.1.1
+Version: 1.1.2
 Summary: You can play Izmon with this libraly.
 Home-page: https://github.com/akita0724
 Author: Yohei Akita, nabe, miso
 Author-email: akita.yohei0724@gmail.com
 License: GPL v2.0
 Keywords: Izmon
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `Izmon-1.1.1/Izmon.egg-info/SOURCES.txt` & `Izmon-1.1.2/Izmon.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 Izmon/Class/Basic/Settings.py
 Izmon/Class/Basic/__init__.py
 Izmon/Class/Battle/Battle.py
 Izmon/Class/Battle/Battle_Caluculate.py
 Izmon/Class/Battle/Battle_Other.py
 Izmon/Class/Battle/Battle_Set.py
 Izmon/Class/Battle/__init__.py
+Izmon/Class/CloudSave/Common.py
+Izmon/Class/CloudSave/Download.py
+Izmon/Class/CloudSave/Upload.py
+Izmon/Class/CloudSave/__init__.py
 Izmon/Class/Events/Events_Latest.py
 Izmon/Class/Events/Events_Passed.py
 Izmon/Class/Events/__init__.py
 Izmon/Class/Save_Code/Decode.py
 Izmon/Class/Save_Code/Encode.py
 Izmon/Class/Save_Code/__init__.py
 Izmon/Class/Start_End/End.py
```

### Comparing `Izmon-1.1.1/LICENSE.txt` & `Izmon-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.1/PKG-INFO` & `Izmon-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Izmon
-Version: 1.1.1
+Version: 1.1.2
 Summary: You can play Izmon with this libraly.
 Home-page: https://github.com/akita0724
 Author: Yohei Akita, nabe, miso
 Author-email: akita.yohei0724@gmail.com
 License: GPL v2.0
 Keywords: Izmon
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `Izmon-1.1.1/setup.py` & `Izmon-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 package_name = "Izmon"
 root_dir = path.abspath(path.dirname(__file__))
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version='1.1.1',
+    version='1.1.2',
     description='You can play Izmon with this libraly.',
     long_description=long_description,
     requires=["requests"],
     long_description_content_type='text/markdown',
     url='https://github.com/akita0724',
     author='Yohei Akita, nabe, miso',
     author_email='akita.yohei0724@gmail.com',
```

