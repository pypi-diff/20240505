# Comparing `tmp/Buke_autoTrade_Pypi-4.4.4.tar.gz` & `tmp/Buke_autoTrade_Pypi-4.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.4.4.tar", last modified: Sun May  5 17:25:17 2024, max compression
+gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.4.5.tar", last modified: Sun May  5 17:29:55 2024, max compression
```

## Comparing `Buke_autoTrade_Pypi-4.4.4.tar` & `Buke_autoTrade_Pypi-4.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/
-drwxrwxrwx   0        0        0        0 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/
--rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
--rw-rw-rw-   0        0        0     8996 2024-05-05 16:53:49.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
--rw-rw-rw-   0        0        0    14807 2024-05-05 16:15:04.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
--rw-rw-rw-   0        0        0     9066 2024-05-05 17:25:12.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
--rw-rw-rw-   0        0        0    15439 2024-05-05 16:15:04.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
--rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_day_price.py
--rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_kosdaq_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_trading_days.py
--rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_trval_data.py
--rw-rw-rw-   0        0        0    66423 2024-05-05 16:40:58.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/parameter.py
--rw-rw-rw-   0        0        0     4686 2024-05-05 06:51:28.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1001 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.4.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 17:25:17.000000 Buke_autoTrade_Pypi-4.4.4/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-05-05 17:25:12.000000 Buke_autoTrade_Pypi-4.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/
+drwxrwxrwx   0        0        0        0 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/
+-rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
+-rw-rw-rw-   0        0        0     8821 2024-05-05 17:29:52.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
+-rw-rw-rw-   0        0        0    14807 2024-05-05 16:15:04.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
+-rw-rw-rw-   0        0        0     9089 2024-05-05 17:29:52.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
+-rw-rw-rw-   0        0        0    15439 2024-05-05 16:15:04.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
+-rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_day_price.py
+-rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_kosdaq_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_trading_days.py
+-rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_trval_data.py
+-rw-rw-rw-   0        0        0    66423 2024-05-05 16:40:58.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/parameter.py
+-rw-rw-rw-   0        0        0     4686 2024-05-05 06:51:28.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.4.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 17:29:55.000000 Buke_autoTrade_Pypi-4.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-05-05 17:29:52.000000 Buke_autoTrade_Pypi-4.4.5/setup.py
```

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S002_buy_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S002_sell_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S004_buy_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S004_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S004_sell_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_S005_buy_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_S005_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,18 +121,16 @@
         day_price_dict[key] = group
 
     # Market Timing
     index_day_price['이평선_3'] = sma(index_day_price['종가'], 3)
     index_day_price['이평선_5'] = sma(index_day_price['종가'], 5)
     index_day_price['이평선_10'] = sma(index_day_price['종가'], 10)
 
-    index_day_price['#market_timing'] = ((index_day_price['종가'] > index_day_price['이평선_3'])  | \
-                                         (index_day_price['종가'] > index_day_price['이평선_5'])  | \
-                                         (index_day_price['종가'] > index_day_price['이평선_10']))& \
-                                         (index_day_price['종가'] > 0.)
+    index_day_price['#market_timing'] = (index_day_price['종가'] > index_day_price[['이평선_3', '이평선_5', '이평선_10']].min(axis=1))& \
+                                        (index_day_price['종가'] > 0.)
 
     index_day_price = index_day_price.set_index('날짜')
 
     return day_price_dict, index_day_price
 
 
 def Buke_ST001_buy_list(dir, day):
```

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
             pre_buy_list.append(ticker_data)
         # except:
         #     continue
 
     pre_buy_list.sort(reverse=True)
 
     pre_buy_list = pre_buy_list[:10]
+    print(pre_buy_list)
 
     basket = {'종목코드': [],'종목명':[], '매수가격1': []}
 
     for priority_value, ticker in pre_buy_list:
 
         # try:
         yesterday_low = int(day_price[ticker]['저가'].loc[trading_days_list[-1]])
@@ -216,15 +217,14 @@
 
         if ticker in kospi_ticker_list:
             buy_price1 = get_ask_price(yesterday_mid * 0.98, Market.kospi, day)
 
         else:
             buy_price1 = get_ask_price(yesterday_mid * 0.98, Market.kosdaq, day)
 
-
         basket['종목코드'].append(ticker)
         basket['종목명'].append(ticker_name)
         basket['매수가격1'].append(f"{buy_price1}원")
 
         print(ticker_name, buy_price1)
 
         # except:
```

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/function.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/function.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_day_price.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_index_day_price.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_kosdaq_price.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_kosdaq_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_stock_list.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_trading_days.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/generate_trval_data.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/generate_trval_data.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/indicator.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/indicator.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/parameter.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/parameter.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi/tools.py` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi/tools.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/Buke_autoTrade_Pypi.egg-info/SOURCES.txt` & `Buke_autoTrade_Pypi-4.4.5/Buke_autoTrade_Pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.4.4/setup.py` & `Buke_autoTrade_Pypi-4.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(name='Buke_autoTrade_Pypi', # 패키지 명
 
-version='4.4.4',
+version='4.4.5',
 
 description='Test Package',
 
 author='zaza011',
 
 author_email='yesben@naver.com',
```

