# Comparing `tmp/itunizer-1.0.3.tar.gz` & `tmp/itunizer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/itunizer-1.0.3.tar", last modified: Wed Nov  6 04:29:34 2019, max compression
+gzip compressed data, was "dist/itunizer-1.0.4.tar", last modified: Wed Nov  6 04:36:51 2019, max compression
```

## Comparing `itunizer-1.0.3.tar` & `itunizer-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:29:34.000000 itunizer-1.0.3/
--rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:29:34.000000 itunizer-1.0.3/PKG-INFO
--rw-r--r--   0 jamescampbell   (501) staff       (20)     1558 2019-06-16 23:55:39.000000 itunizer-1.0.3/README.md
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer/
--rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-01-13 17:29:13.000000 itunizer-1.0.3/itunizer/__init__.py
--rw-r--r--   0 jamescampbell   (501) staff       (20)       34 2019-11-06 04:21:52.000000 itunizer-1.0.3/itunizer/__main__.py
--rw-r--r--   0 jamescampbell   (501) staff       (20)     6035 2019-11-06 04:23:23.000000 itunizer-1.0.3/itunizer/itunizer.py
-drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/
--rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/PKG-INFO
--rw-r--r--   0 jamescampbell   (501) staff       (20)      285 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/SOURCES.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/dependency_links.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       53 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/entry_points.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       32 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/requires.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)        9 2019-11-06 04:29:34.000000 itunizer-1.0.3/itunizer.egg-info/top_level.txt
--rw-r--r--   0 jamescampbell   (501) staff       (20)       79 2019-11-06 04:29:34.000000 itunizer-1.0.3/setup.cfg
--rw-r--r--   0 jamescampbell   (501) staff       (20)     1000 2019-11-06 04:21:52.000000 itunizer-1.0.3/setup.py
+drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/
+-rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:36:51.000000 itunizer-1.0.4/PKG-INFO
+-rw-r--r--   0 jamescampbell   (501) staff       (20)     1558 2019-06-16 23:55:39.000000 itunizer-1.0.4/README.md
+drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer/
+-rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-01-13 17:29:13.000000 itunizer-1.0.4/itunizer/__init__.py
+-rw-r--r--   0 jamescampbell   (501) staff       (20)       35 2019-11-06 04:36:33.000000 itunizer-1.0.4/itunizer/__main__.py
+-rw-r--r--   0 jamescampbell   (501) staff       (20)     6674 2019-11-06 04:36:33.000000 itunizer-1.0.4/itunizer/itunizer.py
+drwxr-xr-x   0 jamescampbell   (501) staff       (20)        0 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/
+-rw-r--r--   0 jamescampbell   (501) staff       (20)      501 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/PKG-INFO
+-rw-r--r--   0 jamescampbell   (501) staff       (20)      285 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/SOURCES.txt
+-rw-r--r--   0 jamescampbell   (501) staff       (20)        1 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/dependency_links.txt
+-rw-r--r--   0 jamescampbell   (501) staff       (20)       53 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/entry_points.txt
+-rw-r--r--   0 jamescampbell   (501) staff       (20)       32 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/requires.txt
+-rw-r--r--   0 jamescampbell   (501) staff       (20)        9 2019-11-06 04:36:51.000000 itunizer-1.0.4/itunizer.egg-info/top_level.txt
+-rw-r--r--   0 jamescampbell   (501) staff       (20)       79 2019-11-06 04:36:51.000000 itunizer-1.0.4/setup.cfg
+-rw-r--r--   0 jamescampbell   (501) staff       (20)      914 2019-11-06 04:36:33.000000 itunizer-1.0.4/setup.py
```

### Comparing `itunizer-1.0.3/README.md` & `itunizer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `itunizer-1.0.3/itunizer/itunizer.py` & `itunizer-1.0.4/itunizer/itunizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 from pprint import pprint
 from statistics import mean, median
 import requests
 import argparse
 import pandas as pd
 import json
-pd.set_option('display.max_columns', 500)
-pd.set_option('display.width', 1000)
+
+pd.set_option("display.max_columns", 500)
+pd.set_option("display.width", 1000)
 
 # globals
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 logo = """
 ┌────────────────────────┐
 │            ┌───▶       │
 │        ┌───┘   │       │
 │        │   ┌───▶       │
 │        │───┘   │       │
 │        │       │       │
@@ -31,118 +32,200 @@
 │       .│     (█)       │
 │      (█)      '        │
 │       '                │
 │      ┌───────────┐     │
 │      │ itunizer  │     │
 └──────┴───────────┴─────┘
 """
-itunes_url_endpoint = 'https://itunes.apple.com/search?term={}&country={}&entity={}'
+itunes_url_endpoint = "https://itunes.apple.com/search?term={}&country={}&entity={}"
 
 # arguments
-parser = argparse.ArgumentParser(description='collects and processes itunes data including ibook, application, and other store items with metadata, example: itunizer -c ibook -s "corn" -t',
-                                 formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-parser.add_argument('-s', '--search', dest='search_term',
-                    help='search term to search itunes store for', default='nginx', required=False)
-parser.add_argument('-c', '--category', dest='category_location',
-                    help='category in store to search for', default='software', required=False)
-parser.add_argument('-p', '--print', dest='print_me',
-                    help='print to screen results, helpful for testing', action='store_true', default=False)
-parser.add_argument('-n', '--no-logo', dest='logo_off',
-                    help='disables printing logo', action='store_true', default=False)
-parser.add_argument('-t', '--table', dest='output_table',
-                    help='prints out table as format for data', action='store_true', default=False)
-parser.add_argument('--country', dest='store_country', default='us',
-                    help='the store country you want to use for search results')
-parser.add_argument('--version', '-v', dest='app_version', help='prints the version', action='store_true', default=False)
+parser = argparse.ArgumentParser(
+    description='collects and processes itunes data including ibook, application, and other store items with metadata, example: itunizer -c ibook -s "corn" -t',
+    formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+)
+parser.add_argument(
+    "-s",
+    "--search",
+    dest="search_term",
+    help="search term to search itunes store for",
+    default="nginx",
+    required=False,
+)
+parser.add_argument(
+    "-c",
+    "--category",
+    dest="category_location",
+    help="category in store to search for; what is available is movie, podcast, music, musicVideo, audiobook, shortFilm, tvShow, software, ebook, all",
+    default="software",
+    required=False,
+)
+parser.add_argument(
+    "-p",
+    "--print",
+    dest="print_me",
+    help="print to screen results, helpful for testing",
+    action="store_true",
+    default=False,
+)
+parser.add_argument(
+    "-n",
+    "--no-logo",
+    dest="logo_off",
+    help="disables printing logo",
+    action="store_true",
+    default=False,
+)
+parser.add_argument(
+    "-t",
+    "--table",
+    dest="output_table",
+    help="prints out table as format for data",
+    action="store_true",
+    default=False,
+)
+parser.add_argument(
+    "--country",
+    dest="store_country",
+    default="us",
+    help="the store country you want to use for search results",
+)
+parser.add_argument(
+    "--version",
+    "-v",
+    dest="app_version",
+    help="prints the version",
+    action="store_true",
+    default=False,
+)
 args = vars(parser.parse_args())
 
 
 # functions section
 
 
 def get_content():
     """Get data from requests object from itunes endpoint."""
-    r = requests.get(itunes_url_endpoint.format(
-        args['search_term'], args['store_country'], args['category_location']))
+    r = requests.get(
+        itunes_url_endpoint.format(
+            args["search_term"], args["store_country"], args["category_location"]
+        )
+    )
     return r
 
 
 def get_mean(jsondata):
     """Get average of list of items using numpy."""
-    if len(jsondata['results']) > 1:
+    if len(jsondata["results"]) > 1:
         # key name from itunes
-        return mean([float(price.get('price')) for price in jsondata['results'] if 'price' in price])
+        return mean(
+            [
+                float(price.get("price"))
+                for price in jsondata["results"]
+                if "price" in price
+            ]
+        )
         # [a.get('a') for a in alist if 'a' in a]
     else:
-        return float(jsondata['results'][0]['price'])
+        return float(jsondata["results"][0]["price"])
 
 
 def get_max(jsondata):
     """Get max of list of items using max built in."""
-    if len(jsondata['results']) > 1:
+    if len(jsondata["results"]) > 1:
         # key name from itunes
-        return max([float(price.get('price')) for price in jsondata['results'] if 'price' in price])
+        return max(
+            [
+                float(price.get("price"))
+                for price in jsondata["results"]
+                if "price" in price
+            ]
+        )
         # [a.get('a') for a in alist if 'a' in a]
     else:
-        return float(jsondata['results'][0]['price'])
+        return float(jsondata["results"][0]["price"])
 
 
 def get_min(jsondata):
     """Get max of list of items using max built in."""
-    if len(jsondata['results']) > 1:
+    if len(jsondata["results"]) > 1:
         # key name from itunes
-        return min([float(price.get('price')) for price in jsondata['results'] if 'price' in price])
+        return min(
+            [
+                float(price.get("price"))
+                for price in jsondata["results"]
+                if "price" in price
+            ]
+        )
         # [a.get('a') for a in alist if 'a' in a]
     else:
-        return float(jsondata['results'][0]['price'])
+        return float(jsondata["results"][0]["price"])
 
 
 def get_median(jsondata):
     """Get median of list of items using statistics.median built in."""
-    if len(jsondata['results']) > 1:
+    if len(jsondata["results"]) > 1:
         # key name from itunes
-        return median([float(price.get('price')) for price in jsondata['results'] if 'price' in price])
+        return median(
+            [
+                float(price.get("price"))
+                for price in jsondata["results"]
+                if "price" in price
+            ]
+        )
         # [a.get('a') for a in alist if 'a' in a]
     else:
-        return median(jsondata['results'][0]['price'])
+        return median(jsondata["results"][0]["price"])
+
 
 # main section
 
 
 def main():
     """Main function that runs everything."""
-    if not args['logo_off']:  # print or not print logo
+    if not args["logo_off"]:  # print or not print logo
         print(logo)
-    if args['app_version']:
+    if args["app_version"]:
         print(f"Current version: {__version__}")
         exit(0)
     request_response = get_content()
     jsondata = request_response.json()
     # [trend['name'] for trend in the_data[0]['trends']]
     print()
-    if args['print_me']:  # if we are running a test or not
-        print('json data:')
+    if args["print_me"]:  # if we are running a test or not
+        print("json data:")
         pprint(jsondata)
-        print('fields available:')
-        for k, _ in jsondata['results'][0].items():
+        print("fields available:")
+        for k, _ in jsondata["results"][0].items():
             print(k)
-        exit('thanks for trying')
+        exit("thanks for trying")
     average_price = get_mean(jsondata)
     max_price = get_max(jsondata)
     min_price = get_min(jsondata)
     median_price = get_median(jsondata)
     print("Results of the query")
-    print("*****"*5)
-    print("The average price of the \033[94m{0}\033[0m items matching search term\033[92m {1}\033[0m: ${2:.2f}, the median is \033[94m{3:.2f}\033[0m, the min is \033[94m{4:.2f}\033[0m, and the max is \033[94m{5:.2f}\033[0m".format(
-        jsondata['resultCount'], args['search_term'], average_price, median_price, min_price, max_price))
+    print("*****" * 5)
+    print(
+        "The average price of the \033[94m{0}\033[0m items matching search term\033[92m {1}\033[0m: ${2:.2f}, the median is \033[94m{3:.2f}\033[0m, the min is \033[94m{4:.2f}\033[0m, and the max is \033[94m{5:.2f}\033[0m".format(
+            jsondata["resultCount"],
+            args["search_term"],
+            average_price,
+            median_price,
+            min_price,
+            max_price,
+        )
+    )
     print("")
-    if args['output_table']:  # if we want to output a table instead of json
-        print(pd.DataFrame(jsondata['results'], columns=[
-              "price", "artistName", "trackName"]))
+    if args["output_table"]:  # if we want to output a table instead of json
+        print(
+            pd.DataFrame(
+                jsondata["results"], columns=["price", "artistName", "trackName"]
+            )
+        )
     else:
-        with open('{}.json'.format(args['search_term']), 'w') as f:
+        with open("{}.json".format(args["search_term"]), "w") as f:
             f.write(json.dumps(request_response.json()))
-        exit('file saved as {}.json'.format(args['search_term']))
+        exit("file saved as {}.json".format(args["search_term"]))
 
 
 if __name__ == "__main__":
     main()
```

