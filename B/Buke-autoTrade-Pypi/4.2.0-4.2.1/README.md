# Comparing `tmp/Buke_autoTrade_Pypi-4.2.0.tar.gz` & `tmp/Buke_autoTrade_Pypi-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.2.0.tar", last modified: Thu Feb 29 14:09:31 2024, max compression
+gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.2.1.tar", last modified: Sun May  5 02:29:17 2024, max compression
```

## Comparing `Buke_autoTrade_Pypi-4.2.0.tar` & `Buke_autoTrade_Pypi-4.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/
-drwxrwxrwx   0        0        0        0 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/
--rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
--rw-rw-rw-   0        0        0     8984 2024-02-29 14:05:40.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
--rw-rw-rw-   0        0        0    16895 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
--rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_day_price.py
--rw-rw-rw-   0        0        0     4165 2023-03-19 08:06:52.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_kosdaq_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_trading_days.py
--rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_trval_data.py
--rw-rw-rw-   0        0        0    66073 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/parameter.py
--rw-rw-rw-   0        0        0     4119 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/
--rw-rw-rw-   0        0        0        1 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       20 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      244 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-29 14:09:31.000000 Buke_autoTrade_Pypi-4.2.0/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-02-29 14:09:19.000000 Buke_autoTrade_Pypi-4.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/
+-rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
+-rw-rw-rw-   0        0        0     8984 2024-02-29 14:05:40.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
+-rw-rw-rw-   0        0        0    16895 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
+-rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_day_price.py
+-rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_kosdaq_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trading_days.py
+-rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trval_data.py
+-rw-rw-rw-   0        0        0    66073 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/parameter.py
+-rw-rw-rw-   0        0        0     4119 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-05-05 02:28:59.000000 Buke_autoTrade_Pypi-4.2.1/setup.py
```

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S002_buy_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S002_sell_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S004_buy_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S004_sell_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_S005_buy_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S005_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/function.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/function.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_day_price.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_index_day_price.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_index_day_price.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 def generate_index_day_price(dir, day):
 
     # VIX 지수
     df = yf.download('^VIX')
     df = df.reset_index()
 
     df['날짜'] = df['Date']
+    df['날짜'] = df['날짜'].apply(lambda x: str_to_date(str(x)[:10]))
     df['시가'] = round(df['Open'], 3)
     df['고가'] = round(df['High'], 3)
     df['저가'] = round(df['Low'], 3)
     df['종가'] = round(df['Close'], 3)
     df['거래량'] = round(df['Volume'], 3)
 
     df = df[['날짜', '시가', '고가', '저가', '종가', '거래량']]
@@ -102,14 +103,15 @@
     print("VIX 지수 수집완료")
 
 # MSCI 한국 ETF
     df = yf.download('EWY')
     df = df.reset_index()
 
     df['날짜'] = df['Date']
+    df['날짜'] = df['날짜'].apply(lambda x: str_to_date(str(x)[:10]))
     df['시가'] = round(df['Open'], 3)
     df['고가'] = round(df['High'], 3)
     df['저가'] = round(df['Low'], 3)
     df['종가'] = round(df['Close'], 3)
     df['거래량'] = round(df['Volume'], 3)
 
     df = df[['날짜', '시가', '고가', '저가', '종가', '거래량']]
```

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_kosdaq_price.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_kosdaq_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_stock_list.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_trading_days.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/generate_trval_data.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trval_data.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/indicator.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/indicator.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/parameter.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/parameter.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi/tools.py` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/tools.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/Buke_autoTrade_Pypi.egg-info/SOURCES.txt` & `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.0/setup.py` & `Buke_autoTrade_Pypi-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(name='Buke_autoTrade_Pypi', # 패키지 명
 
-version='4.2.0',
+version='4.2.1',
 
 description='Test Package',
 
 author='zaza011',
 
 author_email='yesben@naver.com',
```

