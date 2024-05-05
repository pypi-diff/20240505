# Comparing `tmp/Buke_autoTrade_Pypi-4.3.2.tar.gz` & `tmp/Buke_autoTrade_Pypi-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.3.2.tar", last modified: Sun May  5 13:26:06 2024, max compression
+gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.3.3.tar", last modified: Sun May  5 16:04:55 2024, max compression
```

## Comparing `Buke_autoTrade_Pypi-4.3.2.tar` & `Buke_autoTrade_Pypi-4.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/
-drwxrwxrwx   0        0        0        0 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/
--rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
--rw-rw-rw-   0        0        0     8994 2024-05-05 13:26:00.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
--rw-rw-rw-   0        0        0    14806 2024-05-05 12:38:01.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
--rw-rw-rw-   0        0        0     9074 2024-05-05 13:26:00.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
--rw-rw-rw-   0        0        0    15443 2024-05-05 12:52:28.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
--rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_day_price.py
--rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_kosdaq_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_trading_days.py
--rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_trval_data.py
--rw-rw-rw-   0        0        0    66421 2024-05-05 12:31:29.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/parameter.py
--rw-rw-rw-   0        0        0     4686 2024-05-05 06:51:28.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.3.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 13:26:05.000000 Buke_autoTrade_Pypi-4.3.2/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-05-05 13:26:00.000000 Buke_autoTrade_Pypi-4.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:04:55.000000 Buke_autoTrade_Pypi-4.3.3/
+drwxrwxrwx   0        0        0        0 2024-05-05 16:04:55.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/
+-rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
+-rw-rw-rw-   0        0        0     8994 2024-05-05 13:26:00.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
+-rw-rw-rw-   0        0        0    14806 2024-05-05 12:38:01.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
+-rw-rw-rw-   0        0        0     9074 2024-05-05 13:26:00.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
+-rw-rw-rw-   0        0        0    15438 2024-05-05 16:04:31.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
+-rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_day_price.py
+-rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_kosdaq_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_trading_days.py
+-rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_trval_data.py
+-rw-rw-rw-   0        0        0    66421 2024-05-05 12:31:29.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/parameter.py
+-rw-rw-rw-   0        0        0     4686 2024-05-05 06:51:28.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:04:55.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-05 16:04:54.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 16:04:54.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2024-05-05 16:04:54.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 16:04:54.000000 Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 16:04:55.000000 Buke_autoTrade_Pypi-4.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 16:04:55.000000 Buke_autoTrade_Pypi-4.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-05-05 16:04:52.000000 Buke_autoTrade_Pypi-4.3.3/setup.py
```

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S002_buy_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S002_sell_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S004_buy_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S004_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S004_sell_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_S005_buy_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_S005_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     # 4. 매수 조건 및 우선순위 생성
     day_price, index_day_price = add_indicator(day_price, index_day_price)
     print(f"Finished data preprocessing...")
     # print(day_price[['#final_result','#priority','market_timing']])
     # print(day_price.tail())
 
     # 5. 백테스트
-    for i, day in enumerate(trading_days_list[:-2]):
+    for i, day in enumerate(trading_days_list):
 
         if i > 1:
             # 당일 코스피, 코스닥 구성 종목 내역 가져오기
             kospi_ticker_list = kospi_history['종목리스트'].loc[day].split(',')
             kosdaq_ticker_list = kosdaq_history['종목리스트'].loc[day].split(',')
 
             # Market Timing
```

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/function.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/function.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_day_price.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_index_day_price.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_kosdaq_price.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_kosdaq_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_stock_list.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_trading_days.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/generate_trval_data.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/generate_trval_data.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/indicator.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/indicator.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/parameter.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/parameter.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi/tools.py` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi/tools.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/Buke_autoTrade_Pypi.egg-info/SOURCES.txt` & `Buke_autoTrade_Pypi-4.3.3/Buke_autoTrade_Pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.3.2/setup.py` & `Buke_autoTrade_Pypi-4.3.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(name='Buke_autoTrade_Pypi', # 패키지 명
 
-version='4.3.2',
+version='4.3.3',
 
 description='Test Package',
 
 author='zaza011',
 
 author_email='yesben@naver.com',
```

