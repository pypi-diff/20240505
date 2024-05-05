# Comparing `tmp/lottokit-1.0.tar.gz` & `tmp/lottokit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lottokit-1.0.tar", last modified: Fri Apr 26 15:00:00 2024, max compression
+gzip compressed data, was "lottokit-1.1.tar", last modified: Sun May  5 07:35:03 2024, max compression
```

## Comparing `lottokit-1.0.tar` & `lottokit-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.737191 lottokit-1.0/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.0/LICENSE
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-26 15:00:00.737076 lottokit-1.0/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.0/README.md
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.735698 lottokit-1.0/lottokit/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.0/lottokit/__init__.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    60914 2024-04-26 14:59:00.000000 lottokit-1.0/lottokit/daletou.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    85145 2024-04-26 14:52:49.000000 lottokit-1.0/lottokit/util.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.736664 lottokit-1.0/lottokit.egg-info/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/requires.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/top_level.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.0/pyproject.toml
--rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-04-26 15:00:00.737230 lottokit-1.0/setup.cfg
--rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-04-26 14:59:00.000000 lottokit-1.0/setup.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.736793 lottokit-1.0/tests/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.0/tests/test.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756945 lottokit-1.1/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.1/LICENSE
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-05 07:35:03.756829 lottokit-1.1/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.1/README.md
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.755363 lottokit-1.1/lottokit/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.1/lottokit/__init__.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    69087 2024-05-05 07:33:47.000000 lottokit-1.1/lottokit/daletou.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    85918 2024-05-05 05:42:52.000000 lottokit-1.1/lottokit/util.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756439 lottokit-1.1/lottokit.egg-info/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/requires.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-05-05 07:35:03.000000 lottokit-1.1/lottokit.egg-info/top_level.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.1/pyproject.toml
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-05-05 07:35:03.756990 lottokit-1.1/setup.cfg
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-05-05 07:33:54.000000 lottokit-1.1/setup.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-05-05 07:35:03.756546 lottokit-1.1/tests/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.1/tests/test.py
```

### Comparing `lottokit-1.0/LICENSE` & `lottokit-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lottokit-1.0/PKG-INFO` & `lottokit-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.0
+Version: 1.1
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.0/lottokit/daletou.py` & `lottokit-1.1/lottokit/daletou.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 @Usage   :
 @FileName: daletou.py
 @DateTime: 2023/12/7 19:58
 @SoftWare:
 """
 
 import os
+import random
 import time
 import math
-from scipy.stats import randint
 from datetime import datetime, timedelta
 from itertools import combinations
 from collections import Counter, namedtuple
-from typing import List, Tuple, Any, Optional, Union, Dict, NamedTuple, Callable, Generator, Iterable
+from typing import List, Tuple, Any, Optional, Union, Dict, NamedTuple, Callable, Generator, Iterable, Set
 from selenium.webdriver.common.by import By
 from .util import IOUtil, ModelUtil, SpiderUtil, CalculateUtil, AnalyzeUtil, re, WebDriverWait, EC
 
 
 class Daletou(IOUtil, ModelUtil, SpiderUtil, CalculateUtil, AnalyzeUtil):
     # Default values for t prediction configuration
     AWARD_URL = 'https://www.lottery.gov.cn/kj/kjlb.html?dlt'
@@ -623,17 +623,17 @@
             int: The next draw day (1 for Sunday/Monday, 3 for Tuesday/Wednesday, 6 for Thursday-Saturday).
         """
         now: datetime = datetime.now()
         weekday: int = now.weekday()
         hour: int = now.hour
         minute: int = now.minute
         if (hour, minute) < (21, 30):
-            return 3 if weekday in [1, 2] else 6 if weekday in [3, 4, 5] else 1
+            return 3 if weekday in [2, 3] else 6 if weekday in [4, 5, 6] else 1
         else:
-            return 3 if weekday < 2 else 6 if weekday < 5 else 1
+            return 3 if weekday <= 2 else 6 if weekday <= 5 else 1
 
     @staticmethod
     def get_next_period() -> int:
         now = datetime.now()
         current_year = now.year
         # Determine the first day of the year
         first_day_of_year = datetime(current_year, 1, 1)
@@ -657,14 +657,146 @@
         for i in range(delta.days % 7 + 1):
             if (first_day_of_year + timedelta(days=i)).weekday() in [0, 2, 5]:
                 next_period += 1
 
         # Return the draw number of the next t for the current year
         return next_period
 
+    def get_kill_numbers(self, data: List[Any], next_period: int = None, next_weekday: int = None) -> Tuple[
+        Set[int], Set[int]]:
+        """
+        Calculate and return sets of 'kill numbers' for both front and back sequences based on provided data.
+
+        Parameters:
+            data (List[Any]): The data to process.
+            next_period (int, optional): The next period number. If None, it's calculated.
+            next_weekday (int, optional): The next weekday number. If None, it's calculated.
+
+        Returns:
+            Tuple[Set[int], Set[int]]: A tuple containing two sets of kill numbers for front and back sequences.
+        """
+        front_sequences = [self.calculate_front(d) for d in data]
+        back_sequences = [self.calculate_back(d) for d in data]
+        next_weekday = next_weekday or self.get_next_weekday()
+        next_period = next_period or self.get_next_period()
+
+        front_kill_numbers = self.calculate_front_kills(front_sequences, next_period, next_weekday)
+        back_kill_numbers = self.calculate_back_kills(back_sequences, next_weekday)
+
+        # Ensure numbers are within the valid range
+        front_kill_numbers = {num for num in front_kill_numbers if 1 <= num <= self.front_vocab_size}
+        back_kill_numbers = {num for num in back_kill_numbers if 1 <= num <= self.back_vocab_size}
+
+        return front_kill_numbers, back_kill_numbers
+
+    def calculate_front_kills(self, sequences: List[List[int]], next_period: int, next_weekday: int) -> Set[int]:
+        """Helper function to calculate front kill numbers based on the last sequence."""
+        last_sequence = sequences[-1]
+        a1, a2, a3, a4, a5 = last_sequence
+        fb = abs(a5 - a3 - a1)
+        fc = a4 - a2
+        average = sum(last_sequence) // self.front_size
+
+        kills = {fb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
+        if fb == 0:
+            kills.update({a1, a3, a5})
+        kills.update({fc, (fc + next_period) % self.front_vocab_size, abs(fc - next_period) % self.front_vocab_size})
+        kills.update({average, sum([a1, a2, a3]) // 3})
+        kills.update({(a1 + a2) - (a3 + a4) - a5, a1 + a2 + a3 + a4 - a5})
+        return kills
+
+    def calculate_back_kills(self, sequences: List[List[int]], next_weekday: int) -> Set[int]:
+        """Helper function to calculate back kill numbers based on the last sequence."""
+        last_sequence = sequences[-1]
+        b1, b2 = last_sequence
+        bb = abs(b1 - b2)
+        kills = {bb + t for t in [0, 1, 3, 6] if abs(t) != next_weekday}
+        kills.update(sequences[-2])
+        if bb == 0:
+            kills.update({b1, b2})
+        kills.update({sum(last_sequence) // self.back_size})
+        return kills
+
+    def get_banker_numbers(self, data: List[Any], next_period: int = None, next_weekday: int = None) -> Tuple[
+        Set[int], Set[int]]:
+        """
+        Calculate and return sets of 'banker numbers' for both front and back sequences based on provided data.
+
+        Parameters:
+            data (List[Any]): The data to process.
+            next_period (int, optional): The next period number. If None, it's calculated.
+            next_weekday (int, optional): The next weekday number. If None, it's calculated.
+
+        Returns:
+            Tuple[Set[int], Set[int]]: A tuple containing two sets of banker numbers for front and back sequences.
+        """
+        front_sequences = [self.calculate_front(d) for d in data]
+        back_sequences = [self.calculate_back(d) for d in data]
+        next_weekday = next_weekday or self.get_next_weekday()
+        next_period = next_period or self.get_next_period()
+
+        front_banker_numbers = self.calculate_front_bankers(front_sequences, next_period, next_weekday)
+        back_backer_numbers = self.calculate_back_bankers(back_sequences, next_weekday)
+
+        # Ensure numbers are within the valid range
+        front_banker_numbers = {num for num in front_banker_numbers if 1 <= num <= self.front_vocab_size}
+        back_banker_numbers = {num for num in back_backer_numbers if 1 <= num <= self.back_vocab_size}
+
+        return front_banker_numbers, back_banker_numbers
+
+    @staticmethod
+    def calculate_front_bankers(sequences: List[List[int]], next_period: int, next_weekday: int) -> Set[int]:
+        """Helper function to calculate front banker numbers based on the last sequence."""
+        last_sequence = sequences[-1]
+        a1, a2, a3, a4, a5 = last_sequence
+        bankers = {a1, a2, a3, a4, a5}
+        for i in last_sequence:
+            bankers.update({i - 1, i + 1})
+        return bankers
+
+    @staticmethod
+    def calculate_back_bankers(sequences: List[List[int]], next_weekday: int) -> Set[int]:
+        """Helper function to calculate back banker numbers based on the last sequence."""
+        last_sequence = sequences[-1]
+        b1, b2 = last_sequence
+        bankers = {b1, b2}
+        for i in last_sequence:
+            bankers.update({i - 1, i + 1})
+        return bankers
+
+    def get_previous_history_data(self, next_period: int = None):
+        history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
+        if next_period is None:
+            history_data = history_data[:]
+        else:
+            index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
+            history_data = history_data[:index] if index != -1 else history_data[:]
+        return history_data
+
+    def get_previous_period_data(self, next_period: int = None):
+        period_data = self.read_json_data_from_file(self.period_record_path, app_log=self.app_log)
+        if next_period is None:
+            period_data = period_data.get(str(self.get_next_period()).zfill(3))
+        else:
+            period_data = period_data.get(str(next_period % 100).zfill(3))
+            index = next((i for i, sublist in enumerate(period_data) if sublist[0] == str(next_period)), -1)
+            period_data = period_data[:index] if index != -1 else period_data[:]
+        return period_data
+
+    def get_previous_weekday_data(self, next_weekday: int = None, next_period: int = None):
+        weekday_data = self.read_json_data_from_file(self.weekday_record_path, app_log=self.app_log)
+        if next_weekday is None:
+            weekday_data = weekday_data.get(str(self.get_next_weekday()))
+        else:
+            weekday_data = weekday_data.get(str(next_weekday))
+            if next_period is not None:
+                index = next((i for i, sublist in enumerate(weekday_data) if sublist[0] == str(next_period)), -1)
+                weekday_data = weekday_data[:index] if index != -1 else weekday_data[:]
+        return weekday_data
+
     def convert_lottery_data(self, data: List[Any]) -> Lottery:
         """
         Creates a Lottery named tuple from the provided data.
 
         :param data: A list containing t data.
         :return: A Lottery named tuple with the processed data.
         """
@@ -678,26 +810,29 @@
             )
         except Exception as ex:
             # self.app_log.info(ex)
             # If there is an error, create a Lottery with the raw data
             # Ensure that 'data' can be unpacked into the Lottery named tuple
             return self.Lottery(*data)
 
-    def calculate_front(self, data: Iterable[int]) -> List[int]:
+    def calculate_front(self, data: Iterable[Any]) -> List[int]:
         """
         Calculate the 'front' portion of the data based on predefined size settings.
 
         :param data: The input data list whose 'front' part is to be calculated.
         :return: A list representing the 'front' portion of the data.
         :raises IndexError: If the length of data does not match any expected size.
         """
         length = len(list(data))
 
         # If data length is equal to the origin size, return the middle part of the data.
-        if length == self.origin_size:
+        if isinstance(data, self.Lottery):
+            return data.front
+
+        elif length == self.origin_size:
             return list(map(int, data[self.back_size:-self.back_size]))
 
         # If data length is equal to the normal size, return the front part of the data.
         elif length == self.normal_size:
             return list(map(int, data[:self.front_size]))
 
         # If data length is equal to the front size, return the data as is.
@@ -718,15 +853,17 @@
         :param data: The input data list whose 'back' part is to be calculated.
         :return: A list representing the 'back' portion of the data.
         :raises IndexError: If the length of data does not match any expected size.
         """
         length = len(list(data))
 
         # If data length matches one of the expected sizes, return the 'back' part of the data.
-        if length in (self.origin_size, self.normal_size):
+        if isinstance(data, self.Lottery):
+            return data.back
+        elif length in (self.origin_size, self.normal_size):
             return list(map(int, data[-self.back_size:]))
         elif length == self.back_size:
             return list(map(int, data))
         elif length == self.front_size:
             return []
 
         # If none of the above conditions are met, raise an IndexError.
@@ -954,20 +1091,15 @@
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
         :param window_size: int, default is 15
         """
-        history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
-        if next_period is None:
-            history_data = history_data[:]
-        else:
-            index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
-            history_data = history_data[:index] if index != -1 else history_data[:]
+        history_data = self.get_previous_history_data(next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(history_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=history_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
@@ -983,21 +1115,15 @@
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
         :param window_size: int, default is 15
         """
-        period_data = self.read_json_data_from_file(self.period_record_path, app_log=self.app_log)
-        if next_period is None:
-            period_data = period_data.get(str(self.get_next_period()).zfill(3))
-        else:
-            period_data = period_data.get(str(next_period % 100).zfill(3))
-            index = next((i for i, sublist in enumerate(period_data) if sublist[0] == str(next_period)), -1)
-            period_data = period_data[:index] if index != -1 else period_data[:]
+        period_data = self.get_previous_period_data(next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(period_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=period_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
@@ -1015,62 +1141,55 @@
         Predicts features by the last weekday window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_weekday: int eg: [1 | 3 | 6]
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
         :param window_size: int, default is 15
         """
-        weekday_data = self.read_json_data_from_file(self.weekday_record_path, app_log=self.app_log)
-        if next_weekday is None:
-            weekday_data = weekday_data.get(str(self.get_next_weekday()))
-        else:
-            weekday_data = weekday_data.get(str(next_weekday))
-            if next_period is not None:
-                index = next((i for i, sublist in enumerate(weekday_data) if sublist[0] == str(next_period)), -1)
-                weekday_data = weekday_data[:index] if index != -1 else weekday_data[:]
+        weekday_data = self.get_previous_weekday_data(next_weekday=next_weekday, next_period=next_period)
 
         maybe_combinations = self.predict_by_last_window_data(weekday_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
         handle_result = self.handle_last_window_data(data=weekday_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
 
         return predict_data
 
-    def predict(
+    def model_predict(
             self,
             next_period: int = None,
             next_weekday: int = None,
             show_details: bool = False,
             window_size: int = 15
     ) -> List[List[int]]:
         """
         :param next_period: int eg: 24001
         :param next_weekday: int eg: [1 | 3 | 6]
         :param show_details: boolean flag to output details about the prediction
         :param window_size: int, the default is 15
         """
-        predict_data = []
-        predict_data.extend(self.predict_by_last_period(next_period=next_period,
+        predictions = []
+        predictions.extend(self.predict_by_last_period(next_period=next_period,
+                                                       show_details=show_details,
+                                                       window_size=window_size))
+        predictions.extend(self.predict_by_same_period(next_period=next_period,
+                                                       show_details=show_details,
+                                                       window_size=window_size))
+        predictions.extend(self.predict_by_last_weekday(next_weekday=next_weekday,
+                                                        next_period=next_period,
                                                         show_details=show_details,
                                                         window_size=window_size))
-        predict_data.extend(self.predict_by_same_period(next_period=next_period,
-                                                        show_details=show_details,
-                                                        window_size=window_size))
-        predict_data.extend(self.predict_by_last_weekday(next_weekday=next_weekday,
-                                                         next_period=next_period,
-                                                         show_details=show_details,
-                                                         window_size=window_size))
 
         if show_details is True:
             self.app_log.info("The following is a preliminary forecast of the data analysis : ")
             # Splitting the data into first 5 and last 2 numbers
-            front_zone = [num for row in predict_data for num in row[:5]]
-            back_zone = [num for row in predict_data for num in row[5:]]
+            front_zone = [num for row in predictions for num in row[:5]]
+            back_zone = [num for row in predictions for num in row[5:]]
 
             # Counting occurrences
             front_zone_frequency = Counter(front_zone)
             back_zone_frequency = Counter(back_zone)
 
             # Sorting the counts
             sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
@@ -1084,17 +1203,17 @@
 
             self.app_log.info("\nCounts of the back zone numbers in each row sorted by frequency:")
             for number, count in sorted_back_zone_frequency:
                 self.app_log.info(f"Number {number}: {count} times")
             self.app_log.info(f"Total count of the back zone numbers in each row: {len(sorted_back_zone_frequency)}")
 
             self.app_log.info("\nHere are the preliminary predictions: ")
-            for data in predict_data:
+            for data in predictions:
                 self.app_log.info(', '.join(map(str, data)))
-        return predict_data
+        return predictions
 
     def calculate_predictions_and_intervals(
             self,
             data: List[Union[float, int]],
             sd_threshold: float,
             rolling_size: int,
             warm_start: bool = False,
@@ -1155,96 +1274,147 @@
     def analyze_predict(
             self,
             next_period: int = None,
             next_weekday: int = None,
             show_details: bool = False,
             window_size: int = 15
     ) -> List[List[int]]:
-        def filter_combs(combs, criteria, intersection_set, required_intersection_count):
-            filtered_combs = []
-            for comb in combs:
-                sum_val = self.calculate_sum_total(comb)
-                span_val = self.calculate_span(comb)
-                avg_val = self.calculate_avg(comb)
-
-                if all([
-                    criteria['sum_total']['min'] <= sum_val <= criteria['sum_total']['max'],
-                    criteria['span']['min'] <= span_val <= criteria['span']['max'],
-                    criteria['avg']['min'] <= avg_val <= criteria['avg']['max'],
-                    # len(intersection_set.intersection(set(comb))) >= required_intersection_count,
-                ]):
-                    filtered_combs.append(comb)
-            return filtered_combs
-
-        predict_data = self.predict(next_period=next_period, next_weekday=next_weekday,
-                                    show_details=show_details, window_size=window_size)
-        front_set, back_set = set(), set()
+        """
+        :param next_period: int eg: 24001
+        :param next_weekday: int eg: [1 | 3 | 6]
+        :param show_details: boolean flag to output details about the prediction
+        :param window_size: int, the default is 15
+        """
+        # use model predict combinations and handle number set
+        predict_data = self.model_predict(next_period=next_period, next_weekday=next_weekday,
+                                          show_details=False, window_size=window_size)
+        predict_front_set, predict_back_set = set(), set()
         for data in predict_data:
-            front_set.update(self.calculate_front(data))
-            back_set.update(self.calculate_back(data))
+            predict_front_set.update(self.calculate_front(data))
+            predict_back_set.update(self.calculate_back(data))
+        exclude_front_set = predict_front_set.difference(set(range(1, self.front_vocab_size + 1)))
+        exclude_back_set = predict_back_set.difference(set(range(1, self.back_vocab_size + 1)))
+
+        # generate kill and banker numbers
+        history_data = self.get_previous_history_data(next_period=next_period)
+        period_data = self.get_previous_period_data(next_period=next_period)
+        weekday_data = self.get_previous_weekday_data(next_period=next_period, next_weekday=next_weekday)
+        front_kill_numbers, back_kill_numbers = self.get_kill_numbers(history_data, next_period=next_period,
+                                                                      next_weekday=next_weekday)
+        front_banker_numbers, back_banker_numbers = self.get_banker_numbers(history_data, next_period=next_period,
+                                                                            next_weekday=next_weekday)
 
         self.app_log.info("Now, Will analyze the predictions..., Then adjust data")
-        history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
-        if next_period is not None:
-            index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
-            history_data = history_data[:index] if index != -1 else history_data[:]
+        # Calculate available numbers avoiding both kill and banker numbers for the front
+        available_front_numbers = set(range(1, self.front_vocab_size + 1)) - front_kill_numbers - front_banker_numbers
+        # Calculate intersection of kill and banker numbers for the back
+        available_back_numbers = back_kill_numbers & back_banker_numbers
+
+        # Convert sets to lists for sampling
+        available_front_numbers = list(available_front_numbers)
+        available_back_numbers = list(available_back_numbers)
+
+        predictions = []
+
+        # Generate a prediction if there are enough numbers to sample from
+        if len(available_front_numbers) >= 5 and len(available_back_numbers) >= 2:
+            predictions.append(
+                sorted(random.sample(available_front_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
+
+        # Generate prediction from kill numbers if there are enough
+        if len(front_kill_numbers) >= 5 and len(available_back_numbers) >= 2:
+            predictions.append(
+                sorted(random.sample(front_kill_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
+
+        # Generate prediction from banker numbers if there are enough
+        if len(front_banker_numbers) >= 5 and len(available_back_numbers) >= 2:
+            predictions.append(
+                sorted(random.sample(front_banker_numbers, 5)) + sorted(random.sample(available_back_numbers, 2)))
 
-        features = ['sum_total', 'span', 'avg']
-        history_data_features = {zone: {feat: [] for feat in features} for zone in ['front', 'back']}
-        # Use results as needed
-        for data in history_data:
-            for zone in ['front', 'back']:
-                zone_data = self.calculate_front(data) if zone == 'front' else self.calculate_back(data)
-                for feature in features:
-                    func = getattr(self, f'calculate_{feature}')
-                    history_data_features[zone][feature].append(func(zone_data))
-
-        params = {
-            'front': {
-                'sum_total': {'sd_threshold': sum([31, 32, 33, 34, 35]), 'rolling_size': 5, 'warm_start': True,
-                              'random_state': 12},
-                'span': {'sd_threshold': abs(35 - 1), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
-                'avg': {'sd_threshold': sum([31, 32, 33, 34, 35]) // 5, 'rolling_size': 5, 'warm_start': True,
-                        'random_state': 12}
-            },
-            'back': {
-                'sum_total': {'sd_threshold': sum([11, 12]), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
-                'span': {'sd_threshold': abs(12 - 1), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
-                'avg': {'sd_threshold': sum([11, 12]) // 2, 'rolling_size': 5, 'warm_start': True, 'random_state': 12}
-            }
-        }
-        results = {'front': {}, 'back': {}}
+        # Combine front and back combinations
+        if show_details is True:
+            self.app_log.info("The following is a preliminary forecast of the data analysis : ")
+            self.app_log.info(f"available front numbers: {available_front_numbers}")
+            self.app_log.info(f"available back numbers: {available_back_numbers}")
+            self.app_log.info(f"front kill numbers: {front_kill_numbers}")
+            self.app_log.info(f"back kill numbers: {back_kill_numbers}")
+            self.app_log.info(f"front banker numbers: {front_banker_numbers}")
+            self.app_log.info(f"back banker numbers: {back_banker_numbers}")
+
+            self.app_log.info(f"last combination: {history_data[-1]}")
+            self.app_log.info(f"model predict front: {sorted(predict_front_set)}")
+            self.app_log.info(f"model predict back: {sorted(predict_back_set)}")
+            self.app_log.info(f"exclude model predict front: {sorted(exclude_front_set)}")
+            self.app_log.info(f"exclude model predict back: {sorted(exclude_back_set)}")
 
-        for zone in ['front', 'back']:
-            for feature in features:
-                pred, min_val, max_val = self.calculate_predictions_and_intervals(
-                    history_data_features[zone][feature],
-                    params[zone][feature]['sd_threshold'],
-                    params[zone][feature]['rolling_size'],
-                    params[zone][feature]['warm_start'],
-                    params[zone][feature]['random_state'],
-                    param_distributions={
-                        'n_estimators': randint(100, 500),
-                        'max_depth': [None, ] + [i for i in range(10, 100)],
-                        'max_features': ['sqrt', 'log2'],
-                        'min_samples_split': randint(2, 80),
-                        'min_samples_leaf': randint(1, 40)
-                    }
-                )
-                results[zone][feature] = {'prediction': pred, 'min': min_val, 'max': max_val}
-                self.app_log.info(f'zone:{zone} {feature}: {pred}, min: {min_val}, max: {max_val}')
+            # Splitting the data into first 5 and last 2 numbers
+            front_zone = [num for row in predictions for num in row[:5]]
+            back_zone = [num for row in predictions for num in row[5:]]
 
-        # Filter front and back combinations
-        # filter_front_comb = filter_combs(self.all_fronts, results['front'], front_set, 4)
-        filter_front_comb = filter_combs(list(combinations(front_set, self.front_size)), results['front'], front_set, 4)
-        # filter_back_comb = filter_combs(self.all_backs, results['back'], back_set, 1)
-        filter_back_comb = filter_combs(list(combinations(back_set, self.back_size)), results['back'], back_set, 1)
-        self.app_log.info(f'Front filter result count: {len(filter_front_comb)}')
-        self.app_log.info(f'Back filter result count: {len(filter_back_comb)}')
+            # Counting occurrences
+            front_zone_frequency = Counter(front_zone)
+            back_zone_frequency = Counter(back_zone)
 
-        # Combine front and back combinations
-        final_combinations = [front + back for front in filter_front_comb for back in filter_back_comb]
-        self.app_log.info(f'Final result count: {len(final_combinations)}')
-        return final_combinations
+            # Sorting the counts
+            sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
+            sorted_back_zone_frequency = sorted(back_zone_frequency.items(), key=lambda x: x[1], reverse=True)
+
+            # Printing the results
+            self.app_log.info("Counts of the front zone numbers in each row sorted by frequency:")
+            for number, count in sorted_front_zone_frequency:
+                self.app_log.info(f"Number {number}: {count} times")
+            self.app_log.info(f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}")
+
+            self.app_log.info("\nCounts of the back zone numbers in each row sorted by frequency:")
+            for number, count in sorted_back_zone_frequency:
+                self.app_log.info(f"Number {number}: {count} times")
+            self.app_log.info(f"Total count of the back zone numbers in each row: {len(sorted_back_zone_frequency)}")
+
+            self.app_log.info("\nHere are the preliminary predictions: ")
+            for data in predictions:
+                self.app_log.info(', '.join(map(str, data)))
+        return predictions
+
+    def predict(
+            self,
+            next_period: int = None,
+            next_weekday: int = None,
+            show_details: bool = False,
+            window_size: int = 15,
+            predict_type: str = 'model'
+    ) -> List[List[int]]:
+        """
+        Generates predictions based on the specified prediction type.
+
+        Parameters:
+        next_period (int, optional): The next period to predict, defaults to None.
+        next_weekday (int, optional): The next weekday to predict, defaults to None.
+        show_details (bool): Whether to show detailed predictions, defaults to False.
+        window_size (int): The window size used for predictions, defaults to 15.
+        predict_type (str): The type of prediction, can be 'model', 'analyze', or 'train', defaults to 'model'.
+
+        Returns:
+        List[List[int]]: A list of prediction results based on the prediction type.
+
+        Raises:
+        KeyError: If the provided prediction type is not in the supported types list.
+        """
+        # Define supported prediction types and their corresponding functions
+        types: Dict[str, Callable] = {
+            'model': self.model_predict,
+            'analyze': self.analyze_predict,
+        }
+
+        # Select the appropriate function based on the provided prediction type and execute prediction
+        if predict_type not in types:
+            raise KeyError(f"Predict type '{predict_type}' is not supported.")
+        predictions = types[predict_type](
+            next_period=next_period,
+            next_weekday=next_weekday,
+            show_details=show_details,
+            window_size=window_size
+        )
+
+        return predictions
 
     def test(self):
         pass
```

### Comparing `lottokit-1.0/lottokit/util.py` & `lottokit-1.1/lottokit/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,41 +326,56 @@
         except Exception as ex:
             app_log.exception(f"An error occurred while reading the JSON file: {ex}")
             return None
 
 
 class ModelUtil:
     @staticmethod
-    def exponential_moving_average_next_value(numeric_sequence: List[int], span: int = 5) -> int:
+    def exponential_moving_average_next_value(
+            numeric_sequence: List[int],
+            span: int = 5,
+            enable_rolling_difference: bool = False
+    ) -> int:
         """
-        Calculate the Exponential Moving Average (EMA) of a given numeric sequence.
+        Calculate the Exponential Moving Average (EMA) and use rolling difference to predict the next value of a sequence.
 
         EMA is a type of moving average that places a greater weight and significance
         on the most recent data points. It's more responsive to new information compared
         to a simple moving average (SMA).
 
         :param numeric_sequence: A list or sequence of numbers for which the EMA is to be calculated.
         :param span: The number of periods over which to calculate the EMA. Default is 5.
-        :return: The EMA value as an integer.
+        :param enable_rolling_difference: weather to enable rolling. default is False
+        :return: Predicted next value of the sequence based on EMA and rolling difference.
         :raises ValueError: If the input list is empty or contains non-numeric values.
         """
         if not numeric_sequence:
             raise ValueError("The numeric sequence cannot be empty.")
         if not all(isinstance(x, (int, float)) for x in numeric_sequence):
             raise ValueError("All elements in the numeric sequence must be numbers.")
 
         # Convert the numeric sequence into a pandas Series object
         series = pd.Series(numeric_sequence)
 
         # Calculate the EMA using pandas' ewm method
         # Adjust 'min_periods' to handle shorter sequences gracefully
         ema = series.ewm(span=span, min_periods=min(span, len(numeric_sequence)), adjust=False).mean()
 
-        # Return the last value of the EMA series as an integer
-        return round(ema.iloc[-1])
+        # Calculate rolling difference
+        rolling_difference = series.diff()
+
+        # Predict the next value by extrapolating the last rolling difference and the last EMA value
+        if len(rolling_difference) > 1 and enable_rolling_difference is True:
+            predicted_next_value = ema.iloc[-1] + rolling_difference.iloc[-1]
+        else:
+            # If there's no enough data to calculate difference, use the last EMA as the prediction
+            predicted_next_value = ema.iloc[-1]
+
+        # Return the predicted next value rounded to the nearest integer
+        return round(predicted_next_value)
 
     @staticmethod
     def linear_regression_next_value_by_index(numeric_sequence: List[int]) -> int:
         """
         Predicts the next value in a sequence using linear regression.
 
         Linear regression involves fitting a line to the data points in such a way
```

### Comparing `lottokit-1.0/lottokit.egg-info/PKG-INFO` & `lottokit-1.1/lottokit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 1.0
+Version: 1.1
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-1.0/setup.py` & `lottokit-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lottokit',
-    version='1.0',
+    version='1.1',
     keywords=['lottokit', 'lottery'],
     packages=find_packages(),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True,
     author="nickdecodes",
     author_email="nickdecodes@163.com",
     description="Lotto Kit Package",
```

