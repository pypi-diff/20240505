# Comparing `tmp/innertube-de-1.0.0.post3.tar.gz` & `tmp/innertube-de-1.0.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube-de-1.0.0.post3.tar", last modified: Thu May  2 13:15:44 2024, max compression
+gzip compressed data, was "innertube-de-1.0.0.post4.tar", last modified: Sun May  5 10:17:18 2024, max compression
```

## Comparing `innertube-de-1.0.0.post3.tar` & `innertube-de-1.0.0.post4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:15:44.658417 innertube-de-1.0.0.post3/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 13:15:44.658417 innertube-de-1.0.0.post3/PKG-INFO
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-02 13:15:33.000000 innertube-de-1.0.0.post3/README.md
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:15:44.655083 innertube-de-1.0.0.post3/innertube_de/
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1703 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/__init__.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     5262 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/containers.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8158 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/endpoints.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/errors.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    60173 2024-05-02 13:14:41.000000 innertube-de-1.0.0.post3/innertube_de/extractor.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/itags.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    26289 2024-05-02 11:22:37.000000 innertube-de-1.0.0.post3/innertube_de/items.py
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post3/innertube_de/stream.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4796 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post3/innertube_de/types.py
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8543 2024-05-02 10:48:08.000000 innertube-de-1.0.0.post3/innertube_de/utils.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:15:44.658417 innertube-de-1.0.0.post3/innertube_de.egg-info/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-02 13:15:44.000000 innertube-de-1.0.0.post3/innertube_de.egg-info/PKG-INFO
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-02 13:15:44.000000 innertube-de-1.0.0.post3/innertube_de.egg-info/SOURCES.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-02 13:15:44.000000 innertube-de-1.0.0.post3/innertube_de.egg-info/dependency_links.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-02 13:15:44.000000 innertube-de-1.0.0.post3/innertube_de.egg-info/top_level.txt
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-02 13:15:44.658417 innertube-de-1.0.0.post3/setup.cfg
--rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-02 13:15:38.000000 innertube-de-1.0.0.post3/setup.py
-drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-02 13:15:44.658417 innertube-de-1.0.0.post3/tests/
--rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13806 2024-05-02 11:22:31.000000 innertube-de-1.0.0.post3/tests/tester.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/PKG-INFO
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2708 2024-05-05 10:17:12.000000 innertube-de-1.0.0.post4/README.md
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/innertube_de/
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     1651 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/__init__.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2435 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/containers.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     2970 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/endpoints.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     1098 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/errors.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    60408 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/extractor.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     4223 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/itags.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)    10562 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/items.py
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3970 2024-04-29 11:36:23.000000 innertube-de-1.0.0.post4/innertube_de/stream.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     4796 2024-05-02 13:02:55.000000 innertube-de-1.0.0.post4/innertube_de/types.py
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)     8634 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/innertube_de/utils.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/innertube_de.egg-info/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)     3078 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/PKG-INFO
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)      416 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/SOURCES.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)        1 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/dependency_links.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       13 2024-05-05 10:17:17.000000 innertube-de-1.0.0.post4/innertube_de.egg-info/top_level.txt
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)       38 2024-05-05 10:17:18.002547 innertube-de-1.0.0.post4/setup.cfg
+-rwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)      785 2024-05-05 10:17:07.000000 innertube-de-1.0.0.post4/setup.py
+drwxr-xr-x   0 g3nsy     (1000) g3nsy     (1000)        0 2024-05-05 10:17:17.999213 innertube-de-1.0.0.post4/tests/
+-rw-r--r--   0 g3nsy     (1000) g3nsy     (1000)    13856 2024-05-05 10:16:24.000000 innertube-de-1.0.0.post4/tests/tester.py
```

### Comparing `innertube-de-1.0.0.post3/PKG-INFO` & `innertube-de-1.0.0.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post3
+Version: 1.0.0.post4
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-3-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post3/README.md` & `innertube-de-1.0.0.post4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-3-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post3/innertube_de/__init__.py` & `innertube-de-1.0.0.post4/innertube_de/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     VideoItem,
     AlbumItem,
     SongItem,
     SingleItem,
     PodcastItem,
     ProfileItem,
     EPItem,
-    ItemWithSubscribers,
     YouTubeVideoItem,
     YouTubeMusicVideoItem,
     YouTubePlaylistItem,
     YouTubeMusicPlaylistItem
 )
 
 from innertube_de.types import (
@@ -84,15 +83,14 @@
     "VideoItem",
     "AlbumItem",
     "SongItem",
     "PodcastItem",
     "ProfileItem",
     "EPItem",
     "SingleItem",
-    "ItemWithSubscribers",
     "YouTubeVideoItem",
     "YouTubeMusicVideoItem",
     "YouTubePlaylistItem",
     "YouTubeMusicPlaylistItem",
 
     "ItemType",
     "EndpointType",
```

### Comparing `innertube-de-1.0.0.post3/innertube_de/errors.py` & `innertube-de-1.0.0.post4/innertube_de/errors.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post3/innertube_de/extractor.py` & `innertube-de-1.0.0.post4/innertube_de/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ItemType,
     TextDivisorType
 )
 
 from innertube_de.utils import (
     get_item_type,
     to_int,
-    check_input,
+    return_on_input_none,
     get,
     clc_length,
     clc_publication_date,
     clc_int,
     clc_views
 )
 
@@ -573,76 +573,76 @@
         """
         # YouTube Music
         if ShelfStructType.MUSIC_CARD_SHELF.value in entry_item:
             ds = self._get(entry_item, ShelfStructType.MUSIC_CARD_SHELF.value)
             item_type = get_item_type(self._get(ds, "subtitle", "runs", 0, "text"))
             name = self._get(ds, "title", "runs", 0, "text")
             endpoint = self._extract_endpoint(self._get(ds, "title", "runs", 0, "navigationEndpoint"))
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
 
             match item_type:
                 case ItemType.ALBUM:
-                    item = AlbumItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = AlbumItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.ARTIST:
                     subscribers = self._clc_int(self._get(ds, "subtitle", "runs", -1, "text"))
                     item = ArtistItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, subscribers=subscribers
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, subscribers=subscribers
                     )
 
                 case ItemType.YOUTUBE_MUSIC_VIDEO:
                     views = self._clc_int(self._get(ds, "subtitle", "runs", -3, "text"))
                     length = self._clc_length(self._get(ds, "subtitle", "runs", -1, "text"))
                     item = YouTubeMusicVideoItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, views=views, length=length
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, views=views, length=length
                     )
 
                 case ItemType.EP:
-                    item = EPItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = EPItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.SONG:
                     length = self._clc_length(self._get(ds, "subtitle", "runs", -1, "text"))
                     album_name = self._get(ds, "subtitle", "runs", -3, "text")
                     album_endpoint = self._extract_endpoint(
                         self._get(ds, "subtitle", "runs", -3, "navigationEndpoint")
                     )
 
                     album_item = AlbumItem(
-                        name=album_name, thumbnail_url=thumbnail_url, endpoint=album_endpoint
+                        name=album_name, thumbnail_urls=thumbnail_urls, endpoint=album_endpoint
                     )
 
                     item = SongItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, 
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, 
                         length=length, album_item=album_item
                     )
 
                 case ItemType.EPISODE:
                     publication_date = self._clc_publication_date(self._get(ds, "subtitle", "runs", 2))
                     item = EpisodeItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, 
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, 
                         publication_date=publication_date
                     )
 
                 case _:
-                    item = Item(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = Item(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
         # YouTube Music
         elif ItemStructType.MUSIC_RESPONSIVE_LIST_ITEM.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_RESPONSIVE_LIST_ITEM.value)
             endpoint = self._extract_endpoint(self._get(ds, "navigationEndpoint", opt=True))
             if endpoint is None:
                 endpoint = self._extract_endpoint(
                     self._get(
                         ds, "flexColumns", 0, "musicResponsiveListItemFlexColumnRenderer",
                         "text", "runs", -1, "navigationEndpoint"
                     )
                 )
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "musicThumbnailRenderer", "thumbnail", "thumbnails", opt=True)
             )
             name = self._get(
                 ds, "flexColumns", 0, "musicResponsiveListItemFlexColumnRenderer", "text", "runs", 0, "text"
             )
             if item_type is None:
                 item_type = get_item_type(
@@ -660,26 +660,26 @@
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                             "text", "runs", -1, "text", opt=True
                         ), 
                         opt=True
                     )
                     item = ArtistItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, subscribers=subscribers
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, subscribers=subscribers
                     )
 
                 case ItemType.ALBUM:
                     release_year = to_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                             "text", "runs", -1, "text"
                         )
                     )
                     item = AlbumItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url,
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls,
                         release_year=release_year, artist_items=None
                     )
 
                 case ItemType.YOUTUBE_MUSIC_VIDEO:
                     length = self._clc_length(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
@@ -690,15 +690,15 @@
                     views = self._clc_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                             "text", "runs", -3, "text", opt=True
                         )
                     )
                     item = YouTubeMusicVideoItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, length=length, views=views
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, length=length, views=views
                     )
 
                 case ItemType.YOUTUBE_MUSIC_PLAYLIST:
                     tracks_num = to_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text", opt=True
@@ -710,27 +710,27 @@
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text", opt=True
                         ),
                         opt=True
                     )
 
                     item = YouTubeMusicPlaylistItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, 
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, 
                         tracks_num=tracks_num, views=views
                     )
 
                 case ItemType.SINGLE:
                     release_year = to_int(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", "text",
                             "runs", -1, "text", opt=True
                         )
                     )
                     item = SingleItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, release_year=release_year
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, release_year=release_year
                     )
 
                 case ItemType.SONG:
                     length = self._clc_length(
                         self._get(
                             ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer", 
                             "text", "runs", -1, "text", opt=True
@@ -761,42 +761,42 @@
                             opt=True
                         )
                         reproductions = attempt2
                     else:
                         reproductions = attempt1
 
                     item = SongItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url,
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls,
                         length=length, reproductions=reproductions, album_item=None
                     )
 
                 case ItemType.EPISODE:
-                    item = EpisodeItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = EpisodeItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.PODCAST:
-                    item = PodcastItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = PodcastItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.PROFILE:
                     item_handle = self._get(
                         ds, "flexColumns", 1, "musicResponsiveListItemFlexColumnRenderer",
                         "text", "runs", -1, "text"
                     )
-                    item = ProfileItem(name=name, thumbnail_url=thumbnail_url, handle=item_handle)
+                    item = ProfileItem(name=name, thumbnail_urls=thumbnail_urls, handle=item_handle)
 
                 case ItemType.EP:
-                    item = EPItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = EPItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case _:
                     return None
 
 
         # YouTube Music
         elif ItemStructType.MUSIC_TWO_ROW_ITEM.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_TWO_ROW_ITEM.value)
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnailRenderer", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
             name = self._get(ds, "title", "runs", 0, "text")
             endpoint = self._extract_endpoint(self._get(ds, "navigationEndpoint"))
             if item_type is None:
                 try:
                     item_type = ItemType(
@@ -808,102 +808,102 @@
                 except ValueError:
                     item_type = None
 
             match item_type:
                 case ItemType.ARTIST:
                     subscribers = self._clc_int(self._get(ds, "subtitle", "runs", 0, "text"))
                     item = ArtistItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, subscribers=subscribers
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, subscribers=subscribers
                     )
 
                 case ItemType.ALBUM:
                     release_year = to_int(self._get(ds, "subtitle", "runs", -1, "text", opt=True))
                     item = AlbumItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, release_year=release_year
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, release_year=release_year
                     )
 
                 case ItemType.EP:
                     release_year = to_int(self._get(ds, "subtitle", "runs", -1, "text", opt=True))
                     item = EPItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, release_year=release_year
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, release_year=release_year
                     )
 
                 case ItemType.YOUTUBE_MUSIC_VIDEO:
                     views = self._clc_int(self._get(ds, "subtitle", "runs", -1, "text"))
                     item = YouTubeMusicVideoItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, views=views
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, views=views
                     )
 
                 case ItemType.YOUTUBE_MUSIC_PLAYLIST:
-                    item = YouTubeMusicPlaylistItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = YouTubeMusicPlaylistItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.SINGLE:
                     release_year = to_int(self._get(ds, "subtitle", "runs", -1, "text", opt=True))
                     item = SingleItem(
-                        name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, release_year=release_year
+                        name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, release_year=release_year
                     )
 
                 case ItemType.SONG:
-                    item = SongItem(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = SongItem(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
                 case ItemType.EPISODE | ItemType.PODCAST | ItemType.PROFILE:
                     return None
 
                 case _:
-                    item = Item(name=name, endpoint=endpoint, thumbnail_url=thumbnail_url)
+                    item = Item(name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls)
 
         # YouTube Music
         elif ItemStructType.PLAYLIST_PANEL_VIDEO.value in entry_item:
             ds = self._get(entry_item, ItemStructType.PLAYLIST_PANEL_VIDEO.value)
             name = self._get(ds, "title", "runs", -1, "text")
             endpoint = self._extract_endpoint(self._get(ds, "navigationEndpoint"))
             length = self._clc_length(self._get(ds, "lengthText", "runs", -1, "text"))
-            thumbnail_url = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
+            thumbnail_urls = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
             tmp = self._get(ds, "thumbnail", "thumbnails", -1)
             width = self._get(tmp, "width")
             height = self._get(tmp, "height")
             if width / height == 1:
                 item = SongItem(
-                    name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, length=length, album_item=None
+                    name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, length=length, album_item=None
                 )
             else:
                 views = self._clc_int(self._get(ds, "longBylineText", "runs", -3, "text", opt=True), opt=True)
                 item = YouTubeMusicVideoItem(
-                    name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, length=length, views=views
+                    name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, length=length, views=views
                 )
 
         # YouTube Music
         elif ItemStructType.MUSIC_IMMERSIVE_HEADER.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_IMMERSIVE_HEADER.value)
             description = self._extract_description(self._get(ds, "description", "runs", opt=True))
             name = self._get(ds, "title", "runs", 0, "text")
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
             subscribers = self._clc_int(
                 self._get(
                     ds, "subscriptionButton", "subscribeButtonRenderer", 
                     "subscriberCountText", "runs", 0, "text"
                 )
             )
             item = ArtistItem(
-                name=name, subscribers=subscribers, description=description, thumbnail_url=thumbnail_url
+                name=name, subscribers=subscribers, description=description, thumbnail_urls=thumbnail_urls
             )
 
         # YouTube Music
         elif ItemStructType.MUSIC_DETAIL_HEADER.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_DETAIL_HEADER.value)
             try:
                 item_type = ItemType(self._get(ds, "subtitle", "runs", 0, "text"))
             except ValueError:
                 return None
 
             name = self._get(ds, "title", "runs", 0, "text")
 
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "croppedSquareThumbnailRenderer", "thumbnail", "thumbnails")
             )
 
             release_year = to_int(self._get(ds, "subtitle", "runs", -1, "text", opt=True))
 
             if item_type is ItemType.YOUTUBE_MUSIC_PLAYLIST:
                 tracks_num = clc_int(self._get(ds, "secondSubtitle", "runs", 2, "text"))
@@ -913,58 +913,58 @@
             description = self._extract_description(self._get(ds, "description", "runs", opt=True))
 
             # TODO extract length: X minutes, N hour (?), K seconds (?)
 
             match item_type:
                 case ItemType.ALBUM:
                     item = AlbumItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num,
+                        name=name, endpoint=None, thumbnail_urls=thumbnail_urls, tracks_num=tracks_num,
                         release_year=release_year, description=description
                     )
 
                 case ItemType.EP:
                     item = EPItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num, 
+                        name=name, endpoint=None, thumbnail_urls=thumbnail_urls, tracks_num=tracks_num, 
                         release_year=release_year, description=description
                     )
 
                 case ItemType.SINGLE:
                     item = SingleItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num, 
+                        name=name, endpoint=None, thumbnail_urls=thumbnail_urls, tracks_num=tracks_num, 
                         release_year=release_year, description=description
                     )
 
                 case ItemType.YOUTUBE_MUSIC_PLAYLIST:
                     views = self._clc_int(self._get(ds, "secondSubtitle", "runs", 0, "text"))
                     item = YouTubeMusicPlaylistItem(
-                        name=name, endpoint=None, thumbnail_url=thumbnail_url, tracks_num=tracks_num,
+                        name=name, endpoint=None, thumbnail_urls=thumbnail_urls, tracks_num=tracks_num,
                         release_year=release_year, description=description, views=views
                     )
 
                 case _:
                     return None
 
         # YouTube Music
         elif ItemStructType.MUSIC_VISUAL_HEADER.value in entry_item:
             ds = self._get(entry_item, ItemStructType.MUSIC_VISUAL_HEADER.value)
             name = self._get(ds, "title", "runs", -1, "text")
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
-            item = Item(name=name, thumbnail_url=thumbnail_url)
+            item = Item(name=name, thumbnail_urls=thumbnail_urls)
 
         # YouTube Music
         elif ItemStructType.MUSIC_MULTI_ROW_LIST_ITEM.value in entry_item:
             ds = self._get(entry_item)
             name = self._get(ds, "title", "runs", 0, "text")
-            thumbnail_url = self._extract_urls(
+            thumbnail_urls = self._extract_urls(
                 self._get(ds, "thumbnail", "musicThumbnailRenderer", "thumbnail", "thumbnails")
             )
             endpoint = self._extract_endpoint(self._get(ds, "title", "runs", 0, "navigationEndpoint"))
-            item = Item(name=name, thumbnail_url=thumbnail_url, endpoint=endpoint)
+            item = Item(name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint)
 
         # YouTube (custom)
         elif ItemStructType.NEXT_PRIMARY_VIDEO.value in entry_item:
             ds = self._get(entry_item, ItemStructType.NEXT_PRIMARY_VIDEO.value)
             video_data = self._get(ds, ItemType.YOUTUBE_VIDEO.value)
             item_name = self._get(video_data, "title", "runs", 0, "text")
             item_views = self._clc_views(
@@ -986,20 +986,20 @@
             )
 
             item_description = self._extract_description(
                 self._get(ds, ItemType.CHANNEL.value, "attributedDescription")
             )
 
             channel_data = self._get(ds, ItemType.CHANNEL.value, "owner", "videoOwnerRenderer")
-            channel_thumbnail_url = self._extract_urls(self._get(channel_data, "thumbnail", "thumbnails"))
+            channel_thumbnail_urls = self._extract_urls(self._get(channel_data, "thumbnail", "thumbnails"))
             channel_name = self._get(channel_data, "title", "runs", 0, "text")
             channel_endpoint = self._extract_endpoint(self._get(channel_data, "navigationEndpoint"))
             channel_subscribers = self._clc_int(self._get(channel_data, "subscriberCountText", "simpleText"))
             channel_item = ChannelItem(
-                name=channel_name, thumbnail_url=channel_thumbnail_url,
+                name=channel_name, thumbnail_urls=channel_thumbnail_urls,
                 endpoint=channel_endpoint, subscribers=channel_subscribers
             )
 
             item = YouTubeVideoItem(
                 name=item_name, views=item_views, endpoint=item_endpoint, 
                 channel_item=channel_item, description=item_description
             )
@@ -1026,17 +1026,17 @@
             or ItemStructType.GRID_CHANNEL.value in entry_item
             or ItemStructType.GRID_PLAYLIST.value in entry_item
         ):
             ds = self._get(entry_item, list(entry_item.keys())[0])
             name = self._get(ds, "title", "simpleText", opt=True)
             if name is None:
                 name = self._get(ds, "title", "runs", 0, "text")
-            thumbnail_url = self._extract_urls(self._get(ds, "thumbnail", "thumbnails", opt=True))
-            if thumbnail_url is None:
-                thumbnail_url = self._extract_urls(self._get(ds, "thumbnails", 0, "thumbnails"))
+            thumbnail_urls = self._extract_urls(self._get(ds, "thumbnail", "thumbnails", opt=True))
+            if thumbnail_urls is None:
+                thumbnail_urls = self._extract_urls(self._get(ds, "thumbnails", 0, "thumbnails"))
             endpoint = self._extract_endpoint(self._get(ds, "navigationEndpoint"))
 
             if (
                 ItemStructType.PLAYLIST_VIDEO.value in entry_item
                 or ItemStructType.COMPACT_PLAYLIST.value in entry_item
                 or ItemStructType.COMPACT_VIDEO.value in entry_item
                 or ItemStructType.GRID_VIDEO.value in entry_item
@@ -1065,87 +1065,87 @@
                 channel_data = self._get(ds, "shortBylineText", "runs", 0, opt=True)
                 if channel_data is None:
                     channel_data = self._get(ds, "longBylineText", "runs", 0, opt=True)
 
                 if channel_data is not None:
                     channel_name = self._get(channel_data, "text")
                     channel_endpoint = self._extract_endpoint(self._get(channel_data, "navigationEndpoint"))
-                    channel_thumbnail_url = self._extract_urls(
+                    channel_thumbnail_urls = self._extract_urls(
                         self._get(
                             ds, "channelThumbnailSupportedRenderers", "channelThumbnailWithLinkRenderer",
                             "thumbnail", "thumbnails", opt=True
                         )
                     )
                     channel_item = ChannelItem(
-                        name=channel_name, endpoint=channel_endpoint, thumbnail_url=channel_thumbnail_url
+                        name=channel_name, endpoint=channel_endpoint, thumbnail_urls=channel_thumbnail_urls
                     )
                 else:
                     channel_item = None
 
                 item = YouTubeVideoItem(
-                    name=name, thumbnail_url=thumbnail_url, endpoint=endpoint, views=views, length=length, 
+                    name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint, views=views, length=length, 
                     channel_item=channel_item, description=description, published_time=published_time
                 )
 
             elif (
                 ItemStructType.CHANNEL.value in entry_item 
                 or ItemStructType.GRID_CHANNEL.value in entry_item
             ):
                 subscribers = self._clc_int(
                     self._get(ds, "subscriberCountText", "simpleText", opt=True), opt=True
                 )
                 videos_num = self._clc_int(self._get(ds, "videoCountText", "runs", 0, "text", opt=True))
             
                 item = ChannelItem(
-                    name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, subscribers=subscribers, 
+                    name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, subscribers=subscribers, 
                     videos_num=videos_num 
                 )
 
             elif ItemStructType.GRID_PLAYLIST.value in entry_item:
                 videos_num = self._clc_int(self._get(ds, "videoCountText", "runs", 0, "text"))
 
                 channel_data = self._get(ds, "shortBylineText", "runs", 0, opt=True)
                 channel_name = self._get(channel_data, "text")
                 channel_endpoint = self._extract_endpoint(self._get(channel_data, "navigationEndpoint"))
                 channel_item = ChannelItem(name=channel_name, endpoint=channel_endpoint)
 
                 item = YouTubePlaylistItem(
-                    name=name, endpoint=endpoint, thumbnail_url=thumbnail_url, channel_item=channel_item, 
+                    name=name, endpoint=endpoint, thumbnail_urls=thumbnail_urls, channel_item=channel_item, 
                     videos_num=videos_num
                 )
 
             elif ItemStructType.COMPACT_RADIO.value in entry_item:
-                item = RadioItem(name=name, thumbnail_url=thumbnail_url, endpoint=endpoint)
+                item = RadioItem(name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint)
 
             elif ItemStructType.PLAYLIST.value in entry_item:
                 video_items = self._extract_child_videos(self._get(ds, "videos"))
                 videos_num = self._get(ds, "videoCount")
 
                 channel_data = self._get(ds, "shortBylineText", "runs", 0, opt=True)
                 channel_name = self._get(channel_data, "text")
                 channel_endpoint = self._extract_endpoint(self._get(channel_data, "navigationEndpoint"))
                 channel_item = ChannelItem(name=channel_name, endpoint=channel_endpoint)
 
                 item = YouTubePlaylistItem(
-                    name=name, thumbnail_url=thumbnail_url, endpoint=endpoint, video_items=video_items,
+                    name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint, video_items=video_items,
                     channel_item=channel_item, videos_num=videos_num
                 )
 
             else:  # ItemStructType.RADIO
                 video_items = self._extract_child_videos(self._get(ds, "videos"))
                 item = RadioItem(
-                    name=name, thumbnail_url=thumbnail_url, endpoint=endpoint, video_items=video_items
+                    name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint, video_items=video_items
                 )
 
         elif ItemStructType.REEL_ITEM.value in entry_item:
             ds = self._get(entry_item, ItemStructType.REEL_ITEM.value)
             name = self._get(ds, "headline", "simpleText")
-            thumbnail_url = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
+            thumbnail_urls = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
             endpoint = WatchEndpoint(video_id=self._get(ds, "videoId"))
-            item = YouTubeVideoItem(name=name, thumbnail_url=thumbnail_url, endpoint=endpoint)
+            item = YouTubeVideoItem(name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint)
 
         elif ItemStructType.WATCH_CARD_COMPACT_VIDEO.value in entry_item:
             ds = self._get(entry_item, ItemStructType.WATCH_CARD_COMPACT_VIDEO.value)
             name = self._get(ds, "title", "simpleText")
             length = self._clc_length(self._get(ds, "lengthText", "simpleText"))
             endpoint = self._extract_endpoint(self._get(ds, "navigationEndpoint"))
             views = self._clc_int(self._get(ds, "subtitle", "simpleText"))
@@ -1159,35 +1159,36 @@
                 name=name, endpoint=endpoint, length=length, views=views, 
                 channel_item=channel_item, published_time=published_time
             )
 
         elif ItemStructType.SEARCH_REFINEMENT_CARD.value in entry_item:
             ds = self._get(entry_item, ItemStructType.SEARCH_REFINEMENT_CARD.value)
             name = self._get(ds, "query", "runs", 0, "text")
-            thumbnail_url = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
+            thumbnail_urls = self._extract_urls(self._get(ds, "thumbnail", "thumbnails"))
             endpoint = WatchEndpoint(
                 playlist_id=self._get(ds, "searchEndpoint", "watchPlaylistEndpoint", "playlistId")
             )
-            item = AlbumItem(name=name, thumbnail_url=thumbnail_url, endpoint=endpoint)
+            item = AlbumItem(name=name, thumbnail_urls=thumbnail_urls, endpoint=endpoint)
 
         # Item structures ignored
         elif (
             ItemStructType.AUTOMIX_PREVIEW_VIDEO.value in entry_item
             or ItemStructType.RELATED_CHIP_CLOUD.value in entry_item
             or ItemStructType.AD_SLOT.value in entry_item
             or ItemStructType.CONTINUATION_ITEM.value in entry_item
+            or ItemStructType.MESSAGE.value in entry_item
         ):
             return None
 
         else:
             raise AccessError(data=entry_item)
 
         return item
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _extract_endpoint(self, data: Dict) -> Optional[Endpoint]:
         """
         Method for extracting an endpoint from the specified dictionary.
         @param data: A portion of the data provided by InnerTube containing
         the details of an endpoint object.
         @return: An Endpoint object otherwise None if no registered endpoint
@@ -1233,48 +1234,48 @@
             endpoint = ContinuationEndpoint(continuation=continuation)
 
         else:
             raise AccessError(data=data)
 
         return endpoint
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _clc_length(self, string: str) -> Optional[time]:
         """
         Wrapper to the innertube_de.utils.clc_length function that allows
         its decoration without modifying the original code.
         @param string: The string to pass to the innertube_de.utils.clc_length function
         @return: The result of the innertube_de.utils.clc_length function
         """
         return clc_length(string)
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _clc_publication_date(self, string: str) -> Optional[date]:
         """
         Wrapper to the innertube_de.utils.clc_publication_date function
         that allows its decoration without modifying the original code
         @param string: The string to pass to the innertube_de.utils.clc_publication_date function
         @return: The result of the innertube_de.utils.clc_publication_date function
         """
         return clc_publication_date(string)
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _clc_int(self, string: str) -> Optional[int]:
         """
         Wrapper to the innertube_de.utils.clc_int function that allows
         its decoration without modifying the original code
         @param string: The string to pass to the innertube_de.utils.clc_int method
         @return: The result of the innertube.utils.clc_int function
         """
         return clc_int(string)
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _clc_views(self, string: str) -> Optional[int]:
         return clc_views(string)
 
     @_handle_exception
     def _get(self, ds: Union[List, Dict], *keys) -> Optional[Any]:
         """
@@ -1287,15 +1288,15 @@
         @param ds: The dictionary to pass to the innertube.utils.get function
         @param keys: All remaining parameters used to access the specified dictionary
         by the innertube_de.utils.get function.
         @return: The result of the innertube_de.utils.get function
         """
         return get(ds, *keys)
 
-    @check_input
+    @return_on_input_none
     @_handle_exception
     def _extract_description(self, ds: Union[List[Dict], Dict]) -> List[Tuple[str, Optional[Endpoint]]]:
         if isinstance(ds, List):
             return [
                 (self._get(e, "text"), self._extract_endpoint(self._get(e, "navigationEndpoint", opt=True))) 
                 for e in ds
             ]
@@ -1314,15 +1315,15 @@
                     description.append((content[index: start], None))
                 description.append((content[start: end], endpoint))
                 index = end
             if index < len(content):
                 description.append((content[index:], None))
             return description
 
-    @check_input
+    @return_on_input_none
     def _extract_urls(self, urls_data: List[Dict]) -> List[Dict]:
         urls = urls_data if self.include_all_urls is True else [self._get(urls_data, -1)]
         for entry in urls:
             if not entry["url"].startswith("https:"):
                 entry["url"] = f"https:{entry['url']}"
         return urls
```

### Comparing `innertube-de-1.0.0.post3/innertube_de/itags.py` & `innertube-de-1.0.0.post4/innertube_de/itags.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post3/innertube_de/stream.py` & `innertube-de-1.0.0.post4/innertube_de/stream.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post3/innertube_de/types.py` & `innertube-de-1.0.0.post4/innertube_de/types.py`

 * *Files identical despite different names*

### Comparing `innertube-de-1.0.0.post3/innertube_de/utils.py` & `innertube-de-1.0.0.post4/innertube_de/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 import re
 
 from datetime import time, date
 
 from typing import (
     Optional,
     Callable,
@@ -43,24 +44,15 @@
 
 from innertube_de.types import (
     EndpointType,
     ItemType
 )
 
 
-def get_items(data: List) -> List[Item]:
-    items: List[Item] = []
-    for item_data in data:
-        item = get_item(item_data)
-        if item is not None:
-            items.append(item)
-    return items
-
-
-def check_input(func: Callable) -> Callable:
+def return_on_input_none(func: Callable) -> Callable:
     """
     Decorator that allows you to return None when the first argument
     of the function (other than self) is None.
     @param func: The function to decorate.
     @return: The decorated function.
     """
     def inner(*args, **kwargs) -> Optional[str]:
@@ -69,15 +61,25 @@
         elif len(args) > 1 and args[1] is None or len(args) == 1 and args[0] is None:
             return
         else:
             return func(*args, **kwargs)
     return inner
 
 
-@check_input
+@return_on_input_none
+def get_items(data: List) -> List[Item]:
+    items: List[Item] = []
+    for item_data in data:
+        item = get_item(item_data)
+        if item is not None:
+            items.append(item)
+    return items
+
+
+@return_on_input_none
 def get_item_type(string: str) -> Optional[ItemType]:
     """
     [YouTube Music only]
     Returns the object of the ItemType enumeration class
     corresponding to the specified string. For example,
     if the shelf is "Latest songs" the returned object is ItemType.SONG.
     @param string: The name of a shelf.
@@ -110,25 +112,25 @@
         return ItemType.EP
 
 
 def _match(seq: str, title: str) -> bool:
     return re.search(seq, title, re.IGNORECASE) is not None
 
 
-@check_input
+@return_on_input_none
 def get_publication_date(data: Dict) -> Optional[date]:
     return date(month=data["month"], day=data["day"], year=data["year"])
 
 
-@check_input
+@return_on_input_none
 def get_length(data: Dict) -> Optional[time]:
     return time(hour=data["hour"], minute=data["minute"], second=data["second"])
 
 
-@check_input
+@return_on_input_none
 def get_item(data: Dict) -> Item:
     match data["type"]:
         case ItemType.RADIO.value:
             item = RadioItem()
         case ItemType.ARTIST.value:
             item = ArtistItem()
         case ItemType.YOUTUBE_VIDEO.value:
@@ -162,15 +164,15 @@
                 f"Invalid key type: {data['type']}. Expected key type: "
                 f"{', '.join([str(x) for x in ItemType.__members__.values()])}"
             )
     item.load(data)
     return item
 
 
-@check_input
+@return_on_input_none
 def get_endpoint(data: Dict) -> Endpoint:
     match data["type"]:
         case EndpointType.URL.value:
             endpoint = UrlEndpoint()
         case EndpointType.BROWSE.value:
             endpoint = BrowseEndpoint()
         case EndpointType.YOUTUBE_BROWSE.value:
```

### Comparing `innertube-de-1.0.0.post3/innertube_de.egg-info/PKG-INFO` & `innertube-de-1.0.0.post4/innertube_de.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: innertube-de
-Version: 1.0.0.post3
+Version: 1.0.0.post4
 Summary: InnerTube Data Extractor
 Home-page: https://github.com/g3nsy/innertube-de
 Author: g3nsy
 Author-email: g3nsydev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # InnerTube Data Extractor (ITDE)
-![Version](https://img.shields.io/badge/version-1.0.0-3-blue)
+![Version](https://img.shields.io/badge/version-1.0.0-4-blue)
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://en.wikipedia.org/wiki/MIT_License)
 
 ITDE is a Python-based tool designed to extract valuable information, including multimedia content and associated metadata, from the data provided by InnerTube, Google's private API. 
 InnerTube serves as a comprehensive source of data, and ITDE empowers developers to seamlessly retrieve and organize essential details from this platform.
 
 ### Features
```

### Comparing `innertube-de-1.0.0.post3/setup.py` & `innertube-de-1.0.0.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 here = Path(__file__).parent
 long_description = (here / "README.md").read_text()
 
 
 setup(
     name="innertube-de",
-    version="1.0.0-3",
+    version="1.0.0-4",
     description="InnerTube Data Extractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="g3nsy",
     author_email="g3nsydev@gmail.com",
     python_requires=">=3.6.0",
     url="https://github.com/g3nsy/innertube-de",
```

### Comparing `innertube-de-1.0.0.post3/tests/tester.py` & `innertube-de-1.0.0.post4/tests/tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,16 @@
                     if j > 0:
                         table_line += " " * distance
                     table_line += get_table_line(tester, i)
             cs.print(table_line)
 
 
 def print_container(container: Container) -> None:
+    if container.contents is None:
+        return
     for shelf in container.contents:
         shelf_type = "CardShelf" if isinstance(shelf, CardShelf) else "Shelf"
         cs.print()
         cs.print(f"{shelf_type} Name: {shelf.name}")
         cs.print(f"{shelf_type} Endpoint: {shelf.endpoint}")
         if isinstance(shelf, CardShelf):
             cs.print(f"{shelf_type} Item: {shelf.item}")
```

