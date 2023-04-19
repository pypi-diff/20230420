# Comparing `tmp/wg_utilities-3.5.0.tar.gz` & `tmp/wg_utilities-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.5.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.6.0.tar", max compression
```

## Comparing `wg_utilities-3.5.0.tar` & `wg_utilities-3.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-18 20:41:10.833203 wg_utilities-3.5.0/LICENSE
--rw-r--r--   0        0        0     2297 2023-04-18 20:41:10.833203 wg_utilities-3.5.0/README.md
--rw-r--r--   0        0        0     4825 2023-04-18 20:41:10.833203 wg_utilities-3.5.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      685 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4305 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10390 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24119 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56658 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7692 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    13531 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    15915 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    27118 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49179 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    22398 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-18 20:41:10.905202 wg_utilities-3.5.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/README.md
+-rw-r--r--   0        0        0     4825 2023-04-19 22:42:56.512128 wg_utilities-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      685 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4305 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24119 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56658 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7692 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13531 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15915 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    27248 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    50664 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    22398 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-19 22:42:56.592130 wg_utilities-3.6.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.6.0/PKG-INFO
```

### Comparing `wg_utilities-3.5.0/LICENSE` & `wg_utilities-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/README.md` & `wg_utilities-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/pyproject.toml` & `wg_utilities-3.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.5.0"
+version = "3.6.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.5.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.6.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.6.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/_google.py` & `wg_utilities-3.6.0/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.6.0/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.6.0/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.6.0/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.6.0/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.6.0/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.6.0/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.6.0/wg_utilities/clients/oauth_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             if not k.startswith("_") and not callable(v)
         }
 
         *_, validation_error = validate_model(
             self.__class__, model_dict, self.__class__  # type: ignore[arg-type]
         )
 
-        if validation_error:
+        if validation_error:  # pragma: no cover
             LOGGER.error(repr(validation_error))
             raise validation_error
 
 
 class BaseModelWithConfig(_ModelBase, BaseModel):
     """Reusable `BaseModel` with Config to apply to all subclasses."""
 
@@ -221,15 +221,18 @@
 
     ACCESS_TOKEN_ENDPOINT: str
     AUTH_LINK_BASE: str
     BASE_URL: str
 
     ACCESS_TOKEN_EXPIRY_THRESHOLD = 150
 
-    DEFAULT_CACHE_DIR = getenv("WG_UTILITIES_CREDS_CACHE_DIR")
+    # Second env var added for compatibility
+    DEFAULT_CACHE_DIR = getenv(
+        "WG_UTILITIES_CACHE_DIR", getenv("WG_UTILITIES_CREDS_CACHE_DIR")
+    )
     DEFAULT_PARAMS: dict[
         StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None
     ] = {}
     DEFAULT_SCOPES: list[str] = []
 
     HEADLESS_MODE = getenv("WG_UTILITIES_HEADLESS_MODE", "0") == "1"
 
@@ -693,15 +696,16 @@
             bool: has the access token expired?
         """
         if not hasattr(self, "_credentials"):
             if not self._load_local_credentials():
                 return True
 
         return (
-            self.credentials.expiry_epoch < time() + self.ACCESS_TOKEN_EXPIRY_THRESHOLD
+            self.credentials.expiry_epoch
+            < int(time()) + self.ACCESS_TOKEN_EXPIRY_THRESHOLD
         )
 
     @property
     def client_id(self) -> str:
         """Client ID for the Google API.
 
         Returns:
```

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.6.0/wg_utilities/clients/spotify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1062,14 +1062,44 @@
     )
     type: Literal["playlist"]
 
     _tracks: list[Track]
     _owner: User
 
     sj_type: ClassVar[type_[SpotifyEntityJson]] = PlaylistSummaryJson
+    _live_snapshot_id_timestamp: datetime
+    _live_snapshot_id: str
+
+    @property
+    def live_snapshot_id(self) -> str:
+        """The live snapshot ID of the playlist.
+
+        Returns:
+            str: the live snapshot ID of the playlist
+        """
+        if (
+            not hasattr(self, "_live_snapshot_id_timestamp")
+            or not hasattr(self, "_live_snapshot_id")
+            or datetime.utcnow() - self._live_snapshot_id_timestamp
+            > timedelta(minutes=1)
+        ):
+            self._set_private_attr(
+                "_live_snapshot_id",
+                self.spotify_client.get_json_response(
+                    f"/playlists/{self.id}", params={"fields": "snapshot_id"}
+                )[
+                    "snapshot_id"  # type: ignore[typeddict-item]
+                ],
+            )
+            self._set_private_attr(
+                "_live_snapshot_id_timestamp",
+                datetime.utcnow(),
+            )
+
+        return self._live_snapshot_id
 
     @property
     def owner(self) -> User:
         """Playlist owner.
 
         Returns:
             User: the Spotify user who owns this playlist
@@ -1089,31 +1119,45 @@
     def tracks(self) -> list[Track]:
         """Return a list of tracks in the playlist.
 
         Returns:
             list: a list of tracks in this playlist
         """
 
-        if not hasattr(self, "_tracks"):
+        if not hasattr(self, "_tracks") or self.updates_available:
             tracks = [
                 Track.from_json_response(
                     item["track"],
                     spotify_client=self.spotify_client,
                 )
                 for item in cast(
                     list[PlaylistFullJsonTracks],
                     self.spotify_client.get_items(f"/playlists/{self.id}/tracks"),
                 )
                 if "track" in item.keys() and item["is_local"] is False
             ]
 
             self._set_private_attr("_tracks", tracks)
 
+            if hasattr(self, "_live_snapshot_id"):
+                self.snapshot_id = self._live_snapshot_id
+            else:
+                self._set_private_attr("_live_snapshot_id", self.snapshot_id)
+
         return self._tracks
 
+    @property
+    def updates_available(self) -> bool:
+        """Check if the playlist has updates available.
+
+        Returns:
+            bool: whether the playlist has updates available
+        """
+        return self.live_snapshot_id != self.snapshot_id
+
     def __contains__(self, track: Track) -> bool:
         """Check if a track is in the playlist."""
         return track in self.tracks
 
     def __gt__(self, other: object) -> bool:
         """Compare two playlists by name and ID."""
         if not isinstance(other, Playlist):
```

### Comparing `wg_utilities-3.5.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.6.0/wg_utilities/clients/truelayer.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.6.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.6.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.6.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.6.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.6.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.6.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.6.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.6.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.6.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.6.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/json.py` & `wg_utilities-3.6.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/processes.py` & `wg_utilities-3.6.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.6.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/functions/xml.py` & `wg_utilities-3.6.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.6.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.6.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.5.0/PKG-INFO` & `wg_utilities-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.5.0
+Version: 3.6.0
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

