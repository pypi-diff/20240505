# Comparing `tmp/abstract_distances-0.0.0.4.tar.gz` & `tmp/abstract_distances-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_distances-0.0.0.4.tar", last modified: Fri May  3 17:05:06 2024, max compression
+gzip compressed data, was "abstract_distances-0.0.0.5.tar", last modified: Sun May  5 09:03:55 2024, max compression
```

## Comparing `abstract_distances-0.0.0.4.tar` & `abstract_distances-0.0.0.5.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:05:06.960636 abstract_distances-0.0.0.4/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 17:05:06.960636 abstract_distances-0.0.0.4/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.4/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-03 17:05:06.960636 abstract_distances-0.0.0.4/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      982 2024-05-03 17:05:00.000000 abstract_distances-0.0.0.4/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:05:06.956637 abstract_distances-0.0.0.4/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:05:06.956637 abstract_distances-0.0.0.4/src/abstract_distances/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-26 00:28:14.000000 abstract_distances-0.0.0.4/src/abstract_distances/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.4/src/abstract_distances/char_compar.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11430 2024-05-03 17:03:04.000000 abstract_distances-0.0.0.4/src/abstract_distances/distance_cals.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.4/src/abstract_distances/do_distance.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    28890 2024-04-24 20:49:04.000000 abstract_distances-0.0.0.4/src/abstract_distances/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    11516 2024-04-10 19:06:49.000000 abstract_distances-0.0.0.4/src/abstract_distances/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5669 2024-05-03 17:04:51.000000 abstract_distances-0.0.0.4/src/abstract_distances/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1460 2024-04-30 05:13:04.000000 abstract_distances-0.0.0.4/src/abstract_distances/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1975 2024-04-30 09:59:39.000000 abstract_distances-0.0.0.4/src/abstract_distances/get_conversion.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.4/src/abstract_distances/word_compare.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-03 17:05:06.956637 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-03 17:05:06.000000 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      625 2024-05-03 17:05:06.000000 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-03 17:05:06.000000 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-03 17:05:06.000000 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-03 17:05:06.000000 abstract_distances-0.0.0.4/src/abstract_distances.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:03:55.385520 abstract_distances-0.0.0.5/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-05 09:03:55.385520 abstract_distances-0.0.0.5/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_distances-0.0.0.5/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-05 09:03:55.385520 abstract_distances-0.0.0.5/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      982 2024-05-05 09:03:48.000000 abstract_distances-0.0.0.5/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:03:55.381520 abstract_distances-0.0.0.5/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:03:55.385520 abstract_distances-0.0.0.5/src/abstract_distances/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-26 00:28:14.000000 abstract_distances-0.0.0.5/src/abstract_distances/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    10114 2024-04-25 03:57:30.000000 abstract_distances-0.0.0.5/src/abstract_distances/char_compar.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     9511 2024-05-05 09:03:34.000000 abstract_distances-0.0.0.5/src/abstract_distances/distance_cals.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8631 2024-04-26 22:25:41.000000 abstract_distances-0.0.0.5/src/abstract_distances/do_distance.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-05 09:03:20.000000 abstract_distances-0.0.0.5/src/abstract_distances/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8858 2024-04-26 22:24:51.000000 abstract_distances-0.0.0.5/src/abstract_distances/word_compare.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-05 09:03:55.385520 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      613 2024-05-05 09:03:55.000000 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      473 2024-05-05 09:03:55.000000 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-05 09:03:55.000000 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-05-05 09:03:55.000000 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       19 2024-05-05 09:03:55.000000 abstract_distances-0.0.0.5/src/abstract_distances.egg-info/top_level.txt
```

### Comparing `abstract_distances-0.0.0.4/PKG-INFO` & `abstract_distances-0.0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_distances-0.0.0.4/setup.py` & `abstract_distances-0.0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_distances',
-    version='0.0.0.4',
+    version='0.0.0.5',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_distances-0.0.0.4/src/abstract_distances/char_compar.py` & `abstract_distances-0.0.0.5/src/abstract_distances/char_compar.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.4/src/abstract_distances/distance_cals.py` & `abstract_distances-0.0.0.5/src/abstract_distances/distance_cals.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,32 @@
 import numpy as np
-import pandas as pd
-from .geo_pandas import *
-from .excel_module import *
+from abstract_pandas import get_df,get_closest_headers,append_unique_to_excels,get_address_header_association
+from abstract_pandas.landManager import get_bp
 from .word_compare import *
-from abstract_utilities import *
-import math,re,requests, httpx, asyncio
-from math import sin, cos, asin, atan2, radians, degrees, pi,atan2, sqrt
+from abstract_utilities import get_any_value,get_closest_boudary
+import re,requests, httpx, asyncio
 from openlocationcode import openlocationcode as olc
+from .functions import *
 def get_default_google_api_key():
     return get_env_value(key="google_maps_api_key")
-def haversine(lat1, lon1, lat2, lon2):
-    """
-    Calculate the great circle distance in kilometers between two points 
-    on the earth (specified in decimal degrees)
-    """
-    # Convert decimal degrees to radians 
-    lat1, lon1, lat2, lon2 = map(radians, [lat1, lon1, lat2, lon2])
-    
-    # Haversine formula 
-    dlat = lat2 - lat1 
-    dlon = lon2 - lon1 
-    a = sin(dlat/2)**2 + cos(lat1) * cos(lat2) * sin(dlon/2)**2
-    c = 2 * atan2(sqrt(a), sqrt(1-a)) 
-    distance = 3959 * c  # Earth's radius in kilometers
-    return distance
-def get_closest_boudary(D_lat, D_lon, boundary_polygon=None):
-    boundary_polygon = get_bp(boundary_polygon)
-    # Assuming read_excel_as_dicts is meant to read Excel file and convert it into a list of dictionaries
-    # Assuming each dict has 'lat' and 'lon' keys
-    closest_point = None
-    shortest_distance = float('inf')
-    for i,dist in enumerate(boundary_polygon):
-        lat, lon = dist[0], dist[1]
-
-        distance = haversine(D_lat, D_lon, lat, lon)
-        if distance < shortest_distance:
-            shortest_distance = distance
-            closest_point = (lat, lon)
-    
-    return shortest_distance, closest_point
 def get_closest_exact_boudary(D_lat, D_lon, boundary_polygon=None,api_key=None):
     api_key = api_key or get_default_google_api_key()
     boundary_polygon = get_bp(boundary_polygon)
     shortest,coordinates = get_closest_boudary(D_lat, D_lon, boundary_polygon)
     address_2 = get_address_from_latlngs(coordinates[0],coordinates[1])
     return get_lat_long(address_2,api_key)
-def is_point_inside_polygon(point_lat, point_lon, polygon):
-    """
-    Determine if a point is inside a given polygon or not.
-    
-    Polygon is a list of (latitude, longitude) tuples, and point is defined by (point_lat, point_lon).
-    """
-    num = len(polygon)
-    inside = False
-    x, y = point_lon, point_lat
-    if None not in [x,y]:
-  
-        p1x, p1y = polygon[0]
-        for i in range(num+1):
-            p2x, p2y = polygon[i % num]
-            
-            if y > min(p1y, p2y):
-                if y <= max(p1y, p2y):
-                    if x <= max(p1x, p2x):
-                        if p1y != p2y:
-                            xints = (y-p1y)*(p2x-p1x)/(p2y-p1y)+p1x
-                        if p1x == p2x or x <= xints:
-                            inside = not inside
-            p1x, p1y = p2x, p2y
-
-    return inside
+def get_from_distance_response(json_response):
+    text_finds = get_any_value(json_response, 'text')
+    if text_finds:
+        text_find_list = make_list(text_finds)
+        if text_find_list and isinstance(text_find_list, list) and len(text_find_list) > 0:
+            text_find_list = text_find_list[0]
+        if text_find_list and isinstance(text_find_list, str):
+            return text_find_list.split(' ')[0]
+    return text_finds
 def get_lat_long(address,boundary_polygon=None, api_key=None):
     api_key =api_key or get_default_google_api_key()
     boundary_polygon = get_bp(boundary_polygon)
     
     base_url = "https://maps.googleapis.com/maps/api/geocode/json"
     params = {
         "address": address,
@@ -86,23 +39,40 @@
         if results:
             location = results[0]['geometry']['location']
             return location['lat'], location['lng']
         else:
             return None, None
     else:
         return None, None
-def get_from_distance_response(json_response):
-    text_finds = get_any_value(json_response, 'text')
-    if text_finds:
-        text_find_list = make_list(text_finds)
-        if text_find_list and isinstance(text_find_list, list) and len(text_find_list) > 0:
-            text_find_list = text_find_list[0]
-        if text_find_list and isinstance(text_find_list, str):
-            return text_find_list.split(' ')[0]
-    return text_finds
+def get_address_from_latlngs(lat, lng, api_key=None):
+    api_key = api_key or get_default_google_api_key()
+    # Endpoint URL
+    base_url = "https://maps.googleapis.com/maps/api/geocode/json"
+    
+    # Parameters for the API request
+    params = {
+        "latlng": f"{lat},{lng}",
+        "key": api_key
+    }
+    
+    # Send request and get response data
+    response = requests.get(base_url, params=params)
+    
+    # Convert response to JSON format
+
+    results = response.json()
+    
+    # Check if any results were returned
+    if results["status"] == "OK":
+        # Return the formatted address of the first result
+        address = results["results"][0]["formatted_address"]
+        return f"{address.split(' ')[0].split('+')[0]} {' '.join(address.split(' ')[1:])}"
+    else:
+        # Return error message if no results found
+        return "No address found for this latitude and longitude"
 async def calculateDistance(origin, destination,travelMode = 'DRIVING',api_key=None,print_response = True,return_all = False):
     api_key =api_key or get_default_google_api_key()
     base_url = f"https://maps.googleapis.com/maps/api/distancematrix/json?origins={origin}&destinations={destination}&travelMode={travelMode}&units=imperial&key={api_key}"
     
     async with httpx.AsyncClient() as client:
         response = await client.get(base_url)
         
@@ -114,14 +84,25 @@
         if print_response:
             print(response.text)
         response = response.json()
         # Your existing logic to extract distance
         if return_all == False:
             response = get_from_distance_response(response)
         return response
+async def get_distance_calculation(address, boundary_polygon=None,api_key=None):
+    boundary_polygon = get_bp(boundary_polygon)
+    if isinstance(address,str):
+        dest_latitude,dest_longitude = get_lat_long(address,boundary_polygon)
+    in_city_limit = is_point_inside_polygon(dest_latitude, dest_longitude, boundary_polygon)
+    if in_city_limit:
+        return 0
+    coordinates = get_closest_exact_boudary(dest_latitude,dest_longitude,boundary_polygon)
+    src_latitude,src_longitude= coordinates[0],coordinates[1]
+    distance = await calculateDistance(f"{src_latitude} {src_longitude}",f"{dest_latitude} {dest_longitude}",travelMode="DRIVING")
+    return distance
 
 def get_address_header_association(headers_js,df,index,spec_headers=False):
     print(headers_js)
     if not isinstance(headers_js,dict):
         headers_js = get_closest_headers(headers_js)
     if isinstance(headers_js,dict):
         address = f"{df[headers_js['address']].loc[index]} {df[headers_js['city']].loc[index]} {df[headers_js['state']].loc[index]} {df[headers_js['zip']].loc[index]}"
@@ -147,36 +128,26 @@
             distance = await get_distance_calculation(address,boundary_polygon)
     elif isinstance(distance, str) and distance.isdigit():
         if int(distance) == 0:  # Additional check if the string number is zero
             address = get_address_header_association(headers_js, new_data)
             distance = await get_distance_calculation(address,boundary_polygon)
 
     return distance  # Return the processed or retrieved distance
-async def get_distance_for_excel_row(df,file_path=None,row_itter=0,distance=None,row_data=None,address=None,headers_js=None,search_column=None,boundary_polygon=None, search_value=None):
+async def get_distance_for_excel_row(df,file_path=None,row_itter=0,distance=None,row_data=None,address=None,headers_js=None,search_column=None,boundary_polygon=None, search_value=None,distance_header='distance'):
     boundary_polygon = get_bp(boundary_polygon)
     df=get_df(df or file_path,make_excel=row_data)
     if row_data==None:
        row_data = get_row_as_list(df,index=row_itter) or {}
     if address == None:
         address = get_address_header_association(headers_js,df,row_itter)
     if distance == None:
         distance = await get_distance_calculation(address, boundary_polygon)
-    row_data['distance'] = distance or 0
+    row_data[distance_header] = distance or 0
     return append_unique_to_excels(df,file_path = file_path, new_data = row_data,search_column=search_column, search_value=search_value)
-async def get_distance_calculation(address, boundary_polygon=None,api_key=None):
-    boundary_polygon = get_bp(boundary_polygon)
-    if isinstance(address,str):
-        dest_latitude,dest_longitude = get_lat_long(address,boundary_polygon)
-    in_city_limit = is_point_inside_polygon(dest_latitude, dest_longitude, boundary_polygon)
-    if in_city_limit:
-        return 0
-    coordinates = get_closest_exact_boudary(dest_latitude,dest_longitude,boundary_polygon)
-    src_latitude,src_longitude= coordinates[0],coordinates[1]
-    distance = await calculateDistance(f"{src_latitude} {src_longitude}",f"{dest_latitude} {dest_longitude}",travelMode="DRIVING")
-    return distance
+
 async def add_distance_calculatuions_to_excel_data(excel_file_path,boundary_polygon=None,append=False,new_excel_path="new_excel_file.xlsx"):
     boundary_polygon = get_bp(boundary_polygon)
     api_key = api_key or get_default_google_api_key()
     if not os.path.isfile(excel_file_path):
         return
     all_distance = safe_read_from_json("all_distances.json")
     headers_js = get_closest_headers(excel_file_path)
@@ -201,40 +172,14 @@
                     address = get_address_header_association(headers_js,main_df,index)
                     row['distance']=await get_distance_calculation(address, boundary_polygon=boundary_polygon)
                     all_distance[zip_now] = row['distance']
                     safe_dump_to_json(data=all_distance,file_path=-'all_distances.js')
             main_df = append_unique_to_excels(main_df, new_data = row,search_column=headers_js['external'], search_value=row.get(headers_js['external']),print_it=False)
             
             safe_excel_save(main_df,new_excel_path)
-def get_address_from_latlngs(lat, lng, api_key=None):
-    api_key = api_key or get_default_google_api_key()
-    # Endpoint URL
-    base_url = "https://maps.googleapis.com/maps/api/geocode/json"
-    
-    # Parameters for the API request
-    params = {
-        "latlng": f"{lat},{lng}",
-        "key": api_key
-    }
-    
-    # Send request and get response data
-    response = requests.get(base_url, params=params)
-    
-    # Convert response to JSON format
-
-    results = response.json()
-    
-    # Check if any results were returned
-    if results["status"] == "OK":
-        # Return the formatted address of the first result
-        address = results["results"][0]["formatted_address"]
-        return f"{address.split(' ')[0].split('+')[0]} {' '.join(address.split(' ')[1:])}"
-    else:
-        # Return error message if no results found
-        return "No address found for this latitude and longitude"
 
 def convert_to_str_lalng(obj):
     if isinstance(obj,str):
         obj = obj.replace(',',' ').split(' ')
         return f"{obj[0]} {obj[-1]}"
     for ty in [set,list,tuple]:
         if isinstance(obj,ty):
```

### Comparing `abstract_distances-0.0.0.4/src/abstract_distances/do_distance.py` & `abstract_distances-0.0.0.5/src/abstract_distances/do_distance.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.4/src/abstract_distances/word_compare.py` & `abstract_distances-0.0.0.5/src/abstract_distances/word_compare.py`

 * *Files identical despite different names*

### Comparing `abstract_distances-0.0.0.4/src/abstract_distances.egg-info/PKG-INFO` & `abstract_distances-0.0.0.5/src/abstract_distances.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_distances
-Version: 0.0.0.4
+Version: 0.0.0.5
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

