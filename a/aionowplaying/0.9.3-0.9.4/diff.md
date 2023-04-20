# Comparing `tmp/aionowplaying-0.9.3.tar.gz` & `tmp/aionowplaying-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aionowplaying-0.9.3.tar", max compression
+gzip compressed data, was "aionowplaying-0.9.4.tar", max compression
```

## Comparing `aionowplaying-0.9.3.tar` & `aionowplaying-0.9.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2022-01-17 01:33:16.709617 aionowplaying-0.9.3/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-01-17 01:23:49.022832 aionowplaying-0.9.3/README.md
--rw-r--r--   0        0        0      522 2022-02-07 03:32:14.444699 aionowplaying-0.9.3/aionowplaying/__init__.py
--rw-r--r--   0        0        0      626 2022-04-08 05:52:38.131792 aionowplaying-0.9.3/aionowplaying/interface/__init__.py
--rw-r--r--   0        0        0     7604 2022-04-08 05:52:08.749871 aionowplaying-0.9.3/aionowplaying/interface/base.py
--rw-r--r--   0        0        0     2745 2022-05-12 11:12:29.545349 aionowplaying-0.9.3/aionowplaying/interface/macos.py
--rw-r--r--   0        0        0    11957 2022-01-26 09:17:40.338085 aionowplaying-0.9.3/aionowplaying/interface/mpris2.py
--rw-r--r--   0        0        0    10211 2023-04-13 15:30:05.909042 aionowplaying-0.9.3/aionowplaying/interface/windows.py
--rw-r--r--   0        0        0      845 2023-04-13 15:34:24.635413 aionowplaying-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 aionowplaying-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-01-17 01:33:16.709617 aionowplaying-0.9.4/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-01-17 01:23:49.022832 aionowplaying-0.9.4/README.md
+-rw-r--r--   0        0        0      522 2022-02-07 03:32:14.444699 aionowplaying-0.9.4/aionowplaying/__init__.py
+-rw-r--r--   0        0        0      626 2022-04-08 05:52:38.131792 aionowplaying-0.9.4/aionowplaying/interface/__init__.py
+-rw-r--r--   0        0        0     7472 2023-04-20 09:47:26.269522 aionowplaying-0.9.4/aionowplaying/interface/base.py
+-rw-r--r--   0        0        0     4492 2023-04-20 09:47:26.269522 aionowplaying-0.9.4/aionowplaying/interface/macos.py
+-rw-r--r--   0        0        0    12045 2023-04-14 08:04:55.689069 aionowplaying-0.9.4/aionowplaying/interface/mpris2.py
+-rw-r--r--   0        0        0    10636 2023-04-20 09:47:26.271522 aionowplaying-0.9.4/aionowplaying/interface/windows.py
+-rw-r--r--   0        0        0      931 2023-04-20 09:47:42.453853 aionowplaying-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 aionowplaying-0.9.4/PKG-INFO
```

### Comparing `aionowplaying-0.9.3/LICENSE.txt` & `aionowplaying-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aionowplaying-0.9.3/aionowplaying/__init__.py` & `aionowplaying-0.9.4/aionowplaying/__init__.py`

 * *Files identical despite different names*

### Comparing `aionowplaying-0.9.3/aionowplaying/interface/__init__.py` & `aionowplaying-0.9.4/aionowplaying/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `aionowplaying-0.9.3/aionowplaying/interface/base.py` & `aionowplaying-0.9.4/aionowplaying/interface/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     PlaybackStatus = "PlaybackStatus"
     LoopStatus = "LoopStatus"
     Rate = "Rate"
     Shuffle = "Shuffle"
     Metadata = "Metadata"
     Volume = "Volume"
     Position = "Position"
+    Duration = "Duration"
     MinimumRate = "MinimumRate"
     MaximumRate = "MaximumRate"
     CanGoNext = "CanGoNext"
     CanGoPrevious = "CanGoPrevious"
     CanPlay = "CanPlay"
     CanPause = "CanPause"
     CanSeek = "CanSeek"
@@ -94,14 +95,15 @@
     PlaybackStatus: 'PlaybackStatus' = PlaybackStatus.Stopped
     LoopStatus: 'LoopStatus' = LoopStatus.None_
     Rate: float = 1.0
     Shuffle: bool = False
     Metadata: MetadataBean = MetadataBean()
     Volume: float = 1.0
     Position: int = 0  # in microseconds
+    Duration: int = 0  # in microseconds
     MinimumRate: float = 1.0
     MaximumRate: float = 1.0
     CanGoNext: bool = False
     CanGoPrevious: bool = False
     CanPlay: bool = False
     CanPause: bool = False
     CanSeek: bool = False
@@ -206,18 +208,16 @@
     async def on_play_pause(self):
         """
         This will be called when nowplaying backend want to play or pause playback.
         This will only be called if you set :attr:`PlaybackProperties.CanPause` to True.
         """
         if self.get_playback_property(PlaybackPropertyName.PlaybackStatus) == PlaybackStatus.Playing:
             await self.on_pause()
-            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Paused)
         else:
             await self.on_play()
-            self.set_playback_property(PlaybackPropertyName.PlaybackStatus, PlaybackStatus.Playing)
 
     async def on_play(self):
         """
         This will be called when nowplaying backend want to play playback.
         This will only be called if you set :attr:`PlaybackProperties.CanPlay` to True.
         """
         pass
```

### Comparing `aionowplaying-0.9.3/aionowplaying/interface/mpris2.py` & `aionowplaying-0.9.4/aionowplaying/interface/mpris2.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,19 +294,22 @@
     def get_tracklist_property(self, name: TrackListPropertyName) -> Any:
         return self._tracklist_bus.get_property(name.value)
 
     async def seeked(self, position: int):
         await self._player_bus.seeked(position)
 
     async def start(self):
-        bus = await MessageBus().connect()
-        bus.export(self._object_path, self._bus)
-        bus.export(self._object_path, self._player_bus)
-        await bus.request_name(self._bus_name)
-        await bus.wait_for_disconnect()
+        self.dbus = await MessageBus().connect()
+        self.dbus.export(self._object_path, self._bus)
+        self.dbus.export(self._object_path, self._player_bus)
+        await self.dbus.request_name(self._bus_name)
+        await self.dbus.wait_for_disconnect()
+
+    async def stop(self):
+        self.dbus.disconnect()
 
 
 if __name__ == '__main__':
     import asyncio
 
     mp = Mpris2Interface('aionowplaying')
     mp.set_property(PropertyName.CanQuit, True)
```

### Comparing `aionowplaying-0.9.3/aionowplaying/interface/windows.py` & `aionowplaying-0.9.4/aionowplaying/interface/windows.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import threading
 from typing import Any
 from datetime import timedelta
 
 from winsdk.windows.foundation import Uri
 from winsdk.windows.foundation.collections import IVector
 from winsdk.windows.media import SystemMediaTransportControlsTimelineProperties, SystemMediaTransportControls, \
     SystemMediaTransportControlsDisplayUpdater, MediaPlaybackStatus, MediaPlaybackType, MediaPlaybackAutoRepeatMode, \
@@ -21,14 +22,15 @@
 def TimeSpan(x):
     return timedelta(microseconds=x/10000)
 
 
 class WindowsInterface(BaseInterface):
     def __init__(self, name):
         super(WindowsInterface, self).__init__(name)
+        self._loop = asyncio.get_event_loop()
         self._running = True
         self._playback_properties = PlaybackProperties()
         self._player = MediaPlayer()
         self._controls: SystemMediaTransportControls = self._player.system_media_transport_controls
         self._updater: SystemMediaTransportControlsDisplayUpdater = self._controls.display_updater
         self._timeline = SystemMediaTransportControlsTimelineProperties()
         self._controls.add_auto_repeat_mode_change_requested(self.auto_repeat_mode_change_requested)
@@ -37,79 +39,79 @@
         self._controls.add_playback_rate_change_requested(self.playback_rate_change_requested)
         self._controls.add_property_changed(self.property_changed)
         self._controls.add_shuffle_enabled_change_requested(self.shuffle_change_requested)
 
     def shuffle_change_requested(self, _, args: ShuffleEnabledChangeRequestedEventArgs):
         shuffle_enabled: bool = args.requested_shuffle_enabled
         if asyncio.iscoroutinefunction(self.on_shuffle):
-            asyncio.run(self.on_shuffle(shuffle_enabled))
+            self._run_task(self.on_shuffle(shuffle_enabled))
         else:
             self.on_shuffle(shuffle_enabled)
 
     def property_changed(self, _, args: SystemMediaTransportControlsPropertyChangedEventArgs):
         property_: SystemMediaTransportControlsProperty = args.property
         if property_ == SystemMediaTransportControlsProperty.SOUND_LEVEL:
             if asyncio.iscoroutinefunction(self.on_volume):
-                asyncio.run(self.on_volume(self._controls.sound_level))
+                self._run_task(self.on_volume(self._controls.sound_level))
             else:
                 self.on_volume(self._controls.sound_level)
 
     def playback_rate_change_requested(self, _, args: PlaybackRateChangeRequestedEventArgs):
         rate: float = args.requested_playback_rate
         if asyncio.iscoroutinefunction(self.on_rate):
-            asyncio.run(self.on_rate(rate))
+            self._run_task(self.on_rate(rate))
         else:
             self.on_rate(rate)
 
     def playback_position_change_requested(self, _, args: PlaybackPositionChangeRequestedEventArgs):
         position = args.requested_playback_position
         if self._playback_properties.CanSeek:
             if asyncio.iscoroutinefunction(self.on_set_position):
-                asyncio.run(self.on_set_position(self._playback_properties.Metadata.id_, int(position.duration / 10000)))
-                asyncio.run(self.on_seek(int(position.duration / 10000)))
+                self._run_task(self.on_set_position(self._playback_properties.Metadata.id_, int(position.duration / 10000)))
+                self._run_task(self.on_seek(int(position.duration / 10000)))
             else:
                 self.on_set_position(self._playback_properties.Metadata.id_, int(position.duration / 10000))
                 self.on_seek(int(position.duration / 10000))
 
     def button_pressed(self, _, args: SystemMediaTransportControlsButtonPressedEventArgs):
         button: SystemMediaTransportControlsButton = args.button
         if button == SystemMediaTransportControlsButton.PLAY and self._playback_properties.CanPlay:
             if asyncio.iscoroutinefunction(self.on_play):
-                asyncio.run(self.on_play())
+                self._run_task(self.on_play())
             else:
                 self.on_play()
             self._controls.playback_status = MediaPlaybackStatus.PLAYING
             self._playback_properties.PlaybackStatus = PlaybackStatus.Playing
         if button == SystemMediaTransportControlsButton.PAUSE and self._playback_properties.CanPause:
             if asyncio.iscoroutinefunction(self.on_pause):
-                asyncio.run(self.on_pause())
+                self._run_task(self.on_pause())
             else:
                 self.on_pause()
             self._controls.playback_status = MediaPlaybackStatus.PAUSED
             self._playback_properties.PlaybackStatus = PlaybackStatus.Paused
         if button == SystemMediaTransportControlsButton.NEXT and self._playback_properties.CanGoNext:
             if asyncio.iscoroutinefunction(self.on_next):
-                asyncio.run(self.on_next())
+                self._run_task(self.on_next())
             else:
                 self.on_next()
         if button == SystemMediaTransportControlsButton.PREVIOUS and self._playback_properties.CanGoPrevious:
             if asyncio.iscoroutinefunction(self.on_previous):
-                asyncio.run(self.on_previous())
+                self._run_task(self.on_previous())
             else:
                 self.on_previous()
 
     def auto_repeat_mode_change_requested(self, _, args: AutoRepeatModeChangeRequestedEventArgs):
         value = LoopStatus.None_
         mode: MediaPlaybackAutoRepeatMode = args.requested_auto_repeat_mode
         if mode == MediaPlaybackAutoRepeatMode.LIST:
             value = LoopStatus.Playlist
         elif mode == MediaPlaybackAutoRepeatMode.TRACK:
             value = LoopStatus.Track
         if asyncio.iscoroutinefunction(self.on_loop_status):
-            asyncio.run(self.on_loop_status(value))
+            self._run_task(self.on_loop_status(value))
         else:
             self.on_loop_status(value)
         self._playback_properties.LoopStatus = value
 
     def set_property(self, name: PropertyName, value: Any):
         pass
 
@@ -165,16 +167,16 @@
             self._updater.type = MediaPlaybackType.MUSIC
         self._updater.app_media_id = value.id_
         self._updater.music_properties.artist = ','.join(value.artist)
         self._updater.music_properties.title = value.title
         self._updater.music_properties.album_title = value.album
         self._updater.music_properties.genres: IVector
         self._updater.music_properties.genres.replace_all(value.genre)
-        if value.url is not None and value.url != '':
-            self._updater.thumbnail = RandomAccessStreamReference.create_from_uri(Uri(value.url))
+        if value.cover:  # not None and not empty
+            self._updater.thumbnail = RandomAccessStreamReference.create_from_uri(Uri(value.cover))
         self._updater.update()
         # update timeline
         self._timeline.start_time = TimeSpan(0)
         self._timeline.end_time = TimeSpan(value.duration * 10000)
         self._timeline.min_seek_time = TimeSpan(0)
         self._timeline.max_seek_time = TimeSpan(value.duration * 10000)
         self._controls.update_timeline_properties(self._timeline)
@@ -192,7 +194,15 @@
         try:
             self._player.close()
         except:
             pass
 
     async def stop(self):
         self._running = False
+
+    def _run_task(self, task):
+        # Windows callbacks may be invoked in non-main thread, besides,
+        # they may run in different threads.
+        if threading.current_thread() is not threading.main_thread():
+            asyncio.run_coroutine_threadsafe(task, self._loop)
+        else:
+            asyncio.create_task(task)
```

### Comparing `aionowplaying-0.9.3/pyproject.toml` & `aionowplaying-0.9.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "aionowplaying"
-version = "0.9.3"
+version = "0.9.4"
 license = "GPL-3.0-only"
 description = "A cross-platform Now Playing client"
 authors = ["Bruce Zhang <zttt183525594@gmail.com>"]
 maintainers = ["Bruce Zhang <zttt183525594@gmail.com>"]
 keywords = ["nowplaying", "mpris"]
 readme = "README.md"
 repository = "https://github.com/BruceZhang1993/aionowplaying"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
+python = ">=3.7,<3.12"
 pydantic = "*"
 dbus-next = { version = "*", platform = "linux" }
 winsdk = { version = "*", platform = "win32" }
-pyobjc = { version = "*", platform = "darwin" }
+pyobjc-framework-MediaPlayer = { version = "*", platform = "darwin" }
+pyobjc-framework-Cocoa = { version = "*", platform = "darwin" }
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 poetry2setup = "^1.0.0"
 
 [build-system]
```

### Comparing `aionowplaying-0.9.3/PKG-INFO` & `aionowplaying-0.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: aionowplaying
-Version: 0.9.3
+Version: 0.9.4
 Summary: A cross-platform Now Playing client
 Home-page: https://github.com/BruceZhang1993/aionowplaying
 License: GPL-3.0-only
 Keywords: nowplaying,mpris
 Author: Bruce Zhang
 Author-email: zttt183525594@gmail.com
 Maintainer: Bruce Zhang
 Maintainer-email: zttt183525594@gmail.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dbus-next ; sys_platform == "linux"
 Requires-Dist: pydantic
-Requires-Dist: pyobjc ; sys_platform == "darwin"
+Requires-Dist: pyobjc-framework-Cocoa ; sys_platform == "darwin"
+Requires-Dist: pyobjc-framework-MediaPlayer ; sys_platform == "darwin"
 Requires-Dist: winsdk ; sys_platform == "win32"
 Project-URL: Bug Tracker, https://github.com/BruceZhang1993/aionowplaying/issues
 Project-URL: Repository, https://github.com/BruceZhang1993/aionowplaying
 Description-Content-Type: text/markdown
```

