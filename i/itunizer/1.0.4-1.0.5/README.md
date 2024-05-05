# Comparing `tmp/itunizer-1.0.4.tar.gz` & `tmp/itunizer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itunizer-1.0.4.tar", last modified: Wed Nov  6 04:36:51 2019, max compression
+gzip compressed data, was "itunizer-1.0.5.tar", max compression
```

## Comparing `itunizer-1.0.4.tar` & `itunizer-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/
--rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:36:51.000000 itunizer-1.0.4/PKG-INFO
--rw-r--r--   0 jamescampbell   (501) staff       (20)     1558 2019-06-16 23:55:39.000000 itunizer-1.0.4/README.md
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer/
--rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-01-13 17:29:13.000000 itunizer-1.0.4/itunizer/__init__.py
--rw-r--r--   0 jamescampbell   (501) staff       (20)       35 2019-11-06 04:36:33.000000 itunizer-1.0.4/itunizer/__main__.py
--rw-r--r--   0 jamescampbell   (501) staff       (20)     6674 2019-11-06 04:36:33.000000 itunizer-1.0.4/itunizer/itunizer.py
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/
--rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/PKG-INFO
--rw-r--r--   0 jamescampbell   (501) staff       (20)      285 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/SOURCES.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/dependency_links.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       53 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/entry_points.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       32 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/requires.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)        9 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/top_level.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       79 2019-11-06 04:36:51.000000 itunizer-1.0.4/setup.cfg
--rw-r--r--   0 jamescampbell   (501) staff       (20)      914 2019-11-06 04:36:33.000000 itunizer-1.0.4/setup.py
+-rw-r--r--   0        0        0    35147 2024-05-05 16:55:39.804868 itunizer-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1558 2024-05-05 16:55:39.805276 itunizer-1.0.5/README.md
+-rw-r--r--   0        0        0        1 2024-05-05 16:55:39.805480 itunizer-1.0.5/itunizer/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-05 16:55:39.805570 itunizer-1.0.5/itunizer/__main__.py
+-rw-r--r--   0        0        0     6250 2024-05-05 17:41:30.888830 itunizer-1.0.5/itunizer/itunizer.py
+-rw-r--r--   0        0        0    24902 2024-05-05 17:00:26.877153 itunizer-1.0.5/itunizer/nginx.json
+-rw-r--r--   0        0        0      630 2024-05-05 17:49:17.848430 itunizer-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 itunizer-1.0.5/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `itunizer-1.0.4/README.md` & `itunizer-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `itunizer-1.0.4/itunizer/itunizer.py` & `itunizer-1.0.5/itunizer/itunizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-"""A script to grab itunes items for sale for market research and data research purposes."""
+"""A script to grab itunes items for sale for market and data research."""
 # coding: utf-8
 # !/usr/bin/python3
 # Author: James Campbell
 # License: Please see the license file in this repo
 # First Create Date: 28-Jan-2018
-# Last Update: 03-03-2019
-# Requirements: minimal. check requirements.txt and run pip/pip3 install -f requirements.txt
+# Last Update: 05-May-2024
+# Requirements: minimal. check requirements.txt
 
 # imports section
 
+import json
+import argparse
 from pprint import pprint
 from statistics import mean, median
-import requests
-import argparse
-import pandas as pd
-import json
 
-pd.set_option("display.max_columns", 500)
-pd.set_option("display.width", 1000)
+import pandas as pd
+import requests
 
 # globals
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 logo = """
 ┌────────────────────────┐
 │            ┌───▶       │
 │        ┌───┘   │       │
 │        │   ┌───▶       │
 │        │───┘   │       │
 │        │       │       │
@@ -32,19 +30,20 @@
 │       .│     (█)       │
 │      (█)      '        │
 │       '                │
 │      ┌───────────┐     │
 │      │ itunizer  │     │
 └──────┴───────────┴─────┘
 """
-itunes_url_endpoint = "https://itunes.apple.com/search?term={}&country={}&entity={}"
+ITUNES_URL_ENDPOINT = "https://itunes.apple.com/search?term={}&country={}&entity={}"
 
 # arguments
 parser = argparse.ArgumentParser(
-    description='collects and processes itunes data including ibook, application, and other store items with metadata, example: itunizer -c ibook -s "corn" -t',
+    description='collects and processes itunes data including ibook, application, '
+                'and other store items with metadata, example: itunizer -c ibook -s "corn" -t',
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
 parser.add_argument(
     "-s",
     "--search",
     dest="search_term",
     help="search term to search itunes store for",
@@ -102,17 +101,19 @@
 
 # functions section
 
 
 def get_content():
     """Get data from requests object from itunes endpoint."""
     r = requests.get(
-        itunes_url_endpoint.format(
-            args["search_term"], args["store_country"], args["category_location"]
-        )
+        ITUNES_URL_ENDPOINT.format(
+            args["search_term"], args["store_country"],
+            args["category_location"]
+        ),
+        timeout=10  # Timeout after 10 seconds
     )
     return r
 
 
 def get_mean(jsondata):
     """Get average of list of items using numpy."""
     if len(jsondata["results"]) > 1:
@@ -120,65 +121,57 @@
         return mean(
             [
                 float(price.get("price"))
                 for price in jsondata["results"]
                 if "price" in price
             ]
         )
-        # [a.get('a') for a in alist if 'a' in a]
-    else:
-        return float(jsondata["results"][0]["price"])
+    return float(jsondata["results"][0]["price"])
 
 
 def get_max(jsondata):
     """Get max of list of items using max built in."""
     if len(jsondata["results"]) > 1:
         # key name from itunes
         return max(
             [
                 float(price.get("price"))
                 for price in jsondata["results"]
                 if "price" in price
             ]
         )
-        # [a.get('a') for a in alist if 'a' in a]
-    else:
-        return float(jsondata["results"][0]["price"])
+    return float(jsondata["results"][0]["price"])
 
 
 def get_min(jsondata):
     """Get max of list of items using max built in."""
     if len(jsondata["results"]) > 1:
         # key name from itunes
         return min(
             [
                 float(price.get("price"))
                 for price in jsondata["results"]
                 if "price" in price
             ]
         )
-        # [a.get('a') for a in alist if 'a' in a]
-    else:
-        return float(jsondata["results"][0]["price"])
+    return float(jsondata["results"][0]["price"])
 
 
 def get_median(jsondata):
     """Get median of list of items using statistics.median built in."""
     if len(jsondata["results"]) > 1:
         # key name from itunes
         return median(
             [
                 float(price.get("price"))
                 for price in jsondata["results"]
                 if "price" in price
             ]
         )
-        # [a.get('a') for a in alist if 'a' in a]
-    else:
-        return median(jsondata["results"][0]["price"])
+    return float(jsondata["results"][0]["price"])
 
 
 # main section
 
 
 def main():
     """Main function that runs everything."""
@@ -201,31 +194,24 @@
     average_price = get_mean(jsondata)
     max_price = get_max(jsondata)
     min_price = get_min(jsondata)
     median_price = get_median(jsondata)
     print("Results of the query")
     print("*****" * 5)
     print(
-        "The average price of the \033[94m{0}\033[0m items matching search term\033[92m {1}\033[0m: ${2:.2f}, the median is \033[94m{3:.2f}\033[0m, the min is \033[94m{4:.2f}\033[0m, and the max is \033[94m{5:.2f}\033[0m".format(
-            jsondata["resultCount"],
-            args["search_term"],
-            average_price,
-            median_price,
-            min_price,
-            max_price,
-        )
+        f"The average price of the \033[94m{jsondata['resultCount']}\033[0m items matching search term\033[92m {args['search_term']}\033[0m: ${average_price:.2f}, the median is \033[94m{median_price:.2f}\033[0m, the min is \033[94m{min_price:.2f}\033[0m, and the max is \033[94m{max_price:.2f}\033[0m"
     )
     print("")
     if args["output_table"]:  # if we want to output a table instead of json
         print(
             pd.DataFrame(
                 jsondata["results"], columns=["price", "artistName", "trackName"]
             )
         )
     else:
-        with open("{}.json".format(args["search_term"]), "w") as f:
+        with open(f"{args['search_term']}.json", "w", encoding='utf-8') as f:
             f.write(json.dumps(request_response.json()))
-        exit("file saved as {}.json".format(args["search_term"]))
+        exit(f"file saved as {args['search_term']}.json")
 
 
 if __name__ == "__main__":
     main()
```

