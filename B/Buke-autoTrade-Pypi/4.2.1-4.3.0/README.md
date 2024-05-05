# Comparing `tmp/Buke_autoTrade_Pypi-4.2.1.tar.gz` & `tmp/Buke_autoTrade_Pypi-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.2.1.tar", last modified: Sun May  5 02:29:17 2024, max compression
+gzip compressed data, was "dist\Buke_autoTrade_Pypi-4.3.0.tar", last modified: Sun May  5 12:43:37 2024, max compression
```

## Comparing `Buke_autoTrade_Pypi-4.2.1.tar` & `Buke_autoTrade_Pypi-4.3.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/
-drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/
--rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
--rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
--rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
--rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
--rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
--rw-rw-rw-   0        0        0     8984 2024-02-29 14:05:40.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
--rw-rw-rw-   0        0        0    16895 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
--rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/function.py
--rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_day_price.py
--rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_index_day_price.py
--rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_kosdaq_price.py
--rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_stock_list.py
--rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trading_days.py
--rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trval_data.py
--rw-rw-rw-   0        0        0    66073 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/indicator.py
--rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/parameter.py
--rw-rw-rw-   0        0        0     4119 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/tools.py
--rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      914 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       20 2024-05-05 02:29:16.000000 Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      244 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 02:29:17.000000 Buke_autoTrade_Pypi-4.2.1/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-05-05 02:28:59.000000 Buke_autoTrade_Pypi-4.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/
+-rw-rw-rw-   0        0        0     8973 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S002_buy_list.py
+-rw-rw-rw-   0        0        0    17423 2024-01-07 13:14:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S002_sell_list.py
+-rw-rw-rw-   0        0        0     8992 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S004_buy_list.py
+-rw-rw-rw-   0        0        0    17309 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S004_sell_list.py
+-rw-rw-rw-   0        0        0     8952 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S005_buy_list.py
+-rw-rw-rw-   0        0        0     8984 2024-02-29 14:05:40.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
+-rw-rw-rw-   0        0        0    14806 2024-05-05 12:38:01.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
+-rw-rw-rw-   0        0        0     9064 2024-05-05 12:38:01.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
+-rw-rw-rw-   0        0        0    15443 2024-05-05 12:43:03.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
+-rw-rw-rw-   0        0        0    21696 2024-01-07 07:26:50.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/function.py
+-rw-rw-rw-   0        0        0     8943 2023-03-19 08:20:07.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_day_price.py
+-rw-rw-rw-   0        0        0     4315 2024-05-05 02:22:28.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_index_day_price.py
+-rw-rw-rw-   0        0        0     2951 2023-08-13 15:23:52.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_kosdaq_price.py
+-rw-rw-rw-   0        0        0     2307 2023-03-19 08:27:27.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_stock_list.py
+-rw-rw-rw-   0        0        0     2481 2023-03-19 07:22:24.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_trading_days.py
+-rw-rw-rw-   0        0        0     3156 2024-01-07 12:09:14.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_trval_data.py
+-rw-rw-rw-   0        0        0    66421 2024-05-05 12:31:29.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/indicator.py
+-rw-rw-rw-   0        0        0      561 2021-08-12 12:11:28.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/parameter.py
+-rw-rw-rw-   0        0        0     4686 2024-05-05 06:51:28.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/tools.py
+-rw-rw-rw-   0        0        0        0 2023-03-19 07:24:19.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       20 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      244 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-01-07 07:30:34.000000 Buke_autoTrade_Pypi-4.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 12:43:37.000000 Buke_autoTrade_Pypi-4.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-05-05 12:40:02.000000 Buke_autoTrade_Pypi-4.3.0/setup.py
```

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_buy_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S002_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S002_sell_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S002_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_buy_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S004_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S004_sell_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S004_sell_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_S005_buy_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_S005_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST001_buy_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/Buke_ST001_sell_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,38 +138,34 @@
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
 
 
-
 def back_testing(dir, start_date, end_date):
 
     # 0. 변수
     max_basket_size = 10
     liquidation_holding_days = 1
     close_holding_days = 2
     cut_period = 0
     seed_money = 10000000
     fee = 0.00015  # when using kiwoom
     basket = {}  # key:ticker, value:buy_price, stock_num, holding_days
     pnl = {'date': [start_date], 'balance': [seed_money]}
     p_len = []
 
-
     # 1. 거래일 가져오기
     trading_days_list = read_trading_days(dir, start_date, end_date)
 
     # 2. 일봉 가져오기
     day_price = read_day_price(dir, start_date, end_date)
 
     index_day_price = read_index_day_price(dir, start_date, end_date)
@@ -179,189 +175,151 @@
 
     # 4. 매수 조건 및 우선순위 생성
     day_price, index_day_price = add_indicator(day_price, index_day_price)
     print(f"Finished data preprocessing...")
     # print(day_price[['#final_result','#priority','market_timing']])
     # print(day_price.tail())
 
-
     # 5. 백테스트
     for i, day in enumerate(trading_days_list):
 
-        # if i > 1:
-        # 당일 코스피, 코스닥 구성 종목 내역 가져오기
-        kospi_ticker_list = kospi_history['종목리스트'].loc[day].split(',')
-        kosdaq_ticker_list = kosdaq_history['종목리스트'].loc[day].split(',')
-
-        # Market Timing
-        buy_check = 1
-        try:
-            yesterday_market_time = bool(index_day_price['#market_timing'].loc[trading_days_list[i - 1]])
-        except:
-            buy_check = 0
-
-            # 매수
-        if len(basket) < max_basket_size and buy_check == 1:
-            # buy at open price
-            pre_buy_list = []
-            for ticker in kospi_ticker_list + kosdaq_ticker_list:
-
-                if ticker in basket:
-                    continue
-                try:
-                    yesterday_buy_condition = bool(
-                        day_price[ticker]['#final_result'].loc[trading_days_list[i - 1]])
-
-                    # Market Time
-
-                    if yesterday_market_time and yesterday_buy_condition :
-                        priority_value = float(day_price[ticker]['#priority'].loc[trading_days_list[i - 1]])
-                        ticker_data = (priority_value, ticker)
-                        pre_buy_list.append(ticker_data)
-                except:
-                    pass
-
-            if len(pre_buy_list) > 0:
-                p_len.append(len(pre_buy_list))
-                pre_buy_list.sort(reverse=True)
-                # print(f"{day}, {pre_buy_list}")
-                for priority_value, ticker in pre_buy_list[:max_basket_size - len(basket)]:
+        if i > 1:
+            # 당일 코스피, 코스닥 구성 종목 내역 가져오기
+            kospi_ticker_list = kospi_history['종목리스트'].loc[day].split(',')
+            kosdaq_ticker_list = kosdaq_history['종목리스트'].loc[day].split(',')
+
+            # Market Timing
+            buy_check = 1
+            try:
+                yesterday_market_time = bool(index_day_price['#market_timing'].loc[trading_days_list[i - 1]])
+            except:
+                buy_check = 0
+
+                # 매수
+            if len(basket) < max_basket_size and buy_check == 1:
+                # buy at open price
+                pre_buy_list = []
+                for ticker in kospi_ticker_list + kosdaq_ticker_list:
 
-                    yesterday_low = int(day_price[ticker]['저가'].loc[trading_days_list[i - 1]])
-                    tomorrow_pivot_standard_price = float(day_price[ticker]['pivot_기준선_for_sell'].loc[day])
+                    if ticker in basket:
+                        continue
+                    try:
+                        yesterday_buy_condition = bool(
+                            day_price[ticker]['#final_result'].loc[trading_days_list[i - 1]])
+
+                        # Market Time
+
+                        if yesterday_market_time and yesterday_buy_condition:
+                            priority_value = float(day_price[ticker]['#priority'].loc[trading_days_list[i - 1]])
+                            ticker_data = (priority_value, ticker)
+                            pre_buy_list.append(ticker_data)
+                    except:
+                        continue
 
-                    # yesterday_close = int(day_price[ticker]['close'].loc[trading_days_list[i - 1]])
+                if len(pre_buy_list) > 0:
+                    p_len.append(len(pre_buy_list))
+                    pre_buy_list.sort(reverse=True)
+
+                    for priority_value, ticker in pre_buy_list[:max_basket_size - len(basket)]:
+
+                        yesterday_low = int(day_price[ticker]['저가'].loc[trading_days_list[i - 1]])
+                        yesterday_close = int(day_price[ticker]['종가'].loc[trading_days_list[i - 1]])
+                        yesterday_mid = (yesterday_low + yesterday_close) / 2
 
-                    if ticker in kospi_ticker_list:
-                        today_target_buy_price = get_ask_price(yesterday_low * 0.98, Market.kospi)
+                        if ticker in kospi_ticker_list:
+                            today_target_buy_price = get_ask_price(yesterday_mid * 0.98, Market.kospi, day)
 
-                    else:
-                        today_target_buy_price = get_ask_price(yesterday_low * 0.98, Market.kosdaq)
+                        else:
+                            today_target_buy_price = get_ask_price(yesterday_mid * 0.98, Market.kosdaq, day)
 
+                        today_open = int(day_price[ticker]['시가'].loc[day])
+                        today_low = int(day_price[ticker]['저가'].loc[day])
+                        today_name = day_price[ticker]['종목명'].loc[day]
 
-                    today_open = int(day_price[ticker]['시가'].loc[day])
-                    today_low = int(day_price[ticker]['저가'].loc[day])
-                    today_name = day_price[ticker]['종목명'].loc[day]
+                        real_buy_price = 0.
 
-                    real_buy_price = 0.
+                        if today_open <= today_target_buy_price:
+                            buy_price = math.ceil(today_open * (1 + fee))
+                            real_buy_price = today_open
 
-                    if today_open <= today_target_buy_price:
-                        buy_price = math.ceil(today_open * (1 + fee))
-                        real_buy_price = today_open
+                        elif today_low < today_target_buy_price:
+                            buy_price = math.ceil(today_target_buy_price * (1 + fee))
+                            real_buy_price = today_target_buy_price
+                        else:
+                            continue
 
-                    elif today_low < today_target_buy_price:
-                        buy_price = math.ceil(today_target_buy_price * (1 + fee))
-                        real_buy_price = today_target_buy_price
-                    else:
-                        continue
+                        if ticker in kospi_ticker_list:
+                            sell_price = get_ask_price(buy_price * 1.05, Market.kospi, day)
 
-                    if ticker in kospi_ticker_list:
-                        sell_price = get_ask_price(real_buy_price * 1.05, Market.kospi)
+                        else:
+                            sell_price = get_ask_price(buy_price * 1.05, Market.kosdaq, day)
 
-                    else:
-                        sell_price = get_ask_price(real_buy_price * 1.05, Market.kosdaq)
+                        stock_num = (pnl['balance'][-1] // max_basket_size) // buy_price
+                        stock_info = {'stock_num': stock_num, 'buy_price': buy_price, 'holding_days': 0,
+                                      'name': today_name, 'buy_date': day, 'real_buy_price': real_buy_price,
+                                      'sell_price': sell_price}
 
-                    stock_num = (pnl['balance'][-1] // max_basket_size) // buy_price
-                    stock_info = {'stock_num': stock_num, 'buy_price': buy_price, 'holding_days': 0, 'name':today_name, 'buy_date':day, 'real_buy_price':real_buy_price, 'sell_price':sell_price}
+                        basket[ticker] = stock_info
 
-                    basket[ticker] = stock_info
-                    #print(f"<Buy> date: {day}, ticker: {ticker}, buy_price: {buy_price}")
+            # 매도
+            today_profit = 0
+            if len(basket) > 0:
+                tax = get_stock_exchange_tax(day)
 
-        # 매도
-        today_profit = 0
-        if len(basket) > 0:
-            tax = get_stock_exchange_tax(day)
+                sell_list = []
+                for ticker in basket:
 
-            sell_list = []
-            for ticker in basket:
+                    holding_condition1 = basket[ticker]['holding_days'] >= liquidation_holding_days
 
-                holding_condition1 = basket[ticker]['holding_days'] >= liquidation_holding_days
+                    if holding_condition1:
 
-                if holding_condition1:
+                        try:
 
-                    yesterday_close = int(day_price[ticker]['종가'].loc[trading_days_list[i - 1]])
-                    today_open = int(day_price[ticker]['시가'].loc[day])
-                    today_high = int(day_price[ticker]['고가'].loc[day])
-                    today_close = int(day_price[ticker]['종가'].loc[day])
+                            today_open = int(day_price[ticker]['시가'].loc[day])
+                            today_high = int(day_price[ticker]['고가'].loc[day])
 
-                    pivot_standard_price = float(day_price[ticker]['pivot_기준선'].loc[day])
-                    tomorrow_pivot_standard_price = float(day_price[ticker]['pivot_기준선_for_sell'].loc[day])
+                            tomorrow_pivot_standard_price = float(day_price[ticker]['pivot_기준선_for_sell'].loc[day])
+                            target_sell_price = float(basket[ticker]['sell_price'])
 
-                    buy_date = basket[ticker]['buy_date']
-                    sell_date = day
-                    name = basket[ticker]['name']
-                    sell_price = int(basket[ticker]['sell_price'])
-                    real_buy_price = int(basket[ticker]['real_buy_price'])
+                            if ticker in kospi_ticker_list:
+                                tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
+                                                                           Market.kospi, day)
+                            else:
+                                tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
+                                                                           Market.kosdaq, day)
 
-                    # 익일 상폐 여부 확인
-                    # trash_condition = ticker not in tomorrow_kospi_ticker_list + tomorrow_kosdaq_ticker_list
+                            basket[ticker]['sell_price'] = tomorrow_target_sell_price
 
-                    if basket[ticker]['holding_days'] < close_holding_days:
+                            if today_open >= target_sell_price:
+                                sell_price = today_open
+                            elif today_high > target_sell_price:
+                                sell_price = target_sell_price
+                            else:
+                                basket[ticker]['holding_days'] += 1
+                                continue
 
-                        target_sell_price = sell_price
+                            profit = basket[ticker]['stock_num'] * (
+                                    math.floor(sell_price * (1 - (tax + fee))) - float(basket[ticker]['buy_price']))
+                            today_profit += profit
 
-                        if ticker in kospi_ticker_list:
-                            tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
-                                                              Market.kospi)
-                        else:
-                            tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
-                                                              Market.kosdaq)
-                        basket[ticker]['sell_price'] = tomorrow_target_sell_price
-
-                        if today_open >= target_sell_price:
-                            sell_price = today_open
-                        elif today_high > target_sell_price:
-                            sell_price = target_sell_price
-                        else:
+                            sell_list.append(ticker)
+
+                        except:
                             basket[ticker]['holding_days'] += 1
                             continue
 
                     else:
+                        basket[ticker]['holding_days'] += 1
+                for ticker in sell_list:
+                    basket.pop(ticker)
+
+            # Balance Update
+            pnl['date'].append(day)
+            pnl['balance'].append(pnl['balance'][-1] + today_profit)
 
-                        if ticker in kospi_ticker_list:
-                            target_sell_price = get_bid_price(pivot_standard_price * 1.01,
-                                                              Market.kospi)
-                            tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
-                                                                       Market.kospi)
-                        else:
-                            target_sell_price = get_bid_price(pivot_standard_price * 1.01,
-                                                              Market.kosdaq)
-                            tomorrow_target_sell_price = get_bid_price(tomorrow_pivot_standard_price * 1.01,
-                                                                       Market.kosdaq)
-
-                        basket[ticker]['sell_price'] = tomorrow_target_sell_price
-
-                        if today_open >= target_sell_price:
-                            sell_price = today_open
-                        elif today_high > target_sell_price:
-                            sell_price = target_sell_price
-                        else:
-                            basket[ticker]['holding_days'] += 1
-                            continue
-
-                    profit = basket[ticker]['stock_num'] * (
-                            math.floor(sell_price * (1 - (tax + fee))) - basket[ticker]['buy_price'])
-                    today_profit += profit
-
-                    profit = basket[ticker]['stock_num'] * (
-                            math.floor(sell_price * (1 - (tax + fee))) - basket[ticker]['buy_price'])
-                    today_profit += profit
-
-                    #print(f"<Sell> date: {day}, ticker: {ticker}, sell_price: {sell_price}, profit: {profit}")
-                    sell_list.append(ticker)
-
-                else:
-                    basket[ticker]['holding_days'] += 1
-            for ticker in sell_list:
-                basket.pop(ticker)
-
-
-        # Balance Update
-        pnl['date'].append(day)
-        pnl['balance'].append(pnl['balance'][-1] + today_profit)
 
     return basket
 
 
 def Buke_ST001_sell_list(dir, today):
```

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/function.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/function.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_day_price.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_index_day_price.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_index_day_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_kosdaq_price.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_kosdaq_price.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_stock_list.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_stock_list.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trading_days.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_trading_days.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/generate_trval_data.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/generate_trval_data.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/indicator.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/indicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1327,7 +1327,17 @@
         trn = ema(tr, period)
     elif moving_average == MovingAverage.ewma:
         trn = ewma(tr, period)
     elif moving_average == MovingAverage.wma:
         trn = wma(tr, period)
 
     return pdmn.divide(trn)
+
+
+def RSI(price: Series, period: int):
+    U = np.where(price.diff(1) > 0, price.diff(1), 0)
+    D = np.where(price.diff(1) < 0, price.diff(1) * (-1), 0)
+
+    AU = DataFrame(U).rolling(window=period, min_periods=period).mean()
+    AD = DataFrame(D).rolling(window=period, min_periods=period).mean()
+    RSI = AU.div(AD + AU)
+    return RSI
```

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/parameter.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/parameter.py`

 * *Files identical despite different names*

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi/tools.py` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,94 +4,102 @@
 from Buke_autoTrade_Pypi.parameter import Market
 
 
 def year_to_date(year: int):
     return date(year=year, month=1, day=1)
 
 
-def get_hoga(price: int, market: Market) -> int:
+def get_hoga(price: int or float, market: Market, day: date) -> int:
     """
     주가에 따른 1호가 가격을 구하는 함수
     :param price: 주가
     :param market: kospi / kosdaq
     :return: 1호가 가격
     """
+    if day < date(2023,1,25):
 
-    """ 
-    if market == Market.kospi:
-        if price >= 500000:
-            hoga = 1000
-        elif price >= 100000:
-            hoga = 500
-        elif price >= 50000:
-            hoga = 100
-        elif price >= 10000:
-            hoga = 50
-        elif price >= 5000:
-            hoga = 10
-        elif price >= 1000:
-            hoga = 5
-        else:
-            hoga = 1
+        if market == Market.kospi:
+            if price >= 500000:
+                hoga = 1000
+            elif price >= 100000:
+                hoga = 500
+            elif price >= 50000:
+                hoga = 100
+            elif price >= 10000:
+                hoga = 50
+            elif price >= 5000:
+                hoga = 10
+            elif price >= 1000:
+                hoga = 5
+            else:
+                hoga = 1
+
+        elif market == Market.kosdaq:
+            if price >= 50000:
+                hoga = 100
+            elif price >= 10000:
+                hoga = 50
+            elif price >= 5000:
+                hoga = 10
+            elif price >= 1000:
+                hoga = 5
+            else:
+                hoga = 1
 
-    elif market == Market.kosdaq:
-        if price >= 50000:
-            hoga = 100
-        elif price >= 10000:
-            hoga = 50
-        elif price >= 5000:
-            hoga = 10
-        elif price >= 1000:
+        elif market == Market.etf:
             hoga = 5
         else:
-            hoga = 1
-    """
+            raise ValueError("market should be kospi or kosdaq")
+
+    else :
+
+        if market == Market.kospi or market == Market.kosdaq:
+            if price >= 500000:
+                hoga = 1000
+            elif price >= 200000:
+                hoga = 500
+            elif price >= 50000:
+                hoga = 100
+            elif price >= 20000:
+                hoga = 50
+            elif price >= 5000:
+                hoga = 10
+            elif price >= 2000:
+                hoga = 5
+            else:
+                hoga = 1
 
-    if market == Market.kospi or market == Market.kosdaq:
-        if price >= 500000:
-            hoga = 1000
-        elif price >= 200000:
-            hoga = 500
-        elif price >= 50000:
-            hoga = 100
-        elif price >= 20000:
-            hoga = 50
-        elif price >= 5000:
-            hoga = 10
-        elif price >= 2000:
+        elif market == Market.etf:
             hoga = 5
-        else:
-            hoga = 1
 
-    elif market == Market.etf:
-        hoga = 5
-    else:
-        raise ValueError("market should be kospi or kosdaq")
+        else:
+            raise ValueError("market should be kospi or kosdaq")
 
     return hoga
 
-def get_bid_price(price: int or float, market: Market) -> int:
+
+def get_bid_price(price: int or float, market: Market, day: date) -> int:
     """
     살 가격을 구하는 함수
     :param price: 현재가
     :param market: 시장
     :return: 매수 가격
     """
-    hoga = get_hoga(floor(price), market)
+    hoga = get_hoga(floor(price), market, day)
     return int(price // hoga) * hoga + hoga
 
 
-def get_ask_price(price: int, market: Market) -> int:
+def get_ask_price(price: int or float, market: Market, day: date) -> int:
     """
     팔 가격을 구하는 함수
     :param price: 현재가
     :param market: 시장
     :return: 매도 가격
     """
-    hoga = get_hoga(floor(price), market)
+    hoga = get_hoga(floor(price), market, day)
     if price % hoga == 0:
         return int(price // hoga) * hoga - hoga
     else:
         return int(price // hoga) * hoga
 
 
 def get_limit_percent(today: date) -> float:
@@ -107,15 +115,15 @@
     :param yesterday_close: 전일 종가
     :param today: 당일 날짜
     :param market: kospi 또는 kosdaq
     :return: 당일 상한가
     """
     limit_percent = get_limit_percent(today)
     predict_upper_limit_price = yesterday_close * (1 + limit_percent)
-    hoga = get_hoga(floor(predict_upper_limit_price), market)
+    hoga = get_hoga(floor(predict_upper_limit_price), market, today)
     real_upper_limit_price = int(predict_upper_limit_price // hoga) * hoga
 
     return real_upper_limit_price
 
 
 def get_lower_limit_price(yesterday_close: int, today: date, market: Market) -> int:
     """
@@ -123,15 +131,15 @@
     :param yesterday_close: 전일 종가
     :param today: 당일 날짜
     :param market: kospi 또는 kosdaq
     :return: 당일 하한가
     """
     limit_percent = get_limit_percent(today)
     predict_lower_limit_price = yesterday_close * (1 - limit_percent)
-    hoga = get_hoga(floor(predict_lower_limit_price), market)
+    hoga = get_hoga(floor(predict_lower_limit_price), market, today)
     real_lower_limit_price = int(predict_lower_limit_price // hoga) * hoga + hoga
 
     return real_lower_limit_price
 
 
 def get_stock_exchange_tax(day: date):
     """
@@ -141,10 +149,14 @@
     """
     if day < date(2019, 6, 3):
         stock_exchange_tax = 0.003
     elif day < date(2021, 1, 1):
         stock_exchange_tax = 0.0025
     elif day < date(2023, 1, 1):
         stock_exchange_tax = 0.0023
+    elif day < date(2024, 1, 1):
+        stock_exchange_tax = 0.002
+    elif day < date(2025, 1, 1):
+        stock_exchange_tax = 0.0018
     else:
         stock_exchange_tax = 0.0015
     return stock_exchange_tax
```

### Comparing `Buke_autoTrade_Pypi-4.2.1/Buke_autoTrade_Pypi.egg-info/SOURCES.txt` & `Buke_autoTrade_Pypi-4.3.0/Buke_autoTrade_Pypi.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 Buke_autoTrade_Pypi/Buke_S002_buy_list.py
 Buke_autoTrade_Pypi/Buke_S002_sell_list.py
 Buke_autoTrade_Pypi/Buke_S004_buy_list.py
 Buke_autoTrade_Pypi/Buke_S004_sell_list.py
 Buke_autoTrade_Pypi/Buke_S005_buy_list.py
 Buke_autoTrade_Pypi/Buke_ST001_buy_list.py
 Buke_autoTrade_Pypi/Buke_ST001_sell_list.py
+Buke_autoTrade_Pypi/Buke_ST002_buy_list.py
+Buke_autoTrade_Pypi/Buke_ST002_sell_list.py
 Buke_autoTrade_Pypi/__init__.py
 Buke_autoTrade_Pypi/function.py
 Buke_autoTrade_Pypi/generate_day_price.py
 Buke_autoTrade_Pypi/generate_index_day_price.py
 Buke_autoTrade_Pypi/generate_kosdaq_price.py
 Buke_autoTrade_Pypi/generate_stock_list.py
 Buke_autoTrade_Pypi/generate_trading_days.py
```

### Comparing `Buke_autoTrade_Pypi-4.2.1/setup.py` & `Buke_autoTrade_Pypi-4.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(name='Buke_autoTrade_Pypi', # 패키지 명
 
-version='4.2.1',
+version='4.3.0',
 
 description='Test Package',
 
 author='zaza011',
 
 author_email='yesben@naver.com',
```

