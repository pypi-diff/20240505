# Comparing `tmp/momonga-0.1.0-py3-none-any.whl.zip` & `tmp/momonga-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15761 bytes, number of entries: 11
+Zip file size: 15832 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      135 b- defN 24-May-03 15:05 momonga/__init__.py
--rw-r--r--  2.0 unx    15714 b- defN 24-May-03 19:10 momonga/momonga.py
+-rw-r--r--  2.0 unx    15818 b- defN 24-May-05 09:52 momonga/momonga.py
 -rw-r--r--  2.0 unx      973 b- defN 24-May-03 02:36 momonga/momonga_exception.py
 -rw-r--r--  2.0 unx     2712 b- defN 24-May-03 19:01 momonga/momonga_response.py
--rw-r--r--  2.0 unx    12539 b- defN 24-May-03 19:01 momonga/momonga_session_manager.py
+-rw-r--r--  2.0 unx    12496 b- defN 24-May-05 09:32 momonga/momonga_session_manager.py
 -rw-r--r--  2.0 unx    10110 b- defN 24-May-03 19:02 momonga/momonga_sk_wrapper.py
--rw-r--r--  2.0 unx     1061 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    10439 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      884 b- defN 24-May-03 19:13 momonga-0.1.0.dist-info/RECORD
-11 files, 54667 bytes uncompressed, 14275 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-05 10:14 momonga-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10661 b- defN 24-May-05 10:14 momonga-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-05 10:14 momonga-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-05 10:14 momonga-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      884 b- defN 24-May-05 10:14 momonga-0.1.1.dist-info/RECORD
+11 files, 54950 bytes uncompressed, 14346 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.1.0.dist-info/LICENSE
+Filename: momonga-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.1.0.dist-info/METADATA
+Filename: momonga-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.1.0.dist-info/WHEEL
+Filename: momonga-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.1.0.dist-info/top_level.txt
+Filename: momonga-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.1.0.dist-info/RECORD
+Filename: momonga-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/momonga.py

```diff
@@ -236,15 +236,16 @@
                     0x0D: 10000}
         return unit_map.get(unit_index)
 
     def get_historical_cumulative_energy_1(self,
                                            day: int = 0,
                                            reverse: bool = False,
                                            ) -> list[dict[str: datetime.datetime,
-                                                          str: int | float | None]]:
+                                                          str: dict[str: int | float | None,
+                                                                    str: int | float | None]]]:
         self.__prepare_to_get_cumulative_energy()
         self.set_day_for_historical_data_1(day)
 
         if reverse is False:
             epc = 0xE2
         else:
             epc = 0xE4
```

## momonga/momonga_session_manager.py

```diff
@@ -52,33 +52,33 @@
         self.xmit_lock = threading.Lock()
         self.rejoin_lock = threading.Lock()
 
         self.pkt_sbsc_q = queue.Queue()
         self.recv_q = queue.Queue()
         self.xmit_q = queue.Queue()
 
-    #def __enter__(self) -> Self:
+    # def __enter__(self) -> Self:
     def __enter__(self):
         return self.open()
 
     def __exit__(self, type, value, traceback) -> None:
         self.close()
 
-    #def open(self) -> Self:
+    # def open(self) -> Self:
     def open(self):
         logger.info('Opening a Momonga session...')
         try:
             self.skw.open()
 
             if self.reset_dev is True:
                 # to reset the specified wi-sun module.
                 self.skw.skreset()
 
             # to disable echoback.
-            #self.sksreg('SFE', '0')
+            # self.sksreg('SFE', '0')
 
             # to show the rssi of the received packets.
             self.skw.sksreg('SA2', '1')
 
             # scanning a PAN from here.
             # to set a route b id.
             self.skw.sksetrbid(self.rbid)
@@ -209,17 +209,18 @@
                     self.unrestrict_to_xmit()
                 elif res.startswith('EVENT 27'):
                     self.restrict_to_xmit()
                     logger.debug('The PANA session has been closed successfully.')
                 elif res.startswith('EVENT 28'):  # there was no session to close.
                     self.restrict_to_xmit()
                     logger.warning('There was no PANA session to close.')
-                elif self.is_restricted_to_xmit() is False and (res.startswith("EVENT 21") or
-                                                                res.startswith("EVENT 02") or
-                                                                res.startswith("ERXUDP")):
+                elif res.startswith("EVENT 21") or res.startswith("EVENT 02"):
+                    if self.is_restricted_to_xmit() is False:
+                        self.recv_q.put(res)
+                elif res.startswith("ERXUDP"):
                     self.recv_q.put(res)
         except Exception as e:
             logger.error('An exception was raised from the receiver thread. %s: %s' % (type(e).__name__, e))
             self.receiver_exception = e
 
         logger.debug('The packet receiver has been stopped.')
```

## Comparing `momonga-0.1.0.dist-info/LICENSE` & `momonga-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.1.0.dist-info/METADATA` & `momonga-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 Home-page: https://github.com/nbtk/momonga
 Author: nbtk
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial ~=3.5
 
-[![Downloads](https://static.pepy.tech/badge/momonga)](https://pepy.tech/project/momonga)
+[![Downloads](https://static.pepy.tech/personalized-badge/momonga?period=total&units=none&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/momonga)
 
 # Momonga
 Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 
 # Description
 MomongaはBルートサービスを利用してスマートメーターと通信するライブラリです。ターゲットデバイスはROHM社製Wi-SUNモジュールBP35C2を搭載したラトックシステムRS-WSUHA-Pです。
 
@@ -167,34 +167,35 @@
 - None
 
 ## momonga.get_operation_status()
 スマートメーターの状態を取得する。
 ### Arguments
 - Void
 ### Return Value
-- bool: スマートメーターの状態 (True: オン False: オフ None: 不明)
+- bool | None: スマートメーターの状態 (True: オン False: オフ None: 不明)
 
 ## momonga.get_coefficient_for_cumulative_energy()
 積算電力量計測値、履歴を実使用量に換算する係数を取得する。Momongaが出力する結果には適宜この値が乗じられている。
 ### Arguments
 - Void
 ### Return Value
 - int: 係数
 
 ## momonga.get_number_of_effective_digits_for_cumulative_energy()
 積算電力量計測値の有効桁数を取得する。
 - Void
 ### Return Value
 - int: 有効桁数
+
 ## momonga.get_measured_cumulative_energy(reverse: bool = False)
 積算電力量計測値を取得する。
 ### Arguments
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
-- float: 積算電力量(kWh)
+- int | float: 積算電力量(kWh)
 
 ## momonga.get_unit_for_cumulative_energy()
 積算電力量計測値、履歴の乗率を取得する。Momongaが出力する結果には適宜この値が乗じられている。
 ### Arguments
 - Void
 ### Return Value
 - int | float: 積算電力量の乗率
@@ -206,15 +207,15 @@
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
 - list: 収集日時と積算電力量(kWh)
 
 e.g.
 ```python3
 [{'timestamp': datetime.datetime,
-  'cumulative energy': float}]
+  'cumulative energy': int | float | None}]
 ```
 注意: 収集日時はスマートメーター側で設定されたものではなくMomonga自身が設定しているため、実行中に日を跨ぐと収集日時に齟齬が生じる可能性がある。
 
 ## momonga.set_day_for_historical_data_1(day: int = 0)
 積算履歴収集日1を設定する。
 ### Arguments
 - day: 積算履歴収集日(0:当日、1~:前日の日数)
@@ -253,46 +254,46 @@
 ### Arguments
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
 - dict: 収集日時と積算電力量(kWh)
 
 e.g.
 ```python3
-{'datetime': datetime.datetime,
- 'cumulative energy': float}
+{'timestamp': datetime.datetime,
+ 'cumulative energy': int | float}
 ```
 
 ## momonga.get_historical_cumulative_energy_2(timestamp: datetime.datetime = None, num_of_data_points: int = 12)
 積算履歴収集日時、収集コマ数ならびに積算電力量の計測結果履歴を、正・逆 30 分毎のデータで過去最大6時間分取得する。
 ### Arguments
-- timestamp: 収集日時
+- timestamp: 収集日時 (Noneのときは現時刻)
 - num_of_data_points: 収集コマ数 1~12
 ### Return Value
 - list: 収集日時と正方向および逆方向の積算電力量(kWh)
 
 e.g.
 ```python3
 [{'timestamp': datetime.datetime,
-  'cumulative energy': {'normal direction': float,
-                        'reverse direction': float}}]
+  'cumulative energy': {'normal direction': int | float | None,
+                        'reverse direction': int | float | None}}]
 ```
 
 ## momonga.set_time_for_historical_data_2(timestamp: datetime.datetime, num_of_data_points: int = 12)
 積算履歴収集日時ならびに収集コマ数を設定する。
 ### Arguments
-- timestamp: 収集日時
+- timestamp: 収集日時 (Noneのときは現時刻)
 - num_of_data_points: 収集コマ数
 ### Return Value
 - None
 
 ## momonga.get_time_for_historical_data_2()
 積算履歴収集日時ならびに収集コマ数を取得する。
 ### Arguments
 - Void
 ### Return Value
 - dict: 収集日時と収集コマ数
 
 e.g.
 ```python3
-{'timestamp': datetime,
+{'timestamp': datetime.datetime | None,
  'number of data points': int}
 ```
```

## Comparing `momonga-0.1.0.dist-info/RECORD` & `momonga-0.1.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=DJfFmQ8oRnm69XfkH5TL0n9CXJsiqrgdO7D7D7GyLSk,135
-momonga/momonga.py,sha256=VX4bSPGHDL1-UZb_Gw3VG3THyEHcxn-r50ZX4eBx3Xg,15714
+momonga/momonga.py,sha256=Qfcl4VUDkUpl0VazsQWqKBM-m2oB2ckvV-5sAvBJ1_Q,15818
 momonga/momonga_exception.py,sha256=Cc7Jo3rjczP9-LqblFuyUq8jSjR7wjO4AXmDKjIARWw,973
 momonga/momonga_response.py,sha256=vj37u7FZUO-SAQvBSt71OLH5N6-cjLtPSIpKmDehSi8,2712
-momonga/momonga_session_manager.py,sha256=Q1yfcNnSSf7P2o6nNf7nyiNWmK8KcmpsLnaD3Oqr_fo,12539
+momonga/momonga_session_manager.py,sha256=tYJpMrkxMdDwQkhPOWT8kL0K5fNv7Qz72XQeq__Z6mo,12496
 momonga/momonga_sk_wrapper.py,sha256=S4T-DsRzEJf9ifzxKxZ86we1DjlYqVunVqGaF0G6GRw,10110
-momonga-0.1.0.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.1.0.dist-info/METADATA,sha256=oJ4aFZEzdkDnrj2qJ0yorHgk85QsI5fRR8ezcOTjbaw,10439
-momonga-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.1.0.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.1.0.dist-info/RECORD,,
+momonga-0.1.1.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.1.1.dist-info/METADATA,sha256=6raGnyYrraLCmrg9W7Rs34sdZ7FtQF3288JiPJhW9SY,10661
+momonga-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.1.1.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.1.1.dist-info/RECORD,,
```

