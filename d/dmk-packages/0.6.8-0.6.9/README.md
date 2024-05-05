# Comparing `tmp/dmk_packages-0.6.8.tar.gz` & `tmp/dmk_packages-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.6.8.tar", last modified: Thu May  2 02:41:18 2024, max compression
+gzip compressed data, was "dmk_packages-0.6.9.tar", last modified: Sun May  5 04:27:50 2024, max compression
```

## Comparing `dmk_packages-0.6.8.tar` & `dmk_packages-0.6.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.109289 dmk_packages-0.6.8/
--rw-r--r--   0 tommie     (501) staff       (20)    11347 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/LICENSE
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-05-02 02:41:18.109029 dmk_packages-0.6.8/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)     1365 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/README.md
--rw-r--r--   0 tommie     (501) staff       (20)      584 2024-05-02 02:36:23.000000 dmk_packages-0.6.8/pyproject.toml
--rw-r--r--   0 tommie     (501) staff       (20)       38 2024-05-02 02:41:18.109345 dmk_packages-0.6.8/setup.cfg
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.103052 dmk_packages-0.6.8/src/
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.104195 dmk_packages-0.6.8/src/dmk_packages/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/__init__.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.107914 dmk_packages-0.6.8/src/dmk_packages/crawler/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3534 2024-04-30 04:52:14.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/bigkinds.py
--rw-r--r--   0 tommie     (501) staff       (20)     6580 2024-04-30 04:52:14.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/clien.py
--rw-r--r--   0 tommie     (501) staff       (20)     6685 2024-05-02 02:39:36.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/fnguide.py
--rw-r--r--   0 tommie     (501) staff       (20)     2321 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 tommie     (501) staff       (20)    15349 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/naver_search_volume.py
--rw-r--r--   0 tommie     (501) staff       (20)     1382 2024-04-24 08:52:39.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/pdf_to_text.py
--rw-r--r--   0 tommie     (501) staff       (20)    13362 2024-04-23 05:01:14.000000 dmk_packages-0.6.8/src/dmk_packages/crawler/youtube.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.108446 dmk_packages-0.6.8/src/dmk_packages/database/
--rw-r--r--   0 tommie     (501) staff       (20)        0 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/database/__init__.py
--rw-r--r--   0 tommie     (501) staff       (20)     3057 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/database/database.py
--rw-r--r--   0 tommie     (501) staff       (20)     1895 2024-04-04 04:45:57.000000 dmk_packages-0.6.8/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 tommie     (501) staff       (20)        0 2024-05-02 02:41:18.108711 dmk_packages-0.6.8/src/dmk_packages.egg-info/
--rw-r--r--   0 tommie     (501) staff       (20)     1854 2024-05-02 02:41:18.000000 dmk_packages-0.6.8/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 tommie     (501) staff       (20)      677 2024-05-02 02:41:18.000000 dmk_packages-0.6.8/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 tommie     (501) staff       (20)        1 2024-05-02 02:41:18.000000 dmk_packages-0.6.8/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 tommie     (501) staff       (20)       41 2024-05-02 02:41:18.000000 dmk_packages-0.6.8/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 tommie     (501) staff       (20)       13 2024-05-02 02:41:18.000000 dmk_packages-0.6.8/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.791354 dmk_packages-0.6.9/
+-rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/LICENSE
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-05 04:27:50.790473 dmk_packages-0.6.9/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/README.md
+-rw-r--r--   0 layla      (501) staff       (20)      584 2024-05-05 04:26:40.000000 dmk_packages-0.6.9/pyproject.toml
+-rw-r--r--   0 layla      (501) staff       (20)       38 2024-05-05 04:27:50.791592 dmk_packages-0.6.9/setup.cfg
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.771828 dmk_packages-0.6.9/src/
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.774927 dmk_packages-0.6.9/src/dmk_packages/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/__init__.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.785877 dmk_packages-0.6.9/src/dmk_packages/crawler/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3534 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/bigkinds.py
+-rw-r--r--   0 layla      (501) staff       (20)     6580 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/clien.py
+-rw-r--r--   0 layla      (501) staff       (20)     6685 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/fnguide.py
+-rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-15 02:00:30.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 layla      (501) staff       (20)     1382 2024-05-04 15:01:16.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/pdf_to_text.py
+-rw-r--r--   0 layla      (501) staff       (20)    14699 2024-05-05 04:01:44.000000 dmk_packages-0.6.9/src/dmk_packages/crawler/youtube.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.788163 dmk_packages-0.6.9/src/dmk_packages/database/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-15 03:09:28.000000 dmk_packages-0.6.9/src/dmk_packages/database/database.py
+-rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.6.9/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-05-05 04:27:50.789484 dmk_packages-0.6.9/src/dmk_packages.egg-info/
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)      677 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 layla      (501) staff       (20)        1 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 layla      (501) staff       (20)       41 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 layla      (501) staff       (20)       13 2024-05-05 04:27:50.000000 dmk_packages-0.6.9/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.6.8/LICENSE` & `dmk_packages-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/PKG-INFO` & `dmk_packages-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.8
+Version: 0.6.9
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.8/README.md` & `dmk_packages-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/pyproject.toml` & `dmk_packages-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.6.8"
+version = "0.6.9"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/bigkinds.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/bigkinds.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/clien.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/clien.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/fnguide.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/fnguide.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/pdf_to_text.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/crawler/youtube.py` & `dmk_packages-0.6.9/src/dmk_packages/crawler/youtube.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 import time
 from typing import List
 
 import pendulum
 from loguru import logger
 from sqlalchemy.sql import func
-from sqlalchemy import text, Column, Integer, String, Date, DateTime, UniqueConstraint
+from sqlalchemy import text, Column, Integer, String, Date, TIMESTAMP, UniqueConstraint
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
 from dmk_packages.database import database as db
 
 
-class YoutubeDBHandler:
+class YoutubeTokenHandler:
     # ==============================================================================
     # NOTE : 한투(postgres)로 데이터베이스 설정
-    def __init__(self, target="KOREAINVESTMENT_DMK", meta_table_name="t_metadata_youtube"):
+    def __init__(self, target, meta_table_name):
         self._db_engine = db.get_engine(target)
         self._meta_table = meta_table_name
-        db.create_to_postgres(
-            self._db_engine,
-            self._meta_table,
-            Column("id", Integer, primary_key=True, autoincrement=True),
-            Column("keyword", String),
-            Column("next_page_token", String),
-            Column("target_date", Date),
-            Column("created_at", DateTime, nullable=False, server_default=func.now()),
-            UniqueConstraint("id", name="t_metadata_youtube_pk")
-        )
         if not self._db_engine:
             raise ValueError("데이터베이스 엔진 설정에 실패했습니다.")
+
+        self._create_meta_table(self._db_engine, self._meta_table)
+    # ==============================================================================
+
+    # ==============================================================================
+    # NOTE : 메타테이블 생성 함수
+    @staticmethod
+    def _create_meta_table(engine, meta_table_name):
+        try:
+            db.create_to_postgres(
+                engine,
+                meta_table_name,
+                Column("id", Integer, primary_key=True, autoincrement=True),
+                Column("keyword", String),
+                Column("next_page_token", String),
+                Column("target_date", Date),
+                Column("created_at", TIMESTAMP(timezone=False), server_default=func.timezone('KST', func.current_timestamp()), nullable=False),
+                UniqueConstraint("id", name="t_metadata_youtube_pk_test")
+            )
+        except Exception as err:
+            logger.error(err)
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : json 응답에 있는 "next_page_token" 키에 해당하는 값을 metadata 테이블에 저장
     def _save_page_token(self, keyword, target_date, next_page_token):
         query = f"""
         INSERT INTO {self._meta_table} (keyword, next_page_token, target_date)
@@ -85,15 +96,15 @@
             logger.error(err)
     # ==============================================================================
 
 
 class YoutubeKeyHandler:
     # ==============================================================================
     # NOTE : 마대리(postgres)로 데이터베이스 설정
-    def __init__(self, target="MADERI_AUTH"):
+    def __init__(self, target):
         self._maderi_engine = db.get_engine(target)
         self._api_key_table = 't_auth_yt_api_key_v2'
         if not self._maderi_engine:
             raise ValueError("데이터베이스 엔진 설정에 실패했습니다.")
 
         self.__reset_youtube_apikey()
         self._youtube_api_key = self._get_youtube_apikey()
@@ -173,27 +184,38 @@
         if err.resp.status == 400:
             self._update_youtube_apikey_state(self._api_key["key_id"], "valid")
         elif err.resp.status == 403:
             self._update_youtube_apikey_state(self._api_key["key_id"], "active")
     # ==============================================================================
 
 
-class YoutubeCrawler(YoutubeKeyHandler, YoutubeDBHandler):
+class YoutubeCrawler(YoutubeKeyHandler, YoutubeTokenHandler):
     tz = pendulum.timezone("Asia/Seoul")
     DEFAULT_DT = pendulum.yesterday(tz=tz)
 
-    def __init__(self):
-        super(YoutubeKeyHandler, self).__init__()
-        super(YoutubeDBHandler, self).__init__()
-        super(YoutubeCrawler, self).__init__()
+    def __init__(self, key_auth, token_auth, meta_name):
+        YoutubeKeyHandler.__init__(self, target=key_auth)
+        YoutubeTokenHandler.__init__(self, target=token_auth, meta_table_name=meta_name)
 
         self._keywords: List[str] | None = None
         self._api_key = self._get_youtube_apikey()
         self._results = []
 
+    @staticmethod
+    def _kst_to_utc(kst_string):
+        kst_datetime = pendulum.parse(kst_string, tz="Asia/Seoul")
+        utc_datetime = kst_datetime.in_timezone("UTC")
+        return utc_datetime.isoformat()
+
+    @staticmethod
+    def _utc_to_kst(utc_string):
+        utc_datetime = pendulum.parse(utc_string, tz="UTC")
+        kst_datetime = utc_datetime.in_timezone("Asia/Seoul")
+        return kst_datetime.isoformat()
+
     def get_keywords(self) -> List[str]:
         """해당 메서드를 오버라이딩하여 키워드를 세팅합니다."""
 
         # NOTE: 예시를 위한 키워드입니다.
         return ["Python", "Rust", "JavaScript", "Java", "Flutter"]
 
     # ==============================================================================
@@ -215,15 +237,15 @@
             video_id = video_info.get("id", {}).get("videoId")
             video_snippet = video.get("snippet", {})
             video_statistics = video.get("statistics", {})
             result = {
                 "title": video_snippet.get("title", ""),
                 "creator": video_snippet.get("channelTitle", ""),
                 "contents": video_snippet.get("description", "").replace("\n\n", "").replace("\n", " "),
-                "regist_date": pendulum.parse(video_snippet.get("publishedAt")),
+                "regist_date": self._utc_to_kst(video_snippet.get("publishedAt")),
                 "view": int(video_statistics.get("viewCount", 0)),
                 "recommend": int(video_statistics.get("likeCount", 0)),
                 "comment": int(video_statistics.get("commentCount", 0)),
                 "url": f"https://www.youtube.com/watch?v={video_id}",
                 "keyword": keyword
             }
             return result
@@ -240,35 +262,40 @@
     # ==============================================================================
 
     # ==============================================================================
     # NOTE : 주어진 날짜, 키워드에 대한 전체 결과를 _results 리스트에 추가 후 반환
     def _stack_videos_info(self, keyword, target_date, page_token=None):
         try:
             next_page_token = page_token
+            published_after = self._kst_to_utc(f"{target_date} 00:00:00").replace("+00:00", "Z")
+            published_before = self._kst_to_utc(f"{target_date} 23:59:59").replace("+00:00", "Z")
             youtube = build(
                 serviceName="youtube",
                 version="v3",
                 developerKey=self._api_key["api_key"]
             )
             response = youtube.search().list(
                 q=keyword,
                 type="video",
                 part="id,snippet",
                 maxResults=50,  # NOTE: 최대 50개
                 pageToken=next_page_token,
-                publishedAfter=target_date + "T00:00:00Z",
-                publishedBefore=target_date + "T23:59:59Z",
+                publishedAfter=published_after,
+                publishedBefore=published_before,
                 order="date",
                 regionCode="KR",
             ).execute()
             time.sleep(0.1)
 
             videos = response.get("items", [])
             next_page_token = response.get("nextPageToken")
-            results = [self._get_video_info(keyword, video) for video in videos]
+
+            # 일부 지정한 시간대 범위에서 벗어난 업로드 시간의 영상이 있음 -> 해당 영상은 걸러내기
+            results = [self._get_video_info(keyword, video) for video in videos
+                       if published_after <= video["snippet"]["publishedAt"] <= published_before]
             self._results.extend(results)
             logger.info(f"[{keyword}][{target_date}]: {len(results)} 개 추가 수집")
 
             if not page_token:
                 self._save_page_token(keyword, target_date, next_page_token)
             else:
                 self._update_page_token(keyword, target_date, next_page_token)
```

### Comparing `dmk_packages-0.6.8/src/dmk_packages/database/database.py` & `dmk_packages-0.6.9/src/dmk_packages/database/database.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.6.9/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.6.8/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.6.9/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.6.8
+Version: 0.6.9
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.6.8/src/dmk_packages.egg-info/SOURCES.txt` & `dmk_packages-0.6.9/src/dmk_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

