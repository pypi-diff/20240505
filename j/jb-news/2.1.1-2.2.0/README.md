# Comparing `tmp/jb_news-2.1.1-py3-none-any.whl.zip` & `tmp/jb_news-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2072 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2796 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      297 b- defN 24-Apr-13 22:47 jb_news-2.1.1.dist-info/RECORD
-4 files, 3186 bytes uncompressed, 1490 bytes compressed:  53.2%
+Zip file size: 2143 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2942 b- defN 24-May-05 17:53 jb_news-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 17:53 jb_news-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-05 17:53 jb_news-2.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      297 b- defN 24-May-05 17:53 jb_news-2.2.0.dist-info/RECORD
+4 files, 3332 bytes uncompressed, 1561 bytes compressed:  53.2%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: jb_news-2.1.1.dist-info/METADATA
+Filename: jb_news-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: jb_news-2.1.1.dist-info/WHEEL
+Filename: jb_news-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: jb_news-2.1.1.dist-info/top_level.txt
+Filename: jb_news-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: jb_news-2.1.1.dist-info/RECORD
+Filename: jb_news-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jb_news-2.1.1.dist-info/METADATA` & `jb_news-2.2.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jb-news
-Version: 2.1.1
+Version: 2.2.0
 Summary: A comprehensive wrapper for JBlanked's News API, leveraging OpenAI, Machine Learning, and MQL5's Calendar.
 Home-page: https://jblanked.com/news/api/docs/
 Author: JBlanked
 License: MIT
 Description-Content-Type: text/markdown
 
 # JB-News
@@ -82,7 +82,16 @@
         outcome = event.outcome 
         strength = event.strength 
         quality = event.quality 
         projection = event.projection 
 
         # print the calendar info
         print(f"Event Name: {name}\nEvent ID: {event_id}\nCurrency: {currency}\nDate: {date}\nActual: {actual}\nForecast: {forecast}\nPrevious: {previous}")
+```
+
+You can also access our NewsGPT model:
+
+```python
+gpt_response = jb.GPT(api_key,"What does bullish mean in forex?")
+
+print(gpt_response)
+```
```

