# Comparing `tmp/pybangla-1.0.2.tar.gz` & `tmp/pybangla-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.2.tar", last modified: Thu May  2 17:13:59 2024, max compression
+gzip compressed data, was "pybangla-1.0.4.tar", last modified: Sun May  5 18:27:29 2024, max compression
```

## Comparing `pybangla-1.0.2.tar` & `pybangla-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:59.203124 pybangla-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:54.000000 pybangla-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-02 17:13:59.203124 pybangla-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-05-02 17:13:54.000000 pybangla-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:59.199124 pybangla-1.0.2/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:59.199124 pybangla-1.0.2/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17932 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-02 17:13:54.000000 pybangla-1.0.2/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:59.203124 pybangla-1.0.2/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-02 17:13:59.000000 pybangla-1.0.2/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 17:13:59.000000 pybangla-1.0.2/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:13:59.000000 pybangla-1.0.2/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 17:13:59.000000 pybangla-1.0.2/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 17:13:59.000000 pybangla-1.0.2/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:13:59.203124 pybangla-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 17:13:54.000000 pybangla-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:13:59.199124 pybangla-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-02 17:13:54.000000 pybangla-1.0.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:21.000000 pybangla-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-05 18:27:29.479811 pybangla-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-05-05 18:27:21.000000 pybangla-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.475811 pybangla-1.0.4/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18145 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-05 18:27:21.000000 pybangla-1.0.4/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15746 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 18:27:29.000000 pybangla-1.0.4/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 18:27:29.479811 pybangla-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-05 18:27:21.000000 pybangla-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 18:27:29.479811 pybangla-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-05 18:27:21.000000 pybangla-1.0.4/tests/test.py
```

### Comparing `pybangla-1.0.2/PKG-INFO` & `pybangla-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.2
+Version: 1.0.4
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.2/README.md` & `pybangla-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.2/pybangla/module/config.py` & `pybangla-1.0.4/pybangla/module/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -126,14 +126,29 @@
                 ("হাফিঃ", "হাফিযাহুল্লাহ"),
                 ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
                 ("মোঃ",  "মোহাম্মদ"),
                 ("মোসাঃ",  "মোসাম্মত"),
                 ("মোছাঃ", "মোছাম্মত"),
                 ("আ:" , "আব্দুর"),
                 ("ডাঃ" , "ডাক্তার"),
+                (" কিমি ", "কিলোমিটার"),
+                (" সেমি ", "সেন্টিমিটার"),
+                (" বিডি ", "বাংলাদেশ"),
+                ("আ/এ", "আবাসিক এলাকা"),  
+                (" একনেক ", "জাতীয় অর্থনৈতিক পরিষদের নির্বাহী কমিটি"),
+                (" সওজ ", "সড়ক ও জনপথ অধিদপ্তর"),
+                (" পাউবো ",  "পানি উন্নয়ন বোর্ড"),	
+
+                (" টেশিস ", "টেলিফোন শিল্প সংস্থা"),
+                (" পবিস ",  "পল্লী বিদ্যুৎ সমিতি"), 
+                (" ইউপি ", "ইউনিয়ন পরিষদ"),
+                (" ঢাবি ", "ঢাকা বিশ্ববিদ্যালয়"),
+                (" বাগ ", "বাগান"),
+                (" স. ", "সড়ক"), 
+                (" সে. ", "সেতু")
             ]
         ]
     }
 
     _symbols = {
             "en": [
                 (re.compile(r"%s" % re.escape(x[0]), re.IGNORECASE), x[1])
```

### Comparing `pybangla-1.0.2/pybangla/module/date_extractor.py` & `pybangla-1.0.4/pybangla/module/date_extractor.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.2/pybangla/module/main.py` & `pybangla-1.0.4/pybangla/module/main.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.2/pybangla/module/number_parser.py` & `pybangla-1.0.4/pybangla/module/number_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,27 @@
 
         """
         Grouping of the word from the list of text
         """
         output, temp_sequence = [], []
         i = 0
         while i < len(input_list):
+            input_list[i] = input_list[i].replace("শত00", "শত")
+            input_list[i] = input_list[i].replace("শো00", "শত")
             if input_list[i].isdigit():
-                if len(input_list)-1 == i:
+                if len(input_list[i])==2 and len(input_list)-1 != i:
+                    if input_list[i+1] in cfg.checking_hunderds:
+                        temp_sequence.append(input_list[i])
+                        output.append(temp_sequence)
+                    else:
+                        temp_sequence.append(input_list[i])
+                        output.append(temp_sequence)
+                        temp_sequence = []
+
+                elif len(input_list)-1 == i:
                     temp_sequence.append(input_list[i])
                     output.append(temp_sequence)
                 else:
                     temp_sequence.append(input_list[i])
             elif input_list[i] in cfg.decimale_chunks or input_list[i] in cfg.fraction_int:
                 temp_sequence.append(input_list[i])
             elif input_list[i] in cfg.hundreds:
@@ -289,14 +300,16 @@
             else:
                 text_list.append(word)
         return text_list
 
     def convert_word2number(self, text):
         text = self.normalize(text+" ")
         text_list = self.replace_word_to_number(text)
+
+        # print("text_list : ", text_list)
         results = self.word_clustering(text_list)
         sum_status_list = self.sum_status(results)
         text = self.converting2digits(results, text_list, sum_status_list)
         return text
```

### Comparing `pybangla-1.0.2/pybangla/module/parser.py` & `pybangla-1.0.4/pybangla/module/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,24 +123,26 @@
         
         """
         # print("number  : ", number, language)
 
         if language=="en":
             extracted_number = list(re.finditer(self.bn_regex, str(number), re.UNICODE))
             if extracted_number:
-                number = "".join([cfg._bangla2english_digits_mapping[i] for i in number])
+                number = "".join([cfg._bangla2english_digits_mapping[i.replance(",", "")] for i in number])
                 # print("extracted : ", number)
         c_number = ""
         for n in number:
-            if n in data[language]["number"]:
-                c_number += n
-            else:
-                if n.strip() in data[language]["digits_mapping"]:
-                    b_n = data[language]["digits_mapping"][n.strip()]
-                    c_number+=b_n
+            n = n.replace(",", "")
+            if n:
+                if n in data[language]["number"]:
+                    c_number += n
+                else:
+                    if n.strip() in data[language]["digits_mapping"]:
+                        b_n = data[language]["digits_mapping"][n.strip()]
+                        c_number+=b_n
         return c_number
     
     def get_weekday(self, date_:list=[], language="bn"):
 
         """
         Get weekday name Bangla or English
         
@@ -209,21 +211,23 @@
     def number_processing(self, text):
 
         # bn_regex, en_regex = r'[০-৯]+', r'[0-9]+'
         bn_matches, en_matches = list(re.finditer(self.bn_regex, text, re.UNICODE)), \
             list(re.finditer(self.en_regex, text, re.UNICODE))
         if en_matches:
             for m in en_matches:
-                if m[0]:
-                    bn_m= self.number_to_words(self._digit_converter(m[0]))
+                m = m[0].replace(",", "")
+                if m:
+                    bn_m= self.number_to_words(self._digit_converter(m))
                     text = text.replace(m[0], bn_m)
         if bn_matches:
             for m in bn_matches:
+                m = m[0].replace(",", "")
                 if m[0]:
-                    bn_m= self.number_to_words(m[0])
+                    bn_m= self.number_to_words(m)
                     text = text.replace(m[0], bn_m)
         return text
 
 class DateParser:
     def __init__(self):
         self.samples = cfg.samples
 
@@ -427,14 +431,15 @@
             # Use findall to extract matches
             currency = re.findall(pattern, m)
 
             # print(currency)
             if currency:
                 # print("m : ", m)
                 n_m = m.replace(currency[0], "")
+                n_m = n_m.replace(",", "")
                 if "." in n_m:
                     s_m = n_m.split(".")
                     before_dot_word, after_dot_word = self.npr.number_to_words(s_m[0]), self.npr.digit_number_to_digit_word(s_m[1])
                     word =  before_dot_word+" দশমিক "+after_dot_word+ " "+_currency[currency[0]]
                     text = text.replace(m, word)
                     # print(s_m, before_dot_word, after_dot_word)
                 else:
```

### Comparing `pybangla-1.0.2/pybangla/module/word_to_number.py` & `pybangla-1.0.4/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.2/pybangla/test.py` & `pybangla-1.0.4/pybangla/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 import time
 from module.main import Normalizer
 
 if __name__ == "__main__":
 
 
     # # Testing Date format
-    date_list = [
-        "সেপ্টেম্বর ০৫ ২০২৩",
-        "এপ্রিল ২০২৩" 
-        "2023-04-05",  
-        "06-04-2023", 
-        "04/01/2023",  
-        "07 April, 2023", 
-        "Apr 1, 2023",  
-        "2023/04/01", 
-        "01-Apr-2023", 
-        "01-Apr/2023",  
-        "20230401",  
-        "20042024",
-        ["1", "4", "2025"]
-    ]
-    # # number = "123456" or "২০২৩"
-    number = "২০২৩"
+    # date_list = [
+    #     "সেপ্টেম্বর ০৫ ২০২৩",
+    #     "এপ্রিল ২০২৩" 
+    #     "2023-04-05",  
+    #     "06-04-2023", 
+    #     "04/01/2023",  
+    #     "07 April, 2023", 
+    #     "Apr 1, 2023",  
+    #     "2023/04/01", 
+    #     "01-Apr-2023", 
+    #     "01-Apr/2023",  
+    #     "20230401",  
+    #     "20042024",
+    #     ["1", "4", "2025"]
+    # ]
+    # # # number = "123456" or "২০২৩"
+    # number = "২০২৩"
     nrml = Normalizer()
-    # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
-    # print("Date format Testing : ", end ="", flush=True)
-    for date_ in date_list:
-        start_time = time.time()
-        formated_date = nrml.date_format(date_, language="bn")
-        print(formated_date)
-    print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
+    # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
+    # # print("Date format Testing : ", end ="", flush=True)
+    # for date_ in date_list:
+    #     start_time = time.time()
+    #     formated_date = nrml.date_format(date_, language="bn")
+    #     print(formated_date)
+    # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
 
-    print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
-    number = nrml.number_convert(number, language="bn")
+    # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
+    # number = nrml.number_convert(number, language="bn")
     
     
-    number = nrml.number_convert(number, language="bn")
+    # number = nrml.number_convert(number, language="bn")
 
-    print("Bn Number : ", number)
-    print("++++++++++++++++++++ stop number convert ++++++++++++++++++++++")
+    # print("Bn Number : ", number)
+    # print("++++++++++++++++++++ stop number convert ++++++++++++++++++++++")
 
-    # print("++++++++++++++++ Today +++++++++++++++++++++")
-    today_date = nrml.today(language="bn")
-    # today_date = nrml.today(language="en")
-    print(today_date)
-
-    # print("++++++++++++++++ End Today +++++++++++++++++++++")
-    # # print(today_date)
-    # print("++++++++++++++++ weekdays +++++++++++++++++++++")
-    weekdays = nrml.weekdays()
-    weekdays = nrml.weekdays(language="bn")
-    weekdays = nrml.weekdays(language="en")
-    weekdays = nrml.weekdays(day = "সোমবার")
-    weekdays = nrml.weekdays(day = "Monday")
-    print(weekdays)
-
-    # print("++++++++++++++++ end weekdays +++++++++++++++++++++")
-    # # print(weekdays)
-    # print("+++++++++++++++ seasons ++++++++++++++++++++++++")
-    seasons = nrml.seasons()
-    seasons = nrml.seasons(language="bn")
-    seasons = nrml.seasons(language="en")
-    seasons = nrml.seasons(seasons = "গ্রীষ্ম")
-    print(seasons)
-
-    # print("+++++++++++++++ end seasons ++++++++++++++++++++++++")
-
-    # print("+++++++++++++++++ months +++++++++++++++++++++++++++")
-    month = nrml.months()
-    month = nrml.months(month="মার্চ")
-    print(month)
+    # # print("++++++++++++++++ Today +++++++++++++++++++++")
+    # today_date = nrml.today(language="bn")
+    # # today_date = nrml.today(language="en")
+    # print(today_date)
+
+    # # print("++++++++++++++++ End Today +++++++++++++++++++++")
+    # # # print(today_date)
+    # # print("++++++++++++++++ weekdays +++++++++++++++++++++")
+    # weekdays = nrml.weekdays()
+    # weekdays = nrml.weekdays(language="bn")
+    # weekdays = nrml.weekdays(language="en")
+    # weekdays = nrml.weekdays(day = "সোমবার")
+    # weekdays = nrml.weekdays(day = "Monday")
+    # print(weekdays)
+
+    # # print("++++++++++++++++ end weekdays +++++++++++++++++++++")
+    # # # print(weekdays)
+    # # print("+++++++++++++++ seasons ++++++++++++++++++++++++")
+    # seasons = nrml.seasons()
+    # seasons = nrml.seasons(language="bn")
+    # seasons = nrml.seasons(language="en")
+    # seasons = nrml.seasons(seasons = "গ্রীষ্ম")
+    # print(seasons)
+
+    # # print("+++++++++++++++ end seasons ++++++++++++++++++++++++")
+
+    # # print("+++++++++++++++++ months +++++++++++++++++++++++++++")
+    # month = nrml.months()
+    # month = nrml.months(month="মার্চ")
+    # print(month)
 
 
-    text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
+    # text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
     
-    text = nrml.text_normalizer(text)
+    # text = nrml.text_normalizer(text)
 
-    print(text)
+    # print(text)
 
     input_texts = [
         "আমি এক দুই তিন চার পাঁচ টু থ্রি ফাইভ ছয় সেভেন এইট নাইন শূন্য আমার ফোন নাম্বার জিরো ওয়ান ডাবল সেভেন",
         "ওয়ান ডাবল নাইন টু",
         "একশ বিশ টাকা",
         "জিরো টু ডাবল ওয়ান",
         "জিরো ওয়ান ডাবল সেভেন থ্রি ডাবল ফাইভ নাইন থ্রি সেভেন নাইন",
@@ -149,23 +149,24 @@
         "তিনশ পঁচিশ পাঁচশ",
         "তিনশ পঁচিশ পাঁচশ এক",
         "চা-পুন",
         "ওকে",
         "ডের আউটস্ট্যান্ডিং কত",
         "ডাবল",
         "নাইন ডাবল এইট",
-        "দশ বারো এ এগুলা একশ একশ দুই"
+        "দশ বারো এ এগুলা একশ একশ দুই",
+        "এক লক্ষ তেত্রিশ চার"
         ]
     for i in input_texts:
         print("="*40)
         print("input : ", i)
         text = nrml.word2number(i)
         print("output : ", text)
         print("="*40)
-    text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
+    text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২,০২৩"
     formated_date = nrml.date_extraction(text)
 
     print(formated_date)
 
     text = nrml.text_normalizer(text)
     print(text)
```

### Comparing `pybangla-1.0.2/pybangla.egg-info/PKG-INFO` & `pybangla-1.0.4/pybangla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.2
+Version: 1.0.4
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.0.2/setup.py` & `pybangla-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.2',
+    version='1.0.4',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.0.2/tests/test.py` & `pybangla-1.0.4/tests/test.py`

 * *Files identical despite different names*

