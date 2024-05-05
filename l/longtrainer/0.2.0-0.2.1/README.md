# Comparing `tmp/longtrainer-0.2.0.tar.gz` & `tmp/longtrainer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longtrainer-0.2.0.tar", last modified: Sun Mar 10 09:40:28 2024, max compression
+gzip compressed data, was "longtrainer-0.2.1.tar", last modified: Sun May  5 16:35:06 2024, max compression
```

## Comparing `longtrainer-0.2.0.tar` & `longtrainer-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-03-10 09:40:28.646403 longtrainer-0.2.0/
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     1070 2023-12-29 13:50:59.000000 longtrainer-0.2.0/LICENSE
--rw-r--r--   0 muzammil  (1000) muzammil  (1000)     3821 2024-03-10 09:40:28.646403 longtrainer-0.2.0/PKG-INFO
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     2709 2024-03-10 09:37:56.000000 longtrainer-0.2.0/README.md
-drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-03-10 09:40:28.646403 longtrainer-0.2.0/longtrainer/
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)        0 2024-02-05 10:04:17.000000 longtrainer-0.2.0/longtrainer/__init__.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     1728 2024-01-24 10:09:25.000000 longtrainer-0.2.0/longtrainer/bot.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     5732 2024-01-24 10:10:05.000000 longtrainer-0.2.0/longtrainer/loaders.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     6255 2024-03-10 09:08:34.000000 longtrainer-0.2.0/longtrainer/retrieval.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)    35814 2024-03-10 08:23:48.000000 longtrainer-0.2.0/longtrainer/trainer.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      593 2023-12-30 04:41:54.000000 longtrainer-0.2.0/longtrainer/utils.py
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)    11949 2024-03-10 09:19:04.000000 longtrainer-0.2.0/longtrainer/vision_bot.py
-drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-03-10 09:40:28.646403 longtrainer-0.2.0/longtrainer.egg-info/
--rw-r--r--   0 muzammil  (1000) muzammil  (1000)     3821 2024-03-10 09:40:28.000000 longtrainer-0.2.0/longtrainer.egg-info/PKG-INFO
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      361 2024-03-10 09:40:28.000000 longtrainer-0.2.0/longtrainer.egg-info/SOURCES.txt
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)        1 2024-03-10 09:40:28.000000 longtrainer-0.2.0/longtrainer.egg-info/dependency_links.txt
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      387 2024-03-10 09:40:28.000000 longtrainer-0.2.0/longtrainer.egg-info/requires.txt
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)       12 2024-03-10 09:40:28.000000 longtrainer-0.2.0/longtrainer.egg-info/top_level.txt
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)       38 2024-03-10 09:40:28.646403 longtrainer-0.2.0/setup.cfg
--rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      630 2024-03-09 12:43:02.000000 longtrainer-0.2.0/setup.py
+drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-05-05 16:35:06.274250 longtrainer-0.2.1/
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     1070 2023-12-29 13:50:59.000000 longtrainer-0.2.1/LICENSE
+-rw-r--r--   0 muzammil  (1000) muzammil  (1000)     4913 2024-05-05 16:35:06.274250 longtrainer-0.2.1/PKG-INFO
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     3800 2024-05-05 16:29:36.000000 longtrainer-0.2.1/README.md
+drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-05-05 16:35:06.274250 longtrainer-0.2.1/longtrainer/
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)        0 2024-02-05 10:04:17.000000 longtrainer-0.2.1/longtrainer/__init__.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     1728 2024-01-24 10:09:25.000000 longtrainer-0.2.1/longtrainer/bot.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     5732 2024-01-24 10:10:05.000000 longtrainer-0.2.1/longtrainer/loaders.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)     6255 2024-03-10 09:08:34.000000 longtrainer-0.2.1/longtrainer/retrieval.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)    35813 2024-05-05 15:05:56.000000 longtrainer-0.2.1/longtrainer/trainer.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      593 2023-12-30 04:41:54.000000 longtrainer-0.2.1/longtrainer/utils.py
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)    11949 2024-03-10 09:19:04.000000 longtrainer-0.2.1/longtrainer/vision_bot.py
+drwxrwxr-x   0 muzammil  (1000) muzammil  (1000)        0 2024-05-05 16:35:06.274250 longtrainer-0.2.1/longtrainer.egg-info/
+-rw-r--r--   0 muzammil  (1000) muzammil  (1000)     4913 2024-05-05 16:35:06.000000 longtrainer-0.2.1/longtrainer.egg-info/PKG-INFO
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      361 2024-05-05 16:35:06.000000 longtrainer-0.2.1/longtrainer.egg-info/SOURCES.txt
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)        1 2024-05-05 16:35:06.000000 longtrainer-0.2.1/longtrainer.egg-info/dependency_links.txt
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      388 2024-05-05 16:35:06.000000 longtrainer-0.2.1/longtrainer.egg-info/requires.txt
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)       12 2024-05-05 16:35:06.000000 longtrainer-0.2.1/longtrainer.egg-info/top_level.txt
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)       38 2024-05-05 16:35:06.278249 longtrainer-0.2.1/setup.cfg
+-rw-rw-r--   0 muzammil  (1000) muzammil  (1000)      630 2024-05-05 14:41:56.000000 longtrainer-0.2.1/setup.py
```

### Comparing `longtrainer-0.2.0/LICENSE` & `longtrainer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/README.md` & `longtrainer-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,238 @@
-00000000: 0a23 204c 6f6e 6754 7261 696e 6572 202d  .# LongTrainer -
-00000010: 2050 726f 6475 6374 696f 6e2d 5265 6164   Production-Read
-00000020: 7920 4c61 6e67 4368 6169 6e0a 3c69 6d67  y LangChain.<img
-00000030: 2073 7263 3d22 6173 7365 7473 2f6c 6f6e   src="assets/lon
-00000040: 6774 7261 696e 6572 2d6c 6f67 6f2e 706e  gtrainer-logo.pn
-00000050: 6722 2068 6569 6768 743d 3230 3070 7820  g" height=200px 
-00000060: 7769 6474 683d 3530 3070 783e 0a0a 0a23  width=500px>...#
-00000070: 2320 4665 6174 7572 6573 20f0 9f8c 9f0a  # Features .....
-00000080: 0a2d 20e2 9c85 202a 2a4c 6f6e 6720 4d65  .- ... **Long Me
-00000090: 6d6f 7279 3a2a 2a20 5265 7461 696e 7320  mory:** Retains 
-000000a0: 636f 6e74 6578 7420 6566 6665 6374 6976  context effectiv
-000000b0: 656c 7920 666f 7220 6578 7465 6e64 6564  ely for extended
-000000c0: 2069 6e74 6572 6163 7469 6f6e 732e 0a2d   interactions..-
-000000d0: 20e2 9c85 202a 2a55 6e69 7175 6520 426f   ... **Unique Bo
-000000e0: 7473 2f43 6861 7420 4d61 6e61 6765 6d65  ts/Chat Manageme
-000000f0: 6e74 3a2a 2a20 536f 7068 6973 7469 6361  nt:** Sophistica
-00000100: 7465 6420 6d61 6e61 6765 6d65 6e74 206f  ted management o
-00000110: 6620 6d75 6c74 6970 6c65 2063 6861 7462  f multiple chatb
-00000120: 6f74 732e 0a2d 20e2 9c85 202a 2a45 6e68  ots..- ... **Enh
-00000130: 616e 6365 6420 4375 7374 6f6d 697a 6174  anced Customizat
-00000140: 696f 6e3a 2a2a 2054 6169 6c6f 7220 7468  ion:** Tailor th
-00000150: 6520 6265 6861 7669 6f72 2074 6f20 6669  e behavior to fi
-00000160: 7420 7370 6563 6966 6963 206e 6565 6473  t specific needs
-00000170: 2e0a 2d20 e29c 8520 2a2a 4d65 6d6f 7279  ..- ... **Memory
-00000180: 204d 616e 6167 656d 656e 743a 2a2a 2045   Management:** E
-00000190: 6666 6963 6965 6e74 2068 616e 646c 696e  fficient handlin
-000001a0: 6720 6f66 2063 6861 7420 6869 7374 6f72  g of chat histor
-000001b0: 6965 7320 616e 6420 636f 6e74 6578 7473  ies and contexts
-000001c0: 2e0a 2d20 e29c 8520 2a2a 4750 5420 5669  ..- ... **GPT Vi
-000001d0: 7369 6f6e 2053 7570 706f 7274 3a2a 2a20  sion Support:** 
-000001e0: 496e 7465 6772 6174 696f 6e20 436f 6e74  Integration Cont
-000001f0: 6578 7420 4177 6172 6520 4750 542d 706f  ext Aware GPT-po
-00000200: 7765 7265 6420 7669 7375 616c 206d 6f64  wered visual mod
-00000210: 656c 732e 0a2d 20e2 9c85 202a 2a44 6966  els..- ... **Dif
-00000220: 6665 7265 6e74 2044 6174 6120 466f 726d  ferent Data Form
-00000230: 6174 733a 2a2a 2053 7570 706f 7274 7320  ats:** Supports 
-00000240: 7661 7269 6f75 7320 6461 7461 2069 6e70  various data inp
-00000250: 7574 2066 6f72 6d61 7473 2e0a 2d20 e29c  ut formats..- ..
-00000260: 8520 2a2a 5665 6374 6f72 5374 6f72 6520  . **VectorStore 
-00000270: 4d61 6e61 6765 6d65 6e74 3a2a 2a20 4164  Management:** Ad
-00000280: 7661 6e63 6564 206d 616e 6167 656d 656e  vanced managemen
-00000290: 7420 6f66 2076 6563 746f 7220 7374 6f72  t of vector stor
-000002a0: 6167 6520 666f 7220 6566 6669 6369 656e  age for efficien
-000002b0: 7420 7265 7472 6965 7661 6c2e 0a0a 2323  t retrieval...##
-000002c0: 2057 6f72 6b73 2066 6f72 2041 6c6c 204c   Works for All L
-000002d0: 616e 6763 6861 696e 2053 7570 706f 7274  angchain Support
-000002e0: 6564 204c 4c4d 2061 6e64 2045 6d62 6564  ed LLM and Embed
-000002f0: 6469 6e67 730a 0a2d 20e2 9c85 204f 7065  dings..- ... Ope
-00000300: 6e41 4920 2864 6566 6175 6c74 290a 2d20  nAI (default).- 
-00000310: e29c 8520 5665 7274 6578 4149 0a2d 20e2  ... VertexAI.- .
-00000320: 9c85 2048 7567 6769 6e67 4661 6365 0a0a  .. HuggingFace..
-00000330: 2320 4578 616d 706c 650a 0a20 5665 7274  # Example.. Vert
-00000340: 6578 4149 204c 4c4d 730a 6060 6070 7974  exAI LLMs.```pyt
-00000350: 686f 6e0a 6672 6f6d 206c 6f6e 6774 7261  hon.from longtra
-00000360: 696e 6572 2e74 7261 696e 6572 2069 6d70  iner.trainer imp
-00000370: 6f72 7420 4c6f 6e67 5472 6169 6e65 720a  ort LongTrainer.
-00000380: 6672 6f6d 206c 616e 6763 6861 696e 5f63  from langchain_c
-00000390: 6f6d 6d75 6e69 7479 2e6c 6c6d 7320 696d  ommunity.llms im
-000003a0: 706f 7274 2056 6572 7465 7841 490a 0a6c  port VertexAI..l
-000003b0: 6c6d 203d 2056 6572 7465 7841 4928 290a  lm = VertexAI().
-000003c0: 0a74 7261 696e 6572 203d 204c 6f6e 6754  .trainer = LongT
-000003d0: 7261 696e 6572 286d 6f6e 676f 5f65 6e64  rainer(mongo_end
-000003e0: 706f 696e 743d 276d 6f6e 676f 6462 3a2f  point='mongodb:/
-000003f0: 2f6c 6f63 616c 686f 7374 3a32 3730 3137  /localhost:27017
-00000400: 2f27 2c20 6c6c 6d3d 6c6c 6d29 0a60 6060  /', llm=llm).```
-00000410: 0a20 546f 6765 7468 6572 4149 204c 4c4d  . TogetherAI LLM
-00000420: 730a 6060 6070 7974 686f 6e0a 6672 6f6d  s.```python.from
-00000430: 206c 6f6e 6774 7261 696e 6572 2e74 7261   longtrainer.tra
-00000440: 696e 6572 2069 6d70 6f72 7420 4c6f 6e67  iner import Long
-00000450: 5472 6169 6e65 720a 6672 6f6d 206c 616e  Trainer.from lan
-00000460: 6763 6861 696e 5f63 6f6d 6d75 6e69 7479  gchain_community
-00000470: 2e6c 6c6d 7320 696d 706f 7274 2054 6f67  .llms import Tog
-00000480: 6574 6865 720a 0a6c 6c6d 203d 2054 6f67  ether..llm = Tog
-00000490: 6574 6865 7228 0a20 2020 206d 6f64 656c  ether(.    model
-000004a0: 3d22 746f 6765 7468 6572 636f 6d70 7574  ="togethercomput
-000004b0: 6572 2f52 6564 5061 6a61 6d61 2d49 4e43  er/RedPajama-INC
-000004c0: 4954 452d 3742 2d42 6173 6522 2c0a 2020  ITE-7B-Base",.  
-000004d0: 2020 7465 6d70 6572 6174 7572 653d 302e    temperature=0.
-000004e0: 372c 0a20 2020 206d 6178 5f74 6f6b 656e  7,.    max_token
-000004f0: 733d 3132 382c 0a20 2020 2074 6f70 5f6b  s=128,.    top_k
-00000500: 3d31 2c0a 2020 2020 2320 746f 6765 7468  =1,.    # togeth
-00000510: 6572 5f61 7069 5f6b 6579 3d22 2e2e 2e22  er_api_key="..."
-00000520: 0a29 0a0a 7472 6169 6e65 7220 3d20 4c6f  .)..trainer = Lo
-00000530: 6e67 5472 6169 6e65 7228 6d6f 6e67 6f5f  ngTrainer(mongo_
-00000540: 656e 6470 6f69 6e74 3d27 6d6f 6e67 6f64  endpoint='mongod
-00000550: 623a 2f2f 6c6f 6361 6c68 6f73 743a 3237  b://localhost:27
-00000560: 3031 372f 272c 206c 6c6d 3d6c 6c6d 290a  017/', llm=llm).
-00000570: 0a60 6060 0a0a 2323 2055 7361 6765 2045  .```..## Usage E
-00000580: 7861 6d70 6c65 20f0 9f9a 800a 0a60 6060  xample ......```
-00000590: 7079 7468 6f6e 0a70 6970 2069 6e73 7461  python.pip insta
-000005a0: 6c6c 206c 6f6e 6774 7261 696e 6572 0a60  ll longtrainer.`
-000005b0: 6060 0a0a 4865 7265 2773 2061 2071 7569  ``..Here's a qui
-000005c0: 636b 2073 7461 7274 2067 7569 6465 206f  ck start guide o
-000005d0: 6e20 686f 7720 746f 2075 7365 204c 6f6e  n how to use Lon
-000005e0: 6754 7261 696e 6572 3a0a 0a60 6060 7079  gTrainer:..```py
-000005f0: 7468 6f6e 0a66 726f 6d20 6c6f 6e67 7472  thon.from longtr
-00000600: 6169 6e65 722e 7472 6169 6e65 7220 696d  ainer.trainer im
-00000610: 706f 7274 204c 6f6e 6754 7261 696e 6572  port LongTrainer
-00000620: 0a69 6d70 6f72 7420 6f73 0a20 2020 2020  .import os.     
-00000630: 2020 200a 2320 5365 7420 796f 7572 204f     .# Set your O
-00000640: 7065 6e41 4920 4150 4920 6b65 790a 6f73  penAI API key.os
-00000650: 2e65 6e76 6972 6f6e 5b22 4f50 454e 4149  .environ["OPENAI
-00000660: 5f41 5049 5f4b 4559 225d 203d 2022 736b  _API_KEY"] = "sk
-00000670: 2d22 0a20 2020 2020 2020 200a 2320 496e  -".        .# In
-00000680: 6974 6961 6c69 7a65 204c 6f6e 6754 7261  itialize LongTra
-00000690: 696e 6572 0a74 7261 696e 6572 203d 204c  iner.trainer = L
-000006a0: 6f6e 6754 7261 696e 6572 286d 6f6e 676f  ongTrainer(mongo
-000006b0: 5f65 6e64 706f 696e 743d 276d 6f6e 676f  _endpoint='mongo
-000006c0: 6462 3a2f 2f6c 6f63 616c 686f 7374 3a32  db://localhost:2
-000006d0: 3730 3137 2f27 2c20 656e 6372 7970 745f  7017/', encrypt_
-000006e0: 6368 6174 733d 5472 7565 290a 626f 745f  chats=True).bot_
-000006f0: 6964 203d 2074 7261 696e 6572 2e69 6e69  id = trainer.ini
-00000700: 7469 616c 697a 655f 626f 745f 6964 2829  tialize_bot_id()
-00000710: 0a70 7269 6e74 2827 426f 7420 4944 3a20  .print('Bot ID: 
-00000720: 272c 2062 6f74 5f69 6429 0a20 2020 2020  ', bot_id).     
-00000730: 2020 200a 2320 4164 6420 4461 7461 0a70     .# Add Data.p
-00000740: 6174 6820 3d20 2770 6174 682f 746f 2f79  ath = 'path/to/y
-00000750: 6f75 722f 6461 7461 270a 7472 6169 6e65  our/data'.traine
-00000760: 722e 6164 645f 646f 6375 6d65 6e74 5f66  r.add_document_f
-00000770: 726f 6d5f 7061 7468 2870 6174 682c 2062  rom_path(path, b
-00000780: 6f74 5f69 6429 0a20 2020 2020 2020 200a  ot_id).        .
-00000790: 2320 496e 6974 6961 6c69 7a65 2042 6f74  # Initialize Bot
-000007a0: 0a74 7261 696e 6572 2e63 7265 6174 655f  .trainer.create_
-000007b0: 626f 7428 626f 745f 6964 290a 2020 2020  bot(bot_id).    
-000007c0: 2020 2020 0a23 2053 7461 7274 2061 204e      .# Start a N
-000007d0: 6577 2043 6861 740a 6368 6174 5f69 6420  ew Chat.chat_id 
-000007e0: 3d20 7472 6169 6e65 722e 6e65 775f 6368  = trainer.new_ch
-000007f0: 6174 2862 6f74 5f69 6429 0a20 2020 2020  at(bot_id).     
-00000800: 2020 200a 2320 5365 6e64 2061 2051 7565     .# Send a Que
-00000810: 7279 2061 6e64 2047 6574 2061 2052 6573  ry and Get a Res
-00000820: 706f 6e73 650a 7175 6572 7920 3d20 2759  ponse.query = 'Y
-00000830: 6f75 7220 7175 6572 7920 6865 7265 270a  our query here'.
-00000840: 7265 7370 6f6e 7365 203d 2074 7261 696e  response = train
-00000850: 6572 2e5f 6765 745f 7265 7370 6f6e 7365  er._get_response
-00000860: 2871 7565 7279 2c20 626f 745f 6964 2c20  (query, bot_id, 
-00000870: 6368 6174 5f69 6429 0a70 7269 6e74 2827  chat_id).print('
-00000880: 5265 7370 6f6e 7365 3a20 272c 2072 6573  Response: ', res
-00000890: 706f 6e73 6529 0a20 2060 6060 0a0a 4865  ponse).  ```..He
-000008a0: 7265 2773 2061 2067 7569 6465 206f 6e20  re's a guide on 
-000008b0: 686f 7720 746f 2075 7365 2056 6973 696f  how to use Visio
-000008c0: 6e20 4368 6174 3a0a 0a60 6060 7079 7468  n Chat:..```pyth
-000008d0: 6f6e 0a63 6861 745f 6964 203d 2074 7261  on.chat_id = tra
-000008e0: 696e 6572 2e6e 6577 5f76 6973 696f 6e5f  iner.new_vision_
-000008f0: 6368 6174 2862 6f74 5f69 6429 0a0a 7175  chat(bot_id)..qu
-00000900: 6572 7920 3d20 2759 6f75 7220 7175 6572  ery = 'Your quer
-00000910: 7920 6865 7265 270a 696d 6167 655f 7061  y here'.image_pa
-00000920: 7468 733d 5b27 6e76 6964 6961 2e6a 7067  ths=['nvidia.jpg
-00000930: 275d 0a72 6573 706f 6e73 6520 3d20 7472  '].response = tr
-00000940: 6169 6e65 722e 5f67 6574 5f76 6973 696f  ainer._get_visio
-00000950: 6e5f 7265 7370 6f6e 7365 2871 7565 7279  n_response(query
-00000960: 2c20 696d 6167 655f 7061 7468 732c 2073  , image_paths, s
-00000970: 7472 2862 6f74 5f69 6429 2c73 7472 2876  tr(bot_id),str(v
-00000980: 6973 696f 6e5f 6964 2929 0a70 7269 6e74  ision_id)).print
-00000990: 2827 5265 7370 6f6e 7365 3a20 272c 2072  ('Response: ', r
-000009a0: 6573 706f 6e73 6529 0a60 6060 0a0a 4c69  esponse).```..Li
-000009b0: 7374 2043 6861 7473 2061 6e64 2044 6973  st Chats and Dis
-000009c0: 706c 6179 2043 6861 7420 4869 7374 6f72  play Chat Histor
-000009d0: 793a 0a0a 6060 6070 7974 686f 6e0a 7472  y:..```python.tr
-000009e0: 6169 6e65 722e 6c69 7374 5f63 6861 7473  ainer.list_chats
-000009f0: 2862 6f74 5f69 6429 0a0a 7472 6169 6e65  (bot_id)..traine
-00000a00: 722e 6765 745f 6368 6174 5f62 795f 6964  r.get_chat_by_id
-00000a10: 2863 6861 745f 6964 3d63 6861 745f 6964  (chat_id=chat_id
-00000a20: 290a 6060 600a 0a54 6869 7320 7072 6f6a  ).```..This proj
-00000a30: 6563 7420 6973 2073 7469 6c6c 2075 6e64  ect is still und
-00000a40: 6572 2061 6374 6976 6520 6465 7665 6c6f  er active develo
-00000a50: 706d 656e 742e 2043 6f6d 6d75 6e69 7479  pment. Community
-00000a60: 2066 6565 6462 6163 6b20 616e 6420 636f   feedback and co
-00000a70: 6e74 7269 6275 7469 6f6e 7320 6172 6520  ntributions are 
-00000a80: 6869 6768 6c79 2061 7070 7265 6369 6174  highly appreciat
-00000a90: 6564 2e20 0a                             ed. .
+00000000: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+00000010: 223e 0a20 203c 696d 6720 7372 633d 2268  ">.  <img src="h
+00000020: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000030: 6d2f 454e 4445 5653 4f4c 532f 4c6f 6e67  m/ENDEVSOLS/Long
+00000040: 2d54 7261 696e 6572 2f62 6c6f 622f 6d61  -Trainer/blob/ma
+00000050: 7374 6572 2f61 7373 6574 732f 6c6f 6e67  ster/assets/long
+00000060: 7472 6169 6e65 722d 6c6f 676f 2e70 6e67  trainer-logo.png
+00000070: 3f72 6177 3d74 7275 6522 2061 6c74 3d22  ?raw=true" alt="
+00000080: 4c6f 6e67 5472 6169 6e65 7220 4c6f 676f  LongTrainer Logo
+00000090: 223e 0a3c 2f70 3e0a 0a3c 6831 2061 6c69  ">.</p>..<h1 ali
+000000a0: 676e 3d22 6365 6e74 6572 223e 4c6f 6e67  gn="center">Long
+000000b0: 5472 6169 6e65 7220 2d20 5072 6f64 7563  Trainer - Produc
+000000c0: 7469 6f6e 2d52 6561 6479 204c 616e 6743  tion-Ready LangC
+000000d0: 6861 696e 3c2f 6831 3e0a 0a3c 7020 616c  hain</h1>..<p al
+000000e0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000000f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000100: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000110: 742f 6c6f 6e67 7472 6169 6e65 722f 223e  t/longtrainer/">
+00000120: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000130: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000140: 6473 2e69 6f2f 7079 7069 2f76 2f6c 6f6e  ds.io/pypi/v/lon
+00000150: 6774 7261 696e 6572 2220 616c 743d 2250  gtrainer" alt="P
+00000160: 7950 4920 5665 7273 696f 6e22 3e0a 2020  yPI Version">.  
+00000170: 3c2f 613e 0a20 203c 6120 6872 6566 3d22  </a>.  <a href="
+00000180: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
+00000190: 682f 7072 6f6a 6563 742f 6c6f 6e67 7472  h/project/longtr
+000001a0: 6169 6e65 7222 3e0a 2020 2020 3c69 6d67  ainer">.    <img
+000001b0: 2073 7263 3d22 6874 7470 733a 2f2f 7374   src="https://st
+000001c0: 6174 6963 2e70 6570 792e 7465 6368 2f62  atic.pepy.tech/b
+000001d0: 6164 6765 2f6c 6f6e 6774 7261 696e 6572  adge/longtrainer
+000001e0: 2220 616c 743d 2254 6f74 616c 2044 6f77  " alt="Total Dow
+000001f0: 6e6c 6f61 6473 223e 0a20 203c 2f61 3e0a  nloads">.  </a>.
+00000200: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000210: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
+00000220: 6a65 6374 2f6c 6f6e 6774 7261 696e 6572  ject/longtrainer
+00000230: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+00000240: 2268 7474 7073 3a2f 2f73 7461 7469 632e  "https://static.
+00000250: 7065 7079 2e74 6563 682f 6261 6467 652f  pepy.tech/badge/
+00000260: 6c6f 6e67 7472 6169 6e65 722f 6d6f 6e74  longtrainer/mont
+00000270: 6822 2061 6c74 3d22 4d6f 6e74 686c 7920  h" alt="Monthly 
+00000280: 446f 776e 6c6f 6164 7322 3e0a 2020 3c2f  Downloads">.  </
+00000290: 613e 0a20 203c 6120 6872 6566 3d22 6874  a>.  <a href="ht
+000002a0: 7470 733a 2f2f 636f 6c61 622e 7265 7365  tps://colab.rese
+000002b0: 6172 6368 2e67 6f6f 676c 652e 636f 6d2f  arch.google.com/
+000002c0: 6472 6976 652f 3148 4533 3044 3571 356f  drive/1HE30D5q5o
+000002d0: 6e44 3873 6653 3530 2d30 3658 5044 586e  nD8sfS50-06XPDXn
+000002e0: 6264 766e 6a49 793f 7573 703d 7368 6172  bdvnjIy?usp=shar
+000002f0: 696e 6722 3e0a 2020 2020 3c69 6d67 2073  ing">.    <img s
+00000300: 7263 3d22 6874 7470 733a 2f2f 636f 6c61  rc="https://cola
+00000310: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00000320: 652e 636f 6d2f 6173 7365 7473 2f63 6f6c  e.com/assets/col
+00000330: 6162 2d62 6164 6765 2e73 7667 2220 616c  ab-badge.svg" al
+00000340: 743d 224f 7065 6e20 696e 2043 6f6c 6162  t="Open in Colab
+00000350: 223e 0a20 203c 2f61 3e0a 3c2f 703e 0a0a  ">.  </a>.</p>..
+00000360: 3c68 7220 2f3e 0a0a 0a0a 0a23 2320 4665  <hr />.....## Fe
+00000370: 6174 7572 6573 20f0 9f8c 9f0a 0a2d 20e2  atures ......- .
+00000380: 9c85 202a 2a4c 6f6e 6720 4d65 6d6f 7279  .. **Long Memory
+00000390: 3a2a 2a20 5265 7461 696e 7320 636f 6e74  :** Retains cont
+000003a0: 6578 7420 6566 6665 6374 6976 656c 7920  ext effectively 
+000003b0: 666f 7220 6578 7465 6e64 6564 2069 6e74  for extended int
+000003c0: 6572 6163 7469 6f6e 732e 0a2d 20e2 9c85  eractions..- ...
+000003d0: 202a 2a55 6e69 7175 6520 426f 7473 2f43   **Unique Bots/C
+000003e0: 6861 7420 4d61 6e61 6765 6d65 6e74 3a2a  hat Management:*
+000003f0: 2a20 536f 7068 6973 7469 6361 7465 6420  * Sophisticated 
+00000400: 6d61 6e61 6765 6d65 6e74 206f 6620 6d75  management of mu
+00000410: 6c74 6970 6c65 2063 6861 7462 6f74 732e  ltiple chatbots.
+00000420: 0a2d 20e2 9c85 202a 2a45 6e68 616e 6365  .- ... **Enhance
+00000430: 6420 4375 7374 6f6d 697a 6174 696f 6e3a  d Customization:
+00000440: 2a2a 2054 6169 6c6f 7220 7468 6520 6265  ** Tailor the be
+00000450: 6861 7669 6f72 2074 6f20 6669 7420 7370  havior to fit sp
+00000460: 6563 6966 6963 206e 6565 6473 2e0a 2d20  ecific needs..- 
+00000470: e29c 8520 2a2a 4d65 6d6f 7279 204d 616e  ... **Memory Man
+00000480: 6167 656d 656e 743a 2a2a 2045 6666 6963  agement:** Effic
+00000490: 6965 6e74 2068 616e 646c 696e 6720 6f66  ient handling of
+000004a0: 2063 6861 7420 6869 7374 6f72 6965 7320   chat histories 
+000004b0: 616e 6420 636f 6e74 6578 7473 2e0a 2d20  and contexts..- 
+000004c0: e29c 8520 2a2a 4750 5420 5669 7369 6f6e  ... **GPT Vision
+000004d0: 2053 7570 706f 7274 3a2a 2a20 496e 7465   Support:** Inte
+000004e0: 6772 6174 696f 6e20 436f 6e74 6578 7420  gration Context 
+000004f0: 4177 6172 6520 4750 542d 706f 7765 7265  Aware GPT-powere
+00000500: 6420 7669 7375 616c 206d 6f64 656c 732e  d visual models.
+00000510: 0a2d 20e2 9c85 202a 2a44 6966 6665 7265  .- ... **Differe
+00000520: 6e74 2044 6174 6120 466f 726d 6174 733a  nt Data Formats:
+00000530: 2a2a 2053 7570 706f 7274 7320 7661 7269  ** Supports vari
+00000540: 6f75 7320 6461 7461 2069 6e70 7574 2066  ous data input f
+00000550: 6f72 6d61 7473 2e0a 2d20 e29c 8520 2a2a  ormats..- ... **
+00000560: 5665 6374 6f72 5374 6f72 6520 4d61 6e61  VectorStore Mana
+00000570: 6765 6d65 6e74 3a2a 2a20 4164 7661 6e63  gement:** Advanc
+00000580: 6564 206d 616e 6167 656d 656e 7420 6f66  ed management of
+00000590: 2076 6563 746f 7220 7374 6f72 6167 6520   vector storage 
+000005a0: 666f 7220 6566 6669 6369 656e 7420 7265  for efficient re
+000005b0: 7472 6965 7661 6c2e 0a0a 2323 2057 6f72  trieval...## Wor
+000005c0: 6b73 2066 6f72 2041 6c6c 204c 616e 6763  ks for All Langc
+000005d0: 6861 696e 2053 7570 706f 7274 6564 204c  hain Supported L
+000005e0: 4c4d 2061 6e64 2045 6d62 6564 6469 6e67  LM and Embedding
+000005f0: 730a 0a2d 20e2 9c85 204f 7065 6e41 4920  s..- ... OpenAI 
+00000600: 2864 6566 6175 6c74 290a 2d20 e29c 8520  (default).- ... 
+00000610: 5665 7274 6578 4149 0a2d 20e2 9c85 2048  VertexAI.- ... H
+00000620: 7567 6769 6e67 4661 6365 0a0a 2320 4578  uggingFace..# Ex
+00000630: 616d 706c 650a 0a20 5665 7274 6578 4149  ample.. VertexAI
+00000640: 204c 4c4d 730a 6060 6070 7974 686f 6e0a   LLMs.```python.
+00000650: 6672 6f6d 206c 6f6e 6774 7261 696e 6572  from longtrainer
+00000660: 2e74 7261 696e 6572 2069 6d70 6f72 7420  .trainer import 
+00000670: 4c6f 6e67 5472 6169 6e65 720a 6672 6f6d  LongTrainer.from
+00000680: 206c 616e 6763 6861 696e 5f63 6f6d 6d75   langchain_commu
+00000690: 6e69 7479 2e6c 6c6d 7320 696d 706f 7274  nity.llms import
+000006a0: 2056 6572 7465 7841 490a 0a6c 6c6d 203d   VertexAI..llm =
+000006b0: 2056 6572 7465 7841 4928 290a 0a74 7261   VertexAI()..tra
+000006c0: 696e 6572 203d 204c 6f6e 6754 7261 696e  iner = LongTrain
+000006d0: 6572 286d 6f6e 676f 5f65 6e64 706f 696e  er(mongo_endpoin
+000006e0: 743d 276d 6f6e 676f 6462 3a2f 2f6c 6f63  t='mongodb://loc
+000006f0: 616c 686f 7374 3a32 3730 3137 2f27 2c20  alhost:27017/', 
+00000700: 6c6c 6d3d 6c6c 6d29 0a60 6060 0a20 546f  llm=llm).```. To
+00000710: 6765 7468 6572 4149 204c 4c4d 730a 6060  getherAI LLMs.``
+00000720: 6070 7974 686f 6e0a 6672 6f6d 206c 6f6e  `python.from lon
+00000730: 6774 7261 696e 6572 2e74 7261 696e 6572  gtrainer.trainer
+00000740: 2069 6d70 6f72 7420 4c6f 6e67 5472 6169   import LongTrai
+00000750: 6e65 720a 6672 6f6d 206c 616e 6763 6861  ner.from langcha
+00000760: 696e 5f63 6f6d 6d75 6e69 7479 2e6c 6c6d  in_community.llm
+00000770: 7320 696d 706f 7274 2054 6f67 6574 6865  s import Togethe
+00000780: 720a 0a6c 6c6d 203d 2054 6f67 6574 6865  r..llm = Togethe
+00000790: 7228 0a20 2020 206d 6f64 656c 3d22 746f  r(.    model="to
+000007a0: 6765 7468 6572 636f 6d70 7574 6572 2f52  gethercomputer/R
+000007b0: 6564 5061 6a61 6d61 2d49 4e43 4954 452d  edPajama-INCITE-
+000007c0: 3742 2d42 6173 6522 2c0a 2020 2020 7465  7B-Base",.    te
+000007d0: 6d70 6572 6174 7572 653d 302e 372c 0a20  mperature=0.7,. 
+000007e0: 2020 206d 6178 5f74 6f6b 656e 733d 3132     max_tokens=12
+000007f0: 382c 0a20 2020 2074 6f70 5f6b 3d31 2c0a  8,.    top_k=1,.
+00000800: 2020 2020 2320 746f 6765 7468 6572 5f61      # together_a
+00000810: 7069 5f6b 6579 3d22 2e2e 2e22 0a29 0a0a  pi_key="...".)..
+00000820: 7472 6169 6e65 7220 3d20 4c6f 6e67 5472  trainer = LongTr
+00000830: 6169 6e65 7228 6d6f 6e67 6f5f 656e 6470  ainer(mongo_endp
+00000840: 6f69 6e74 3d27 6d6f 6e67 6f64 623a 2f2f  oint='mongodb://
+00000850: 6c6f 6361 6c68 6f73 743a 3237 3031 372f  localhost:27017/
+00000860: 272c 206c 6c6d 3d6c 6c6d 290a 0a60 6060  ', llm=llm)..```
+00000870: 0a0a 2323 2055 7361 6765 2045 7861 6d70  ..## Usage Examp
+00000880: 6c65 20f0 9f9a 800a 0a60 6060 7079 7468  le ......```pyth
+00000890: 6f6e 0a70 6970 2069 6e73 7461 6c6c 206c  on.pip install l
+000008a0: 6f6e 6774 7261 696e 6572 0a60 6060 0a0a  ongtrainer.```..
+000008b0: 4865 7265 2773 2061 2071 7569 636b 2073  Here's a quick s
+000008c0: 7461 7274 2067 7569 6465 206f 6e20 686f  tart guide on ho
+000008d0: 7720 746f 2075 7365 204c 6f6e 6754 7261  w to use LongTra
+000008e0: 696e 6572 3a0a 0a60 6060 7079 7468 6f6e  iner:..```python
+000008f0: 0a66 726f 6d20 6c6f 6e67 7472 6169 6e65  .from longtraine
+00000900: 722e 7472 6169 6e65 7220 696d 706f 7274  r.trainer import
+00000910: 204c 6f6e 6754 7261 696e 6572 0a69 6d70   LongTrainer.imp
+00000920: 6f72 7420 6f73 0a20 2020 2020 2020 200a  ort os.        .
+00000930: 2320 5365 7420 796f 7572 204f 7065 6e41  # Set your OpenA
+00000940: 4920 4150 4920 6b65 790a 6f73 2e65 6e76  I API key.os.env
+00000950: 6972 6f6e 5b22 4f50 454e 4149 5f41 5049  iron["OPENAI_API
+00000960: 5f4b 4559 225d 203d 2022 736b 2d22 0a20  _KEY"] = "sk-". 
+00000970: 2020 2020 2020 200a 2320 496e 6974 6961         .# Initia
+00000980: 6c69 7a65 204c 6f6e 6754 7261 696e 6572  lize LongTrainer
+00000990: 0a74 7261 696e 6572 203d 204c 6f6e 6754  .trainer = LongT
+000009a0: 7261 696e 6572 286d 6f6e 676f 5f65 6e64  rainer(mongo_end
+000009b0: 706f 696e 743d 276d 6f6e 676f 6462 3a2f  point='mongodb:/
+000009c0: 2f6c 6f63 616c 686f 7374 3a32 3730 3137  /localhost:27017
+000009d0: 2f27 2c20 656e 6372 7970 745f 6368 6174  /', encrypt_chat
+000009e0: 733d 5472 7565 290a 626f 745f 6964 203d  s=True).bot_id =
+000009f0: 2074 7261 696e 6572 2e69 6e69 7469 616c   trainer.initial
+00000a00: 697a 655f 626f 745f 6964 2829 0a70 7269  ize_bot_id().pri
+00000a10: 6e74 2827 426f 7420 4944 3a20 272c 2062  nt('Bot ID: ', b
+00000a20: 6f74 5f69 6429 0a20 2020 2020 2020 200a  ot_id).        .
+00000a30: 2320 4164 6420 4461 7461 0a70 6174 6820  # Add Data.path 
+00000a40: 3d20 2770 6174 682f 746f 2f79 6f75 722f  = 'path/to/your/
+00000a50: 6461 7461 270a 7472 6169 6e65 722e 6164  data'.trainer.ad
+00000a60: 645f 646f 6375 6d65 6e74 5f66 726f 6d5f  d_document_from_
+00000a70: 7061 7468 2870 6174 682c 2062 6f74 5f69  path(path, bot_i
+00000a80: 6429 0a20 2020 2020 2020 200a 2320 496e  d).        .# In
+00000a90: 6974 6961 6c69 7a65 2042 6f74 0a74 7261  itialize Bot.tra
+00000aa0: 696e 6572 2e63 7265 6174 655f 626f 7428  iner.create_bot(
+00000ab0: 626f 745f 6964 290a 2020 2020 2020 2020  bot_id).        
+00000ac0: 0a23 2053 7461 7274 2061 204e 6577 2043  .# Start a New C
+00000ad0: 6861 740a 6368 6174 5f69 6420 3d20 7472  hat.chat_id = tr
+00000ae0: 6169 6e65 722e 6e65 775f 6368 6174 2862  ainer.new_chat(b
+00000af0: 6f74 5f69 6429 0a20 2020 2020 2020 200a  ot_id).        .
+00000b00: 2320 5365 6e64 2061 2051 7565 7279 2061  # Send a Query a
+00000b10: 6e64 2047 6574 2061 2052 6573 706f 6e73  nd Get a Respons
+00000b20: 650a 7175 6572 7920 3d20 2759 6f75 7220  e.query = 'Your 
+00000b30: 7175 6572 7920 6865 7265 270a 7265 7370  query here'.resp
+00000b40: 6f6e 7365 203d 2074 7261 696e 6572 2e5f  onse = trainer._
+00000b50: 6765 745f 7265 7370 6f6e 7365 2871 7565  get_response(que
+00000b60: 7279 2c20 626f 745f 6964 2c20 6368 6174  ry, bot_id, chat
+00000b70: 5f69 6429 0a70 7269 6e74 2827 5265 7370  _id).print('Resp
+00000b80: 6f6e 7365 3a20 272c 2072 6573 706f 6e73  onse: ', respons
+00000b90: 6529 0a20 2060 6060 0a0a 4865 7265 2773  e).  ```..Here's
+00000ba0: 2061 2067 7569 6465 206f 6e20 686f 7720   a guide on how 
+00000bb0: 746f 2075 7365 2056 6973 696f 6e20 4368  to use Vision Ch
+00000bc0: 6174 3a0a 0a60 6060 7079 7468 6f6e 0a63  at:..```python.c
+00000bd0: 6861 745f 6964 203d 2074 7261 696e 6572  hat_id = trainer
+00000be0: 2e6e 6577 5f76 6973 696f 6e5f 6368 6174  .new_vision_chat
+00000bf0: 2862 6f74 5f69 6429 0a0a 7175 6572 7920  (bot_id)..query 
+00000c00: 3d20 2759 6f75 7220 7175 6572 7920 6865  = 'Your query he
+00000c10: 7265 270a 696d 6167 655f 7061 7468 733d  re'.image_paths=
+00000c20: 5b27 6e76 6964 6961 2e6a 7067 275d 0a72  ['nvidia.jpg'].r
+00000c30: 6573 706f 6e73 6520 3d20 7472 6169 6e65  esponse = traine
+00000c40: 722e 5f67 6574 5f76 6973 696f 6e5f 7265  r._get_vision_re
+00000c50: 7370 6f6e 7365 2871 7565 7279 2c20 696d  sponse(query, im
+00000c60: 6167 655f 7061 7468 732c 2073 7472 2862  age_paths, str(b
+00000c70: 6f74 5f69 6429 2c73 7472 2876 6973 696f  ot_id),str(visio
+00000c80: 6e5f 6964 2929 0a70 7269 6e74 2827 5265  n_id)).print('Re
+00000c90: 7370 6f6e 7365 3a20 272c 2072 6573 706f  sponse: ', respo
+00000ca0: 6e73 6529 0a60 6060 0a0a 4c69 7374 2043  nse).```..List C
+00000cb0: 6861 7473 2061 6e64 2044 6973 706c 6179  hats and Display
+00000cc0: 2043 6861 7420 4869 7374 6f72 793a 0a0a   Chat History:..
+00000cd0: 6060 6070 7974 686f 6e0a 7472 6169 6e65  ```python.traine
+00000ce0: 722e 6c69 7374 5f63 6861 7473 2862 6f74  r.list_chats(bot
+00000cf0: 5f69 6429 0a0a 7472 6169 6e65 722e 6765  _id)..trainer.ge
+00000d00: 745f 6368 6174 5f62 795f 6964 2863 6861  t_chat_by_id(cha
+00000d10: 745f 6964 3d63 6861 745f 6964 290a 6060  t_id=chat_id).``
+00000d20: 600a 0a54 6869 7320 7072 6f6a 6563 7420  `..This project 
+00000d30: 6973 2073 7469 6c6c 2075 6e64 6572 2061  is still under a
+00000d40: 6374 6976 6520 6465 7665 6c6f 706d 656e  ctive developmen
+00000d50: 742e 2043 6f6d 6d75 6e69 7479 2066 6565  t. Community fee
+00000d60: 6462 6163 6b20 616e 6420 636f 6e74 7269  dback and contri
+00000d70: 6275 7469 6f6e 7320 6172 6520 6869 6768  butions are high
+00000d80: 6c79 2061 7070 7265 6369 6174 6564 2e20  ly appreciated. 
+00000d90: 0a0a 0a23 2320 4369 7461 7469 6f6e 0a49  ...## Citation.I
+00000da0: 6620 796f 7520 7574 696c 697a 6520 7468  f you utilize th
+00000db0: 6973 2072 6570 6f73 6974 6f72 792c 2070  is repository, p
+00000dc0: 6c65 6173 6520 636f 6e73 6964 6572 2063  lease consider c
+00000dd0: 6974 696e 6720 6974 2077 6974 683a 0a0a  iting it with:..
+00000de0: 6060 600a 406d 6973 637b 6c6f 6e67 7472  ```.@misc{longtr
+00000df0: 6169 6e65 722c 0a20 2061 7574 686f 7220  ainer,.  author 
+00000e00: 3d20 7b45 6e64 6576 736f 6c73 7d2c 0a20  = {Endevsols},. 
+00000e10: 2074 6974 6c65 203d 207b 4c6f 6e67 5472   title = {LongTr
+00000e20: 6169 6e65 723a 2050 726f 6475 6374 696f  ainer: Productio
+00000e30: 6e2d 5265 6164 7920 4c61 6e67 4368 6169  n-Ready LangChai
+00000e40: 6e7d 2c0a 2020 7965 6172 203d 207b 3230  n},.  year = {20
+00000e50: 3233 7d2c 0a20 2070 7562 6c69 7368 6572  23},.  publisher
+00000e60: 203d 207b 4769 7448 7562 7d2c 0a20 206a   = {GitHub},.  j
+00000e70: 6f75 726e 616c 203d 207b 4769 7448 7562  ournal = {GitHub
+00000e80: 2072 6570 6f73 6974 6f72 797d 2c0a 2020   repository},.  
+00000e90: 686f 7770 7562 6c69 7368 6564 203d 207b  howpublished = {
+00000ea0: 5c75 726c 7b68 7474 7073 3a2f 2f67 6974  \url{https://git
+00000eb0: 6875 622e 636f 6d2f 454e 4445 5653 4f4c  hub.com/ENDEVSOL
+00000ec0: 532f 4c6f 6e67 2d54 7261 696e 6572 7d7d  S/Long-Trainer}}
+00000ed0: 2c0a 7d0a 6060 600a                      ,.}.```.
```

### Comparing `longtrainer-0.2.0/longtrainer/bot.py` & `longtrainer-0.2.1/longtrainer/bot.py`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/longtrainer/loaders.py` & `longtrainer-0.2.1/longtrainer/loaders.py`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/longtrainer/retrieval.py` & `longtrainer-0.2.1/longtrainer/retrieval.py`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/longtrainer/trainer.py` & `longtrainer-0.2.1/longtrainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
+import re
+import uuid
 import shutil
+import pandas as pd
 from datetime import datetime
-
+from pymongo import MongoClient
+from cryptography.fernet import Fernet
 from longtrainer.loaders import DocumentLoader, TextSplitter
 from longtrainer.retrieval import DocRetriever
 from longtrainer.bot import ChainBot
 from longtrainer.vision_bot import VisionMemory, VisionBot
 from langchain_openai.chat_models import ChatOpenAI
 from langchain_community.vectorstores import FAISS
 from langchain_openai.embeddings import OpenAIEmbeddings
 from langchain.prompts import PromptTemplate
 from langchain_community.tools import DuckDuckGoSearchResults
 from longtrainer.utils import serialize_document, deserialize_document
-from pymongo import MongoClient
-from cryptography.fernet import Fernet
-import uuid
-import pandas as pd
-import re
 
 
 class LongTrainer:
 
     def __init__(
             self,
             mongo_endpoint='mongodb://localhost:27017/',
```

### Comparing `longtrainer-0.2.0/longtrainer/utils.py` & `longtrainer-0.2.1/longtrainer/utils.py`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/longtrainer/vision_bot.py` & `longtrainer-0.2.1/longtrainer/vision_bot.py`

 * *Files identical despite different names*

### Comparing `longtrainer-0.2.0/setup.py` & `longtrainer-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='longtrainer',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     description='Produciton Ready LangChain',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Endevsols',
     author_email='technology@endevsols.com',
     url='https://github.com/ENDEVSOLS/Long-Trainer',
```

