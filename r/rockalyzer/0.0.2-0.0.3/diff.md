# Comparing `tmp/rockalyzer-0.0.2.tar.gz` & `tmp/rockalyzer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockalyzer-0.0.2.tar", last modified: Fri Apr  7 13:51:35 2023, max compression
+gzip compressed data, was "rockalyzer-0.0.3.tar", last modified: Thu Apr 20 14:57:57 2023, max compression
```

## Comparing `rockalyzer-0.0.2.tar` & `rockalyzer-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:35.007264 rockalyzer-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      971 2023-04-07 13:51:35.007264 rockalyzer-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-07 13:32:17.000000 rockalyzer-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 13:51:35.008264 rockalyzer-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-04-07 13:51:31.000000 rockalyzer-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:35.003266 rockalyzer-0.0.2/src/
--rw-rw-rw-   0        0        0    32560 2023-03-30 15:25:48.000000 rockalyzer-0.0.2/src/Action.py
--rw-rw-rw-   0        0        0    64295 2023-03-30 20:00:09.000000 rockalyzer-0.0.2/src/Game.py
--rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.0.2/src/console_colors.py
--rw-rw-rw-   0        0        0     3696 2023-03-29 13:31:43.000000 rockalyzer-0.0.2/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:35.006264 rockalyzer-0.0.2/src/rockalyzer.egg-info/
--rw-rw-rw-   0        0        0      971 2023-04-07 13:51:34.000000 rockalyzer-0.0.2/src/rockalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-04-07 13:51:34.000000 rockalyzer-0.0.2/src/rockalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 13:51:34.000000 rockalyzer-0.0.2/src/rockalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-07 13:51:34.000000 rockalyzer-0.0.2/src/rockalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2023-04-07 13:51:34.000000 rockalyzer-0.0.2/src/rockalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4948 2023-04-07 13:04:45.000000 rockalyzer-0.0.2/src/rockalyzer.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:57:57.430270 rockalyzer-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-03-07 15:36:40.000000 rockalyzer-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1191 2023-04-20 14:57:57.429270 rockalyzer-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-04-17 18:37:04.000000 rockalyzer-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 14:57:57.430270 rockalyzer-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-04-20 08:13:12.000000 rockalyzer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:57:57.426143 rockalyzer-0.0.3/src/
+-rw-rw-rw-   0        0        0    32560 2023-03-30 15:25:48.000000 rockalyzer-0.0.3/src/Action.py
+-rw-rw-rw-   0        0        0    66086 2023-04-20 08:11:24.000000 rockalyzer-0.0.3/src/Game.py
+-rw-rw-rw-   0        0        0      205 2023-03-27 18:56:29.000000 rockalyzer-0.0.3/src/console_colors.py
+-rw-rw-rw-   0        0        0     4048 2023-04-20 08:11:58.000000 rockalyzer-0.0.3/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-20 14:57:57.429270 rockalyzer-0.0.3/src/rockalyzer.egg-info/
+-rw-rw-rw-   0        0        0     1191 2023-04-20 14:57:57.000000 rockalyzer-0.0.3/src/rockalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-04-20 14:57:57.000000 rockalyzer-0.0.3/src/rockalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 14:57:57.000000 rockalyzer-0.0.3/src/rockalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-20 14:57:57.000000 rockalyzer-0.0.3/src/rockalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 14:57:57.000000 rockalyzer-0.0.3/src/rockalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4948 2023-04-20 08:08:30.000000 rockalyzer-0.0.3/src/rockalyzer.py
```

### Comparing `rockalyzer-0.0.2/LICENSE` & `rockalyzer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.2/PKG-INFO` & `rockalyzer-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.2
-Summary: Rocket League Analyzer
+Version: 0.0.3
+Summary: Rocket League Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Rocket League Boxcars Replayer
+# Rocket League Boxcars-Replay Analyzer
 Here will be the documentation
 
+[![Downloads](https://static.pepy.tech/personalized-badge/rockalyzer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/rockalyzer)
+
 ## Installation
 Run the following to install:
 ```python
 pip install rockalyzer
 ```
 
 ## Usage
```

### Comparing `rockalyzer-0.0.2/setup.py` & `rockalyzer-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # read the contents of your README file for the long description
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='rockalyzer',
-    version='0.0.2',
-    description='Rocket League Analyzer',
+    version='0.0.3',
+    description='Rocket League Replay Analyzer',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/eliastheis/rockalyzer',
     author='Elias Theis',
     author_email='mail@eliastheis.de',
     py_modules=['rockalyzer', 'Game', 'Action', 'console_colors', 'constants'],
     package_dir={'': 'src'},
```

### Comparing `rockalyzer-0.0.2/src/Action.py` & `rockalyzer-0.0.3/src/Action.py`

 * *Files identical despite different names*

### Comparing `rockalyzer-0.0.2/src/Game.py` & `rockalyzer-0.0.3/src/Game.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.event_print = event_print
 
         # state stuff
         self.player_car_pairs = None
         self.ball_id = None
         self.seconds_remaining = 300
         self.frame_index = 0
+        self.game_playlist = None
 
         # render stuff
         if self.b_render:
             plt.style.use('dark_background')
             plt.ion()
             # set size of plot
             plt.figure(figsize=(10, 10))
@@ -344,15 +345,44 @@
                 case Action.ProjectX_GRI_X_Reservations:
                     self.actors[actor_id]['reservation'] = actor['attribute']['Reservation']
                 
                 case Action.ProjectX_GRI_X_ReplicatedServerRegion:
                     self.actors[actor_id]['region'] = actor['attribute']['String']
 
                 case Action.ProjectX_GRI_X_ReplicatedGamePlaylist:
-                    self.actors[actor_id]['game_playlist'] = actor['attribute']['Int']
+
+                    game_playlist_id = actor['attribute']['Int']
+                    game_playlist = 'unknown'
+
+                    if game_playlist_id == GAME_PLAYLIST_CASUAL_DUEL:
+                        game_playlist = 'casual_duel'
+                    elif game_playlist_id == GAME_PLAYLIST_CASUAL_DOUBLE:
+                        game_playlist = 'casual_double'
+                    elif game_playlist_id == GAME_PLAYLIST_CASUAL_STANDARD:
+                        game_playlist = 'casual_standard'
+                    elif game_playlist_id == GAME_PLAYLIST_CASUAL_CHAOS:
+                        game_playlist = 'casual_chaos'
+                    elif game_playlist_id == GAME_PLAYLIST_RANKED_DUEL:
+                        game_playlist = 'ranked_duel'
+                    elif game_playlist_id == GAME_PLAYLIST_RANKED_DOUBLE:
+                        game_playlist = 'ranked_double'
+                    elif game_playlist_id == GAME_PLAYLIST_RANKED_STANDARD:
+                        game_playlist = 'standard'
+                    elif game_playlist_id == GAME_PLAYLIST_RANKED_SNOWDAY:
+                        game_playlist = 'ranked_snowday'
+                    elif game_playlist_id == GAME_PLAYLIST_TOURNAMENT:
+                        game_playlist = 'tournament'
+                    else:
+                        game_playlist = f'unknown_{game_playlist_id}'
+                    
+                    if self.game_playlist is not None and self.game_playlist != game_playlist:
+                        print(WARNING, 'Game playlist changed from', self.game_playlist, 'to', game_playlist, ENDC)
+                        exit()
+                    else:
+                        self.game_playlist = game_playlist
                 
                 case Action.TAGame_Team_TA_GameEvent:
                     other_actor_id = actor['attribute']['ActiveActor']['actor']
                     if 'frames_with_event' not in self.actors[other_actor_id]:
                         self.actors[other_actor_id]['frames_with_event'] = []
                     self.actors[other_actor_id]['frames_with_event'].append(self.frame_index)
                 
@@ -1179,14 +1209,15 @@
         stats['scores'] = {}
         stats['scores']['Blue'] = 0 if 'Team0Score' not in properties else properties['Team0Score']
         stats['scores']['Orange'] = 0 if 'Team1Score' not in properties else properties['Team1Score']
         stats['replay_name'] = None if 'replay_name' not in properties else properties['ReplayName']
         stats['replay_id'] = properties['Id']
         stats['map_name'] = properties['MapName']
         stats['num_frames'] = properties['NumFrames']
+        stats['game_playlist'] = self.game_playlist if self.game_playlist is not None else 'unknown'
         
         # players
         stats['players'] = []
         player_stats = properties['PlayerStats']
         for player_id, car_id in self.player_car_pairs:
 
             player = {}
```

### Comparing `rockalyzer-0.0.2/src/constants.py` & `rockalyzer-0.0.3/src/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,7 +111,20 @@
     DEMO_LOCATION_ORANGE_LEFT_OUTSIDE
 ]
 
 # constants for detecting collisions
 BALL_HIT_BALL_SPEED = 200.0
 BALL_HIT_CAR_TO_BALL_DISTANCE = 310.0
 BALL_HIT_BALL_ANGLE_CHANGE_THRESHOLD = 1_000.0
+
+# Game Playlists (this list is not complete!)
+GAME_PLAYLIST_CASUAL_DUEL = 1
+GAME_PLAYLIST_CASUAL_DOUBLE = 2
+GAME_PLAYLIST_CASUAL_STANDARD = 3
+GAME_PLAYLIST_CASUAL_CHAOS = 4
+
+GAME_PLAYLIST_RANKED_DUEL = 10
+GAME_PLAYLIST_RANKED_DOUBLE = 11
+GAME_PLAYLIST_RANKED_STANDARD = 13
+
+GAME_PLAYLIST_TOURNAMENT = 22
+GAME_PLAYLIST_RANKED_SNOWDAY = 30
```

### Comparing `rockalyzer-0.0.2/src/rockalyzer.egg-info/PKG-INFO` & `rockalyzer-0.0.3/src/rockalyzer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: rockalyzer
-Version: 0.0.2
-Summary: Rocket League Analyzer
+Version: 0.0.3
+Summary: Rocket League Replay Analyzer
 Home-page: https://github.com/eliastheis/rockalyzer
 Author: Elias Theis
 Author-email: mail@eliastheis.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Rocket League Boxcars Replayer
+# Rocket League Boxcars-Replay Analyzer
 Here will be the documentation
 
+[![Downloads](https://static.pepy.tech/personalized-badge/rockalyzer?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/rockalyzer)
+
 ## Installation
 Run the following to install:
 ```python
 pip install rockalyzer
 ```
 
 ## Usage
```

### Comparing `rockalyzer-0.0.2/src/rockalyzer.py` & `rockalyzer-0.0.3/src/rockalyzer.py`

 * *Files identical despite different names*

