# Comparing `tmp/seffaflik2-0.0.1.tar.gz` & `tmp/seffaflik2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seffaflik2-0.0.1.tar", last modified: Sun May  5 00:17:54 2024, max compression
+gzip compressed data, was "seffaflik2-0.0.2.tar", last modified: Sun May  5 06:43:36 2024, max compression
```

## Comparing `seffaflik2-0.0.1.tar` & `seffaflik2-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 00:17:54.175139 seffaflik2-0.0.1/
--rw-r--r--   0 noremas    (501) staff       (20)     2954 2024-05-05 00:17:54.175017 seffaflik2-0.0.1/PKG-INFO
--rw-r--r--   0 noremas    (501) staff       (20)     2572 2024-05-05 00:07:36.000000 seffaflik2-0.0.1/README.md
-drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 00:17:54.174212 seffaflik2-0.0.1/seffaflik2/
--rw-r--r--   0 noremas    (501) staff       (20)       25 2024-05-04 23:37:56.000000 seffaflik2-0.0.1/seffaflik2/__init__.py
--rw-r--r--   0 noremas    (501) staff       (20)    10190 2024-05-04 23:21:04.000000 seffaflik2-0.0.1/seffaflik2/seffaflik2.py
-drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 00:17:54.174857 seffaflik2-0.0.1/seffaflik2.egg-info/
--rw-r--r--   0 noremas    (501) staff       (20)     2954 2024-05-05 00:17:54.000000 seffaflik2-0.0.1/seffaflik2.egg-info/PKG-INFO
--rw-r--r--   0 noremas    (501) staff       (20)      235 2024-05-05 00:17:54.000000 seffaflik2-0.0.1/seffaflik2.egg-info/SOURCES.txt
--rw-r--r--   0 noremas    (501) staff       (20)        1 2024-05-05 00:17:54.000000 seffaflik2-0.0.1/seffaflik2.egg-info/dependency_links.txt
--rw-r--r--   0 noremas    (501) staff       (20)       22 2024-05-05 00:17:54.000000 seffaflik2-0.0.1/seffaflik2.egg-info/requires.txt
--rw-r--r--   0 noremas    (501) staff       (20)       11 2024-05-05 00:17:54.000000 seffaflik2-0.0.1/seffaflik2.egg-info/top_level.txt
--rw-r--r--   0 noremas    (501) staff       (20)       38 2024-05-05 00:17:54.175176 seffaflik2-0.0.1/setup.cfg
--rw-r--r--   0 noremas    (501) staff       (20)      733 2024-05-05 00:16:25.000000 seffaflik2-0.0.1/setup.py
+drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 06:43:36.810629 seffaflik2-0.0.2/
+-rw-r--r--   0 noremas    (501) staff       (20)     3637 2024-05-05 06:43:36.810511 seffaflik2-0.0.2/PKG-INFO
+-rw-r--r--   0 noremas    (501) staff       (20)     3255 2024-05-05 06:41:40.000000 seffaflik2-0.0.2/README.md
+drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 06:43:36.809626 seffaflik2-0.0.2/seffaflik2/
+-rw-r--r--   0 noremas    (501) staff       (20)       25 2024-05-04 23:37:56.000000 seffaflik2-0.0.2/seffaflik2/__init__.py
+-rw-r--r--   0 noremas    (501) staff       (20)    13981 2024-05-05 06:41:43.000000 seffaflik2-0.0.2/seffaflik2/seffaflik2.py
+drwxr-xr-x   0 noremas    (501) staff       (20)        0 2024-05-05 06:43:36.810357 seffaflik2-0.0.2/seffaflik2.egg-info/
+-rw-r--r--   0 noremas    (501) staff       (20)     3637 2024-05-05 06:43:36.000000 seffaflik2-0.0.2/seffaflik2.egg-info/PKG-INFO
+-rw-r--r--   0 noremas    (501) staff       (20)      235 2024-05-05 06:43:36.000000 seffaflik2-0.0.2/seffaflik2.egg-info/SOURCES.txt
+-rw-r--r--   0 noremas    (501) staff       (20)        1 2024-05-05 06:43:36.000000 seffaflik2-0.0.2/seffaflik2.egg-info/dependency_links.txt
+-rw-r--r--   0 noremas    (501) staff       (20)       22 2024-05-05 06:43:36.000000 seffaflik2-0.0.2/seffaflik2.egg-info/requires.txt
+-rw-r--r--   0 noremas    (501) staff       (20)       11 2024-05-05 06:43:36.000000 seffaflik2-0.0.2/seffaflik2.egg-info/top_level.txt
+-rw-r--r--   0 noremas    (501) staff       (20)       38 2024-05-05 06:43:36.810664 seffaflik2-0.0.2/setup.cfg
+-rw-r--r--   0 noremas    (501) staff       (20)      733 2024-05-05 06:43:08.000000 seffaflik2-0.0.2/setup.py
```

### Comparing `seffaflik2-0.0.1/PKG-INFO` & `seffaflik2-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,70 @@
-Metadata-Version: 2.1
-Name: seffaflik2
-Version: 0.0.1
-Summary: EPIAS Transparency Platform 2.0 Unofficial Python Library
-Home-page: https://github.com/berkomeratay/seffaflik2
-Author: Berk Ömer Atay
-Author-email: <berkomeratay@gmail.com>
-Keywords: python,epias,seffaflik,epias transparency platform,transparency,epiaş şeffaflık platformu
-Description-Content-Type: text/markdown
-
 # EPİAŞ Transparency Platform 2.0 Python Library
 
 This library enables users to get data from EPİAŞ's Transparency Platform by using simple python functions.
 
 Please note that this is not an official release, and the accuracy or reliability of the data retrieved through this library cannot be guaranteed. Users are advised to exercise caution and verify the data independently before making any decisions based on it. 
 
 The author(s) of this library shall not be held responsible for any inaccuracies or damages resulting from the use of the data.
 
 Data input formats should be such as: "YYYY-MM-DD". An example would be : "2024-05-29"
 
 All the functions returns a pandas dataframe.
 
 ## Currently few selected datasets are available, which are:
 
-
+### Day-ahead-market
 epias_mcp(start_date,end_date): Function that returns the MCP for a given interval
 
+epias_pi_offer(start_date,end_date):  Function that turns the amount of price independent offers in day-ahead-market for a given interval
+
+epias_pi_bid(start_date,end_date):  Function that turns the amount of price independent bids in day-ahead-market for a given interval
+
+epias_spot(start_date,end_date): Function that turns the amount of matched amount in day-ahead-market for a given interval
+
+epias_ba(start_date,end_date):  Function that turns the amount of block offers (matched and non-matched) of day-ahead-market for a given interval
+
+### Generation
+
 epias_kgup(start_date,end_date): Function that returns the DPP's (KGUP) based on resources for a given interval
 
 epias_plant_kgup(start_date,end_date,pl_id,o_id): Function that returns the DPP's (KGUP) based on resources for a given interval (org_id: Organization ID, pl_id: Plant ID) Organization IDs can be obtained via epias_org function Plant IDs can be obtained via  epias_uevcb function
 
 epias_org(start_date,end_date): Function that returns the organizations for a given interval
 
 epias_uevcb(start_date,end_date,o_id): Function that returns the UEVCB data for a given interval (o_id: Organization ID)
 
+### Consumption
+
 epias_demand(start_date,end_date): Function that returns the real time electricity consumption for a given interval
 
-epias_idmp(start_date,end_date): Function that returns the intraday markey prices for a given interval
+### Intraday market
+
+epias_idmp(start_date,end_date): Function that returns the intraday weighted average prices for a given interval
 
 epias_idma(start_date,end_date): Function that returns the trade amount at intraday market for a given interval 
 
+### Balancing Power Market
+
 epias_smp(start_date,end_date): Function that returns the System Marginal Price for a given interval 
 
 epias_yal(start_date,end_date): Function that returns the amount of load orders (YAL) for a given interval 
 
 epias_yat(start_date,end_date): Function that returns the amount of deload orders (YAT) for a given interval
 
+### Ancillary Services
+
 epias_sfc(start_date,end_date): Function that returns the SFC prices for a given interval
 
 epias_pfc(start_date,end_date): Function that returns the PFC prices for a given interval
 
 
 
+
+
 #### Example 1
 ```python
 from seffaflik2 import epias_mcp
 
 day_ahead_prices = epias_mcp("2024-01-15","2024-03-16")
 
 print(day_ahead_prices)
```

### Comparing `seffaflik2-0.0.1/seffaflik2/seffaflik2.py` & `seffaflik2-0.0.2/seffaflik2/seffaflik2.py`

 * *Files 11% similar despite different names*

```diff
@@ -122,16 +122,16 @@
     Function that turns the organizations for a given interval
     
     """
 
     url = "https://seffaflik.epias.com.tr/electricity-service/v1/generation/data/organization-list"
 
     payload = json.dumps({
-      "endDate": ed+"T00:00:00+03:00",
-      "startDate": sd+"T00:00:00+03:00"
+      "endDate": ed,
+      "startDate": sd
     })
     headers = {
       'Content-Type': 'application/json'
     }
 
     response = requests.post(url, headers=headers, data=payload)
 
@@ -424,8 +424,172 @@
 
         df = pd.json_normalize(response.json()['items'])
 
         df['date'] = pd.to_datetime(df['date'])
 
         return df
     else:
-        return response.text
+        return response.text
+    
+
+def epias_pi_offer(start_date,end_date):
+    
+    sd = date_converter(start_date)
+    ed = date_converter(end_date)
+
+    """
+    Function that turns the amount of price independent offers in day-ahead-market for a given interval
+    
+    """
+
+    url = "https://seffaflik.epias.com.tr/electricity-service/v1/markets/dam/data/price-independent-offer"
+
+    payload = json.dumps({
+      "endDate": ed,
+      "startDate": sd
+    })
+    headers = {
+      'Content-Type': 'application/json'
+    }
+
+    response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code == 200:
+
+        df = pd.json_normalize(response.json()['items'])
+
+        df['date'] = pd.to_datetime(df['date'])
+
+        return df
+    else:
+        return response.text
+    
+def epias_pi_bid(start_date,end_date):
+    
+    sd = date_converter(start_date)
+    ed = date_converter(end_date)
+
+    """
+    Function that turns the amount of price independent bids in day-ahead-market for a given interval
+    
+    """
+
+    url = "https://seffaflik.epias.com.tr/electricity-service/v1/markets/dam/data/price-independent-bid"
+
+    payload = json.dumps({
+      "endDate": ed,
+      "startDate": sd
+    })
+    headers = {
+      'Content-Type': 'application/json'
+    }
+
+    response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code == 200:
+
+        df = pd.json_normalize(response.json()['items'])
+
+        df['date'] = pd.to_datetime(df['date'])
+
+        return df
+    else:
+        return response.text
+    
+def epias_spot(start_date,end_date):
+    
+    sd = date_converter(start_date)
+    ed = date_converter(end_date)
+
+    """
+    Function that turns the amount of matched amount in day-ahead-market for a given interval
+    
+    """
+
+    url = "https://seffaflik.epias.com.tr/electricity-service/v1/markets/dam/data/clearing-quantity"
+
+    payload = json.dumps({
+      "endDate": ed,
+      "startDate": sd
+    })
+    headers = {
+      'Content-Type': 'application/json'
+    }
+
+    response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code == 200:
+
+        df = pd.json_normalize(response.json()['items'])
+
+        df['date'] = pd.to_datetime(df['date'])
+
+        return df
+    else:
+        return response.text
+    
+def epias_ba_offers(start_date,end_date):
+    
+    sd = date_converter(start_date)
+    ed = date_converter(end_date)
+
+    """
+    Function that turns the amount of block offers (matched and non-matched) of day-ahead-market for a given interval
+    
+    """
+
+    url = "https://seffaflik.epias.com.tr/electricity-service/v1/markets/dam/data/amount-of-block-selling"
+
+    payload = json.dumps({
+      "endDate": ed,
+      "startDate": sd
+    })
+    headers = {
+      'Content-Type': 'application/json'
+    }
+
+    response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code == 200:
+
+        df = pd.json_normalize(response.json()['items'])
+
+        df['date'] = pd.to_datetime(df['date'])
+
+        return df
+    else:
+        return response.text
+    
+def epias_ba_bids(start_date,end_date):
+    
+    sd = date_converter(start_date)
+    ed = date_converter(end_date)
+
+    """
+    Function that turns the amount of block bids (matched and non-matched) of day-ahead-market for a given interval
+    
+    """
+
+    url = "https://seffaflik.epias.com.tr/electricity-service/v1/markets/dam/data/amount-of-block-buying"
+
+    payload = json.dumps({
+      "endDate": ed,
+      "startDate": sd
+    })
+    headers = {
+      'Content-Type': 'application/json'
+    }
+
+    response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code == 200:
+
+        df = pd.json_normalize(response.json()['items'])
+
+        df['date'] = pd.to_datetime(df['date'])
+
+        return df
+    else:
+        return response.text
+  
+
+
```

### Comparing `seffaflik2-0.0.1/seffaflik2.egg-info/PKG-INFO` & `seffaflik2-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seffaflik2
-Version: 0.0.1
+Version: 0.0.2
 Summary: EPIAS Transparency Platform 2.0 Unofficial Python Library
 Home-page: https://github.com/berkomeratay/seffaflik2
 Author: Berk Ömer Atay
 Author-email: <berkomeratay@gmail.com>
 Keywords: python,epias,seffaflik,epias transparency platform,transparency,epiaş şeffaflık platformu
 Description-Content-Type: text/markdown
 
@@ -18,43 +18,63 @@
 
 Data input formats should be such as: "YYYY-MM-DD". An example would be : "2024-05-29"
 
 All the functions returns a pandas dataframe.
 
 ## Currently few selected datasets are available, which are:
 
-
+### Day-ahead-market
 epias_mcp(start_date,end_date): Function that returns the MCP for a given interval
 
+epias_pi_offer(start_date,end_date):  Function that turns the amount of price independent offers in day-ahead-market for a given interval
+
+epias_pi_bid(start_date,end_date):  Function that turns the amount of price independent bids in day-ahead-market for a given interval
+
+epias_spot(start_date,end_date): Function that turns the amount of matched amount in day-ahead-market for a given interval
+
+epias_ba(start_date,end_date):  Function that turns the amount of block offers (matched and non-matched) of day-ahead-market for a given interval
+
+### Generation
+
 epias_kgup(start_date,end_date): Function that returns the DPP's (KGUP) based on resources for a given interval
 
 epias_plant_kgup(start_date,end_date,pl_id,o_id): Function that returns the DPP's (KGUP) based on resources for a given interval (org_id: Organization ID, pl_id: Plant ID) Organization IDs can be obtained via epias_org function Plant IDs can be obtained via  epias_uevcb function
 
 epias_org(start_date,end_date): Function that returns the organizations for a given interval
 
 epias_uevcb(start_date,end_date,o_id): Function that returns the UEVCB data for a given interval (o_id: Organization ID)
 
+### Consumption
+
 epias_demand(start_date,end_date): Function that returns the real time electricity consumption for a given interval
 
-epias_idmp(start_date,end_date): Function that returns the intraday markey prices for a given interval
+### Intraday market
+
+epias_idmp(start_date,end_date): Function that returns the intraday weighted average prices for a given interval
 
 epias_idma(start_date,end_date): Function that returns the trade amount at intraday market for a given interval 
 
+### Balancing Power Market
+
 epias_smp(start_date,end_date): Function that returns the System Marginal Price for a given interval 
 
 epias_yal(start_date,end_date): Function that returns the amount of load orders (YAL) for a given interval 
 
 epias_yat(start_date,end_date): Function that returns the amount of deload orders (YAT) for a given interval
 
+### Ancillary Services
+
 epias_sfc(start_date,end_date): Function that returns the SFC prices for a given interval
 
 epias_pfc(start_date,end_date): Function that returns the PFC prices for a given interval
 
 
 
+
+
 #### Example 1
 ```python
 from seffaflik2 import epias_mcp
 
 day_ahead_prices = epias_mcp("2024-01-15","2024-03-16")
 
 print(day_ahead_prices)
```

### Comparing `seffaflik2-0.0.1/setup.py` & `seffaflik2-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 S_DESCRIPTION = 'EPIAS Transparency Platform 2.0 Unofficial Python Library'
 
 # Setting up
 setup(
     name="seffaflik2",
     version=VERSION,
     author="Berk Ömer Atay",
```

