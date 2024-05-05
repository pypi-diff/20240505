# Comparing `tmp/ccxt-unmerged-2.2.tar.gz` & `tmp/ccxt_unmerged-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ccxt-unmerged-2.2.tar", last modified: Tue Aug 24 20:17:58 2021, max compression
+gzip compressed data, was "ccxt_unmerged-4.0.tar", last modified: Sun May  5 07:27:46 2024, max compression
```

## Comparing `ccxt-unmerged-2.2.tar` & `ccxt_unmerged-4.0.tar`

### file list

```diff
@@ -1,95 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/
-drwxrwxrwx   0        0        0        0 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged/
-drwxrwxrwx   0        0        0        0 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/
--rw-rw-rw-   0        0        0    39027 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bcio.py
--rw-rw-rw-   0        0        0    14312 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/beaxy.py
--rw-rw-rw-   0        0        0    17830 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/biki.py
--rw-rw-rw-   0        0        0    24203 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitclude.py
--rw-rw-rw-   0        0        0    10568 2020-05-02 02:30:13.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitforexfu.py
--rw-rw-rw-   0        0        0    16359 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitkub.py
--rw-rw-rw-   0        0        0    21409 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitopro.py
--rw-rw-rw-   0        0        0    14773 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitrue.py
--rw-rw-rw-   0        0        0    40115 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bitzfu.py
--rw-rw-rw-   0        0        0    12083 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/bkex.py
--rw-rw-rw-   0        0        0    28417 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/btse.py
--rw-rw-rw-   0        0        0    10688 2020-07-21 23:03:50.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/ceo.py
--rw-rw-rw-   0        0        0     1092 2021-01-19 03:16:50.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/changellypro.py
--rw-rw-rw-   0        0        0    28535 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/coinbene.py
--rw-rw-rw-   0        0        0    22362 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/coindcx.py
--rw-rw-rw-   0        0        0    16040 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/coinsuper.py
--rw-rw-rw-   0        0        0    55651 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/cossdex.py
--rw-rw-rw-   0        0        0    28656 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/cryptocom.py
--rw-rw-rw-   0        0        0    31966 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/dragonex.py
--rw-rw-rw-   0        0        0    29379 2021-01-19 03:16:50.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/duedex.py
--rw-rw-rw-   0        0        0    10999 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/felixo.py
--rw-rw-rw-   0        0        0    15218 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/foblgate.py
--rw-rw-rw-   0        0        0    15814 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/gateiofu.py
--rw-rw-rw-   0        0        0    47373 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/krakenfu.py
--rw-rw-rw-   0        0        0    28502 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/multi.py
--rw-rw-rw-   0        0        0    19088 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/mxc.py
--rw-rw-rw-   0        0        0    32978 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/nominex.py
--rw-rw-rw-   0        0        0     6830 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/primexbt.py
--rw-rw-rw-   0        0        0    15030 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/remitano.py
--rw-rw-rw-   0        0        0    55675 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/silgonex.py
--rw-rw-rw-   0        0        0    30375 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/slicex.py
--rw-rw-rw-   0        0        0    17483 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/tokenomy.py
--rw-rw-rw-   0        0        0    24693 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/tokensnet.py
--rw-rw-rw-   0        0        0     7769 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/tradeogre.py
--rw-rw-rw-   0        0        0    21811 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/txbit.py
--rw-rw-rw-   0        0        0    18231 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/vinex.py
--rw-rw-rw-   0        0        0    37818 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/vitex.py
--rw-rw-rw-   0        0        0    14656 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/wazirx.py
--rw-rw-rw-   0        0        0    12030 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/yunex.py
--rw-rw-rw-   0        0        0    12030 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/_58coin.py
--rw-rw-rw-   0        0        0     1564 2021-06-09 09:56:31.000000 ccxt-unmerged-2.2/ccxt_unmerged/async_support/__init__.py
--rw-rw-rw-   0        0        0    38611 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bcio.py
--rw-rw-rw-   0        0        0    14184 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/beaxy.py
--rw-rw-rw-   0        0        0    17648 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/biki.py
--rw-rw-rw-   0        0        0    23919 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitclude.py
--rw-rw-rw-   0        0        0    10524 2020-05-02 02:30:13.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitforexfu.py
--rw-rw-rw-   0        0        0    16159 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitkub.py
--rw-rw-rw-   0        0        0    21173 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitopro.py
--rw-rw-rw-   0        0        0    14645 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitrue.py
--rw-rw-rw-   0        0        0    39873 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bitzfu.py
--rw-rw-rw-   0        0        0    11931 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/bkex.py
--rw-rw-rw-   0        0        0    28109 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/btse.py
--rw-rw-rw-   0        0        0    10476 2020-07-21 23:03:49.000000 ccxt-unmerged-2.2/ccxt_unmerged/ceo.py
--rw-rw-rw-   0        0        0     1092 2021-01-19 03:16:50.000000 ccxt-unmerged-2.2/ccxt_unmerged/changellypro.py
--rw-rw-rw-   0        0        0    28275 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/coinbene.py
--rw-rw-rw-   0        0        0    22120 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/coindcx.py
--rw-rw-rw-   0        0        0    15960 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/coinsuper.py
--rw-rw-rw-   0        0        0    55265 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/cossdex.py
--rw-rw-rw-   0        0        0    28414 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/cryptocom.py
--rw-rw-rw-   0        0        0    31652 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/dragonex.py
--rw-rw-rw-   0        0        0    29131 2021-01-19 03:16:50.000000 ccxt-unmerged-2.2/ccxt_unmerged/duedex.py
--rw-rw-rw-   0        0        0    10937 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/felixo.py
--rw-rw-rw-   0        0        0    15030 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/foblgate.py
--rw-rw-rw-   0        0        0    15752 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/gateiofu.py
--rw-rw-rw-   0        0        0    47155 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/krakenfu.py
--rw-rw-rw-   0        0        0    28050 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/multi.py
--rw-rw-rw-   0        0        0    18888 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/mxc.py
--rw-rw-rw-   0        0        0    32574 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/nominex.py
--rw-rw-rw-   0        0        0     6786 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/primexbt.py
--rw-rw-rw-   0        0        0    14896 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/remitano.py
--rw-rw-rw-   0        0        0    55289 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/silgonex.py
--rw-rw-rw-   0        0        0    30097 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/slicex.py
--rw-rw-rw-   0        0        0    17283 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/tokenomy.py
--rw-rw-rw-   0        0        0    24457 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/tokensnet.py
--rw-rw-rw-   0        0        0     7689 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/tradeogre.py
--rw-rw-rw-   0        0        0    21641 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/txbit.py
--rw-rw-rw-   0        0        0    18013 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/vinex.py
--rw-rw-rw-   0        0        0    37510 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/vitex.py
--rw-rw-rw-   0        0        0    14552 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/wazirx.py
--rw-rw-rw-   0        0        0    11878 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/yunex.py
--rw-rw-rw-   0        0        0    11950 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/_58coin.py
--rw-rw-rw-   0        0        0     2189 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/ccxt_unmerged/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/
--rw-rw-rw-   0        0        0        1 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1461 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        5 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/requires.txt
--rw-rw-rw-   0        0        0     2802 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/ccxt_unmerged.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1461 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/PKG-INFO
--rw-rw-rw-   0        0        0      726 2021-07-14 19:17:42.000000 ccxt-unmerged-2.2/README.md
--rw-rw-rw-   0        0        0       42 2021-08-24 20:17:58.000000 ccxt-unmerged-2.2/setup.cfg
--rw-rw-rw-   0        0        0      670 2021-08-24 20:13:43.000000 ccxt-unmerged-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/ccxt_unmerged/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/_ccxtUnmergedExchange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/ccxt_unmerged/async_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17326 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/bitkub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30204 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/btse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/changellypro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23426 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/coindcx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/foblgate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/gateiofutures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34100 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/nominex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/async_support/remitano.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/bitkub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29839 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/btse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/changellypro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23038 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/coindcx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16005 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/foblgate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16777 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/gateiofutures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33558 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/nominex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15795 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/ccxt_unmerged/remitano.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-05 07:27:46.000000 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-05 07:27:46.000000 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:27:46.000000 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 07:27:46.000000 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 07:27:46.000000 ccxt_unmerged-4.0/ccxt_unmerged.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:27:46.203809 ccxt_unmerged-4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-05 07:27:42.000000 ccxt_unmerged-4.0/test/test_markets.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ccxt-unmerged-2.2/ccxt_unmerged/async_support/changellypro.py` & `ccxt_unmerged-4.0/ccxt_unmerged/changellypro.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# -*- coding: utf-8 -*-
-
-# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
-# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
-
-from ccxt.async_support.hitbtc import hitbtc
-
-
-class changellypro(hitbtc):
-
-    def describe(self):
-        return self.deep_extend(super(changellypro, self).describe(), {
-            'id': 'changellypro',
-            'name': 'changelly pro',
-            'countries': ['KN'],
-            'urls': {
-                'logo': '',
-                'api': {
-                    'public': 'https://api.pro.changelly.com',
-                    'private': 'https://api.pro.changelly.com',
-                },
-                'www': 'https://pro.changelly.com',
-                'doc': 'https://api.pro.changelly.com',
-                'fees': 'https://changelly.com/blog/changelly-pro-fee-structure/',
-            },
-            'fees': {
-                'trading': {
-                    'maker': 0.1 / 100,
-                    'taker': 0.1 / 100,
-                },
-            },
-        })
+# -*- coding: utf-8 -*-
+
+# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
+# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
+
+from ccxt.hitbtc import hitbtc
+
+
+class changellypro(hitbtc):
+    def describe(self):
+        return self.deep_extend(
+            super(changellypro, self).describe(),
+            {
+                "id": "changellypro",
+                "name": "changelly pro",
+                "countries": ["KN"],
+                "urls": {
+                    "logo": "",
+                    "api": {
+                        "public": "https://api.pro.changelly.com/api/3",
+                        "private": "https://api.pro.changelly.com/api/3",
+                    },
+                    "www": "https://pro.changelly.com",
+                    "doc": "https://api.pro.changelly.com",
+                    "fees": "https://changelly.com/blog/changelly-pro-fee-structure/",
+                },
+                "fees": {
+                    "trading": {
+                        "maker": 0.1 / 100,
+                        "taker": 0.1 / 100,
+                    },
+                },
+            },
+        )
```

### Comparing `ccxt-unmerged-2.2/ccxt_unmerged/async_support/multi.py` & `ccxt_unmerged-4.0/ccxt_unmerged/async_support/nominex.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,710 +1,893 @@
-# -*- coding: utf-8 -*-
-
-# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
-# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
-
-from ccxt.async_support.base.exchange import Exchange
-import hashlib
-import math
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import ArgumentsRequired
-from ccxt.base.errors import BadRequest
-from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import DDoSProtection
-from ccxt.base.errors import ExchangeNotAvailable
-
-
-class multi(Exchange):
-
-    def describe(self):
-        return self.deep_extend(super(multi, self).describe(), {
-            'id': 'multi',
-            'name': 'multi',
-            'countries': ['SG'],
-            'version': 'v1',
-            'rateLimit': 1000,
-            'has': {
-                'fetchMarkets': True,
-                'fetchCurrencies': True,
-                'fetchTradingLimits': False,
-                'fetchTradingFees': True,
-                'fetchFundingLimits': False,
-                'fetchTicker': True,
-                'fetchOrderBook': True,
-                'fetchTrades': True,
-                'fetchOHLCV': True,
-                'fetchBalance': True,
-                'fetchAccounts': False,
-                'createOrder': True,
-                'cancelOrder': True,
-                'editOrder': False,
-                'fetchOrder': True,
-                'fetchOpenOrders': True,
-                'fetchOrders': True,
-                'fetchMyTrades': True,
-                'fetchDepositAddress': True,
-                'fetchDeposits': True,
-                'fetchWithdrawals': True,
-                'fetchTransactions': True,
-                'fetchLedger': True,
-                'withdraw': True,
-                'transfer': False,
-            },
-            'timeframes': {
-                '1m': '1m',
-                '5m': '5m',
-                '10m': '10m',
-                '15m': '15m',
-                '30m': '30m',
-                '1h': '1h',
-                '2h': '2h',
-                '4h': '4h',
-                '6h': '6h',
-                '8h': '8h',
-                '12h': '12h',
-                '1d': '1d',
-                '1w': '1w',
-                '1M': '1M',
-            },
-            'urls': {
-                'logo': 'https://multi.io/en/static/img/icons/logo_white.svg',
-                'api': 'https://api.multi.io/api',
-                'www': 'https://multi.io/',
-                'doc': 'https://docs.multi.io/',
-            },
-            'api': {
-                'public': {
-                    'get': [
-                        'market/list',
-                        'asset/list',
-                        'order/depth',
-                        'market/kline',
-                        'fee_schedules',
-                        'market/trade',
-                        'market/status/all',
-                    ],
-                },
-                'private': {
-                    'get': [
-                        'asset/balance',
-                        'order/pending/detail',
-                        'order/completed/detail',
-                        'order/pending',
-                        'order/pending/stoplimit',
-                        'order/completed',
-                        'order/completed/detail',
-                        'market/user/trade',
-                        'asset/transactions/withdraw',
-                        'asset/transactions/deposit',
-                        'asset/transactions/all',
-                    ],
-                    'post': [
-                        'asset/deposit',
-                        'order',
-                        'order/cancel',
-                        'asset/withdraw',
-                    ],
-                },
-            },
-            'exceptions': {
-                'exact': {
-                    '1': BadRequest,
-                    '701': ArgumentsRequired,
-                    '603': AuthenticationError,
-                    '10': InvalidOrder,
-                    '600': ArgumentsRequired,
-                },
-            },
-            'whitelistErrorsAPIs': ['order/pending/detail', 'order/completed/detail'],
-        })
-
-    async def fetch_markets(self, params={}):
-        response = await self.publicGetMarketList(params)
-        return self.parse_markets(response)
-
-    def parse_markets(self, markets):
-        result = []
-        for i in range(0, len(markets)):
-            market = markets[i]
-            base = self.safe_currency_code(market['base'])
-            quote = self.safe_currency_code(market['quote'])
-            symbol = base + '/' + quote
-            precision = {
-                'amount': self.safe_integer(market, 'basePrec'),
-                'price': self.safe_integer(market, 'quotePrec'),
-            }
-            result.append({
-                'id': market['name'],
-                'symbol': symbol,
-                'base': base,
-                'quote': quote,
-                'baseId': base.lower(),
-                'quoteId': quote.lower(),
-                'active': True,
-                'precision': precision,
-                'limits': {
-                    'amount': {
-                        'min': None,
-                        'max': None,
-                    },
-                    'price': {
-                        'min': None,
-                        'max': None,
-                    },
-                    'cost': {
-                        'min': None,
-                        'max': None,
-                    },
-                },
-                'info': market,
-            })
-        return result
-
-    async def fetch_currencies(self, params={}):
-        response = await self.publicGetAssetList(params)
-        return self.parse_currencies(response)
-
-    def parse_currencies(self, currencies):
-        result = {}
-        for i in range(0, len(currencies)):
-            currency = currencies[i]
-            currencyCode = self.safe_string(currency, 'name')
-            id = currencyCode.lower()
-            numericId = self.safe_integer(currency, 'id')
-            code = self.safe_currency_code(currencyCode)
-            name = self.safe_string(currency, 'displayName')
-            active = self.safe_value(currency, 'status')
-            fee = self.safe_float(currency, 'withdrawFee')
-            precision = self.safe_float(currency, 'precWithdraw')
-            result[code] = {
-                'id': id,
-                'numericId': numericId,
-                'code': code,
-                'info': currency,
-                'name': name,
-                'active': active,
-                'fee': fee,
-                'precision': precision,
-                'limits': {
-                    'amount': {
-                        'min': None,
-                        'max': None,
-                    },
-                    'price': {
-                        'min': None,
-                        'max': None,
-                    },
-                    'cost': {
-                        'min': None,
-                        'max': None,
-                    },
-                    'withdraw': {
-                        'min': self.safe_float(currency, 'minWithdrawAmount'),
-                        'max': None,
-                    },
-                },
-            }
-        return result
-
-    async def fetch_order_book(self, symbol, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-        }
-        if limit is not None:
-            request['limit'] = limit  # default = 20
-        response = await self.publicGetOrderDepth(self.extend(request, params))
-        timestamp = self.safe_integer(response, 'timestamp')
-        return self.parse_order_book(response, symbol, timestamp * 1000)
-
-    async def fetch_ohlcv(self, symbol, timeframe='1m', since=None, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-        }
-        period = self.safe_string(self.timeframes, timeframe)
-        intervalInSeconds = self.parse_timeframe(period)
-        request['interval'] = intervalInSeconds
-        now = self.seconds()
-        if since is None:
-            if limit is not None:
-                start = now - limit * intervalInSeconds
-                request['start'] = int(start)
-        else:
-            start = int(since / 1000)
-            request['start'] = start
-            if limit is not None:
-                request['end'] = int(self.sum(start, limit * intervalInSeconds))
-        response = await self.publicGetMarketKline(self.extend(request, params))
-        return self.parse_ohlcvs(response, market, timeframe, since, limit)
-
-    def parse_ohlcv(self, ohlcv, market=None):
-        timestamp = self.safe_integer(ohlcv, 0) * 1000
-        return [
-            timestamp,
-            self.safe_float(ohlcv, 1),
-            self.safe_float(ohlcv, 3),
-            self.safe_float(ohlcv, 4),
-            self.safe_float(ohlcv, 2),
-            self.safe_float(ohlcv, 5),
-        ]
-
-    async def fetch_trading_fees(self, params={}):
-        await self.load_markets()
-        response = await self.publicGetFeeSchedules(params)
-        fees = []
-        for i in range(0, len(response)):
-            fee = response[i]
-            fees.append({
-                'minVolume': fee['minVolume'],
-                'maker': fee['makerFee'],
-                'taker': fee['takerFee'],
-            })
-        return {
-            'info': response,
-            'fees': fees,
-        }
-
-    async def fetch_trades(self, symbol, since=None, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-        }
-        if limit is not None:
-            request['limit'] = limit
-        response = await self.publicGetMarketTrade(self.extend(request, params))
-        return self.parse_trades(response['result'], market, since, limit)
-
-    def parse_trade(self, trade, market):
-        symbol = market['symbol']
-        timestamp = self.safe_timestamp(trade, 'time')
-        price = self.safe_float(trade, 'price')
-        amount = self.safe_float(trade, 'amount')
-        role = self.safe_string(trade, 'role')
-        takerOrMaker = 'maker' if (role == '1') else 'taker'
-        side = self.safe_string(trade, 'side')
-        type = self.safe_value(trade, 'type')
-        fee = {}
-        fee['cost'] = self.safe_float(trade, 'fee')
-        if side == '1' or type == 'sell':  # sell
-            fee['currency'] = market['quote']
-            side = 'sell'
-        if side == '2' or type == 'buy':  # buy
-            fee['currency'] = market['quote']
-            side = 'buy'
-        return {
-            'info': trade,
-            'id': self.safe_string(trade, 'id'),
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'symbol': symbol,
-            'side': side,
-            'price': price,
-            'amount': amount,
-            'cost': float(price * amount),
-            'order': self.safe_string(trade, 'id'),
-            'takerOrMaker': takerOrMaker,
-            'type': None,
-            'fee': fee,
-        }
-
-    async def fetch_ticker(self, symbol, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        marketId = market['id']
-        response = await self.publicGetMarketStatusAll(params)
-        marketTicket = self.get_market_ticket(response, marketId)
-        return self.parse_ticker(marketTicket['result'], symbol)
-
-    def get_market_ticket(self, response, marketId):
-        marketTicker = {}
-        for i in range(0, len(response)):
-            if response[i]['market'] == marketId:
-                marketTicker['result'] = response[i]
-                break
-        return marketTicker
-
-    def parse_ticker(self, ticker, symbol):
-        return {
-            'symbol': symbol,
-            'info': ticker,
-            'high': self.safe_float(ticker, 'high'),
-            'low': self.safe_float(ticker, 'low'),
-            'bid': self.safe_float(ticker, 'bid'),
-            'bidVolume': None,
-            'ask': self.safe_float(ticker, 'ask'),
-            'open': self.safe_float(ticker, 'open'),
-            'close': self.safe_float(ticker, 'close'),
-            'last': self.safe_float(ticker, 'close'),
-            'baseVolume': self.safe_float(ticker, 'baseVolume'),
-            'quoteVolume': self.safe_float(ticker, 'quoteVolume'),
-            'askVolume': None,
-            'average': None,
-            'change': None,
-            'datetime': None,
-            'percentage': None,
-            'previousClose': None,
-            'timestamp': None,
-            'vwap': None,
-        }
-
-    async def fetch_balance(self, params={}):
-        await self.load_markets()
-        response = await self.privateGetAssetBalance(params)
-        exchange = response['exchange']
-        keys = list(exchange.keys())
-        result = {'info': exchange}
-        for i in range(0, len(keys)):
-            code = keys[i]
-            result[code] = {
-                'free': float(exchange[code]['available']),
-                'used': float(exchange[code]['freeze']),
-            }
-        return self.parse_balance(result)
-
-    async def fetch_deposit_address(self, code, params={}):
-        await self.load_markets()
-        currency = self.currency(code)
-        request = {
-            'symbol': currency['code'],
-        }
-        response = await self.privatePostAssetDeposit(self.extend(request, params))
-        currencyObject = self.safe_value(response, code)
-        return {
-            'currency': code,
-            'address': currencyObject['address'],
-            'tag': self.safe_value(currencyObject, 'memo'),
-            'info': currencyObject,
-        }
-
-    def parse_order(self, order, market):
-        timestamp = self.safe_timestamp(order, 'cTime')
-        orderType = self.safe_string(order, 'type')
-        orderSide = self.safe_string(order, 'side')
-        type = 'limit' if (orderType == '1') else 'market'
-        side = 'sell' if (orderSide == '1') else 'buy'
-        amount = self.safe_float(order, 'amount')
-        filled = amount - self.safe_float(order, 'left', 0)
-        fee = {}
-        if side == 'buy':
-            fee['cost'] = self.safe_value(order, 'takerFee')
-        else:
-            fee['cost'] = self.safe_value(order, 'makerFee')
-        fee['currency'] = market['quote']
-        return {
-            'id': self.safe_string(order, 'id'),
-            'clientOrderId': None,
-            'datetime': self.iso8601(timestamp),
-            'timestamp': timestamp,
-            'lastTradeTimestamp': None,
-            'status': None,
-            'symbol': market['symbol'],
-            'type': type,
-            'side': side,
-            'price': self.safe_float(order, 'price'),
-            'average': None,
-            'amount': amount,
-            'filled': filled,
-            'remaining': self.safe_float(order, 'left'),
-            'cost': float(filled * self.safe_float(order, 'price')),
-            'trades': None,
-            'fee': fee,
-            'info': order,
-        }
-
-    async def fetch_open_order(self, id, symbol=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-            'orderId': id,
-            'type': 'limit',
-        }
-        fetchLimitOrderResponse = await self.privateGetOrderPendingDetail(self.extend(request, params))
-        if fetchLimitOrderResponse:
-            return self.parse_order(fetchLimitOrderResponse, market)
-        request['type'] = 'stoplimit'
-        fetchStopLimitOrderResponse = await self.privateGetOrderPendingDetail(self.extend(request, params))
-        if fetchStopLimitOrderResponse:
-            return self.parse_order(fetchStopLimitOrderResponse, market)
-        return None
-
-    async def fetch_complete_order(self, id, symbol=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'orderId': id,
-        }
-        response = await self.privateGetOrderCompletedDetail(self.extend(request, params))
-        return self.parse_order(response, market)
-
-    async def fetch_order(self, id, symbol=None, params={}):
-        openOrder = await self.fetch_open_order(id, symbol, params)
-        if openOrder:
-            return openOrder
-        completeOrder = await self.fetch_complete_order(id, symbol)
-        if completeOrder:
-            return completeOrder
-        raise OrderNotFound(self.id + ' order ' + id + ' not found')
-
-    async def fetch_limit_pending_orders(self, marketId, limit=None, params={}):
-        request = {
-            'market': marketId,
-            'limit': limit,
-        }
-        response = await self.privateGetOrderPending(self.extend(request, params))
-        return self.safe_value(response, 'records')
-
-    async def fetch_stop_limit_pending_orders(self, marketId, limit=None, params={}):
-        request = {
-            'market': marketId,
-            'limit': limit,
-        }
-        response = await self.privateGetOrderPendingStoplimit(self.extend(request, params))
-        return self.safe_value(response, 'records')
-
-    async def fetch_complete_orders(self, marketId, limit=None, params={}):
-        request = {
-            'market': marketId,
-            'limit': limit,
-        }
-        response = await self.privateGetOrderCompleted(self.extend(request, params))
-        return self.safe_value(response, 'records')
-
-    async def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        marketId = market['id']
-        pendingLimitOrdersPromise = self.fetch_limit_pending_orders(marketId, limit, params)
-        pendingStopLimitOrdersPromise = self.fetch_stop_limit_pending_orders(marketId, limit, params)
-        limitOrders = await pendingLimitOrdersPromise
-        stopLimitOrders = await pendingStopLimitOrdersPromise
-        return self.parse_orders(limitOrders.concat(stopLimitOrders), market, since, limit, params)
-
-    async def fetch_orders(self, symbol=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        marketId = market['id']
-        pendingLimitOrdersPromise = self.fetch_limit_pending_orders(marketId, limit, params)
-        pendingStopLimitOrdersPromise = self.fetch_stop_limit_pending_orders(marketId, limit, params)
-        completeOrdersPromise = self.fetch_complete_orders(marketId, limit, params)
-        limitOrders = await pendingLimitOrdersPromise
-        stopLimitOrders = await pendingStopLimitOrdersPromise
-        completeOrders = await completeOrdersPromise
-        allOrders = limitOrders.concat(stopLimitOrders, completeOrders)
-        return self.parse_orders(allOrders, market, since, limit, params)
-
-    async def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-        }
-        if since:
-            request['since'] = int(since / 1000)
-        if limit:
-            request['limit'] = limit
-        response = await self.privateGetMarketUserTrade(self.extend(request, params))
-        return self.parse_trades(response['records'], market, since, limit)
-
-    async def create_order(self, symbol, type, side, amount, price=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-            'side': 1 if (side == 'sell') else 2,
-            'amount': amount,
-            'price': price,
-            'type': type,
-        }
-        if self.safe_value(params, 'type') == 'stopLimit':
-            request['type'] = 'stoplimit'
-            request['stop'] = self.safe_value(params, 'stopPrice')
-            request['gtlt'] = self.safe_value(params, 'gtlt', 1)
-            params = self.omit(params, ['type', 'stopPrice', 'gtlt'])
-        response = await self.privatePostOrder(self.extend(request, params))
-        return self.parse_order(response, market)
-
-    async def cancel_order(self, id, symbol=None, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'market': market['id'],
-            'orderId': id,
-            'type': 'limit',  # TODO support cancelling stop limit order
-        }
-        response = await self.privatePostOrderCancel(self.extend(request, params))
-        return {'success': True, 'info': response}
-
-    async def fetch_withdrawals(self, code=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        currency = self.currency(code)
-        request = {
-            'symbol': currency['code'],
-        }
-        if limit is not None:
-            request['limit'] = limit
-        response = await self.privateGetAssetTransactionsWithdraw(self.extend(request, params))
-        return self.parse_transactions(response['result'], currency, since, limit, params)
-
-    async def fetch_deposits(self, code=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        currency = self.currency(code)
-        request = {
-            'symbol': currency['code'],
-        }
-        if limit is not None:
-            request['limit'] = limit
-        response = await self.privateGetAssetTransactionsDeposit(self.extend(request, params))
-        return self.parse_transactions(response['result'], currency, since, limit, params)
-
-    async def fetch_transactions(self, code=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        currency = self.currency(code)
-        request = {
-            'symbol': currency['code'],
-        }
-        if limit is not None:
-            request['limit'] = limit
-        response = await self.privateGetAssetTransactionsAll(self.extend(request, params))
-        return self.parse_transactions(response['result'], currency, since, limit, params)
-
-    def parse_transaction(self, transaction, currency):
-        addressFrom = None
-        addressTo = None
-        tagFrom = None
-        tagTo = None
-        address = self.safe_value(transaction, 'address')
-        tag = self.safe_value(transaction, 'memo')
-        type = self.safe_value(transaction, 'type')
-        if type == 'WITHDRAW':
-            addressTo = address
-            tagTo = tag
-        if type == 'DEPOSIT':
-            addressFrom = address
-            tagFrom = tag
-        return {
-            'info': transaction,
-            'id': self.safe_value(transaction, 'id'),
-            'txid': self.safe_value(transaction, 'txhash'),
-            'timestamp': self.safe_timestamp(transaction, 'nonce'),
-            'datetime': self.safe_value(transaction, 'createdAt'),
-            'addressFrom': addressFrom,
-            'address': address,
-            'addressTo': addressTo,
-            'tagFrom': tagFrom,
-            'tag': tag,
-            'tagTo': tagTo,
-            'type': type.lower(),
-            'amount': self.safe_float(transaction, 'amount'),
-            'currency': self.safe_value(transaction, 'symbol'),
-            'status': self.safe_value(transaction, 'status'),
-            'fee': None,
-        }
-
-    async def withdraw(self, code, amount, address, tag=None, params={}):
-        self.check_address(address)
-        await self.load_markets()
-        currency = self.currency(code)
-        request = {
-            'amount': amount,
-            'symbol': currency['code'],
-            'address': address,
-        }
-        if tag is not None:
-            request['memo'] = tag
-        response = await self.privatePostAssetWithdraw(self.extend(request, params))
-        return {
-            'info': self.extend({'status': 'ok'}, response),
-        }
-
-    def sign(self, path, api='public', method='GET', params=None, headers=None, body=None):
-        url = self.urls['api'] + '/' + self.version + '/' + path
-        query = self.omit(params, self.extract_params(path))
-        if method == 'GET':
-            if params:
-                url += '?' + self.urlencode(params)
-        if api == 'private':
-            self.check_required_credentials()
-            timestamp = int(math.floor(self.milliseconds()) / 1000)
-            payloadToSign = {}
-            if method == 'GET' and params:
-                payloadToSign = {}
-            if method == 'POST':
-                body = self.json(query)
-                payloadToSign = query
-            message = self._make_query_string(self.extend({}, payloadToSign, {timestamp, method, path})).substr(1)
-            signature = self.hmac(self.encode(message), self.encode(self.secret), hashlib.sha256, 'hex')
-            headers = {
-                'Content-Type': 'application/json',
-                'X-MULTI-API-KEY': self.apiKey,
-                'X-MULTI-API-SIGNATURE': signature,
-                'X-MULTI-API-TIMESTAMP': timestamp,
-                'X-MULTI-API-SIGNED-PATH': path,
-            }
-        return {'url': url, 'method': method, 'body': body, 'headers': headers}
-
-    def _make_query_string(self, q):
-        arr = []
-        if q:
-            sortedParams = self.keysort(q)
-            keys = list(sortedParams.keys())
-            for i in range(0, len(keys)):
-                key = keys[i]
-                arr.append(self.encode_uri_component(key) + '=' + self.encode_uri_component(q[key]))
-            return '?' + '&'.join(arr)
-        else:
-            return ''
-
-    def check_if_whitelisted_path(self, url):
-        whitelistedUrl = False
-        for i in range(0, len(self.whitelistErrorsAPIs)):
-            path = self.whitelistErrorsAPIs[i]
-            if url.find(path) != -1:
-                whitelistedUrl = True
-                break
-        return whitelistedUrl
-
-    def handle_errors(self, code, reason, url, method, headers, body, response, requestHeaders, requestBody):
-        status = self.safe_string(response, 'status')
-        if code >= 200 and code < 300:
-            return
-        if self.check_if_whitelisted_path(url):
-            return  # default to defaultErrorHandler
-        if code == 429:
-            raise DDoSProtection(self.id + ' ' + body)
-        if status == 'error':
-            errors = self.safe_value(response, 'errors')
-            errorCode = self.safe_string(errors[0], 'code')
-            message = self.safe_string(errors[0], 'message')
-            self.throw_exactly_matched_exception(self.exceptions['exact'], errorCode, message)
-
-    def default_error_handler(self, code, reason, url, method, headers, body, response):
-        if (code >= 200) and (code <= 299):
-            return
-        details = body
-        codeAsString = str(code)
-        ErrorClass = None
-        if self.check_if_whitelisted_path(url):
-            return
-        if self.httpExceptions.find(codeAsString) != -1:
-            ErrorClass = self.httpExceptions[codeAsString]
-        if ErrorClass == ExchangeNotAvailable:
-            details += '(possible reasons: ' + ', '.join([
-                'invalid API keys',
-                'bad or old nonce',
-                'exchange is down or offline',
-                'on maintenance',
-                'DDoS protection',
-                'rate-limiting',
-            ]) + ')'
-        if ErrorClass is not None:
-            raise ErrorClass(' '.join([self.id, method, url, code, reason, details]))
-
-    async def request(self, path, api='public', method='GET', params={}, headers=None, body=None):
-        response = await self.fetch2(path, api, method, params, headers, body)
-        return self.safe_value(response, 'data')
+# -*- coding: utf-8 -*-
+
+# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
+# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
+
+from ccxt.async_support.base.exchange import Exchange
+import hashlib
+from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import PermissionDenied
+from ccxt.base.errors import ArgumentsRequired
+from ccxt.base.errors import BadRequest
+from ccxt.base.errors import BadSymbol
+from ccxt.base.errors import InsufficientFunds
+from ccxt.base.errors import InvalidAddress
+from ccxt.base.errors import InvalidOrder
+from ccxt.base.errors import OrderNotFound
+from ccxt.base.errors import DuplicateOrderId
+from ccxt.base.errors import RateLimitExceeded
+from ccxt.base.errors import InvalidNonce
+from ccxt.base.decimal_to_precision import TICK_SIZE
+
+
+class nominex(Exchange):
+    def describe(self):
+        return self.deep_extend(
+            super(nominex, self).describe(),
+            {
+                "id": "nominex",
+                "name": "Nominex",
+                "countries": ["SC"],
+                "rateLimit": 1500,
+                "certified": False,
+                "pro": False,
+                "has": {
+                    "CORS": False,
+                    "fetchCurrencies": True,
+                    "fetchOHLCV": True,
+                    "cancelAllOrders": False,
+                    "createDepositAddress": True,
+                    "deposit": False,
+                    "fetchClosedOrders": True,
+                    "fetchDepositAddress": True,
+                    "fetchTradingFees": True,
+                    "fetchMyTrades": True,
+                    "fetchOrder": True,
+                    "fetchOpenOrders": True,
+                    "fetchTickers": True,
+                    "fetchDeposits": True,
+                    "fetchWithdrawals": True,
+                    "withdraw": True,
+                },
+                "timeframes": {
+                    "1m": "TF1M",
+                    "5m": "TF5M",
+                    "15m": "TF15M",
+                    "30m": "TF30M",
+                    "1h": "TF1H",
+                    "3h": "TF3H",
+                    "6h": "TF6H",
+                    "12h": "TF12H",
+                    "1d": "TF1D",
+                    "1w": "TF7D",
+                    "2w": "TF14D",
+                    "1M": "TF1MO",
+                },
+                "urls": {
+                    "logo": "https://nominex.io/media/nominex-logo.png",
+                    "api": {
+                        "public": "https://nominex.io/api/rest/v1",
+                        "private": "https://nominex.io/api/rest/v1/private",
+                    },
+                    "demo": {
+                        "public": "https://demo.nominex.io/api/rest/v1",
+                        "private": "https://demo.nominex.io/api/rest/v1/private",
+                    },
+                    "www": "https://nominex.io",
+                    "doc": [
+                        "https://developer.nominex.io/",
+                    ],
+                },
+                "api": {
+                    "public": {
+                        "get": [
+                            "currencies",
+                            "pairs",
+                            "ticker/{symbol}",
+                            "ticker",
+                            "orderbook/{symbol}/A0/{limit}",
+                            "candles/{symbol}/{timeframe}",
+                            "trades/{symbol}",
+                        ],
+                    },
+                    "private": {
+                        "get": [
+                            "trading-fee-rates",
+                            "deposits",
+                            "withdrawals",
+                            "orders",
+                            "orders/{id}",
+                            "orders/{symbol}",
+                            "trades/{symbol}",
+                            "wallets",
+                            "wallets/{currency}/address",
+                            "wallets/{currency}/deposits",
+                            "wallets/{currency}/withdrawals",
+                        ],
+                        "post": [
+                            "orders",
+                            "wallets/{currency}/address",
+                            "withdrawals/{currency}",
+                        ],
+                        "put": [
+                            "orders/{id}",
+                        ],
+                        "delete": [
+                            "orders/{id}",
+                        ],
+                    },
+                },
+                "fees": {
+                    "trading": {
+                        "tierBased": True,
+                        "percentage": True,
+                    },
+                    "funding": {
+                        "tierBased": False,  # True for tier-based/progressive
+                    },
+                },
+                "exceptions": {
+                    "100.2": BadSymbol,
+                    "101": InvalidNonce,
+                    "103": AuthenticationError,
+                    "103.4": InvalidOrder,
+                    "104.4": InvalidOrder,
+                    "110.110": RateLimitExceeded,
+                    "121": PermissionDenied,
+                    "601": BadRequest,
+                    "1101": InsufficientFunds,
+                    "1102": DuplicateOrderId,
+                    "1106": OrderNotFound,
+                    "20002": InvalidAddress,
+                },
+                "precisionMode": TICK_SIZE,
+                "options": {
+                    "tradeSides": {
+                        "buy": "BUY",
+                        "sell": "SELL",
+                    },
+                    "paths": {
+                        "public": "/api/rest/v1",
+                        "private": "/api/rest/v1/private",
+                    },
+                },
+            },
+        )
+
+    async def fetch_trading_fees(self, params={}):
+        await self.load_markets()
+        response = await self.privateGetTradingFeeRates(params)
+        return {
+            "info": response,
+            "maker": self.safe_float(response, "makerFeeFactor") * 100.0,
+            "taker": self.safe_float(response, "takerFeeFactor") * 100.0,
+        }
+
+    async def fetch_currencies(self, params={}):
+        currencies = await self.publicGetCurrencies(params)
+        result = {}
+        for i in range(0, len(currencies)):
+            currency = self.parse_currency(currencies[i])
+            currencyCode = self.safe_string(currency, "code")
+            result[currencyCode] = currency
+        return result
+
+    def parse_currency(self, currency):
+        code = self.safe_string(currency, "code")
+        return {
+            "id": code,
+            "code": code,
+            "name": self.safe_string(currency, "name"),
+            "active": True,
+            "fee": self.safe_float(currency, "withdrawalFee"),
+            "precision": self.safe_integer(currency, "scale"),
+            "info": currency,
+        }
+
+    async def fetch_markets(self, params={}):
+        pairs = await self.publicGetPairs(params)
+        result = []
+        for i in range(0, len(pairs)):
+            market = pairs[i]
+            id = self.safe_string(market, "name")
+            parts = id.split("/")
+            baseId = parts[0]
+            quoteId = parts[1]
+            base = self.safe_currency_code(baseId)
+            quote = self.safe_currency_code(quoteId)
+            symbol = base + "/" + quote
+            precision = {
+                "price": self.safe_float(market, "quoteStep"),
+                "amount": self.safe_float(market, "baseStep"),
+            }
+            limits = {
+                "amount": {
+                    "min": self.safe_float(market, "minBaseAmount"),
+                    "max": self.safe_float(market, "maxBaseAmount"),
+                },
+                "cost": {
+                    "min": self.safe_float(market, "minQuoteAmount"),
+                    "max": self.safe_float(market, "maxQuoteAmount"),
+                },
+            }
+            result.append(
+                {
+                    "id": id,
+                    "symbol": symbol,
+                    "base": base,
+                    "quote": quote,
+                    "settle": None,
+                    "baseId": baseId,
+                    "quoteId": quoteId,
+                    "settleId": None,
+                    "type": "spot",
+                    "spot": True,
+                    "margin": False,
+                    "swap": False,
+                    "future": False,
+                    "option": False,
+                    "contract": False,
+                    "linear": None,
+                    "inverse": None,
+                    "contractSize": None,
+                    "expiry": None,
+                    "expiryDatetime": None,
+                    "strike": None,
+                    "optionType": None,
+                    "active": self.safe_value(market, "active"),
+                    "precision": precision,
+                    "limits": limits,
+                    "info": market,
+                }
+            )
+        return result
+
+    async def fetch_balance(self, params={}):
+        await self.load_markets()
+        balanceType = self.safe_string(params, "type", "SPOT")
+        query = self.omit(params, "type")
+        response = await self.privateGetWallets(query)
+        result = {"info": response}
+        for i in range(0, len(response)):
+            balance = response[i]
+            if balance["type"] == balanceType:
+                currencyId = self.safe_string(balance, "currency")
+                code = self.safe_currency_code(currencyId)
+                if not (code in result):
+                    account = self.account()
+                    account["free"] = self.safe_float(balance, "balanceAvailable")
+                    account["total"] = self.safe_float(balance, "balance")
+                    result[code] = account
+        return self.parse_balance(result)
+
+    async def fetch_order_book(self, symbol, limit=None, params={}):
+        await self.load_markets()
+        request = {
+            "symbol": self.market_id(symbol),
+            "limit": 100,
+        }
+        if limit == 25:
+            request["limit"] = limit
+        response = await self.publicGetOrderbookSymbolA0Limit(
+            self.extend(request, params)
+        )
+        asks = []
+        bids = []
+        for i in range(0, len(response)):
+            priceLevel = response[i]
+            side = self.safe_string(priceLevel, "side")
+            if side == "SELL":
+                asks.append(priceLevel)
+            else:
+                bids.append(priceLevel)
+        return self.parse_order_book(
+            {"asks": asks, "bids": bids},
+            symbol,
+            None,
+            "bids",
+            "asks",
+            "price",
+            "amount",
+        )
+
+    async def fetch_tickers(self, symbols=None, params={}):
+        await self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        ids = list(self.markets.keys())
+        if symbols is not None:
+            for i in range(0, len(symbols)):
+                symbol = symbols[i]
+                market = self.market(symbol)
+                ids.append(market["id"])
+        urlParams["pairs"] = ",".join(ids)
+        response = await self.publicGetTicker(self.extend(request, params))
+        result = {}
+        for i in range(0, len(response)):
+            marketId = ids[i]
+            market = self.markets[marketId]
+            ticker = self.parse_ticker(response[i], market)
+            symbol = market["symbol"]
+            result[symbol] = ticker
+        return result
+
+    async def fetch_ticker(self, symbol, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "symbol": market["id"],
+        }
+        ticker = await self.publicGetTickerSymbol(self.extend(request, params))
+        return self.parse_ticker(ticker, market)
+
+    def parse_ticker(self, ticker, market=None):
+        timestamp = self.safe_integer(ticker, "timestamp")
+        symbol = None
+        if market is not None:
+            symbol = market["symbol"]
+        elif "pair" in ticker:
+            marketId = self.safe_string(ticker, "pair")
+            if marketId is not None:
+                if marketId in self.markets_by_id:
+                    market = self.markets_by_id[marketId][0]
+                    symbol = market["symbol"]
+                else:
+                    baseId = marketId[0:3]
+                    quoteId = marketId[3:6]
+                    base = self.safe_currency_code(baseId)
+                    quote = self.safe_currency_code(quoteId)
+                    symbol = base + "/" + quote
+        last = self.safe_float(ticker, "price")
+        change = self.safe_float(ticker, "dailyChange")
+        open = None
+        average = None
+        if last is not None and change is not None:
+            open = last - change
+            average = (open + last) / 2
+        volume = self.safe_float(ticker, "baseVolume")
+        quoteVolume = self.safe_float(ticker, "quoteVolume")
+        vwap = (
+            (quoteVolume / volume)
+            if (quoteVolume is not None and volume is not None and volume != 0)
+            else None
+        )
+        return {
+            "symbol": symbol,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "high": self.safe_float(ticker, "high"),
+            "low": self.safe_float(ticker, "low"),
+            "bid": self.safe_float(ticker, "bid"),
+            "bidVolume": self.safe_float(ticker, "bidSize"),
+            "ask": self.safe_float(ticker, "ask"),
+            "askVolume": self.safe_float(ticker, "askSize"),
+            "vwap": vwap,
+            "open": open,
+            "close": last,
+            "last": last,
+            "previousClose": None,
+            "change": change,
+            "percentage": self.safe_float(ticker, "dailyChangeP"),
+            "average": average,
+            "baseVolume": volume,
+            "quoteVolume": quoteVolume,
+            "info": ticker,
+        }
+
+    def parse_ohlcv(self, ohlcv, market=None, timeframe="1m", since=None, limit=None):
+        return [
+            self.safe_integer(ohlcv, "timestamp"),
+            self.safe_float(ohlcv, "open"),
+            self.safe_float(ohlcv, "high"),
+            self.safe_float(ohlcv, "low"),
+            self.safe_float(ohlcv, "close"),
+            self.safe_float(ohlcv, "volume"),
+        ]
+
+    async def fetch_ohlcv(
+        self, symbol, timeframe="1m", since=None, limit=None, params={}
+    ):
+        await self.load_markets()
+        if limit is None:
+            limit = 100
+        market = self.market(symbol)
+        urlParams = {
+            "limit": limit,
+            "end": self.milliseconds(),
+        }
+        request = {
+            "symbol": market["id"],
+            "timeframe": self.timeframes[timeframe],
+            "urlParams": urlParams,
+        }
+        if since is not None:
+            request["start"] = since
+        response = await self.publicGetCandlesSymbolTimeframe(
+            self.extend(request, params)
+        )
+        return self.parse_ohlcvs(response, market, timeframe, since, limit)
+
+    def parse_trade(self, trade, market):
+        id = self.safe_string(trade, "id")
+        timestamp = self.safe_integer(trade, "timestamp")
+        type = None
+        side = self.safe_string_lower(trade, "side").lower()
+        orderId = None
+        if "orderId" in trade:
+            orderId = self.safe_string(trade, "orderId")
+        price = self.safe_float(trade, "price")
+        amount = self.safe_float(trade, "amount")
+        cost = None
+        if price is not None:
+            if amount is not None:
+                cost = price * amount
+        takerOrMaker = None
+        if "maker" in trade:
+            maker = self.safe_value(trade, "maker")
+            takerOrMaker = "maker" if maker else "taker"
+        feeAmount = self.safe_float(trade, "fee")
+        fee = (
+            feeAmount is None
+            if None
+            else {
+                "cost": feeAmount,
+                "currency": self.safe_string(trade, "feeCurrencyCode"),
+            }
+        )
+        return {
+            "id": id,
+            "info": trade,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "symbol": market["symbol"],
+            "type": type,
+            "order": orderId,
+            "side": side,
+            "takerOrMaker": takerOrMaker,
+            "price": price,
+            "amount": amount,
+            "cost": cost,
+            "fee": fee,
+        }
+
+    async def fetch_trades(self, symbol, since=None, limit=50, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        urlParams = {}
+        request = {
+            "symbol": market["id"],
+            "urlParams": urlParams,
+        }
+        if since is not None:
+            urlParams["start"] = int(since)
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = await self.publicGetTradesSymbol(self.extend(request, params))
+        return self.parse_trades(
+            self.safe_value(response, "items"), market, since, limit
+        )
+
+    def calculate_fee(
+        self, symbol, type, side, amount, price, takerOrMaker="taker", params={}
+    ):
+        market = self.markets[symbol]
+        rate = market[takerOrMaker]
+        cost = amount * rate
+        key = "quote"
+        if side == "sell":
+            cost *= price
+        else:
+            key = "base"
+        code = market[key]
+        currency = self.safe_value(self.currencies, code)
+        if currency is not None:
+            precision = self.safe_integer(currency, "precision")
+            if precision is not None:
+                cost = float(self.currency_to_precision(code, cost))
+        return {
+            "type": takerOrMaker,
+            "currency": market[key],
+            "rate": rate,
+            "cost": cost,
+        }
+
+    async def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
+        if symbol is None:
+            raise ArgumentsRequired(
+                self.id + " fetchMyTrades requires a `symbol` argument"
+            )
+        await self.load_markets()
+        market = self.market(symbol)
+        urlParams = {}
+        request = {
+            "symbol": market["id"],
+            "urlParams": urlParams,
+        }
+        if limit is not None:
+            urlParams["limit"] = limit
+        if since is not None:
+            urlParams["start"] = int(since)
+        response = await self.privateGetTradesSymbol(self.extend(request, params))
+        return self.parse_trades(
+            self.safe_value(response, "items"), market, since, limit
+        )
+
+    async def create_order(self, symbol, type, side, amount, price=None, params={}):
+        await self.load_markets()
+        marketId = self.market_id(symbol)
+        request = {
+            "pairName": marketId,
+            "side": self.safe_string(self.options["tradeSides"], side, side),
+            "amount": self.amount_to_precision(symbol, amount),
+            "type": self.upper(type),
+            "walletType": self.safe_string(params, "walletType", "SPOT"),
+        }
+        if "clientOrderId" in params:
+            request["cid"] = self.safe_integer(params, "clientOrderId")
+        if type == "limit":
+            request["limitPrice"] = self.price_to_precision(symbol, price)
+        response = await self.privatePostOrders(self.extend(request, params))
+        return self.parse_order(response)
+
+    async def edit_order(
+        self, id, symbol, type, side, amount=None, price=None, params={}
+    ):
+        await self.load_markets()
+        request = {
+            "walletType": self.safe_string(params, "walletType", "SPOT"),
+        }
+        if id is not None:
+            request["id"] = id
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        if price is not None:
+            request["limitPrice"] = self.price_to_precision(symbol, price)
+        if amount is not None:
+            request["amount"] = self.amount_to_precision(symbol, amount)
+        if symbol is not None:
+            request["pairName"] = self.market_id(symbol)
+        if side is not None:
+            request["side"] = self.safe_string(self.options["tradeSides"], side, side)
+        if type is not None:
+            request["type"] = self.upper(type)
+        response = await self.privatePutOrdersId(self.extend(request, params))
+        return self.parse_order(response)
+
+    async def cancel_order(self, id, symbol=None, params={}):
+        await self.load_markets()
+        request = {}
+        if id is not None:
+            request["id"] = int(id)
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        return await self.privateDeleteOrdersId(self.extend(request, params))
+
+    async def fetch_order(self, id, symbol=None, params={}):
+        await self.load_markets()
+        request = {}
+        if id is not None:
+            request["id"] = int(id)
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        response = await self.privateGetOrdersId(self.extend(request, params))
+        return self.parse_order(response)
+
+    async def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        if symbol is not None:
+            if not (symbol in self.markets):
+                raise ExchangeError(self.id + " has no symbol " + symbol)
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            urlParams["start"] = since
+        if limit is not None:
+            urlParams["limit"] = limit
+        urlParams["active"] = True
+        response = None
+        if symbol is not None:
+            marketId = self.market_id(symbol)
+            request["symbol"] = marketId
+            response = await self.privateGetOrdersSymbol(self.extend(request, params))
+        else:
+            response = await self.privateGetOrders(self.extend(request, params))
+        return self.parse_orders(self.safe_value(response, "items"), None, since, limit)
+
+    async def fetch_closed_orders(self, symbol=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            urlParams["start"] = since
+        if limit is not None:
+            urlParams["limit"] = limit
+        urlParams["active"] = False
+        response = None
+        if symbol is not None:
+            marketId = self.market_id(symbol)
+            request["symbol"] = marketId
+            response = await self.privateGetOrdersSymbol(self.extend(request, params))
+        else:
+            response = await self.privateGetOrders(self.extend(request, params))
+        return self.parse_orders(self.safe_value(response, "items"), None, since, limit)
+
+    def parse_order(self, order, market=None):
+        side = self.safe_string_lower(order, "side")
+        open = self.safe_value(order, "active")
+        status = None
+        if open:
+            status = "open"
+        else:
+            status = "closed"
+        symbol = None
+        if market is None:
+            marketId = self.safe_string(order, "pairName")
+            if marketId is not None:
+                if marketId in self.markets_by_id:
+                    market = self.markets_by_id[marketId][0]
+        if market is not None:
+            symbol = market["symbol"]
+        orderType = self.safe_string_lower(order, "type")
+        timestamp = self.safe_integer(order, "created")
+        id = self.safe_string(order, "id")
+        lastTradeTimestamp = None
+        if order.amount < order.originalAmount:
+            lastTradeTimestamp = timestamp
+        originalAmount = self.safe_float(order, "originalAmount")
+        amount = self.safe_float(order, "amount")
+        filled = originalAmount - amount
+        resultOrder = {
+            "info": order,
+            "id": id,
+            "clientOrderId": order["cid"],
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "lastTradeTimestamp": lastTradeTimestamp,
+            "symbol": symbol,
+            "type": orderType,
+            "side": side,
+            "average": None,
+            "amount": originalAmount,
+            "remaining": amount,
+            "filled": filled,
+            "status": status,
+            "fee": None,
+            "cost": None,
+            "trades": None,
+            "hidden": self.safe_value(order, "hidden"),
+        }
+        if "limitPrice" in order:
+            resultOrder["price"] = self.safe_float(order, "limitPrice")
+        if "stopPrice" in order:
+            resultOrder["stopPrice"] = self.safe_float(order, "stopPrice")
+        if "trailingPrice" in order:
+            resultOrder["trailingPrice"] = self.safe_float(order, "trailingPrice")
+        if "futurePrice" in order:
+            resultOrder["futurePrice"] = self.safe_float(order, "futurePrice")
+        if "distance" in order:
+            resultOrder["distance"] = self.safe_float(order, "distance")
+        return resultOrder
+
+    async def create_deposit_address(self, code, params={}):
+        await self.load_markets()
+        request = {
+            "currency": self.currency(code).id,
+        }
+        response = await self.privatePostWalletsCurrencyAddress(
+            self.extend(request, params)
+        )
+        address = self.safe_value(response, "address")
+        tag = self.safe_value(response, "tag")
+        self.check_address(address)
+        return {
+            "currency": code,
+            "address": address,
+            "tag": tag,
+            "info": response,
+        }
+
+    async def fetch_deposit_address(self, code, params={}):
+        await self.load_markets()
+        request = {
+            "currency": code,
+            "urlParams": {
+                "formatted": True,
+            },
+        }
+        response = await self.privateGetWalletsCurrencyAddress(
+            self.extend(request, params)
+        )
+        address = self.safe_value(response, "address")
+        tag = self.safe_value(response, "tag")
+        self.check_address(address)
+        return {
+            "currency": self.currency(code).id,
+            "address": address,
+            "tag": tag,
+            "info": response,
+        }
+
+    async def fetch_deposits(self, code=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        start = since is not since if None else 0
+        urlParams["start"] = start
+        urlParams["end"] = self.milliseconds()
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = None
+        if code is not None:
+            request["currency"] = self.currency(code).id
+            response = await self.privateGetWalletsCurrencyDeposits(
+                self.extend(request, params)
+            )
+        else:
+            response = await self.privateGetDeposits(self.extend(request, params))
+        deposits = self.safe_value(response, "items")
+        for i in range(0, len(deposits)):
+            deposits[i]["type"] = "DEPOSIT"
+        return self.parse_transactions(deposits, None, since, limit)
+
+    async def fetch_withdrawals(self, code=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            request["form"] = since
+        start = since is not since if None else 0
+        urlParams["start"] = start
+        urlParams["end"] = self.milliseconds()
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = None
+        if code is not None:
+            request["currency"] = self.currency(code).id
+            response = await self.privateGetWalletsCurrencyWithdrawals(
+                self.extend(request, params)
+            )
+        else:
+            response = await self.privateGetWithdrawals(self.extend(request, params))
+        withdrawals = self.safe_value(response, "items")
+        for i in range(0, len(withdrawals)):
+            withdrawals[i]["type"] = "WITHDRAWAL"
+        return self.parse_transactions(withdrawals, None, since, limit)
+
+    def parse_transaction(self, transaction, currency=None):
+        timestamp = self.safe_integer(transaction, "timestamp")
+        updated = self.safe_integer(transaction, "updated")
+        currencyId = self.safe_string(transaction, "currencyCode")
+        code = self.safe_currency_code(currencyId, currency)
+        type = self.safe_string_lower(transaction, "type")  # DEPOSIT or WITHDRAWAL
+        status = self.parse_transaction_status(self.safe_string(transaction, "status"))
+        feeCost = self.safe_float(transaction, "fee")
+        if feeCost is not None:
+            feeCost = abs(feeCost)
+        return {
+            "info": transaction,
+            "id": self.safe_string(transaction, "id"),
+            "txid": self.safe_string(transaction, "txHash"),
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "address": self.safe_string(
+                transaction, "walletId"
+            ),  # todo: self is actually the tag for XRP transfers(the address is missing)
+            "tag": None,  # refix it properly for the tag from description
+            "type": type,
+            "amount": self.safe_float(transaction, "amount"),
+            "currency": code,
+            "status": status,
+            "updated": updated,
+            "fee": {
+                "currency": code,
+                "cost": feeCost,
+                "rate": None,
+            },
+        }
+
+    def parse_transaction_status(self, status):
+        statuses = {
+            "PROCESSED": "pending",
+            "CANCELED": "canceled",
+            "COMPLETED": "ok",
+        }
+        return self.safe_string(statuses, status, status)
+
+    async def withdraw(self, code, amount, address, tag=None, params={}):
+        self.check_address(address)
+        await self.load_markets()
+        currency = self.currency(code)
+        destination = address
+        if tag is not None:
+            destination = address + ":" + tag
+        fee = currency.fee
+        request = {
+            "currency": currency.id,
+            "amount": self.sum(amount, fee),
+            "fee": fee,
+            "currencyCode": currency.id,
+            "destination": destination,
+        }
+        response = await self.privatePostWithdrawalsCurrency(
+            self.extend(request, params)
+        )
+        return {
+            "info": response,
+            "id": self.safe_string(response, "id"),
+        }
+
+    def nonce(self):
+        return self.milliseconds()
+
+    def sign(
+        self, path, api="public", method="GET", params={}, headers=None, body=None
+    ):
+        request = "/" + self.implode_params(path, params)
+        query = self.omit(params, self.extract_params(path))
+        apiUrls = self.urls["api"]
+        urlParams = self.safe_value(query, "urlParams")
+        url = apiUrls[api] + request
+        urlParamsStr = self.urlencode(urlParams) if (urlParams is not None) else ""
+        if urlParamsStr != "":
+            url += "?" + urlParamsStr
+        requestBody = self.omit(query, "urlParams")
+        if api == "private":
+            self.check_required_credentials()
+            nonce = str(self.nonce())
+            urlPath = self.options["paths"]["private"] + request
+            payloadSuffix = ""
+            if method != "GET" and method != "DELETE":
+                body = self.json(requestBody)
+                payloadSuffix = body
+            payload = "/api" + urlPath + nonce + payloadSuffix
+            payload = self.encode(payload)
+            secret = self.encode(self.secret)
+            signature = self.hmac(payload, secret, hashlib.sha384).upper()
+            contentType = "application/json; charset=UTF-8"
+            headers = {
+                "Content-Type": contentType,
+                "nominex-nonce": nonce,
+                "nominex-apikey": self.apiKey,
+                "nominex-signature": signature,
+            }
+        return {"url": url, "method": method, "body": body, "headers": headers}
+
+    def handle_errors(
+        self,
+        code,
+        reason,
+        url,
+        method,
+        headers,
+        body,
+        response,
+        requestHeaders,
+        requestBody,
+    ):
+        if response is None:
+            return
+        if code >= 400:
+            if body[0] == "{":
+                feedback = self.id + " " + body
+                if "code" in response:
+                    code = self.safe_string(response, "code")
+                    self.throw_exactly_matched_exception(
+                        self.exceptions, code, feedback
+                    )
+                if "codes" in response:
+                    codes = self.safe_string(response, "codes")
+                    code = self.asString(codes[0])
+                    self.throw_exactly_matched_exception(
+                        self.exceptions, code, feedback
+                    )
+                raise ExchangeError(feedback)  # unknown message
+            elif body[0] == "[":
+                feedback = self.id + " " + body
+                error = response[0]
+                code = self.safe_string(error, "code")
+                self.throw_exactly_matched_exception(self.exceptions, code, feedback)
+                raise ExchangeError(feedback)  # unknown message
```

### Comparing `ccxt-unmerged-2.2/ccxt_unmerged/async_support/nominex.py` & `ccxt_unmerged-4.0/ccxt_unmerged/nominex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,812 +1,879 @@
-# -*- coding: utf-8 -*-
-
-# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
-# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
-
-from ccxt.async_support.base.exchange import Exchange
-import hashlib
-from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import PermissionDenied
-from ccxt.base.errors import ArgumentsRequired
-from ccxt.base.errors import BadRequest
-from ccxt.base.errors import BadSymbol
-from ccxt.base.errors import InsufficientFunds
-from ccxt.base.errors import InvalidAddress
-from ccxt.base.errors import InvalidOrder
-from ccxt.base.errors import OrderNotFound
-from ccxt.base.errors import DuplicateOrderId
-from ccxt.base.errors import RateLimitExceeded
-from ccxt.base.errors import InvalidNonce
-from ccxt.base.decimal_to_precision import TICK_SIZE
-
-
-class nominex(Exchange):
-
-    def describe(self):
-        return self.deep_extend(super(nominex, self).describe(), {
-            'id': 'nominex',
-            'name': 'Nominex',
-            'countries': ['SC'],
-            'rateLimit': 1500,
-            'certified': False,
-            'pro': False,
-            'has': {
-                'CORS': False,
-                'fetchCurrencies': True,
-                'fetchOHLCV': True,
-                'cancelAllOrders': False,
-                'createDepositAddress': True,
-                'deposit': False,
-                'fetchClosedOrders': True,
-                'fetchDepositAddress': True,
-                'fetchTradingFees': True,
-                'fetchMyTrades': True,
-                'fetchOrder': True,
-                'fetchOpenOrders': True,
-                'fetchTickers': True,
-                'fetchDeposits': True,
-                'fetchWithdrawals': True,
-                'withdraw': True,
-            },
-            'timeframes': {
-                '1m': 'TF1M',
-                '5m': 'TF5M',
-                '15m': 'TF15M',
-                '30m': 'TF30M',
-                '1h': 'TF1H',
-                '3h': 'TF3H',
-                '6h': 'TF6H',
-                '12h': 'TF12H',
-                '1d': 'TF1D',
-                '1w': 'TF7D',
-                '2w': 'TF14D',
-                '1M': 'TF1MO',
-            },
-            'urls': {
-                'logo': 'https://nominex.io/media/nominex-logo.png',
-                'api': {
-                    'public': 'https://nominex.io/api/rest/v1',
-                    'private': 'https://nominex.io/api/rest/v1/private',
-                },
-                'demo': {
-                    'public': 'https://demo.nominex.io/api/rest/v1',
-                    'private': 'https://demo.nominex.io/api/rest/v1/private',
-                },
-                'www': 'https://nominex.io',
-                'doc': [
-                    'https://developer.nominex.io/',
-                ],
-            },
-            'api': {
-                'public': {
-                    'get': [
-                        'currencies',
-                        'pairs',
-                        'ticker/{symbol}',
-                        'ticker',
-                        'orderbook/{symbol}/A0/{limit}',
-                        'candles/{symbol}/{timeframe}',
-                        'trades/{symbol}',
-                    ],
-                },
-                'private': {
-                    'get': [
-                        'trading-fee-rates',
-                        'deposits',
-                        'withdrawals',
-                        'orders',
-                        'orders/{id}',
-                        'orders/{symbol}',
-                        'trades/{symbol}',
-                        'wallets',
-                        'wallets/{currency}/address',
-                        'wallets/{currency}/deposits',
-                        'wallets/{currency}/withdrawals',
-                    ],
-                    'post': [
-                        'orders',
-                        'wallets/{currency}/address',
-                        'withdrawals/{currency}',
-                    ],
-                    'put': [
-                        'orders/{id}',
-                    ],
-                    'delete': [
-                        'orders/{id}',
-                    ],
-                },
-            },
-            'fees': {
-                'trading': {
-                    'tierBased': True,
-                    'percentage': True,
-                },
-                'funding': {
-                    'tierBased': False,  # True for tier-based/progressive
-                },
-            },
-            'exceptions': {
-                '100.2': BadSymbol,
-                '101': InvalidNonce,
-                '103': AuthenticationError,
-                '103.4': InvalidOrder,
-                '104.4': InvalidOrder,
-                '110.110': RateLimitExceeded,
-                '121': PermissionDenied,
-                '601': BadRequest,
-                '1101': InsufficientFunds,
-                '1102': DuplicateOrderId,
-                '1106': OrderNotFound,
-                '20002': InvalidAddress,
-            },
-            'precisionMode': TICK_SIZE,
-            'options': {
-                'tradeSides': {
-                    'buy': 'BUY',
-                    'sell': 'SELL',
-                },
-                'paths': {
-                    'public': '/api/rest/v1',
-                    'private': '/api/rest/v1/private',
-                },
-            },
-        })
-
-    async def fetch_trading_fees(self, params={}):
-        await self.load_markets()
-        response = await self.privateGetTradingFeeRates(params)
-        return {
-            'info': response,
-            'maker': self.safe_float(response, 'makerFeeFactor') * 100.0,
-            'taker': self.safe_float(response, 'takerFeeFactor') * 100.0,
-        }
-
-    async def fetch_currencies(self, params={}):
-        currencies = await self.publicGetCurrencies(params)
-        result = {}
-        for i in range(0, len(currencies)):
-            currency = self.parse_currency(currencies[i])
-            currencyCode = self.safe_string(currency, 'code')
-            result[currencyCode] = currency
-        return result
-
-    def parse_currency(self, currency):
-        code = self.safe_string(currency, 'code')
-        return {
-            'id': code,
-            'code': code,
-            'name': self.safe_string(currency, 'name'),
-            'active': True,
-            'fee': self.safe_float(currency, 'withdrawalFee'),
-            'precision': self.safe_integer(currency, 'scale'),
-            'info': currency,
-        }
-
-    async def fetch_markets(self, params={}):
-        pairs = await self.publicGetPairs(params)
-        result = []
-        for i in range(0, len(pairs)):
-            market = pairs[i]
-            id = self.safe_string(market, 'name')
-            parts = id.split('/')
-            baseId = parts[0]
-            quoteId = parts[1]
-            base = self.safe_currency_code(baseId)
-            quote = self.safe_currency_code(quoteId)
-            symbol = base + '/' + quote
-            precision = {
-                'price': self.safe_float(market, 'quoteStep'),
-                'amount': self.safe_float(market, 'baseStep'),
-            }
-            limits = {
-                'amount': {
-                    'min': self.safe_float(market, 'minBaseAmount'),
-                    'max': self.safe_float(market, 'maxBaseAmount'),
-                },
-                'cost': {
-                    'min': self.safe_float(market, 'minQuoteAmount'),
-                    'max': self.safe_float(market, 'maxQuoteAmount'),
-                },
-            }
-            result.append({
-                'id': id,
-                'symbol': symbol,
-                'base': base,
-                'quote': quote,
-                'baseId': baseId,
-                'quoteId': quoteId,
-                'active': self.safe_value(market, 'active'),
-                'precision': precision,
-                'limits': limits,
-                'info': market,
-            })
-        return result
-
-    async def fetch_balance(self, params={}):
-        await self.load_markets()
-        balanceType = self.safe_string(params, 'type', 'SPOT')
-        query = self.omit(params, 'type')
-        response = await self.privateGetWallets(query)
-        result = {'info': response}
-        for i in range(0, len(response)):
-            balance = response[i]
-            if balance['type'] == balanceType:
-                currencyId = self.safe_string(balance, 'currency')
-                code = self.safe_currency_code(currencyId)
-                if not (code in result):
-                    account = self.account()
-                    account['free'] = self.safe_float(balance, 'balanceAvailable')
-                    account['total'] = self.safe_float(balance, 'balance')
-                    result[code] = account
-        return self.parse_balance(result)
-
-    async def fetch_order_book(self, symbol, limit=None, params={}):
-        await self.load_markets()
-        request = {
-            'symbol': self.market_id(symbol),
-            'limit': 100,
-        }
-        if limit == 25:
-            request['limit'] = limit
-        response = await self.publicGetOrderbookSymbolA0Limit(self.extend(request, params))
-        asks = []
-        bids = []
-        for i in range(0, len(response)):
-            priceLevel = response[i]
-            side = self.safe_string(priceLevel, 'side')
-            if side == 'SELL':
-                asks.append(priceLevel)
-            else:
-                bids.append(priceLevel)
-        return self.parse_order_book({'asks': asks, 'bids': bids}, symbol, None, 'bids', 'asks', 'price', 'amount')
-
-    async def fetch_tickers(self, symbols=None, params={}):
-        await self.load_markets()
-        urlParams = {}
-        request = {'urlParams': urlParams}
-        ids = list(self.markets.keys())
-        if symbols is not None:
-            for i in range(0, len(symbols)):
-                symbol = symbols[i]
-                market = self.market(symbol)
-                ids.append(market['id'])
-        urlParams['pairs'] = ','.join(ids)
-        response = await self.publicGetTicker(self.extend(request, params))
-        result = {}
-        for i in range(0, len(response)):
-            marketId = ids[i]
-            market = self.markets[marketId]
-            ticker = self.parse_ticker(response[i], market)
-            symbol = market['symbol']
-            result[symbol] = ticker
-        return result
-
-    async def fetch_ticker(self, symbol, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'symbol': market['id'],
-        }
-        ticker = await self.publicGetTickerSymbol(self.extend(request, params))
-        return self.parse_ticker(ticker, market)
-
-    def parse_ticker(self, ticker, market=None):
-        timestamp = self.safe_integer(ticker, 'timestamp')
-        symbol = None
-        if market is not None:
-            symbol = market['symbol']
-        elif 'pair' in ticker:
-            marketId = self.safe_string(ticker, 'pair')
-            if marketId is not None:
-                if marketId in self.markets_by_id:
-                    market = self.markets_by_id[marketId]
-                    symbol = market['symbol']
-                else:
-                    baseId = marketId[0:3]
-                    quoteId = marketId[3:6]
-                    base = self.safe_currency_code(baseId)
-                    quote = self.safe_currency_code(quoteId)
-                    symbol = base + '/' + quote
-        last = self.safe_float(ticker, 'price')
-        change = self.safe_float(ticker, 'dailyChange')
-        open = None
-        average = None
-        if last is not None and change is not None:
-            open = last - change
-            average = (open + last) / 2
-        volume = self.safe_float(ticker, 'baseVolume')
-        quoteVolume = self.safe_float(ticker, 'quoteVolume')
-        vwap = (quoteVolume / volume) if (quoteVolume is not None and volume is not None and volume != 0) else None
-        return {
-            'symbol': symbol,
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'high': self.safe_float(ticker, 'high'),
-            'low': self.safe_float(ticker, 'low'),
-            'bid': self.safe_float(ticker, 'bid'),
-            'bidVolume': self.safe_float(ticker, 'bidSize'),
-            'ask': self.safe_float(ticker, 'ask'),
-            'askVolume': self.safe_float(ticker, 'askSize'),
-            'vwap': vwap,
-            'open': open,
-            'close': last,
-            'last': last,
-            'previousClose': None,
-            'change': change,
-            'percentage': self.safe_float(ticker, 'dailyChangeP'),
-            'average': average,
-            'baseVolume': volume,
-            'quoteVolume': quoteVolume,
-            'info': ticker,
-        }
-
-    def parse_ohlcv(self, ohlcv, market=None, timeframe='1m', since=None, limit=None):
-        return [
-            self.safe_integer(ohlcv, 'timestamp'),
-            self.safe_float(ohlcv, 'open'),
-            self.safe_float(ohlcv, 'high'),
-            self.safe_float(ohlcv, 'low'),
-            self.safe_float(ohlcv, 'close'),
-            self.safe_float(ohlcv, 'volume'),
-        ]
-
-    async def fetch_ohlcv(self, symbol, timeframe='1m', since=None, limit=None, params={}):
-        await self.load_markets()
-        if limit is None:
-            limit = 100
-        market = self.market(symbol)
-        urlParams = {
-            'limit': limit,
-            'end': self.milliseconds(),
-        }
-        request = {
-            'symbol': market['id'],
-            'timeframe': self.timeframes[timeframe],
-            'urlParams': urlParams,
-        }
-        if since is not None:
-            request['start'] = since
-        response = await self.publicGetCandlesSymbolTimeframe(self.extend(request, params))
-        return self.parse_ohlcvs(response, market, timeframe, since, limit)
-
-    def parse_trade(self, trade, market):
-        id = self.safe_string(trade, 'id')
-        timestamp = self.safe_integer(trade, 'timestamp')
-        type = None
-        side = self.safe_string_lower(trade, 'side').lower()
-        orderId = None
-        if 'orderId' in trade:
-            orderId = self.safe_string(trade, 'orderId')
-        price = self.safe_float(trade, 'price')
-        amount = self.safe_float(trade, 'amount')
-        cost = None
-        if price is not None:
-            if amount is not None:
-                cost = price * amount
-        takerOrMaker = None
-        if 'maker' in trade:
-            maker = self.safe_value(trade, 'maker')
-            takerOrMaker = 'maker' if maker else 'taker'
-        feeAmount = self.safe_float(trade, 'fee')
-        fee = feeAmount is None if None else {
-            'cost': feeAmount,
-            'currency': self.safe_string(trade, 'feeCurrencyCode'),
-        }
-        return {
-            'id': id,
-            'info': trade,
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'symbol': market['symbol'],
-            'type': type,
-            'order': orderId,
-            'side': side,
-            'takerOrMaker': takerOrMaker,
-            'price': price,
-            'amount': amount,
-            'cost': cost,
-            'fee': fee,
-        }
-
-    async def fetch_trades(self, symbol, since=None, limit=50, params={}):
-        await self.load_markets()
-        market = self.market(symbol)
-        urlParams = {}
-        request = {
-            'symbol': market['id'],
-            'urlParams': urlParams,
-        }
-        if since is not None:
-            urlParams['start'] = int(since)
-        if limit is not None:
-            urlParams['limit'] = limit
-        response = await self.publicGetTradesSymbol(self.extend(request, params))
-        return self.parse_trades(self.safe_value(response, 'items'), market, since, limit)
-
-    def calculate_fee(self, symbol, type, side, amount, price, takerOrMaker='taker', params={}):
-        market = self.markets[symbol]
-        rate = market[takerOrMaker]
-        cost = amount * rate
-        key = 'quote'
-        if side == 'sell':
-            cost *= price
-        else:
-            key = 'base'
-        code = market[key]
-        currency = self.safe_value(self.currencies, code)
-        if currency is not None:
-            precision = self.safe_integer(currency, 'precision')
-            if precision is not None:
-                cost = float(self.currency_to_precision(code, cost))
-        return {
-            'type': takerOrMaker,
-            'currency': market[key],
-            'rate': rate,
-            'cost': cost,
-        }
-
-    async def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
-        if symbol is None:
-            raise ArgumentsRequired(self.id + ' fetchMyTrades requires a `symbol` argument')
-        await self.load_markets()
-        market = self.market(symbol)
-        urlParams = {}
-        request = {
-            'symbol': market['id'],
-            'urlParams': urlParams,
-        }
-        if limit is not None:
-            urlParams['limit'] = limit
-        if since is not None:
-            urlParams['start'] = int(since)
-        response = await self.privateGetTradesSymbol(self.extend(request, params))
-        return self.parse_trades(self.safe_value(response, 'items'), market, since, limit)
-
-    async def create_order(self, symbol, type, side, amount, price=None, params={}):
-        await self.load_markets()
-        marketId = self.market_id(symbol)
-        request = {
-            'pairName': marketId,
-            'side': self.safe_string(self.options['tradeSides'], side, side),
-            'amount': self.amount_to_precision(symbol, amount),
-            'type': self.upper(type),
-            'walletType': self.safe_string(params, 'walletType', 'SPOT'),
-        }
-        if 'clientOrderId' in params:
-            request['cid'] = self.safe_integer(params, 'clientOrderId')
-        if type == 'limit':
-            request['limitPrice'] = self.price_to_precision(symbol, price)
-        response = await self.privatePostOrders(self.extend(request, params))
-        return self.parse_order(response)
-
-    async def edit_order(self, id, symbol, type, side, amount=None, price=None, params={}):
-        await self.load_markets()
-        request = {
-            'walletType': self.safe_string(params, 'walletType', 'SPOT'),
-        }
-        if id is not None:
-            request['id'] = id
-        elif 'clientOrderId' in params:
-            request['id'] = self.safe_integer(params, 'clientOrderId')
-            request['urlParams'] = {'cid': True}
-        if price is not None:
-            request['limitPrice'] = self.price_to_precision(symbol, price)
-        if amount is not None:
-            request['amount'] = self.amount_to_precision(symbol, amount)
-        if symbol is not None:
-            request['pairName'] = self.market_id(symbol)
-        if side is not None:
-            request['side'] = self.safe_string(self.options['tradeSides'], side, side)
-        if type is not None:
-            request['type'] = self.upper(type)
-        response = await self.privatePutOrdersId(self.extend(request, params))
-        return self.parse_order(response)
-
-    async def cancel_order(self, id, symbol=None, params={}):
-        await self.load_markets()
-        request = {}
-        if id is not None:
-            request['id'] = int(id)
-        elif 'clientOrderId' in params:
-            request['id'] = self.safe_integer(params, 'clientOrderId')
-            request['urlParams'] = {'cid': True}
-        return await self.privateDeleteOrdersId(self.extend(request, params))
-
-    async def fetch_order(self, id, symbol=None, params={}):
-        await self.load_markets()
-        request = {}
-        if id is not None:
-            request['id'] = int(id)
-        elif 'clientOrderId' in params:
-            request['id'] = self.safe_integer(params, 'clientOrderId')
-            request['urlParams'] = {'cid': True}
-        response = await self.privateGetOrdersId(self.extend(request, params))
-        return self.parse_order(response)
-
-    async def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        if symbol is not None:
-            if not (symbol in self.markets):
-                raise ExchangeError(self.id + ' has no symbol ' + symbol)
-        urlParams = {}
-        request = {'urlParams': urlParams}
-        if since is not None:
-            urlParams['start'] = since
-        if limit is not None:
-            urlParams['limit'] = limit
-        urlParams['active'] = True
-        response = None
-        if symbol is not None:
-            marketId = self.market_id(symbol)
-            request['symbol'] = marketId
-            response = await self.privateGetOrdersSymbol(self.extend(request, params))
-        else:
-            response = await self.privateGetOrders(self.extend(request, params))
-        return self.parse_orders(self.safe_value(response, 'items'), None, since, limit)
-
-    async def fetch_closed_orders(self, symbol=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        urlParams = {}
-        request = {'urlParams': urlParams}
-        if since is not None:
-            urlParams['start'] = since
-        if limit is not None:
-            urlParams['limit'] = limit
-        urlParams['active'] = False
-        response = None
-        if symbol is not None:
-            marketId = self.market_id(symbol)
-            request['symbol'] = marketId
-            response = await self.privateGetOrdersSymbol(self.extend(request, params))
-        else:
-            response = await self.privateGetOrders(self.extend(request, params))
-        return self.parse_orders(self.safe_value(response, 'items'), None, since, limit)
-
-    def parse_order(self, order, market=None):
-        side = self.safe_string_lower(order, 'side')
-        open = self.safe_value(order, 'active')
-        status = None
-        if open:
-            status = 'open'
-        else:
-            status = 'closed'
-        symbol = None
-        if market is None:
-            marketId = self.safe_string(order, 'pairName')
-            if marketId is not None:
-                if marketId in self.markets_by_id:
-                    market = self.markets_by_id[marketId]
-        if market is not None:
-            symbol = market['symbol']
-        orderType = self.safe_string_lower(order, 'type')
-        timestamp = self.safe_integer(order, 'created')
-        id = self.safe_string(order, 'id')
-        lastTradeTimestamp = None
-        if order.amount < order.originalAmount:
-            lastTradeTimestamp = timestamp
-        originalAmount = self.safe_float(order, 'originalAmount')
-        amount = self.safe_float(order, 'amount')
-        filled = originalAmount - amount
-        resultOrder = {
-            'info': order,
-            'id': id,
-            'clientOrderId': order['cid'],
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'lastTradeTimestamp': lastTradeTimestamp,
-            'symbol': symbol,
-            'type': orderType,
-            'side': side,
-            'average': None,
-            'amount': originalAmount,
-            'remaining': amount,
-            'filled': filled,
-            'status': status,
-            'fee': None,
-            'cost': None,
-            'trades': None,
-            'hidden': self.safe_value(order, 'hidden'),
-        }
-        if 'limitPrice' in order:
-            resultOrder['price'] = self.safe_float(order, 'limitPrice')
-        if 'stopPrice' in order:
-            resultOrder['stopPrice'] = self.safe_float(order, 'stopPrice')
-        if 'trailingPrice' in order:
-            resultOrder['trailingPrice'] = self.safe_float(order, 'trailingPrice')
-        if 'futurePrice' in order:
-            resultOrder['futurePrice'] = self.safe_float(order, 'futurePrice')
-        if 'distance' in order:
-            resultOrder['distance'] = self.safe_float(order, 'distance')
-        return resultOrder
-
-    async def create_deposit_address(self, code, params={}):
-        await self.load_markets()
-        request = {
-            'currency': self.currency(code).id,
-        }
-        response = await self.privatePostWalletsCurrencyAddress(self.extend(request, params))
-        address = self.safe_value(response, 'address')
-        tag = self.safe_value(response, 'tag')
-        self.check_address(address)
-        return {
-            'currency': code,
-            'address': address,
-            'tag': tag,
-            'info': response,
-        }
-
-    async def fetch_deposit_address(self, code, params={}):
-        await self.load_markets()
-        request = {
-            'currency': code,
-            'urlParams': {
-                'formatted': True,
-            },
-        }
-        response = await self.privateGetWalletsCurrencyAddress(self.extend(request, params))
-        address = self.safe_value(response, 'address')
-        tag = self.safe_value(response, 'tag')
-        self.check_address(address)
-        return {
-            'currency': self.currency(code).id,
-            'address': address,
-            'tag': tag,
-            'info': response,
-        }
-
-    async def fetch_deposits(self, code=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        urlParams = {}
-        request = {'urlParams': urlParams}
-        start = since is not since if None else 0
-        urlParams['start'] = start
-        urlParams['end'] = self.milliseconds()
-        if limit is not None:
-            urlParams['limit'] = limit
-        response = None
-        if code is not None:
-            request['currency'] = self.currency(code).id
-            response = await self.privateGetWalletsCurrencyDeposits(self.extend(request, params))
-        else:
-            response = await self.privateGetDeposits(self.extend(request, params))
-        deposits = self.safe_value(response, 'items')
-        for i in range(0, len(deposits)):
-            deposits[i]['type'] = 'DEPOSIT'
-        return self.parse_transactions(deposits, None, since, limit)
-
-    async def fetch_withdrawals(self, code=None, since=None, limit=None, params={}):
-        await self.load_markets()
-        urlParams = {}
-        request = {'urlParams': urlParams}
-        if since is not None:
-            request['form'] = since
-        start = since is not since if None else 0
-        urlParams['start'] = start
-        urlParams['end'] = self.milliseconds()
-        if limit is not None:
-            urlParams['limit'] = limit
-        response = None
-        if code is not None:
-            request['currency'] = self.currency(code).id
-            response = await self.privateGetWalletsCurrencyWithdrawals(self.extend(request, params))
-        else:
-            response = await self.privateGetWithdrawals(self.extend(request, params))
-        withdrawals = self.safe_value(response, 'items')
-        for i in range(0, len(withdrawals)):
-            withdrawals[i]['type'] = 'WITHDRAWAL'
-        return self.parse_transactions(withdrawals, None, since, limit)
-
-    def parse_transaction(self, transaction, currency=None):
-        timestamp = self.safe_integer(transaction, 'timestamp')
-        updated = self.safe_integer(transaction, 'updated')
-        currencyId = self.safe_string(transaction, 'currencyCode')
-        code = self.safe_currency_code(currencyId, currency)
-        type = self.safe_string_lower(transaction, 'type')  # DEPOSIT or WITHDRAWAL
-        status = self.parse_transaction_status(self.safe_string(transaction, 'status'))
-        feeCost = self.safe_float(transaction, 'fee')
-        if feeCost is not None:
-            feeCost = abs(feeCost)
-        return {
-            'info': transaction,
-            'id': self.safe_string(transaction, 'id'),
-            'txid': self.safe_string(transaction, 'txHash'),
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'address': self.safe_string(transaction, 'walletId'),  # todo: self is actually the tag for XRP transfers(the address is missing)
-            'tag': None,  # refix it properly for the tag from description
-            'type': type,
-            'amount': self.safe_float(transaction, 'amount'),
-            'currency': code,
-            'status': status,
-            'updated': updated,
-            'fee': {
-                'currency': code,
-                'cost': feeCost,
-                'rate': None,
-            },
-        }
-
-    def parse_transaction_status(self, status):
-        statuses = {
-            'PROCESSED': 'pending',
-            'CANCELED': 'canceled',
-            'COMPLETED': 'ok',
-        }
-        return self.safe_string(statuses, status, status)
-
-    async def withdraw(self, code, amount, address, tag=None, params={}):
-        self.check_address(address)
-        await self.load_markets()
-        currency = self.currency(code)
-        destination = address
-        if tag is not None:
-            destination = address + ':' + tag
-        fee = currency.fee
-        request = {
-            'currency': currency.id,
-            'amount': self.sum(amount, fee),
-            'fee': fee,
-            'currencyCode': currency.id,
-            'destination': destination,
-        }
-        response = await self.privatePostWithdrawalsCurrency(self.extend(request, params))
-        return {
-            'info': response,
-            'id': self.safe_string(response, 'id'),
-        }
-
-    def nonce(self):
-        return self.milliseconds()
-
-    def sign(self, path, api='public', method='GET', params={}, headers=None, body=None):
-        request = '/' + self.implode_params(path, params)
-        query = self.omit(params, self.extract_params(path))
-        apiUrls = self.urls['api']
-        urlParams = self.safe_value(query, 'urlParams')
-        url = apiUrls[api] + request
-        urlParamsStr = self.urlencode(urlParams) if (urlParams is not None) else ''
-        if urlParamsStr != '':
-            url += '?' + urlParamsStr
-        requestBody = self.omit(query, 'urlParams')
-        if api == 'private':
-            self.check_required_credentials()
-            nonce = str(self.nonce())
-            urlPath = self.options['paths']['private'] + request
-            payloadSuffix = ''
-            if method != 'GET' and method != 'DELETE':
-                body = self.json(requestBody)
-                payloadSuffix = body
-            payload = '/api' + urlPath + nonce + payloadSuffix
-            payload = self.encode(payload)
-            secret = self.encode(self.secret)
-            signature = self.hmac(payload, secret, hashlib.sha384).upper()
-            contentType = 'application/json; charset=UTF-8'
-            headers = {
-                'Content-Type': contentType,
-                'nominex-nonce': nonce,
-                'nominex-apikey': self.apiKey,
-                'nominex-signature': signature,
-            }
-        return {'url': url, 'method': method, 'body': body, 'headers': headers}
-
-    def handle_errors(self, code, reason, url, method, headers, body, response, requestHeaders, requestBody):
-        if response is None:
-            return
-        if code >= 400:
-            if body[0] == '{':
-                feedback = self.id + ' ' + body
-                if 'code' in response:
-                    code = self.safe_string(response, 'code')
-                    self.throw_exactly_matched_exception(self.exceptions, code, feedback)
-                if 'codes' in response:
-                    codes = self.safe_string(response, 'codes')
-                    code = self.asString(codes[0])
-                    self.throw_exactly_matched_exception(self.exceptions, code, feedback)
-                raise ExchangeError(feedback)  # unknown message
-            elif body[0] == '[':
-                feedback = self.id + ' ' + body
-                error = response[0]
-                code = self.safe_string(error, 'code')
-                self.throw_exactly_matched_exception(self.exceptions, code, feedback)
-                raise ExchangeError(feedback)  # unknown message
+# -*- coding: utf-8 -*-
+
+# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
+# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
+
+from ccxt.base.exchange import Exchange
+import hashlib
+from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import PermissionDenied
+from ccxt.base.errors import ArgumentsRequired
+from ccxt.base.errors import BadRequest
+from ccxt.base.errors import BadSymbol
+from ccxt.base.errors import InsufficientFunds
+from ccxt.base.errors import InvalidAddress
+from ccxt.base.errors import InvalidOrder
+from ccxt.base.errors import OrderNotFound
+from ccxt.base.errors import DuplicateOrderId
+from ccxt.base.errors import RateLimitExceeded
+from ccxt.base.errors import InvalidNonce
+from ccxt.base.decimal_to_precision import TICK_SIZE
+
+
+class nominex(Exchange):
+    def describe(self):
+        return self.deep_extend(
+            super(nominex, self).describe(),
+            {
+                "id": "nominex",
+                "name": "Nominex",
+                "countries": ["SC"],
+                "rateLimit": 1500,
+                "certified": False,
+                "pro": False,
+                "has": {
+                    "CORS": False,
+                    "fetchCurrencies": True,
+                    "fetchOHLCV": True,
+                    "cancelAllOrders": False,
+                    "createDepositAddress": True,
+                    "deposit": False,
+                    "fetchClosedOrders": True,
+                    "fetchDepositAddress": True,
+                    "fetchTradingFees": True,
+                    "fetchMyTrades": True,
+                    "fetchOrder": True,
+                    "fetchOpenOrders": True,
+                    "fetchTickers": True,
+                    "fetchDeposits": True,
+                    "fetchWithdrawals": True,
+                    "withdraw": True,
+                },
+                "timeframes": {
+                    "1m": "TF1M",
+                    "5m": "TF5M",
+                    "15m": "TF15M",
+                    "30m": "TF30M",
+                    "1h": "TF1H",
+                    "3h": "TF3H",
+                    "6h": "TF6H",
+                    "12h": "TF12H",
+                    "1d": "TF1D",
+                    "1w": "TF7D",
+                    "2w": "TF14D",
+                    "1M": "TF1MO",
+                },
+                "urls": {
+                    "logo": "https://nominex.io/media/nominex-logo.png",
+                    "api": {
+                        "public": "https://nominex.io/api/rest/v1",
+                        "private": "https://nominex.io/api/rest/v1/private",
+                    },
+                    "demo": {
+                        "public": "https://demo.nominex.io/api/rest/v1",
+                        "private": "https://demo.nominex.io/api/rest/v1/private",
+                    },
+                    "www": "https://nominex.io",
+                    "doc": [
+                        "https://developer.nominex.io/",
+                    ],
+                },
+                "api": {
+                    "public": {
+                        "get": [
+                            "currencies",
+                            "pairs",
+                            "ticker/{symbol}",
+                            "ticker",
+                            "orderbook/{symbol}/A0/{limit}",
+                            "candles/{symbol}/{timeframe}",
+                            "trades/{symbol}",
+                        ],
+                    },
+                    "private": {
+                        "get": [
+                            "trading-fee-rates",
+                            "deposits",
+                            "withdrawals",
+                            "orders",
+                            "orders/{id}",
+                            "orders/{symbol}",
+                            "trades/{symbol}",
+                            "wallets",
+                            "wallets/{currency}/address",
+                            "wallets/{currency}/deposits",
+                            "wallets/{currency}/withdrawals",
+                        ],
+                        "post": [
+                            "orders",
+                            "wallets/{currency}/address",
+                            "withdrawals/{currency}",
+                        ],
+                        "put": [
+                            "orders/{id}",
+                        ],
+                        "delete": [
+                            "orders/{id}",
+                        ],
+                    },
+                },
+                "fees": {
+                    "trading": {
+                        "tierBased": True,
+                        "percentage": True,
+                    },
+                    "funding": {
+                        "tierBased": False,  # True for tier-based/progressive
+                    },
+                },
+                "exceptions": {
+                    "100.2": BadSymbol,
+                    "101": InvalidNonce,
+                    "103": AuthenticationError,
+                    "103.4": InvalidOrder,
+                    "104.4": InvalidOrder,
+                    "110.110": RateLimitExceeded,
+                    "121": PermissionDenied,
+                    "601": BadRequest,
+                    "1101": InsufficientFunds,
+                    "1102": DuplicateOrderId,
+                    "1106": OrderNotFound,
+                    "20002": InvalidAddress,
+                },
+                "precisionMode": TICK_SIZE,
+                "options": {
+                    "tradeSides": {
+                        "buy": "BUY",
+                        "sell": "SELL",
+                    },
+                    "paths": {
+                        "public": "/api/rest/v1",
+                        "private": "/api/rest/v1/private",
+                    },
+                },
+            },
+        )
+
+    def fetch_trading_fees(self, params={}):
+        self.load_markets()
+        response = self.privateGetTradingFeeRates(params)
+        return {
+            "info": response,
+            "maker": self.safe_float(response, "makerFeeFactor") * 100.0,
+            "taker": self.safe_float(response, "takerFeeFactor") * 100.0,
+        }
+
+    def fetch_currencies(self, params={}):
+        currencies = self.publicGetCurrencies(params)
+        result = {}
+        for i in range(0, len(currencies)):
+            currency = self.parse_currency(currencies[i])
+            currencyCode = self.safe_string(currency, "code")
+            result[currencyCode] = currency
+        return result
+
+    def parse_currency(self, currency):
+        code = self.safe_string(currency, "code")
+        return {
+            "id": code,
+            "code": code,
+            "name": self.safe_string(currency, "name"),
+            "active": True,
+            "fee": self.safe_float(currency, "withdrawalFee"),
+            "precision": self.safe_integer(currency, "scale"),
+            "info": currency,
+        }
+
+    def fetch_markets(self, params={}):
+        pairs = self.publicGetPairs(params)
+        result = []
+        for i in range(0, len(pairs)):
+            market = pairs[i]
+            id = self.safe_string(market, "name")
+            parts = id.split("/")
+            baseId = parts[0]
+            quoteId = parts[1]
+            base = self.safe_currency_code(baseId)
+            quote = self.safe_currency_code(quoteId)
+            symbol = base + "/" + quote
+            precision = {
+                "price": self.safe_float(market, "quoteStep"),
+                "amount": self.safe_float(market, "baseStep"),
+            }
+            limits = {
+                "amount": {
+                    "min": self.safe_float(market, "minBaseAmount"),
+                    "max": self.safe_float(market, "maxBaseAmount"),
+                },
+                "cost": {
+                    "min": self.safe_float(market, "minQuoteAmount"),
+                    "max": self.safe_float(market, "maxQuoteAmount"),
+                },
+            }
+            result.append(
+                {
+                    "id": id,
+                    "symbol": symbol,
+                    "base": base,
+                    "quote": quote,
+                    "settle": None,
+                    "baseId": baseId,
+                    "quoteId": quoteId,
+                    "settleId": None,
+                    "type": "spot",
+                    "spot": True,
+                    "margin": False,
+                    "swap": False,
+                    "future": False,
+                    "option": False,
+                    "contract": False,
+                    "linear": None,
+                    "inverse": None,
+                    "contractSize": None,
+                    "expiry": None,
+                    "expiryDatetime": None,
+                    "strike": None,
+                    "optionType": None,
+                    "active": self.safe_value(market, "active"),
+                    "precision": precision,
+                    "limits": limits,
+                    "info": market,
+                }
+            )
+        return result
+
+    def fetch_balance(self, params={}):
+        self.load_markets()
+        balanceType = self.safe_string(params, "type", "SPOT")
+        query = self.omit(params, "type")
+        response = self.privateGetWallets(query)
+        result = {"info": response}
+        for i in range(0, len(response)):
+            balance = response[i]
+            if balance["type"] == balanceType:
+                currencyId = self.safe_string(balance, "currency")
+                code = self.safe_currency_code(currencyId)
+                if not (code in result):
+                    account = self.account()
+                    account["free"] = self.safe_float(balance, "balanceAvailable")
+                    account["total"] = self.safe_float(balance, "balance")
+                    result[code] = account
+        return self.parse_balance(result)
+
+    def fetch_order_book(self, symbol, limit=None, params={}):
+        self.load_markets()
+        request = {
+            "symbol": self.market_id(symbol),
+            "limit": 100,
+        }
+        if limit == 25:
+            request["limit"] = limit
+        response = self.publicGetOrderbookSymbolA0Limit(self.extend(request, params))
+        asks = []
+        bids = []
+        for i in range(0, len(response)):
+            priceLevel = response[i]
+            side = self.safe_string(priceLevel, "side")
+            if side == "SELL":
+                asks.append(priceLevel)
+            else:
+                bids.append(priceLevel)
+        return self.parse_order_book(
+            {"asks": asks, "bids": bids},
+            symbol,
+            None,
+            "bids",
+            "asks",
+            "price",
+            "amount",
+        )
+
+    def fetch_tickers(self, symbols=None, params={}):
+        self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        ids = list(self.markets.keys())
+        if symbols is not None:
+            for i in range(0, len(symbols)):
+                symbol = symbols[i]
+                market = self.market(symbol)
+                ids.append(market["id"])
+        urlParams["pairs"] = ",".join(ids)
+        response = self.publicGetTicker(self.extend(request, params))
+        result = {}
+        for i in range(0, len(response)):
+            marketId = ids[i]
+            market = self.markets[marketId]
+            ticker = self.parse_ticker(response[i], market)
+            symbol = market["symbol"]
+            result[symbol] = ticker
+        return result
+
+    def fetch_ticker(self, symbol, params={}):
+        self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "symbol": market["id"],
+        }
+        ticker = self.publicGetTickerSymbol(self.extend(request, params))
+        return self.parse_ticker(ticker, market)
+
+    def parse_ticker(self, ticker, market=None):
+        timestamp = self.safe_integer(ticker, "timestamp")
+        symbol = None
+        if market is not None:
+            symbol = market["symbol"]
+        elif "pair" in ticker:
+            marketId = self.safe_string(ticker, "pair")
+            if marketId is not None:
+                if marketId in self.markets_by_id:
+                    market = self.markets_by_id[marketId][0]
+                    symbol = market["symbol"]
+                else:
+                    baseId = marketId[0:3]
+                    quoteId = marketId[3:6]
+                    base = self.safe_currency_code(baseId)
+                    quote = self.safe_currency_code(quoteId)
+                    symbol = base + "/" + quote
+        last = self.safe_float(ticker, "price")
+        change = self.safe_float(ticker, "dailyChange")
+        open = None
+        average = None
+        if last is not None and change is not None:
+            open = last - change
+            average = (open + last) / 2
+        volume = self.safe_float(ticker, "baseVolume")
+        quoteVolume = self.safe_float(ticker, "quoteVolume")
+        vwap = (
+            (quoteVolume / volume)
+            if (quoteVolume is not None and volume is not None and volume != 0)
+            else None
+        )
+        return {
+            "symbol": symbol,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "high": self.safe_float(ticker, "high"),
+            "low": self.safe_float(ticker, "low"),
+            "bid": self.safe_float(ticker, "bid"),
+            "bidVolume": self.safe_float(ticker, "bidSize"),
+            "ask": self.safe_float(ticker, "ask"),
+            "askVolume": self.safe_float(ticker, "askSize"),
+            "vwap": vwap,
+            "open": open,
+            "close": last,
+            "last": last,
+            "previousClose": None,
+            "change": change,
+            "percentage": self.safe_float(ticker, "dailyChangeP"),
+            "average": average,
+            "baseVolume": volume,
+            "quoteVolume": quoteVolume,
+            "info": ticker,
+        }
+
+    def parse_ohlcv(self, ohlcv, market=None, timeframe="1m", since=None, limit=None):
+        return [
+            self.safe_integer(ohlcv, "timestamp"),
+            self.safe_float(ohlcv, "open"),
+            self.safe_float(ohlcv, "high"),
+            self.safe_float(ohlcv, "low"),
+            self.safe_float(ohlcv, "close"),
+            self.safe_float(ohlcv, "volume"),
+        ]
+
+    def fetch_ohlcv(self, symbol, timeframe="1m", since=None, limit=None, params={}):
+        self.load_markets()
+        if limit is None:
+            limit = 100
+        market = self.market(symbol)
+        urlParams = {
+            "limit": limit,
+            "end": self.milliseconds(),
+        }
+        request = {
+            "symbol": market["id"],
+            "timeframe": self.timeframes[timeframe],
+            "urlParams": urlParams,
+        }
+        if since is not None:
+            request["start"] = since
+        response = self.publicGetCandlesSymbolTimeframe(self.extend(request, params))
+        return self.parse_ohlcvs(response, market, timeframe, since, limit)
+
+    def parse_trade(self, trade, market):
+        id = self.safe_string(trade, "id")
+        timestamp = self.safe_integer(trade, "timestamp")
+        type = None
+        side = self.safe_string_lower(trade, "side").lower()
+        orderId = None
+        if "orderId" in trade:
+            orderId = self.safe_string(trade, "orderId")
+        price = self.safe_float(trade, "price")
+        amount = self.safe_float(trade, "amount")
+        cost = None
+        if price is not None:
+            if amount is not None:
+                cost = price * amount
+        takerOrMaker = None
+        if "maker" in trade:
+            maker = self.safe_value(trade, "maker")
+            takerOrMaker = "maker" if maker else "taker"
+        feeAmount = self.safe_float(trade, "fee")
+        fee = (
+            feeAmount is None
+            if None
+            else {
+                "cost": feeAmount,
+                "currency": self.safe_string(trade, "feeCurrencyCode"),
+            }
+        )
+        return {
+            "id": id,
+            "info": trade,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "symbol": market["symbol"],
+            "type": type,
+            "order": orderId,
+            "side": side,
+            "takerOrMaker": takerOrMaker,
+            "price": price,
+            "amount": amount,
+            "cost": cost,
+            "fee": fee,
+        }
+
+    def fetch_trades(self, symbol, since=None, limit=50, params={}):
+        self.load_markets()
+        market = self.market(symbol)
+        urlParams = {}
+        request = {
+            "symbol": market["id"],
+            "urlParams": urlParams,
+        }
+        if since is not None:
+            urlParams["start"] = int(since)
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = self.publicGetTradesSymbol(self.extend(request, params))
+        return self.parse_trades(
+            self.safe_value(response, "items"), market, since, limit
+        )
+
+    def calculate_fee(
+        self, symbol, type, side, amount, price, takerOrMaker="taker", params={}
+    ):
+        market = self.markets[symbol]
+        rate = market[takerOrMaker]
+        cost = amount * rate
+        key = "quote"
+        if side == "sell":
+            cost *= price
+        else:
+            key = "base"
+        code = market[key]
+        currency = self.safe_value(self.currencies, code)
+        if currency is not None:
+            precision = self.safe_integer(currency, "precision")
+            if precision is not None:
+                cost = float(self.currency_to_precision(code, cost))
+        return {
+            "type": takerOrMaker,
+            "currency": market[key],
+            "rate": rate,
+            "cost": cost,
+        }
+
+    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
+        if symbol is None:
+            raise ArgumentsRequired(
+                self.id + " fetchMyTrades requires a `symbol` argument"
+            )
+        self.load_markets()
+        market = self.market(symbol)
+        urlParams = {}
+        request = {
+            "symbol": market["id"],
+            "urlParams": urlParams,
+        }
+        if limit is not None:
+            urlParams["limit"] = limit
+        if since is not None:
+            urlParams["start"] = int(since)
+        response = self.privateGetTradesSymbol(self.extend(request, params))
+        return self.parse_trades(
+            self.safe_value(response, "items"), market, since, limit
+        )
+
+    def create_order(self, symbol, type, side, amount, price=None, params={}):
+        self.load_markets()
+        marketId = self.market_id(symbol)
+        request = {
+            "pairName": marketId,
+            "side": self.safe_string(self.options["tradeSides"], side, side),
+            "amount": self.amount_to_precision(symbol, amount),
+            "type": self.upper(type),
+            "walletType": self.safe_string(params, "walletType", "SPOT"),
+        }
+        if "clientOrderId" in params:
+            request["cid"] = self.safe_integer(params, "clientOrderId")
+        if type == "limit":
+            request["limitPrice"] = self.price_to_precision(symbol, price)
+        response = self.privatePostOrders(self.extend(request, params))
+        return self.parse_order(response)
+
+    def edit_order(self, id, symbol, type, side, amount=None, price=None, params={}):
+        self.load_markets()
+        request = {
+            "walletType": self.safe_string(params, "walletType", "SPOT"),
+        }
+        if id is not None:
+            request["id"] = id
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        if price is not None:
+            request["limitPrice"] = self.price_to_precision(symbol, price)
+        if amount is not None:
+            request["amount"] = self.amount_to_precision(symbol, amount)
+        if symbol is not None:
+            request["pairName"] = self.market_id(symbol)
+        if side is not None:
+            request["side"] = self.safe_string(self.options["tradeSides"], side, side)
+        if type is not None:
+            request["type"] = self.upper(type)
+        response = self.privatePutOrdersId(self.extend(request, params))
+        return self.parse_order(response)
+
+    def cancel_order(self, id, symbol=None, params={}):
+        self.load_markets()
+        request = {}
+        if id is not None:
+            request["id"] = int(id)
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        return self.privateDeleteOrdersId(self.extend(request, params))
+
+    def fetch_order(self, id, symbol=None, params={}):
+        self.load_markets()
+        request = {}
+        if id is not None:
+            request["id"] = int(id)
+        elif "clientOrderId" in params:
+            request["id"] = self.safe_integer(params, "clientOrderId")
+            request["urlParams"] = {"cid": True}
+        response = self.privateGetOrdersId(self.extend(request, params))
+        return self.parse_order(response)
+
+    def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
+        self.load_markets()
+        if symbol is not None:
+            if not (symbol in self.markets):
+                raise ExchangeError(self.id + " has no symbol " + symbol)
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            urlParams["start"] = since
+        if limit is not None:
+            urlParams["limit"] = limit
+        urlParams["active"] = True
+        response = None
+        if symbol is not None:
+            marketId = self.market_id(symbol)
+            request["symbol"] = marketId
+            response = self.privateGetOrdersSymbol(self.extend(request, params))
+        else:
+            response = self.privateGetOrders(self.extend(request, params))
+        return self.parse_orders(self.safe_value(response, "items"), None, since, limit)
+
+    def fetch_closed_orders(self, symbol=None, since=None, limit=None, params={}):
+        self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            urlParams["start"] = since
+        if limit is not None:
+            urlParams["limit"] = limit
+        urlParams["active"] = False
+        response = None
+        if symbol is not None:
+            marketId = self.market_id(symbol)
+            request["symbol"] = marketId
+            response = self.privateGetOrdersSymbol(self.extend(request, params))
+        else:
+            response = self.privateGetOrders(self.extend(request, params))
+        return self.parse_orders(self.safe_value(response, "items"), None, since, limit)
+
+    def parse_order(self, order, market=None):
+        side = self.safe_string_lower(order, "side")
+        open = self.safe_value(order, "active")
+        status = None
+        if open:
+            status = "open"
+        else:
+            status = "closed"
+        symbol = None
+        if market is None:
+            marketId = self.safe_string(order, "pairName")
+            if marketId is not None:
+                if marketId in self.markets_by_id:
+                    market = self.markets_by_id[marketId][0]
+        if market is not None:
+            symbol = market["symbol"]
+        orderType = self.safe_string_lower(order, "type")
+        timestamp = self.safe_integer(order, "created")
+        id = self.safe_string(order, "id")
+        lastTradeTimestamp = None
+        if order.amount < order.originalAmount:
+            lastTradeTimestamp = timestamp
+        originalAmount = self.safe_float(order, "originalAmount")
+        amount = self.safe_float(order, "amount")
+        filled = originalAmount - amount
+        resultOrder = {
+            "info": order,
+            "id": id,
+            "clientOrderId": order["cid"],
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "lastTradeTimestamp": lastTradeTimestamp,
+            "symbol": symbol,
+            "type": orderType,
+            "side": side,
+            "average": None,
+            "amount": originalAmount,
+            "remaining": amount,
+            "filled": filled,
+            "status": status,
+            "fee": None,
+            "cost": None,
+            "trades": None,
+            "hidden": self.safe_value(order, "hidden"),
+        }
+        if "limitPrice" in order:
+            resultOrder["price"] = self.safe_float(order, "limitPrice")
+        if "stopPrice" in order:
+            resultOrder["stopPrice"] = self.safe_float(order, "stopPrice")
+        if "trailingPrice" in order:
+            resultOrder["trailingPrice"] = self.safe_float(order, "trailingPrice")
+        if "futurePrice" in order:
+            resultOrder["futurePrice"] = self.safe_float(order, "futurePrice")
+        if "distance" in order:
+            resultOrder["distance"] = self.safe_float(order, "distance")
+        return resultOrder
+
+    def create_deposit_address(self, code, params={}):
+        self.load_markets()
+        request = {
+            "currency": self.currency(code).id,
+        }
+        response = self.privatePostWalletsCurrencyAddress(self.extend(request, params))
+        address = self.safe_value(response, "address")
+        tag = self.safe_value(response, "tag")
+        self.check_address(address)
+        return {
+            "currency": code,
+            "address": address,
+            "tag": tag,
+            "info": response,
+        }
+
+    def fetch_deposit_address(self, code, params={}):
+        self.load_markets()
+        request = {
+            "currency": code,
+            "urlParams": {
+                "formatted": True,
+            },
+        }
+        response = self.privateGetWalletsCurrencyAddress(self.extend(request, params))
+        address = self.safe_value(response, "address")
+        tag = self.safe_value(response, "tag")
+        self.check_address(address)
+        return {
+            "currency": self.currency(code).id,
+            "address": address,
+            "tag": tag,
+            "info": response,
+        }
+
+    def fetch_deposits(self, code=None, since=None, limit=None, params={}):
+        self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        start = since is not since if None else 0
+        urlParams["start"] = start
+        urlParams["end"] = self.milliseconds()
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = None
+        if code is not None:
+            request["currency"] = self.currency(code).id
+            response = self.privateGetWalletsCurrencyDeposits(
+                self.extend(request, params)
+            )
+        else:
+            response = self.privateGetDeposits(self.extend(request, params))
+        deposits = self.safe_value(response, "items")
+        for i in range(0, len(deposits)):
+            deposits[i]["type"] = "DEPOSIT"
+        return self.parse_transactions(deposits, None, since, limit)
+
+    def fetch_withdrawals(self, code=None, since=None, limit=None, params={}):
+        self.load_markets()
+        urlParams = {}
+        request = {"urlParams": urlParams}
+        if since is not None:
+            request["form"] = since
+        start = since is not since if None else 0
+        urlParams["start"] = start
+        urlParams["end"] = self.milliseconds()
+        if limit is not None:
+            urlParams["limit"] = limit
+        response = None
+        if code is not None:
+            request["currency"] = self.currency(code).id
+            response = self.privateGetWalletsCurrencyWithdrawals(
+                self.extend(request, params)
+            )
+        else:
+            response = self.privateGetWithdrawals(self.extend(request, params))
+        withdrawals = self.safe_value(response, "items")
+        for i in range(0, len(withdrawals)):
+            withdrawals[i]["type"] = "WITHDRAWAL"
+        return self.parse_transactions(withdrawals, None, since, limit)
+
+    def parse_transaction(self, transaction, currency=None):
+        timestamp = self.safe_integer(transaction, "timestamp")
+        updated = self.safe_integer(transaction, "updated")
+        currencyId = self.safe_string(transaction, "currencyCode")
+        code = self.safe_currency_code(currencyId, currency)
+        type = self.safe_string_lower(transaction, "type")  # DEPOSIT or WITHDRAWAL
+        status = self.parse_transaction_status(self.safe_string(transaction, "status"))
+        feeCost = self.safe_float(transaction, "fee")
+        if feeCost is not None:
+            feeCost = abs(feeCost)
+        return {
+            "info": transaction,
+            "id": self.safe_string(transaction, "id"),
+            "txid": self.safe_string(transaction, "txHash"),
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "address": self.safe_string(
+                transaction, "walletId"
+            ),  # todo: self is actually the tag for XRP transfers(the address is missing)
+            "tag": None,  # refix it properly for the tag from description
+            "type": type,
+            "amount": self.safe_float(transaction, "amount"),
+            "currency": code,
+            "status": status,
+            "updated": updated,
+            "fee": {
+                "currency": code,
+                "cost": feeCost,
+                "rate": None,
+            },
+        }
+
+    def parse_transaction_status(self, status):
+        statuses = {
+            "PROCESSED": "pending",
+            "CANCELED": "canceled",
+            "COMPLETED": "ok",
+        }
+        return self.safe_string(statuses, status, status)
+
+    def withdraw(self, code, amount, address, tag=None, params={}):
+        self.check_address(address)
+        self.load_markets()
+        currency = self.currency(code)
+        destination = address
+        if tag is not None:
+            destination = address + ":" + tag
+        fee = currency.fee
+        request = {
+            "currency": currency.id,
+            "amount": self.sum(amount, fee),
+            "fee": fee,
+            "currencyCode": currency.id,
+            "destination": destination,
+        }
+        response = self.privatePostWithdrawalsCurrency(self.extend(request, params))
+        return {
+            "info": response,
+            "id": self.safe_string(response, "id"),
+        }
+
+    def nonce(self):
+        return self.milliseconds()
+
+    def sign(
+        self, path, api="public", method="GET", params={}, headers=None, body=None
+    ):
+        request = "/" + self.implode_params(path, params)
+        query = self.omit(params, self.extract_params(path))
+        apiUrls = self.urls["api"]
+        urlParams = self.safe_value(query, "urlParams")
+        url = apiUrls[api] + request
+        urlParamsStr = self.urlencode(urlParams) if (urlParams is not None) else ""
+        if urlParamsStr != "":
+            url += "?" + urlParamsStr
+        requestBody = self.omit(query, "urlParams")
+        if api == "private":
+            self.check_required_credentials()
+            nonce = str(self.nonce())
+            urlPath = self.options["paths"]["private"] + request
+            payloadSuffix = ""
+            if method != "GET" and method != "DELETE":
+                body = self.json(requestBody)
+                payloadSuffix = body
+            payload = "/api" + urlPath + nonce + payloadSuffix
+            payload = self.encode(payload)
+            secret = self.encode(self.secret)
+            signature = self.hmac(payload, secret, hashlib.sha384).upper()
+            contentType = "application/json; charset=UTF-8"
+            headers = {
+                "Content-Type": contentType,
+                "nominex-nonce": nonce,
+                "nominex-apikey": self.apiKey,
+                "nominex-signature": signature,
+            }
+        return {"url": url, "method": method, "body": body, "headers": headers}
+
+    def handle_errors(
+        self,
+        code,
+        reason,
+        url,
+        method,
+        headers,
+        body,
+        response,
+        requestHeaders,
+        requestBody,
+    ):
+        if response is None:
+            return
+        if code >= 400:
+            if body[0] == "{":
+                feedback = self.id + " " + body
+                if "code" in response:
+                    code = self.safe_string(response, "code")
+                    self.throw_exactly_matched_exception(
+                        self.exceptions, code, feedback
+                    )
+                if "codes" in response:
+                    codes = self.safe_string(response, "codes")
+                    code = self.asString(codes[0])
+                    self.throw_exactly_matched_exception(
+                        self.exceptions, code, feedback
+                    )
+                raise ExchangeError(feedback)  # unknown message
+            elif body[0] == "[":
+                feedback = self.id + " " + body
+                error = response[0]
+                code = self.safe_string(error, "code")
+                self.throw_exactly_matched_exception(self.exceptions, code, feedback)
+                raise ExchangeError(feedback)  # unknown message
```

### Comparing `ccxt-unmerged-2.2/ccxt_unmerged/foblgate.py` & `ccxt_unmerged-4.0/ccxt_unmerged/async_support/foblgate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,397 +1,452 @@
-# -*- coding: utf-8 -*-
-
-# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
-# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
-
-from ccxt.base.exchange import Exchange
-import base64
-import hashlib
-from ccxt.base.errors import ExchangeError
-from ccxt.base.errors import AuthenticationError
-from ccxt.base.errors import BadRequest
-from ccxt.base.errors import InvalidOrder
-
-
-class foblgate(Exchange):
-
-    def describe(self):
-        return self.deep_extend(super(foblgate, self).describe(), {
-            'id': 'foblgate',
-            'name': 'FOBLGATE',
-            'countries': ['KR'],  # South Korea
-            'rateLimit': 500,
-            'has': {
-                'CORS': True,
-                'createOrder': True,
-                'cancelOrder': True,
-                'createMarketOrder': True,
-                'fetchTicker': False,
-                'fetchOpenOrders': True,
-                'fetchClosedOrders': True,
-                'fetchOrder': True,
-                'fetchTrades': True,
-                'fetchMyTrades': True,
-            },
-            'urls': {
-                'logo': 'https://user-images.githubusercontent.com/69025125/89286704-a5495200-d68d-11ea-8486-fe3fa693e4a6.jpg',
-                'api': {
-                    'public': 'https://api2.foblgate.com',
-                    'private': 'https://api2.foblgate.com',
-                },
-                'www': 'https://www.foblgate.com',
-                'doc': 'https://api-document.foblgate.com',
-                'fees': 'https://www.foblgate.com/fees',
-            },
-            'api': {
-                'public': {
-                    'post': [
-                        'ccxt/marketList',
-                        'ccxt/orderBook',
-                        'ccxt/trades',
-                    ],
-                },
-                'private': {
-                    'post': [
-                        'ccxt/balance',
-                        'ccxt/myTrades',
-                        'ccxt/createOrder',
-                        'ccxt/cancelOrder',
-                        'ccxt/orderDetail',
-                        'ccxt/openOrders',
-                        'ccxt/closedOrders',
-                    ],
-                },
-            },
-            'requiredCredentials': {
-                'uid': True,
-            },
-            'exceptions': {
-                '400': BadRequest,
-                '401': AuthenticationError,
-                '403': AuthenticationError,
-                '500': ExchangeError,
-            },
-        })
-
-    def fetch_markets(self, params={}):
-        response = self.publicPostCcxtMarketList(params)
-        marketList = self.safe_value(response, 'marketList')
-        # {
-        #     'ETH/BTC': {
-        #         limits: {amount: [Object], price: [Object], cost: [Object]},
-        #         precision: {amount: 8, price: 8},
-        #         tierBased: False,
-        #             percentage: True,
-        #             taker: 0.03,
-        #             maker: 0.03,
-        #             symbol: 'ETH/BTC',
-        #             active: True,
-        #             baseId: 'ETH',
-        #             quoteId: 'BTC',
-        #             quote: 'BTC',
-        #             id: 'ETH-BTC',
-        #             base: 'ETH',
-        #             info: {market: 'ETH/BTC', coinName: 'ETH', coinNameKo: '이더리움'}
-        #     }
-        # }
-        return marketList
-
-    def fetch_order_book(self, symbol, limit=None, params={}):
-        self.load_markets()
-        request = {
-            'pairName': symbol,
-        }
-        if limit is not None:
-            request['count'] = limit
-        response = self.publicPostCcxtOrderBook(self.extend(request, params))
-        # {
-        #     bids: [
-        #         [303100, 11.68805904],
-        #         [303000, 0.61282982],
-        #         [302900, 0.59681086]
-        #     ],
-        #     asks: [
-        #         [303700, 0.99953148],
-        #         [303800, 0.66825562],
-        #         [303900, 1.47346607],
-        #     ],
-        #     timestamp: None,
-        #     datetime: None,
-        #     nonce: None
-        # }
-        return self.parse_order_book(response, symbol, None, 'bids', 'asks', 'price', 'amount')
-
-    def parse_trade(self, trade, market=None):
-        #
-        # fetchTrades(public)
-        #
-        #     {
-        #         "transaction_date":"2020-04-23 22:21:46",
-        #         "type":"ask",
-        #         "units_traded":"0.0125",
-        #         "price":"8667000",
-        #         "total":"108337"
-        #     }
-        #
-        # fetchOrder(private)
-        #
-        #     {
-        #         "transaction_date": "1572497603902030",
-        #         "price": "8601000",
-        #         "units": "0.005",
-        #         "fee_currency": "KRW",
-        #         "fee": "107.51",
-        #         "total": "43005"
-        #     }
-        #
-        # a workaround for their bug in date format, hours are not 0-padded
-        timestamp = None
-        transactionDatetime = self.safe_string(trade, 'transaction_date')
-        if transactionDatetime is not None:
-            parts = transactionDatetime.split(' ')
-            numParts = len(parts)
-            if numParts > 1:
-                transactionDate = parts[0]
-                transactionTime = parts[1]
-                if len(transactionTime) < 8:
-                    transactionTime = '0' + transactionTime
-                timestamp = self.parse8601(transactionDate + ' ' + transactionTime)
-            else:
-                timestamp = self.safe_integer_product(trade, 'transaction_date', 0.001)
-        if timestamp is not None:
-            timestamp -= 9 * 3600000  # they report UTC + 9 hours, server in Korean timezone
-        type = None
-        side = self.safe_string(trade, 'type')
-        side = 'sell' if (side == 'ask') else 'buy'
-        id = self.safe_string(trade, 'cont_no')
-        symbol = None
-        if market is not None:
-            symbol = market['symbol']
-        price = self.safe_float(trade, 'price')
-        amount = self.safe_float(trade, 'units_traded')
-        cost = self.safe_float(trade, 'total')
-        if cost is None:
-            if amount is not None:
-                if price is not None:
-                    cost = price * amount
-        fee = None
-        feeCost = self.safe_float(trade, 'fee')
-        if feeCost is not None:
-            feeCurrencyId = self.safe_string(trade, 'fee_currency')
-            feeCurrencyCode = self.common_currency_code(feeCurrencyId)
-            fee = {
-                'cost': feeCost,
-                'currency': feeCurrencyCode,
-            }
-        return {
-            'id': id,
-            'info': trade,
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'symbol': symbol,
-            'order': None,
-            'type': type,
-            'side': side,
-            'takerOrMaker': None,
-            'price': price,
-            'amount': amount,
-            'cost': cost,
-            'fee': fee,
-        }
-
-    def fetch_trades(self, symbol, since=None, limit=None, params={}):
-        self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'pairName': symbol,
-            'since': since,
-            'cnt': limit,
-        }
-        response = self.publicPostCcxtTrades(self.extend(request, params))
-        data = self.safe_value(response, 'data', [])
-        return self.parse_trades(data, market, since, limit)
-
-    def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
-        self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'pairName': symbol,
-            'cnt': limit,
-            'since': since,
-        }
-        response = self.privatePostCcxtMyTrades(self.extend(request, params))
-        data = self.safe_value(response, 'data', [])
-        return self.parse_trades(data, market, since, limit)
-
-    def fetch_balance(self, params={}):
-        self.load_markets()
-        response = self.privatePostCcxtBalance(params)
-        # {
-        #     BTC: {total: 0, used: 0, free: 0},
-        #     ETH: {total: 0, used: 0, free: 0},
-        #     info: {}
-        # }
-        return self.parse_balance(response)
-
-    def create_order(self, symbol, type, side, amount, price=None, params={}):
-        if type == 'market':
-            raise InvalidOrder(self.id + ' createOrder type = market, currently not supported.')
-        action = None
-        if side == 'buy':
-            action = 'bid'
-        elif side == 'sell':
-            action = 'ask'
-        else:
-            raise InvalidOrder(self.id + ' createOrder allows buy or sell side only!')
-        self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'pairName': market['symbol'],
-            'type': type,
-            'action': action,
-            'amount': self.amount_to_precision(symbol, amount),
-            'price': self.price_to_precision(symbol, price),
-        }
-        response = self.privatePostCcxtCreateOrder(self.extend(request, params))
-        # {
-        #     info: {data: '2008042'},
-        #     id: '2008042',
-        #     symbol: 'BTC/KRW',
-        #     type: 'limit',
-        #     side: 'buy',
-        #     amount: 0.1,
-        #     price: 9000000
-        # }
-        return response
-
-    def cancel_order(self, id, symbol=None, params={}):
-        self.load_markets()
-        request = {
-            'ordNo': id,
-        }
-        response = self.privatePostCcxtCancelOrder(self.extend(request, params))
-        # {status: '0'}
-        return response
-
-    def parse_order(self, order, market=None):
-        id = self.safe_string(order, 'id')
-        timestamp = self.safe_value(order, 'timestamp')
-        lastTradeTimestamp = self.safe_value(order, 'lastTradeTimestamp')
-        symbol = self.safe_string(order, 'symbol')
-        type = self.safe_string(order, 'type')
-        side = self.safe_string(order, 'side')
-        price = self.safe_float(order, 'price')
-        amount = self.safe_float(order, 'amount')
-        cost = self.safe_float(order, 'cost')
-        average = self.safe_float(order, 'average')
-        filled = self.safe_float(order, 'filled')
-        remaining = self.safe_float(order, 'remaining')
-        status = self.safe_string(order, 'status')
-        fee = self.safe_value(order, 'fee')
-        trades = self.safe_value(order, 'trades', [])
-        trades = self.parse_trades(trades, market, None, None, {
-            'order': id,
-            'type': type,
-        })
-        return {
-            'info': order,
-            'id': id,
-            'clientOrderId': None,
-            'timestamp': timestamp,
-            'datetime': self.iso8601(timestamp),
-            'lastTradeTimestamp': lastTradeTimestamp,
-            'symbol': symbol,
-            'type': type,
-            'side': side,
-            'price': price,
-            'amount': amount,
-            'cost': cost,
-            'average': average,
-            'filled': filled,
-            'remaining': remaining,
-            'status': status,
-            'fee': fee,
-            'trades': trades,
-        }
-
-    def fetch_order(self, id, symbol=None, params={}):
-        self.load_markets()
-        request = {
-            'ordNo': id,
-        }
-        response = self.privatePostCcxtOrderDetail(self.extend(request, params))
-        order = self.safe_value(response, 'order')
-        return self.parse_order(order)
-
-    def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
-        self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'pairName': market['symbol'],
-            'since': since,
-            'cnt': limit,
-        }
-        response = self.privatePostCcxtOpenOrders(self.extend(request, params))
-        orderList = self.safe_value(response, 'orderList', [])
-        return self.parse_orders(orderList, market, since, limit)
-
-    def fetch_closed_orders(self, symbol=None, since=None, limit=None, params={}):
-        self.load_markets()
-        market = self.market(symbol)
-        request = {
-            'pairName': market['symbol'],
-            'since': since,
-            'cnt': limit,
-        }
-        response = self.privatePostCcxtClosedOrders(self.extend(request, params))
-        orderList = self.safe_value(response, 'orderList', [])
-        return self.parse_orders(orderList, market, since, limit)
-
-    def nonce(self):
-        return self.milliseconds()
-
-    def sign(self, path, api='public', method='GET', params={}, headers=None, body=None):
-        endpoint = '/' + self.implode_params(path, params)
-        url = self.urls['api'][api] + endpoint
-        query = self.omit(params, self.extract_params(path))
-        if method != 'POST':
-            if query:
-                url += '?' + self.urlencode(query)
-        else:
-            if api == 'private':
-                self.check_required_credentials()
-                body = self.urlencode(query)
-                nonce = str(self.nonce())
-                auth = self.urlencode(self.extend({
-                    'apiKey': self.apiKey,
-                    'mbId': self.uid,
-                    'nonce': nonce,
-                }, query))
-                signature = self.hmac(self.encode(auth), self.encode(self.secret), hashlib.sha512)
-                signature64 = self.decode(base64.b64encode(self.encode(signature)))
-                headers = {
-                    'Accept': 'application/json',
-                    'Content-Type': 'application/x-www-form-urlencoded',
-                    'Api-Key': self.apiKey,
-                    'Api-Uid': self.uid,
-                    'Api-Sign': str(signature64),
-                    'Api-Nonce': nonce,
-                }
-            else:
-                body = self.urlencode(query)
-                headers = {
-                    'Accept': 'application/json',
-                    'Content-Type': 'application/x-www-form-urlencoded',
-                }
-        return {'url': url, 'method': method, 'body': body, 'headers': headers}
-
-    def handle_errors(self, httpCode, reason, url, method, headers, body, response, requestHeaders, requestBody):
-        if response is None:
-            return  # fallback to default error handler
-        code = self.safe_value(response, 'code')
-        if code is not None:
-            if code == '0':
-                return
-            feedback = self.id + ' ' + body
-            self.throw_exactly_matched_exception(self.exceptions, code, feedback)
-            raise ExchangeError(feedback)  # unknown message
+# -*- coding: utf-8 -*-
+
+# PLEASE DO NOT EDIT THIS FILE, IT IS GENERATED AND WILL BE OVERWRITTEN:
+# https://github.com/ccxt/ccxt/blob/master/CONTRIBUTING.md#how-to-contribute-code
+
+from ccxt.async_support.base.exchange import Exchange
+import base64
+import hashlib
+from ccxt.base.errors import ExchangeError
+from ccxt.base.errors import AuthenticationError
+from ccxt.base.errors import BadRequest
+from ccxt.base.errors import InvalidOrder
+
+
+class foblgate(Exchange):
+    def describe(self):
+        return self.deep_extend(
+            super(foblgate, self).describe(),
+            {
+                "id": "foblgate",
+                "name": "FOBLGATE",
+                "countries": ["KR"],  # South Korea
+                "rateLimit": 500,
+                "has": {
+                    "CORS": True,
+                    "createOrder": True,
+                    "cancelOrder": True,
+                    "createMarketOrder": True,
+                    "fetchTicker": False,
+                    "fetchOpenOrders": True,
+                    "fetchClosedOrders": True,
+                    "fetchOrder": True,
+                    "fetchTrades": True,
+                    "fetchMyTrades": True,
+                },
+                "urls": {
+                    "logo": "https://user-images.githubusercontent.com/69025125/89286704-a5495200-d68d-11ea-8486-fe3fa693e4a6.jpg",
+                    "api": {
+                        "public": "https://api2.foblgate.com",
+                        "private": "https://api2.foblgate.com",
+                    },
+                    "www": "https://www.foblgate.com",
+                    "doc": "https://api-document.foblgate.com",
+                    "fees": "https://www.foblgate.com/fees",
+                },
+                "api": {
+                    "public": {
+                        "post": [
+                            "ccxt/marketList",
+                            "ccxt/orderBook",
+                            "ccxt/trades",
+                        ],
+                    },
+                    "private": {
+                        "post": [
+                            "ccxt/balance",
+                            "ccxt/myTrades",
+                            "ccxt/createOrder",
+                            "ccxt/cancelOrder",
+                            "ccxt/orderDetail",
+                            "ccxt/openOrders",
+                            "ccxt/closedOrders",
+                        ],
+                    },
+                },
+                "requiredCredentials": {
+                    "uid": True,
+                },
+                "exceptions": {
+                    "400": BadRequest,
+                    "401": AuthenticationError,
+                    "403": AuthenticationError,
+                    "500": ExchangeError,
+                },
+            },
+        )
+
+    async def fetch_markets(self, params={}):
+        response = await self.publicPostCcxtMarketList(params)
+        marketList = self.safe_value(response, "marketList")
+        # {
+        #     'ETH/BTC': {
+        #         limits: {amount: [Object], price: [Object], cost: [Object]},
+        #         precision: {amount: 8, price: 8},
+        #         tierBased: False,
+        #         percentage: True,
+        #         taker: 0.03,
+        #         maker: 0.03,
+        #         symbol: 'ETH/BTC',
+        #         active: True,
+        #         baseId: 'ETH',
+        #         quoteId: 'BTC',
+        #         quote: 'BTC',
+        #         id: 'ETH-BTC',
+        #         base: 'ETH',
+        #         info: {market: 'ETH/BTC', coinName: 'ETH', coinNameKo: '이더리움'}
+        #     }
+        # }
+        for market in marketList:
+            market.update(
+                {
+                    "settle": None,
+                    "settleId": None,
+                    "type": "spot",
+                    "spot": True,
+                    "margin": False,
+                    "swap": False,
+                    "future": False,
+                    "option": False,
+                    "contract": False,
+                    "linear": None,
+                    "inverse": None,
+                    "contractSize": None,
+                    "expiry": None,
+                    "expiryDatetime": None,
+                    "strike": None,
+                    "optionType": None,
+                }
+            )
+        return marketList
+
+    async def fetch_order_book(self, symbol, limit=None, params={}):
+        await self.load_markets()
+        request = {
+            "pairName": symbol,
+        }
+        if limit is not None:
+            request["count"] = limit
+        response = await self.publicPostCcxtOrderBook(self.extend(request, params))
+        # {
+        #     bids: [
+        #         [303100, 11.68805904],
+        #         [303000, 0.61282982],
+        #         [302900, 0.59681086]
+        #     ],
+        #     asks: [
+        #         [303700, 0.99953148],
+        #         [303800, 0.66825562],
+        #         [303900, 1.47346607],
+        #     ],
+        #     timestamp: None,
+        #     datetime: None,
+        #     nonce: None
+        # }
+        return self.parse_order_book(
+            response, symbol, None, "bids", "asks", "price", "amount"
+        )
+
+    def parse_trade(self, trade, market=None):
+        #
+        # fetchTrades(public)
+        #
+        #     {
+        #         "transaction_date":"2020-04-23 22:21:46",
+        #         "type":"ask",
+        #         "units_traded":"0.0125",
+        #         "price":"8667000",
+        #         "total":"108337"
+        #     }
+        #
+        # fetchOrder(private)
+        #
+        #     {
+        #         "transaction_date": "1572497603902030",
+        #         "price": "8601000",
+        #         "units": "0.005",
+        #         "fee_currency": "KRW",
+        #         "fee": "107.51",
+        #         "total": "43005"
+        #     }
+        #
+        # a workaround for their bug in date format, hours are not 0-padded
+        timestamp = None
+        transactionDatetime = self.safe_string(trade, "transaction_date")
+        if transactionDatetime is not None:
+            parts = transactionDatetime.split(" ")
+            numParts = len(parts)
+            if numParts > 1:
+                transactionDate = parts[0]
+                transactionTime = parts[1]
+                if len(transactionTime) < 8:
+                    transactionTime = "0" + transactionTime
+                timestamp = self.parse8601(transactionDate + " " + transactionTime)
+            else:
+                timestamp = self.safe_integer_product(trade, "transaction_date", 0.001)
+        if timestamp is not None:
+            timestamp -= (
+                9 * 3600000
+            )  # they report UTC + 9 hours, server in Korean timezone
+        type = None
+        side = self.safe_string(trade, "type")
+        side = "sell" if (side == "ask") else "buy"
+        id = self.safe_string(trade, "cont_no")
+        symbol = None
+        if market is not None:
+            symbol = market["symbol"]
+        price = self.safe_float(trade, "price")
+        amount = self.safe_float(trade, "units_traded")
+        cost = self.safe_float(trade, "total")
+        if cost is None:
+            if amount is not None:
+                if price is not None:
+                    cost = price * amount
+        fee = None
+        feeCost = self.safe_float(trade, "fee")
+        if feeCost is not None:
+            feeCurrencyId = self.safe_string(trade, "fee_currency")
+            feeCurrencyCode = self.common_currency_code(feeCurrencyId)
+            fee = {
+                "cost": feeCost,
+                "currency": feeCurrencyCode,
+            }
+        return {
+            "id": id,
+            "info": trade,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "symbol": symbol,
+            "order": None,
+            "type": type,
+            "side": side,
+            "takerOrMaker": None,
+            "price": price,
+            "amount": amount,
+            "cost": cost,
+            "fee": fee,
+        }
+
+    async def fetch_trades(self, symbol, since=None, limit=None, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "pairName": symbol,
+            "since": since,
+            "cnt": limit,
+        }
+        response = await self.publicPostCcxtTrades(self.extend(request, params))
+        data = self.safe_value(response, "data", [])
+        return self.parse_trades(data, market, since, limit)
+
+    async def fetch_my_trades(self, symbol=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "pairName": symbol,
+            "cnt": limit,
+            "since": since,
+        }
+        response = await self.privatePostCcxtMyTrades(self.extend(request, params))
+        data = self.safe_value(response, "data", [])
+        return self.parse_trades(data, market, since, limit)
+
+    async def fetch_balance(self, params={}):
+        await self.load_markets()
+        response = await self.privatePostCcxtBalance(params)
+        # {
+        #     BTC: {total: 0, used: 0, free: 0},
+        #     ETH: {total: 0, used: 0, free: 0},
+        #     info: {}
+        # }
+        return self.parse_balance(response)
+
+    async def create_order(self, symbol, type, side, amount, price=None, params={}):
+        if type == "market":
+            raise InvalidOrder(
+                self.id + " createOrder type = market, currently not supported."
+            )
+        action = None
+        if side == "buy":
+            action = "bid"
+        elif side == "sell":
+            action = "ask"
+        else:
+            raise InvalidOrder(self.id + " createOrder allows buy or sell side only!")
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "pairName": market["symbol"],
+            "type": type,
+            "action": action,
+            "amount": self.amount_to_precision(symbol, amount),
+            "price": self.price_to_precision(symbol, price),
+        }
+        response = await self.privatePostCcxtCreateOrder(self.extend(request, params))
+        # {
+        #     info: {data: '2008042'},
+        #     id: '2008042',
+        #     symbol: 'BTC/KRW',
+        #     type: 'limit',
+        #     side: 'buy',
+        #     amount: 0.1,
+        #     price: 9000000
+        # }
+        return response
+
+    async def cancel_order(self, id, symbol=None, params={}):
+        await self.load_markets()
+        request = {
+            "ordNo": id,
+        }
+        response = await self.privatePostCcxtCancelOrder(self.extend(request, params))
+        # {status: '0'}
+        return response
+
+    def parse_order(self, order, market=None):
+        id = self.safe_string(order, "id")
+        timestamp = self.safe_value(order, "timestamp")
+        lastTradeTimestamp = self.safe_value(order, "lastTradeTimestamp")
+        symbol = self.safe_string(order, "symbol")
+        type = self.safe_string(order, "type")
+        side = self.safe_string(order, "side")
+        price = self.safe_float(order, "price")
+        amount = self.safe_float(order, "amount")
+        cost = self.safe_float(order, "cost")
+        average = self.safe_float(order, "average")
+        filled = self.safe_float(order, "filled")
+        remaining = self.safe_float(order, "remaining")
+        status = self.safe_string(order, "status")
+        fee = self.safe_value(order, "fee")
+        trades = self.safe_value(order, "trades", [])
+        trades = self.parse_trades(
+            trades,
+            market,
+            None,
+            None,
+            {
+                "order": id,
+                "type": type,
+            },
+        )
+        return {
+            "info": order,
+            "id": id,
+            "clientOrderId": None,
+            "timestamp": timestamp,
+            "datetime": self.iso8601(timestamp),
+            "lastTradeTimestamp": lastTradeTimestamp,
+            "symbol": symbol,
+            "type": type,
+            "side": side,
+            "price": price,
+            "amount": amount,
+            "cost": cost,
+            "average": average,
+            "filled": filled,
+            "remaining": remaining,
+            "status": status,
+            "fee": fee,
+            "trades": trades,
+        }
+
+    async def fetch_order(self, id, symbol=None, params={}):
+        await self.load_markets()
+        request = {
+            "ordNo": id,
+        }
+        response = await self.privatePostCcxtOrderDetail(self.extend(request, params))
+        order = self.safe_value(response, "order")
+        return self.parse_order(order)
+
+    async def fetch_open_orders(self, symbol=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "pairName": market["symbol"],
+            "since": since,
+            "cnt": limit,
+        }
+        response = await self.privatePostCcxtOpenOrders(self.extend(request, params))
+        orderList = self.safe_value(response, "orderList", [])
+        return self.parse_orders(orderList, market, since, limit)
+
+    async def fetch_closed_orders(self, symbol=None, since=None, limit=None, params={}):
+        await self.load_markets()
+        market = self.market(symbol)
+        request = {
+            "pairName": market["symbol"],
+            "since": since,
+            "cnt": limit,
+        }
+        response = await self.privatePostCcxtClosedOrders(self.extend(request, params))
+        orderList = self.safe_value(response, "orderList", [])
+        return self.parse_orders(orderList, market, since, limit)
+
+    def nonce(self):
+        return self.milliseconds()
+
+    def sign(
+        self, path, api="public", method="GET", params={}, headers=None, body=None
+    ):
+        endpoint = "/" + self.implode_params(path, params)
+        url = self.urls["api"][api] + endpoint
+        query = self.omit(params, self.extract_params(path))
+        if method != "POST":
+            if query:
+                url += "?" + self.urlencode(query)
+        else:
+            if api == "private":
+                self.check_required_credentials()
+                body = self.urlencode(query)
+                nonce = str(self.nonce())
+                auth = self.urlencode(
+                    self.extend(
+                        {
+                            "apiKey": self.apiKey,
+                            "mbId": self.uid,
+                            "nonce": nonce,
+                        },
+                        query,
+                    )
+                )
+                signature = self.hmac(
+                    self.encode(auth), self.encode(self.secret), hashlib.sha512
+                )
+                signature64 = self.decode(base64.b64encode(self.encode(signature)))
+                headers = {
+                    "Accept": "application/json",
+                    "Content-Type": "application/x-www-form-urlencoded",
+                    "Api-Key": self.apiKey,
+                    "Api-Uid": self.uid,
+                    "Api-Sign": str(signature64),
+                    "Api-Nonce": nonce,
+                }
+            else:
+                body = self.urlencode(query)
+                headers = {
+                    "Accept": "application/json",
+                    "Content-Type": "application/x-www-form-urlencoded",
+                }
+        return {"url": url, "method": method, "body": body, "headers": headers}
+
+    def handle_errors(
+        self,
+        httpCode,
+        reason,
+        url,
+        method,
+        headers,
+        body,
+        response,
+        requestHeaders,
+        requestBody,
+    ):
+        if response is None:
+            return  # fallback to default error handler
+        code = self.safe_value(response, "code")
+        if code is not None:
+            if code == "0":
+                return
+            feedback = self.id + " " + body
+            self.throw_exactly_matched_exception(self.exceptions, code, feedback)
+            raise ExchangeError(feedback)  # unknown message
```

### Comparing `ccxt-unmerged-2.2/setup.py` & `ccxt_unmerged-4.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-import pathlib
-from setuptools import setup, find_packages
-import sys
-
-HERE = pathlib.Path(__file__).parent
-README = (HERE / "README.md").read_text()
-
-is_python_2 = sys.version_info < (3, 0)
-
-setup(
-   name='ccxt-unmerged',
-   version='2.2',
-   description="Some 40 exchanges that haven't been merged into ccxt yet.",
-   long_description=README,
-   long_description_content_type='text/markdown',
-   url='https://github.com/binares/ccxt-unmerged',
-   author='binares',
-   author_email='binares@protonmail.com',
-   packages=find_packages(exclude=['ccxt_unmerged.async_support*'] if is_python_2 else []),
-   install_requires=[
-       'ccxt',
-   ],
-)
+import pathlib
+from setuptools import setup, find_packages
+import sys
+
+HERE = pathlib.Path(__file__).parent
+README = (HERE / "README.md").read_text()
+
+is_python_2 = sys.version_info < (3, 0)
+
+setup(
+    name="ccxt-unmerged",
+    version="4.0",
+    description="Some 40 exchanges that haven't been merged into ccxt yet.",
+    long_description=README,
+    long_description_content_type="text/markdown",
+    url="https://github.com/binares/ccxt-unmerged",
+    author="binares",
+    author_email="binares@protonmail.com",
+    packages=find_packages(
+        exclude=["ccxt_unmerged.async_support*"] if is_python_2 else []
+    ),
+    install_requires=[
+        "ccxt",
+    ],
+)
```

