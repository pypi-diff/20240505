# Comparing `tmp/plextraktsync-0.30.2.tar.gz` & `tmp/plextraktsync-0.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plextraktsync-0.30.2.tar", last modified: Thu May  2 15:28:51 2024, max compression
+gzip compressed data, was "plextraktsync-0.30.3.tar", last modified: Sun May  5 16:36:07 2024, max compression
```

## Comparing `plextraktsync-0.30.2.tar` & `plextraktsync-0.30.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.168800 plextraktsync-0.30.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    30188 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30188 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 15:28:51.000000 plextraktsync-0.30.2/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.140799 plextraktsync-0.30.2/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.144799 plextraktsync-0.30.2/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.144799 plextraktsync-0.30.2/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/ServerConfigFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/coro.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/logger/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/media/
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/media/Media.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/media/MediaFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/RichMarkup.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/mixin/SetWindowTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.148799 plextraktsync-0.30.2/plextraktsync/plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkPlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/WalkPlanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plan/Walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderIMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderMbid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTMDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTVDB.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexId.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexIdFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylistCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexSectionPager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plex/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/queue/TraktScrobbleWorker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.152799 plextraktsync-0.30.2/plextraktsync/rich/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/rich/RichHighlighter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/rich/RichProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.156799 plextraktsync-0.30.2/plextraktsync/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/AddCollectionPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/ClearCollectedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/LikedListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/Sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/SyncRatingsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/SyncWatchedPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/TraktListsPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/WatchListPlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/WatchProgressPlugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.156799 plextraktsync-0.30.2/plextraktsync/sync/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/sync/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.160800 plextraktsync-0.30.2/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktUserList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktUserListCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/WatchProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/trakt/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.160800 plextraktsync-0.30.2/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/util/remove_empty_values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 15:28:47.000000 plextraktsync-0.30.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 15:28:51.168800 plextraktsync-0.30.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:28:51.164800 plextraktsync-0.30.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_plex_id.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_rating.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-02 15:28:43.000000 plextraktsync-0.30.2/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.528859 plextraktsync-0.30.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-05-05 16:36:07.528859 plextraktsync-0.30.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.528859 plextraktsync-0.30.3/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30216 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 16:36:07.000000 plextraktsync-0.30.3/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26812 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.504859 plextraktsync-0.30.3/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.508859 plextraktsync-0.30.3/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.508859 plextraktsync-0.30.3/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/ServerConfigFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.512859 plextraktsync-0.30.3/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/coro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.512859 plextraktsync-0.30.3/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/logger/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.512859 plextraktsync-0.30.3/plextraktsync/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/media/Media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/media/MediaFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.512859 plextraktsync-0.30.3/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/mixin/RichMarkup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/mixin/SetWindowTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.512859 plextraktsync-0.30.3/plextraktsync/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plan/WalkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plan/WalkPlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plan/WalkPlanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plan/Walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.516859 plextraktsync-0.30.3/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderIMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderMbid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderTMDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderTVDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexIdFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexPlaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexPlaylistCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexSectionPager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plex/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.516859 plextraktsync-0.30.3/plextraktsync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.516859 plextraktsync-0.30.3/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/queue/TraktScrobbleWorker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.516859 plextraktsync-0.30.3/plextraktsync/rich/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/rich/RichHighlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/rich/RichProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.520859 plextraktsync-0.30.3/plextraktsync/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/AddCollectionPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/ClearCollectedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/LikedListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/SyncRatingsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/SyncWatchedPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/TraktListsPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/WatchListPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/WatchProgressPlugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.520859 plextraktsync-0.30.3/plextraktsync/sync/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/plugin/SyncPluginInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/plugin/SyncPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/sync/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.520859 plextraktsync-0.30.3/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktUserList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktUserListCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/WatchProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/trakt/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.524859 plextraktsync-0.30.3/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/Rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/util/remove_empty_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.524859 plextraktsync-0.30.3/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-05 16:36:04.000000 plextraktsync-0.30.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-05 16:36:07.528859 plextraktsync-0.30.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:36:07.528859 plextraktsync-0.30.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1923 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2703 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      977 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2104 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_plex_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      529 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_rating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      503 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1174 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      572 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3584 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-05-05 16:35:57.000000 plextraktsync-0.30.3/tests/test_walker.py
```

### Comparing `plextraktsync-0.30.2/LICENSE` & `plextraktsync-0.30.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/PKG-INFO` & `plextraktsync-0.30.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.2
+Version: 0.30.3
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,38 +22,38 @@
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: decorator==5.1.1; python_version >= "3.5"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
+Requires-Dist: exceptiongroup==1.2.1; python_version < "3.11"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.1; python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
-Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
+Requires-Dist: tqdm==4.66.4; python_version >= "3.7"
 Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
```

### Comparing `plextraktsync-0.30.2/PlexTraktSync.egg-info/PKG-INFO` & `plextraktsync-0.30.3/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.30.2
+Version: 0.30.3
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,38 +22,38 @@
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: cattrs==23.2.3; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: certifi==2024.2.2; python_version >= "3.6"
 Requires-Dist: charset-normalizer==3.3.2; python_full_version >= "3.7.0"
 Requires-Dist: click==8.1.7; python_version >= "3.7"
 Requires-Dist: decorator==5.1.1; python_version >= "3.5"
 Requires-Dist: deprecated==1.2.14; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
-Requires-Dist: exceptiongroup==1.2.1; python_version >= "3.7"
+Requires-Dist: exceptiongroup==1.2.1; python_version < "3.11"
 Requires-Dist: humanize==4.9.0; python_version >= "3.8"
 Requires-Dist: idna==3.7; python_version >= "3.5"
 Requires-Dist: inquirerpy==0.3.4; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: markdown-it-py==3.0.0; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: mdurl==0.1.2; python_version >= "3.7"
 Requires-Dist: oauthlib==3.2.2; python_version >= "3.6"
 Requires-Dist: pfzy==0.3.4; python_version >= "3.7" and python_version < "4.0"
-Requires-Dist: platformdirs==4.2.1; python_version >= "3.8"
+Requires-Dist: platformdirs==4.2.1; python_version >= "3.7" and python_version >= "3.8"
 Requires-Dist: plexapi==4.15.12; python_version >= "3.8"
 Requires-Dist: pluggy==1.5.0; python_version >= "3.8"
 Requires-Dist: prompt-toolkit==3.0.43; python_full_version >= "3.7.0"
 Requires-Dist: pygments==2.17.2; python_version >= "3.7"
 Requires-Dist: python-dotenv==1.0.1; python_version >= "3.8"
 Requires-Dist: python-git-info==0.8.3
 Requires-Dist: pytimeparse==1.1.8
 Requires-Dist: pytrakt==3.4.32
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
 Requires-Dist: requests==2.31.0; python_version >= "3.7"
 Requires-Dist: requests-cache==1.2.0; python_version >= "3.8"
 Requires-Dist: requests-oauthlib==2.0.0; python_version >= "3.4"
 Requires-Dist: rich==13.7.1; python_full_version >= "3.7.0"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"
-Requires-Dist: tqdm==4.66.2; python_version >= "3.7"
+Requires-Dist: tqdm==4.66.4; python_version >= "3.7"
 Requires-Dist: types-decorator==5.1.8.20240310; python_version >= "3.8"
 Requires-Dist: typing-extensions==4.11.0; python_version < "3.9"
 Requires-Dist: url-normalize==1.4.3; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5" and python_version >= "3.6"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: wcwidth==0.2.13
 Requires-Dist: websocket-client==1.8.0; python_version >= "3.8"
 Requires-Dist: wrapt==1.16.0; python_version >= "3.5" and python_version >= "3.6"
```

### Comparing `plextraktsync-0.30.2/PlexTraktSync.egg-info/SOURCES.txt` & `plextraktsync-0.30.3/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/PlexTraktSync.egg-info/requires.txt` & `plextraktsync-0.30.3/PlexTraktSync.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 wcwidth==0.2.13
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.3.2
 prompt-toolkit==3.0.43
 rich==13.7.1
 
+[:python_version < "3.11"]
+exceptiongroup==1.2.1
+
 [:python_version < "3.9"]
 typing-extensions==4.11.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
 deprecated==1.2.14
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3" and python_version >= "3.4"]
@@ -34,32 +37,31 @@
 certifi==2024.2.2
 oauthlib==3.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.7"]
 attrs==23.2.0
 click==8.1.7
-exceptiongroup==1.2.1
 mdurl==0.1.2
 pygments==2.17.2
 requests==2.31.0
-tqdm==4.66.2
+tqdm==4.66.4
 
 [:python_version >= "3.7" and python_version < "4.0"]
 inquirerpy==0.3.4
 pfzy==0.3.4
 
 [:python_version >= "3.7" and python_version >= "3.8"]
 cattrs==23.2.3
 markdown-it-py==3.0.0
+platformdirs==4.2.1
 
 [:python_version >= "3.8"]
 apluggy==0.9.4
 humanize==4.9.0
-platformdirs==4.2.1
 plexapi==4.15.12
 pluggy==1.5.0
 python-dotenv==1.0.1
 requests-cache==1.2.0
 types-decorator==5.1.8.20240310
 urllib3==2.2.1
 websocket-client==1.8.0
```

### Comparing `plextraktsync-0.30.2/README.md` & `plextraktsync-0.30.3/README.md`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/cli.py` & `plextraktsync-0.30.3/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/bug_report.py` & `plextraktsync-0.30.3/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/cache.py` & `plextraktsync-0.30.3/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/clear_collections.py` & `plextraktsync-0.30.3/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/config.py` & `plextraktsync-0.30.3/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/download.py` & `plextraktsync-0.30.3/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/imdb_import.py` & `plextraktsync-0.30.3/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/info.py` & `plextraktsync-0.30.3/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/inspect.py` & `plextraktsync-0.30.3/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/login.py` & `plextraktsync-0.30.3/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/plex_login.py` & `plextraktsync-0.30.3/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/self_update.py` & `plextraktsync-0.30.3/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/sync.py` & `plextraktsync-0.30.3/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/trakt_login.py` & `plextraktsync-0.30.3/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/unmatched.py` & `plextraktsync-0.30.3/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/watch.py` & `plextraktsync-0.30.3/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/commands/watched_shows.py` & `plextraktsync-0.30.3/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/Config.py` & `plextraktsync-0.30.3/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/ConfigLoader.py` & `plextraktsync-0.30.3/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/HttpCacheConfig.py` & `plextraktsync-0.30.3/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/PlexServerConfig.py` & `plextraktsync-0.30.3/plextraktsync/config/PlexServerConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/ServerConfigFactory.py` & `plextraktsync-0.30.3/plextraktsync/config/ServerConfigFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config/SyncConfig.py` & `plextraktsync-0.30.3/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/config.default.yml` & `plextraktsync-0.30.3/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/decorators/measure_time.py` & `plextraktsync-0.30.3/plextraktsync/decorators/measure_time.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/decorators/rate_limit.py` & `plextraktsync-0.30.3/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/decorators/retry.py` & `plextraktsync-0.30.3/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/logger/filter.py` & `plextraktsync-0.30.3/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/logger/init.py` & `plextraktsync-0.30.3/plextraktsync/logger/init.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/media/Media.py` & `plextraktsync-0.30.3/plextraktsync/media/Media.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/media/MediaFactory.py` & `plextraktsync-0.30.3/plextraktsync/media/MediaFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/mixin/ChangeNotifier.py` & `plextraktsync-0.30.3/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plan/WalkConfig.py` & `plextraktsync-0.30.3/plextraktsync/plan/WalkConfig.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plan/WalkPlanner.py` & `plextraktsync-0.30.3/plextraktsync/plan/WalkPlanner.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plan/Walker.py` & `plextraktsync-0.30.3/plextraktsync/plan/Walker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexApi.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexAudioCodec.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexGuid.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProvider.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProvider.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderMbid.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderMbid.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexGuidProviderTMDB.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexGuidProviderTMDB.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexId.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexId.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexIdFactory.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexIdFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexLibraryItem.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexLibrarySection.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexPlaylist.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexPlaylist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexRatings.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexSectionPager.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexSectionPager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexServerConnection.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/PlexWatchList.py` & `plextraktsync-0.30.3/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/plex/SessionCollection.py` & `plextraktsync-0.30.3/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/pytrakt_extensions.py` & `plextraktsync-0.30.3/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/queue/BackgroundTask.py` & `plextraktsync-0.30.3/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/queue/Queue.py` & `plextraktsync-0.30.3/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/queue/TraktBatchWorker.py` & `plextraktsync-0.30.3/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/queue/TraktMarkWatchedWorker.py` & `plextraktsync-0.30.3/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/queue/TraktScrobbleWorker.py` & `plextraktsync-0.30.3/plextraktsync/queue/TraktScrobbleWorker.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/rich/RichHighlighter.py` & `plextraktsync-0.30.3/plextraktsync/rich/RichHighlighter.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/rich/RichProgressBar.py` & `plextraktsync-0.30.3/plextraktsync/rich/RichProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/AddCollectionPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/AddCollectionPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/ClearCollectedPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/ClearCollectedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/LikedListsPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/LikedListsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/Sync.py` & `plextraktsync-0.30.3/plextraktsync/sync/Sync.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/SyncRatingsPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/SyncRatingsPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/SyncWatchedPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/SyncWatchedPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/TraktListsPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/TraktListsPlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     @staticmethod
     def enabled(config):
         return any([
             # LikedListsPlugin
             config.sync_liked_lists,
             # WatchListPlugin
-            config.sync_watchlists,
+            config.update_plex_wl_as_pl,
         ])
 
     @classmethod
     def factory(cls, sync):
         return cls()
 
     @hookimpl(trylast=True)
```

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/WatchListPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/WatchListPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/WatchProgressPlugin.py` & `plextraktsync-0.30.3/plextraktsync/sync/WatchProgressPlugin.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginInterface.py` & `plextraktsync-0.30.3/plextraktsync/sync/plugin/SyncPluginInterface.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/sync/plugin/SyncPluginManager.py` & `plextraktsync-0.30.3/plextraktsync/sync/plugin/SyncPluginManager.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerCollection.py` & `plextraktsync-0.30.3/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/ScrobblerProxy.py` & `plextraktsync-0.30.3/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktApi.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktLookup.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktRatingCollection.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktUserList.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktUserList.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktUserListCollection.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktUserListCollection.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/TraktWatchlist.py` & `plextraktsync-0.30.3/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/trakt/WatchProgress.py` & `plextraktsync-0.30.3/plextraktsync/trakt/WatchProgress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/Factory.py` & `plextraktsync-0.30.3/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/Path.py` & `plextraktsync-0.30.3/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/Rating.py` & `plextraktsync-0.30.3/plextraktsync/util/Rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/Timer.py` & `plextraktsync-0.30.3/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/Version.py` & `plextraktsync-0.30.3/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/local_url.py` & `plextraktsync-0.30.3/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/openurl.py` & `plextraktsync-0.30.3/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/packaging.py` & `plextraktsync-0.30.3/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/util/remove_empty_values.py` & `plextraktsync-0.30.3/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/EventDispatcher.py` & `plextraktsync-0.30.3/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/EventFactory.py` & `plextraktsync-0.30.3/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/ProgressBar.py` & `plextraktsync-0.30.3/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/WatchStateUpdater.py` & `plextraktsync-0.30.3/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/WebSocketListener.py` & `plextraktsync-0.30.3/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/plextraktsync/watch/events.py` & `plextraktsync-0.30.3/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/requirements.txt` & `plextraktsync-0.30.3/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 attrs==23.2.0; python_version >= '3.7'
 cattrs==23.2.3; python_version >= '3.7' and python_version >= '3.8'
 certifi==2024.2.2; python_version >= '3.6'
 charset-normalizer==3.3.2; python_full_version >= '3.7.0'
 click==8.1.7; python_version >= '3.7'
 decorator==5.1.1; python_version >= '3.5'
 deprecated==1.2.14; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-exceptiongroup==1.2.1; python_version >= '3.7'
+exceptiongroup==1.2.1; python_version < '3.11'
 humanize==4.9.0; python_version >= '3.8'
 idna==3.7; python_version >= '3.5'
 inquirerpy==0.3.4; python_version >= '3.7' and python_version < '4.0'
 markdown-it-py==3.0.0; python_version >= '3.7' and python_version >= '3.8'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2; python_version >= '3.6'
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==4.2.1; python_version >= '3.8'
+platformdirs==4.2.1; python_version >= '3.7' and python_version >= '3.8'
 plexapi==4.15.12; python_version >= '3.8'
 pluggy==1.5.0; python_version >= '3.8'
 prompt-toolkit==3.0.43; python_full_version >= '3.7.0'
 pygments==2.17.2; python_version >= '3.7'
 python-dotenv==1.0.1; python_version >= '3.8'
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.32
 pyyaml==6.0.1; python_version >= '3.6'
 requests==2.31.0; python_version >= '3.7'
 requests-cache==1.2.0; python_version >= '3.8'
 requests-oauthlib==2.0.0; python_version >= '3.4'
 rich==13.7.1; python_full_version >= '3.7.0'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3' and python_version >= '3.4'
-tqdm==4.66.2; python_version >= '3.7'
+tqdm==4.66.4; python_version >= '3.7'
 types-decorator==5.1.8.20240310; python_version >= '3.8'
 typing-extensions==4.11.0; python_version < '3.9'
 url-normalize==1.4.3; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5' and python_version >= '3.6'
 urllib3==2.2.1; python_version >= '3.8'
 wcwidth==0.2.13
 websocket-client==1.8.0; python_version >= '3.8'
 wrapt==1.16.0; python_version >= '3.5' and python_version >= '3.6'
```

### Comparing `plextraktsync-0.30.2/setup.cfg` & `plextraktsync-0.30.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_collection_metadata.py` & `plextraktsync-0.30.3/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_config.py` & `plextraktsync-0.30.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_events.py` & `plextraktsync-0.30.3/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_new_agent.py` & `plextraktsync-0.30.3/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_plex_id.py` & `plextraktsync-0.30.3/tests/test_plex_id.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_rating.py` & `plextraktsync-0.30.3/tests/test_rating.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_timer.py` & `plextraktsync-0.30.3/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_trakt_progress.py` & `plextraktsync-0.30.3/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_tv_lookup.py` & `plextraktsync-0.30.3/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `plextraktsync-0.30.2/tests/test_walker.py` & `plextraktsync-0.30.3/tests/test_walker.py`

 * *Files identical despite different names*

