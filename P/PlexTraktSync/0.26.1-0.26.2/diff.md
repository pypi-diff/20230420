# Comparing `tmp/PlexTraktSync-0.26.1.tar.gz` & `tmp/PlexTraktSync-0.26.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-mdcu90ke/PlexTraktSync-0.26.1.tar", last modified: Mon Apr 17 14:03:48 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-m15nmrs5/PlexTraktSync-0.26.2.tar", last modified: Thu Apr 20 17:47:05 2023, max compression
```

## Comparing `PlexTraktSync-0.26.1.tar` & `PlexTraktSync-0.26.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 14:03:40.000000 PlexTraktSync-0.26.1/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 14:03:42.000000 PlexTraktSync-0.26.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:03:48.000000 PlexTraktSync-0.26.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-17 14:03:39.000000 PlexTraktSync-0.26.1/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 17:46:54.000000 PlexTraktSync-0.26.2/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-20 17:46:58.000000 PlexTraktSync-0.26.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:47:05.000000 PlexTraktSync-0.26.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-04-20 17:46:53.000000 PlexTraktSync-0.26.2/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.1/LICENSE` & `PlexTraktSync-0.26.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/PKG-INFO` & `PlexTraktSync-0.26.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.1
+Version: 0.26.2
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.2/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.1
+Version: 0.26.2
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.2/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.2/PlexTraktSync.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-attrs==22.2.0
+attrs==23.1.0
 certifi==2022.12.7
 charset-normalizer==3.1.0
 click==8.1.3
 deprecated==1.2.13
 inquirerpy==0.3.4
 oauthlib==3.2.2
 plexapi==4.13.4
 prompt-toolkit==3.0.38
 pygments==2.15.0
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.21
+pytrakt==3.4.22
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests==2.28.2
 rich==13.3.4
 tqdm==4.65.0
 urllib3==1.26.15
 wcwidth==0.2.6
```

### Comparing `PlexTraktSync-0.26.1/README.md` & `PlexTraktSync-0.26.2/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/cli.py` & `PlexTraktSync-0.26.2/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.2/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.2/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.2/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.2/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.2/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.2/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.2/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.2/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.2/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.2/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/logging.py` & `PlexTraktSync-0.26.2/plextraktsync/logging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/media.py` & `PlexTraktSync-0.26.2/plextraktsync/media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.2/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.2/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.2/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.2/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.2/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.2/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.2/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.2/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/sync.py` & `PlexTraktSync-0.26.2/plextraktsync/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.2/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.2/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.2/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.2/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.2/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.2/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.2/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.2/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.2/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.2/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/walker.py` & `PlexTraktSync-0.26.2/plextraktsync/walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.2/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/requirements.txt` & `PlexTraktSync-0.26.2/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # These requirements were autogenerated by pipenv
 # To regenerate from the project's Pipfile, run:
 #
 #    pipenv lock --requirements
 #
 
-attrs==22.2.0
+attrs==23.1.0
 backports.cached-property==1.0.2; python_version <= '3.7'
 cattrs==22.2.0; python_version >= '3.7'
 certifi==2022.12.7
 charset-normalizer==3.1.0
 click==8.1.3
 deprecated==1.2.13
 idna==3.4; python_version >= '3.5'
@@ -21,15 +21,15 @@
 platformdirs==3.2.0; python_version >= '3.7'
 plexapi==4.13.4
 prompt-toolkit==3.0.38
 pygments==2.15.0
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
-pytrakt==3.4.21
+pytrakt==3.4.22
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests-oauthlib==1.3.1; python_version >= '3.4'
 requests==2.28.2
 rich==13.3.4
 six==1.16.0; python_version >= '3.4'
 tqdm==4.65.0
```

### Comparing `PlexTraktSync-0.26.1/setup.cfg` & `PlexTraktSync-0.26.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.2/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_config.py` & `PlexTraktSync-0.26.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_events.py` & `PlexTraktSync-0.26.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_new_agent.py` & `PlexTraktSync-0.26.2/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_timer.py` & `PlexTraktSync-0.26.2/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.2/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.2/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.1/tests/test_walker.py` & `PlexTraktSync-0.26.2/tests/test_walker.py`

 * *Files identical despite different names*

