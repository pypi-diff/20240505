# Comparing `tmp/rnspure-0.7.3.tar.gz` & `tmp/rnspure-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnspure-0.7.3.tar", last modified: Sat Mar  9 20:05:16 2024, max compression
+gzip compressed data, was "rnspure-0.7.4.tar", last modified: Sun May  5 17:55:46 2024, max compression
```

## Comparing `rnspure-0.7.3.tar` & `rnspure-0.7.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2023-12-30 20:55:12.000000 rnspure-0.7.3/LICENSE
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19482 2024-03-09 20:05:16.141478 rnspure-0.7.3/PKG-INFO
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    18743 2024-02-16 16:53:41.000000 rnspure-0.7.3/README.md
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.134811 rnspure-0.7.3/RNS/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13058 2023-09-29 08:24:08.000000 rnspure-0.7.3/RNS/Buffer.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26025 2023-09-18 21:33:08.000000 rnspure-0.7.3/RNS/Channel.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.134811 rnspure-0.7.3/RNS/Cryptography/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/AES.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/Ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3675 2023-10-20 09:56:32.000000 rnspure-0.7.3/RNS/Cryptography/Fernet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.7.3/RNS/Cryptography/HKDF.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/HMAC.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/Hashes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/PKCS7.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2023-11-08 19:55:14.000000 rnspure-0.7.3/RNS/Cryptography/Provider.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/Proxies.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/SHA256.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/SHA512.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/X25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/__init__.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.138145 rnspure-0.7.3/RNS/Cryptography/aes/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/aes/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/aes/aes.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/aes/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.138145 rnspure-0.7.3/RNS/Cryptography/pure25519/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/pure25519/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/pure25519/_ed25519.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/pure25519/basic.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/pure25519/ed25519_oop.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Cryptography/pure25519/eddsa.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    21094 2023-10-27 21:40:40.000000 rnspure-0.7.3/RNS/Destination.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24471 2024-02-29 22:24:35.000000 rnspure-0.7.3/RNS/Identity.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.138145 rnspure-0.7.3/RNS/Interfaces/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14545 2023-10-01 09:35:17.000000 rnspure-0.7.3/RNS/Interfaces/AX25KISSInterface.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.138145 rnspure-0.7.3/RNS/Interfaces/Android/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16766 2023-10-02 15:26:34.000000 rnspure-0.7.3/RNS/Interfaces/Android/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    57478 2023-11-06 22:55:05.000000 rnspure-0.7.3/RNS/Interfaces/Android/RNodeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10378 2023-10-02 15:27:09.000000 rnspure-0.7.3/RNS/Interfaces/Android/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.7.3/RNS/Interfaces/Android/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21187 2023-12-30 00:08:40.000000 rnspure-0.7.3/RNS/Interfaces/AutoInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41618 2023-09-30 16:02:25.000000 rnspure-0.7.3/RNS/Interfaces/I2PInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     9790 2023-12-25 10:34:55.000000 rnspure-0.7.3/RNS/Interfaces/Interface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13816 2023-10-01 09:35:08.000000 rnspure-0.7.3/RNS/Interfaces/KISSInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13934 2024-01-14 22:33:50.000000 rnspure-0.7.3/RNS/Interfaces/LocalInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6568 2023-09-30 11:56:53.000000 rnspure-0.7.3/RNS/Interfaces/PipeInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    39095 2024-02-13 18:00:00.000000 rnspure-0.7.3/RNS/Interfaces/RNodeInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7451 2023-10-01 09:34:57.000000 rnspure-0.7.3/RNS/Interfaces/SerialInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21979 2023-11-05 21:57:12.000000 rnspure-0.7.3/RNS/Interfaces/TCPInterface.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4191 2023-09-30 11:57:53.000000 rnspure-0.7.3/RNS/Interfaces/UDPInterface.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.7.3/RNS/Interfaces/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    59544 2024-02-29 22:04:31.000000 rnspure-0.7.3/RNS/Link.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22407 2023-11-13 21:54:52.000000 rnspure-0.7.3/RNS/Packet.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1221 2023-09-29 10:51:48.000000 rnspure-0.7.3/RNS/Resolver.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    47699 2024-01-14 17:44:45.000000 rnspure-0.7.3/RNS/Resource.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    73824 2024-03-01 16:02:36.000000 rnspure-0.7.3/RNS/Reticulum.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   142882 2024-03-01 15:58:26.000000 rnspure-0.7.3/RNS/Transport.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/RNS/Utilities/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/Utilities/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29208 2023-09-25 13:27:00.000000 rnspure-0.7.3/RNS/Utilities/rncp.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29688 2023-12-02 01:10:31.000000 rnspure-0.7.3/RNS/Utilities/rnid.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2762 2023-10-01 19:31:14.000000 rnspure-0.7.3/RNS/Utilities/rnir.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   223143 2024-03-08 00:13:05.000000 rnspure-0.7.3/RNS/Utilities/rnodeconf.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14103 2023-10-01 09:30:53.000000 rnspure-0.7.3/RNS/Utilities/rnpath.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9333 2024-01-08 22:09:09.000000 rnspure-0.7.3/RNS/Utilities/rnprobe.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    13671 2024-03-01 16:29:53.000000 rnspure-0.7.3/RNS/Utilities/rnsd.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13652 2023-10-04 14:31:37.000000 rnspure-0.7.3/RNS/Utilities/rnstatus.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.7.3/RNS/Utilities/rnx.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     8513 2024-01-14 16:17:35.000000 rnspure-0.7.3/RNS/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2024-03-09 20:00:51.000000 rnspure-0.7.3/RNS/_version.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/RNS/vendor/
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/__init__.py
--rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/configobj.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/RNS/vendor/i2plib/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/__version__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/aiosam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/exceptions.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/log.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/sam.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/tunnel.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/i2plib/utils.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/RNS/vendor/ifaddr/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rnspure-0.7.3/RNS/vendor/ifaddr/__init__.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rnspure-0.7.3/RNS/vendor/ifaddr/_posix.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rnspure-0.7.3/RNS/vendor/ifaddr/_shared.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rnspure-0.7.3/RNS/vendor/ifaddr/_win32.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rnspure-0.7.3/RNS/vendor/ifaddr/niwrapper.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2023-05-04 14:41:10.000000 rnspure-0.7.3/RNS/vendor/ifaddr/py.typed
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.7.3/RNS/vendor/platformutils.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/six.py
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.7.3/RNS/vendor/umsgpack.py
-drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-03-09 20:05:16.141478 rnspure-0.7.3/rnspure.egg-info/
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19482 2024-03-09 20:05:16.000000 rnspure-0.7.3/rnspure.egg-info/PKG-INFO
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2296 2024-03-09 20:05:16.000000 rnspure-0.7.3/rnspure.egg-info/SOURCES.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2024-03-09 20:05:16.000000 rnspure-0.7.3/rnspure.egg-info/dependency_links.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)      323 2024-03-09 20:05:16.000000 rnspure-0.7.3/rnspure.egg-info/entry_points.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2024-03-09 20:05:16.000000 rnspure-0.7.3/rnspure.egg-info/top_level.txt
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2024-03-09 20:05:16.141478 rnspure-0.7.3/setup.cfg
--rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2014 2023-10-01 19:31:59.000000 rnspure-0.7.3/setup.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.589969 rnspure-0.7.4/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1110 2024-03-19 10:52:58.000000 rnspure-0.7.4/LICENSE
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19482 2024-05-05 17:55:46.589969 rnspure-0.7.4/PKG-INFO
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    18743 2024-02-16 16:53:41.000000 rnspure-0.7.4/README.md
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.576636 rnspure-0.7.4/RNS/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13058 2023-09-29 08:24:08.000000 rnspure-0.7.4/RNS/Buffer.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26025 2023-09-18 21:33:08.000000 rnspure-0.7.4/RNS/Channel.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.579969 rnspure-0.7.4/RNS/Cryptography/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2735 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/AES.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      988 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/Ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3675 2023-10-20 09:56:32.000000 rnspure-0.7.4/RNS/Cryptography/Fernet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1961 2023-03-02 11:05:06.000000 rnspure-0.7.4/RNS/Cryptography/HKDF.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6885 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/HMAC.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      769 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/Hashes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1541 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/PKCS7.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      794 2023-11-08 19:55:14.000000 rnspure-0.7.4/RNS/Cryptography/Provider.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2611 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/Proxies.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4777 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/SHA256.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5589 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/SHA512.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4917 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/X25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      929 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/__init__.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.579969 rnspure-0.7.4/RNS/Cryptography/aes/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       20 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/aes/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8905 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/aes/aes.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7045 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/aes/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.579969 rnspure-0.7.4/RNS/Cryptography/pure25519/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/pure25519/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1939 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/pure25519/_ed25519.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13056 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/pure25519/basic.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8193 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/pure25519/ed25519_oop.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3156 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Cryptography/pure25519/eddsa.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    21094 2023-10-27 21:40:40.000000 rnspure-0.7.4/RNS/Destination.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    24471 2024-05-04 13:50:54.000000 rnspure-0.7.4/RNS/Identity.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.583302 rnspure-0.7.4/RNS/Interfaces/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14545 2023-10-01 09:35:17.000000 rnspure-0.7.4/RNS/Interfaces/AX25KISSInterface.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.583302 rnspure-0.7.4/RNS/Interfaces/Android/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    16766 2023-10-02 15:26:34.000000 rnspure-0.7.4/RNS/Interfaces/Android/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    57478 2023-11-06 22:55:05.000000 rnspure-0.7.4/RNS/Interfaces/Android/RNodeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    10378 2023-10-02 15:27:09.000000 rnspure-0.7.4/RNS/Interfaces/Android/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1290 2022-10-20 17:28:52.000000 rnspure-0.7.4/RNS/Interfaces/Android/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21874 2024-05-01 13:44:51.000000 rnspure-0.7.4/RNS/Interfaces/AutoInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    41618 2023-09-30 16:02:25.000000 rnspure-0.7.4/RNS/Interfaces/I2PInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     9790 2023-12-25 10:34:55.000000 rnspure-0.7.4/RNS/Interfaces/Interface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13816 2023-10-01 09:35:08.000000 rnspure-0.7.4/RNS/Interfaces/KISSInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13934 2024-01-14 22:33:50.000000 rnspure-0.7.4/RNS/Interfaces/LocalInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     6568 2023-09-30 11:56:53.000000 rnspure-0.7.4/RNS/Interfaces/PipeInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    39095 2024-02-13 18:00:00.000000 rnspure-0.7.4/RNS/Interfaces/RNodeInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     7451 2023-10-01 09:34:57.000000 rnspure-0.7.4/RNS/Interfaces/SerialInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    21979 2023-11-05 21:57:12.000000 rnspure-0.7.4/RNS/Interfaces/TCPInterface.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4191 2023-09-30 11:57:53.000000 rnspure-0.7.4/RNS/Interfaces/UDPInterface.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     1321 2022-10-21 23:31:41.000000 rnspure-0.7.4/RNS/Interfaces/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    59657 2024-05-04 18:25:52.000000 rnspure-0.7.4/RNS/Link.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    22407 2023-11-13 21:54:52.000000 rnspure-0.7.4/RNS/Packet.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1221 2023-09-29 10:51:48.000000 rnspure-0.7.4/RNS/Resolver.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    47774 2024-03-19 10:51:51.000000 rnspure-0.7.4/RNS/Resource.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    74028 2024-05-01 13:44:17.000000 rnspure-0.7.4/RNS/Reticulum.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   146803 2024-05-04 19:55:41.000000 rnspure-0.7.4/RNS/Transport.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.586636 rnspure-0.7.4/RNS/Utilities/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1291 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/Utilities/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29208 2023-09-25 13:27:00.000000 rnspure-0.7.4/RNS/Utilities/rncp.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    29688 2023-12-02 01:10:31.000000 rnspure-0.7.4/RNS/Utilities/rnid.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2762 2023-10-01 19:31:14.000000 rnspure-0.7.4/RNS/Utilities/rnir.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)   227272 2024-05-03 16:19:23.000000 rnspure-0.7.4/RNS/Utilities/rnodeconf.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    14103 2023-10-01 09:30:53.000000 rnspure-0.7.4/RNS/Utilities/rnpath.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9333 2024-01-08 22:09:09.000000 rnspure-0.7.4/RNS/Utilities/rnprobe.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    13671 2024-03-01 16:29:53.000000 rnspure-0.7.4/RNS/Utilities/rnsd.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    13652 2023-10-04 14:31:37.000000 rnspure-0.7.4/RNS/Utilities/rnstatus.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    26422 2023-02-02 12:55:50.000000 rnspure-0.7.4/RNS/Utilities/rnx.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)     8513 2024-01-14 16:17:35.000000 rnspure-0.7.4/RNS/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       22 2024-05-03 20:20:26.000000 rnspure-0.7.4/RNS/_version.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.586636 rnspure-0.7.4/RNS/vendor/
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)      166 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/__init__.py
+-rwxr-xr-x   0 markqvist  (1000) markqvist  (1000)    89634 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/configobj.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.589969 rnspure-0.7.4/RNS/vendor/i2plib/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      667 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      316 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/__version__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     9939 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/aiosam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1158 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/exceptions.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      122 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/log.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     4397 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/sam.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     8983 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/tunnel.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1203 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/i2plib/utils.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.589969 rnspure-0.7.4/RNS/vendor/ifaddr/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1432 2023-05-05 08:23:36.000000 rnspure-0.7.4/RNS/vendor/ifaddr/__init__.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     3646 2023-05-05 08:19:48.000000 rnspure-0.7.4/RNS/vendor/ifaddr/_posix.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     7321 2023-05-05 08:20:00.000000 rnspure-0.7.4/RNS/vendor/ifaddr/_shared.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     5107 2023-05-05 08:20:05.000000 rnspure-0.7.4/RNS/vendor/ifaddr/_win32.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1141 2023-05-05 08:36:33.000000 rnspure-0.7.4/RNS/vendor/ifaddr/niwrapper.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        0 2023-05-04 14:41:10.000000 rnspure-0.7.4/RNS/vendor/ifaddr/py.typed
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     1184 2022-10-21 23:31:14.000000 rnspure-0.7.4/RNS/vendor/platformutils.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    34549 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/six.py
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    43449 2022-10-20 15:25:41.000000 rnspure-0.7.4/RNS/vendor/umsgpack.py
+drwxr-xr-x   0 markqvist  (1000) markqvist  (1000)        0 2024-05-05 17:55:46.589969 rnspure-0.7.4/rnspure.egg-info/
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)    19482 2024-05-05 17:55:46.000000 rnspure-0.7.4/rnspure.egg-info/PKG-INFO
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2296 2024-05-05 17:55:46.000000 rnspure-0.7.4/rnspure.egg-info/SOURCES.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        1 2024-05-05 17:55:46.000000 rnspure-0.7.4/rnspure.egg-info/dependency_links.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)      323 2024-05-05 17:55:46.000000 rnspure-0.7.4/rnspure.egg-info/entry_points.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)        4 2024-05-05 17:55:46.000000 rnspure-0.7.4/rnspure.egg-info/top_level.txt
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)       38 2024-05-05 17:55:46.589969 rnspure-0.7.4/setup.cfg
+-rw-r--r--   0 markqvist  (1000) markqvist  (1000)     2014 2023-10-01 19:31:59.000000 rnspure-0.7.4/setup.py
```

### Comparing `rnspure-0.7.3/LICENSE` & `rnspure-0.7.4/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License, unless otherwise noted
 
-Copyright (c) 2016-2023 Mark Qvist / unsigned.io
+Copyright (c) 2016-2024 Mark Qvist / unsigned.io
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rnspure-0.7.3/PKG-INFO` & `rnspure-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnspure
-Version: 0.7.3
+Version: 0.7.4
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rnspure-0.7.3/README.md` & `rnspure-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Buffer.py` & `rnspure-0.7.4/RNS/Buffer.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Channel.py` & `rnspure-0.7.4/RNS/Channel.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/AES.py` & `rnspure-0.7.4/RNS/Cryptography/AES.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/Ed25519.py` & `rnspure-0.7.4/RNS/Cryptography/Ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/Fernet.py` & `rnspure-0.7.4/RNS/Cryptography/Fernet.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/HKDF.py` & `rnspure-0.7.4/RNS/Cryptography/HKDF.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/HMAC.py` & `rnspure-0.7.4/RNS/Cryptography/HMAC.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/Hashes.py` & `rnspure-0.7.4/RNS/Cryptography/Hashes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/PKCS7.py` & `rnspure-0.7.4/RNS/Cryptography/PKCS7.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/Provider.py` & `rnspure-0.7.4/RNS/Cryptography/Provider.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/Proxies.py` & `rnspure-0.7.4/RNS/Cryptography/Proxies.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/SHA256.py` & `rnspure-0.7.4/RNS/Cryptography/SHA256.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/SHA512.py` & `rnspure-0.7.4/RNS/Cryptography/SHA512.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/X25519.py` & `rnspure-0.7.4/RNS/Cryptography/X25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/__init__.py` & `rnspure-0.7.4/RNS/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/aes/aes.py` & `rnspure-0.7.4/RNS/Cryptography/aes/aes.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/aes/utils.py` & `rnspure-0.7.4/RNS/Cryptography/aes/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/pure25519/_ed25519.py` & `rnspure-0.7.4/RNS/Cryptography/pure25519/_ed25519.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/pure25519/basic.py` & `rnspure-0.7.4/RNS/Cryptography/pure25519/basic.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/pure25519/ed25519_oop.py` & `rnspure-0.7.4/RNS/Cryptography/pure25519/ed25519_oop.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Cryptography/pure25519/eddsa.py` & `rnspure-0.7.4/RNS/Cryptography/pure25519/eddsa.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Destination.py` & `rnspure-0.7.4/RNS/Destination.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Identity.py` & `rnspure-0.7.4/RNS/Identity.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/AX25KISSInterface.py` & `rnspure-0.7.4/RNS/Interfaces/AX25KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/Android/KISSInterface.py` & `rnspure-0.7.4/RNS/Interfaces/Android/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/Android/RNodeInterface.py` & `rnspure-0.7.4/RNS/Interfaces/Android/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/Android/SerialInterface.py` & `rnspure-0.7.4/RNS/Interfaces/Android/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/Android/__init__.py` & `rnspure-0.7.4/RNS/Interfaces/Android/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/AutoInterface.py` & `rnspure-0.7.4/RNS/Interfaces/AutoInterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
     SCOPE_LINK         = "2"
     SCOPE_ADMIN        = "4"
     SCOPE_SITE         = "5"
     SCOPE_ORGANISATION = "8"
     SCOPE_GLOBAL       = "e"
 
+    MULTICAST_PERMANENT_ADDRESS_TYPE = "0"
+    MULTICAST_TEMPORARY_ADDRESS_TYPE = "1"
+
     PEERING_TIMEOUT    = 7.5
 
     ALL_IGNORE_IFS     = ["lo0"]
     DARWIN_IGNORE_IFS  = ["awdl0", "llw0", "lo0", "en5"]
     ANDROID_IGNORE_IFS = ["dummy0", "lo", "tun0"]
 
     BITRATE_GUESS      = 10*1000*1000
@@ -70,15 +73,15 @@
         ifs = self.netinfo.interfaces()
         return ifs
 
     def list_addresses(self, ifname):
         ifas = self.netinfo.ifaddresses(ifname)
         return ifas
 
-    def __init__(self, owner, name, group_id=None, discovery_scope=None, discovery_port=None, data_port=None, allowed_interfaces=None, ignored_interfaces=None, configured_bitrate=None):
+    def __init__(self, owner, name, group_id=None, discovery_scope=None, discovery_port=None, multicast_address_type=None, data_port=None, allowed_interfaces=None, ignored_interfaces=None, configured_bitrate=None):
         from RNS.vendor.ifaddr import niwrapper
         super().__init__()
         self.netinfo = niwrapper
 
         self.HW_MTU = 1064
 
         self.IN  = True
@@ -124,14 +127,23 @@
             self.group_id = group_id.encode("utf-8")
 
         if discovery_port == None:
             self.discovery_port = AutoInterface.DEFAULT_DISCOVERY_PORT
         else:
             self.discovery_port = discovery_port
 
+        if multicast_address_type == None:
+            self.multicast_address_type = AutoInterface.MULTICAST_TEMPORARY_ADDRESS_TYPE
+        elif str(multicast_address_type).lower() == "temporary":
+            self.multicast_address_type = AutoInterface.MULTICAST_TEMPORARY_ADDRESS_TYPE
+        elif str(multicast_address_type).lower() == "permanent":
+            self.multicast_address_type = AutoInterface.MULTICAST_PERMANENT_ADDRESS_TYPE
+        else:
+            self.multicast_address_type = AutoInterface.MULTICAST_TEMPORARY_ADDRESS_TYPE
+
         if data_port == None:
             self.data_port = AutoInterface.DEFAULT_DATA_PORT
         else:
             self.data_port = data_port
 
         if discovery_scope == None:
             self.discovery_scope = AutoInterface.SCOPE_LINK
@@ -152,15 +164,15 @@
         gt  = "0"
         gt += ":"+"{:02x}".format(g[3]+(g[2]<<8))
         gt += ":"+"{:02x}".format(g[5]+(g[4]<<8))
         gt += ":"+"{:02x}".format(g[7]+(g[6]<<8))
         gt += ":"+"{:02x}".format(g[9]+(g[8]<<8))
         gt += ":"+"{:02x}".format(g[11]+(g[10]<<8))
         gt += ":"+"{:02x}".format(g[13]+(g[12]<<8))
-        self.mcast_discovery_address = "ff1"+self.discovery_scope+":"+gt
+        self.mcast_discovery_address = "ff"+self.multicast_address_type+self.discovery_scope+":"+gt
 
         suitable_interfaces = 0
         for ifname in self.list_interfaces():
             if RNS.vendor.platformutils.is_darwin() and ifname in AutoInterface.DARWIN_IGNORE_IFS and not ifname in self.allowed_interfaces:
                 RNS.log(str(self)+" skipping Darwin AWDL or tethering interface "+str(ifname), RNS.LOG_EXTREME)
             elif RNS.vendor.platformutils.is_darwin() and ifname == "lo0":
                 RNS.log(str(self)+" skipping Darwin loopback interface "+str(ifname), RNS.LOG_EXTREME)
```

### Comparing `rnspure-0.7.3/RNS/Interfaces/I2PInterface.py` & `rnspure-0.7.4/RNS/Interfaces/I2PInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/Interface.py` & `rnspure-0.7.4/RNS/Interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/KISSInterface.py` & `rnspure-0.7.4/RNS/Interfaces/KISSInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/LocalInterface.py` & `rnspure-0.7.4/RNS/Interfaces/LocalInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/PipeInterface.py` & `rnspure-0.7.4/RNS/Interfaces/PipeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/RNodeInterface.py` & `rnspure-0.7.4/RNS/Interfaces/RNodeInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/SerialInterface.py` & `rnspure-0.7.4/RNS/Interfaces/SerialInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/TCPInterface.py` & `rnspure-0.7.4/RNS/Interfaces/TCPInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/UDPInterface.py` & `rnspure-0.7.4/RNS/Interfaces/UDPInterface.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Interfaces/__init__.py` & `rnspure-0.7.4/RNS/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Link.py` & `rnspure-0.7.4/RNS/Link.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,24 +164,27 @@
         self.stale_time = Link.STALE_TIME
         self.watchdog_lock = False
         self.status = Link.PENDING
         self.activated_at = None
         self.type = RNS.Destination.LINK
         self.owner = owner
         self.destination = destination
+        self.expected_hops = None
         self.attached_interface = None
         self.__remote_identity = None
         self.__track_phy_stats = False
         self._channel = None
+
         if self.destination == None:
             self.initiator = False
             self.prv     = X25519PrivateKey.generate()
             self.sig_prv = self.owner.identity.sig_prv
         else:
             self.initiator = True
+            self.expected_hops = RNS.Transport.hops_to(self.destination.hash)
             self.establishment_timeout  = RNS.Reticulum.get_instance().get_first_hop_timeout(destination.hash)
             self.establishment_timeout += Link.ESTABLISHMENT_TIMEOUT_PER_HOP * max(1, RNS.Transport.hops_to(destination.hash))
             self.prv     = X25519PrivateKey.generate()
             self.sig_prv = Ed25519PrivateKey.generate()
 
         self.fernet  = None
```

### Comparing `rnspure-0.7.3/RNS/Packet.py` & `rnspure-0.7.4/RNS/Packet.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Resolver.py` & `rnspure-0.7.4/RNS/Resolver.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Resource.py` & `rnspure-0.7.4/RNS/Resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1019,14 +1019,15 @@
     @staticmethod
     def read_size(advertisement_packet):
         adv = ResourceAdvertisement.unpack(advertisement_packet.plaintext)
         return adv.d
 
 
     def __init__(self, resource=None, request_id=None, is_response=False):
+        self.link = None
         if resource != None:
             self.t = resource.size              # Transfer size
             self.d = resource.total_size        # Total uncompressed data size
             self.n = len(resource.parts)        # Number of parts
             self.h = resource.hash              # Resource hash
             self.r = resource.random_hash       # Resource random hash
             self.o = resource.original_hash     # First-segment hash
@@ -1065,14 +1066,17 @@
 
     def get_hash(self):
         return self.h
 
     def is_compressed(self):
         return self.c
 
+    def get_link(self):
+        return self.link
+
     def pack(self, segment=0):
         hashmap_start = segment*ResourceAdvertisement.HASHMAP_MAX_LEN
         hashmap_end   = min((segment+1)*(ResourceAdvertisement.HASHMAP_MAX_LEN), self.n)
 
         hashmap = b""
         for i in range(hashmap_start,hashmap_end):
             hashmap += self.m[i*Resource.MAPHASH_LEN:(i+1)*Resource.MAPHASH_LEN]
```

### Comparing `rnspure-0.7.3/RNS/Reticulum.py` & `rnspure-0.7.4/RNS/Reticulum.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,24 +536,26 @@
 
                             if (("interface_enabled" in c) and c.as_bool("interface_enabled") == True) or (("enabled" in c) and c.as_bool("enabled") == True):
                                 if c["type"] == "AutoInterface":
                                     if not RNS.vendor.platformutils.is_windows():
                                         group_id        = c["group_id"] if "group_id" in c else None
                                         discovery_scope = c["discovery_scope"] if "discovery_scope" in c else None
                                         discovery_port  = int(c["discovery_port"]) if "discovery_port" in c else None
+                                        multicast_address_type = c["multicast_address_type"] if "multicast_address_type" in c else None
                                         data_port  = int(c["data_port"]) if "data_port" in c else None
                                         allowed_interfaces = c.as_list("devices") if "devices" in c else None
                                         ignored_interfaces = c.as_list("ignored_devices") if "ignored_devices" in c else None
 
                                         interface = AutoInterface.AutoInterface(
                                             RNS.Transport,
                                             name,
                                             group_id,
                                             discovery_scope,
                                             discovery_port,
+                                            multicast_address_type,
                                             data_port,
                                             allowed_interfaces,
                                             ignored_interfaces
                                         )
 
                                         if "outgoing" in c and c.as_bool("outgoing") == False:
                                             interface.OUT = False
```

### Comparing `rnspure-0.7.3/RNS/Transport.py` & `rnspure-0.7.4/RNS/Transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     ROAMING_PATH_TIME = 60*60*6    # Path expiration of 6 hours for Roaming paths
 
     # TODO: Calculate an optimal number for this in
     # various situations
     LOCAL_REBROADCASTS_MAX = 2          # How many local rebroadcasts of an announce is allowed
 
     PATH_REQUEST_TIMEOUT = 15           # Default timuout for client path requests in seconds
-    PATH_REQUEST_GRACE   = 0.35         # Grace time before a path announcement is made, allows directly reachable peers to respond first
-    PATH_REQUEST_RW      = 2            # Path request random window
+    PATH_REQUEST_GRACE   = 0.4          # Grace time before a path announcement is made, allows directly reachable peers to respond first
+    PATH_REQUEST_RG      = 0.6          # Extra grace time for roaming-mode interfaces to allow more suitable peers to respond first
     PATH_REQUEST_MI      = 20           # Minimum interval in seconds for automated path requests
 
     STATE_UNKNOWN        = 0x00
     STATE_UNRESPONSIVE   = 0x01
     STATE_RESPONSIVE     = 0x02
 
     LINK_TIMEOUT         = RNS.Link.STALE_TIME * 1.25
@@ -742,15 +742,16 @@
             packet.sent = True
             packet.sent_at = time.time()
 
             if generate_receipt:
                 packet.receipt = RNS.PacketReceipt(packet)
                 Transport.receipts.append(packet.receipt)
             
-            Transport.cache(packet)
+            # TODO: Enable when caching has been redesigned
+            # Transport.cache(packet)
 
         # Check if we have a known path for the destination in the path table
         if packet.packet_type != RNS.Packet.ANNOUNCE and packet.destination.type != RNS.Destination.PLAIN and packet.destination.type != RNS.Destination.GROUP and packet.destination_hash in Transport.destination_table:
             outbound_interface = Transport.destination_table[packet.destination_hash][5]
 
             # If there's more than one hop to the destination, and we know
             # a path, we insert the packet into transport by adding the next
@@ -968,14 +969,21 @@
         return sent
 
     @staticmethod
     def packet_filter(packet):
         # TODO: Think long and hard about this.
         # Is it even strictly necessary with the current
         # transport rules?
+
+        # Filter packets intended for other transport instances
+        if packet.transport_id != None and packet.packet_type != RNS.Packet.ANNOUNCE:
+            if packet.transport_id != Transport.identity.hash:
+                RNS.log("Ignored packet "+RNS.prettyhexrep(packet.packet_hash)+" in transport for other transport instance", RNS.LOG_EXTREME)
+                return False
+
         if packet.context == RNS.Packet.KEEPALIVE:
             return True
         if packet.context == RNS.Packet.RESOURCE_REQ:
             return True
         if packet.context == RNS.Packet.RESOURCE_PRF:
             return True
         if packet.context == RNS.Packet.RESOURCE:
@@ -1132,18 +1140,39 @@
         if len(Transport.local_client_interfaces) > 0:
             if Transport.is_local_client_interface(interface):
                 packet.hops -= 1
 
         elif Transport.interface_to_shared_instance(interface):
             packet.hops -= 1
 
-
         if Transport.packet_filter(packet):
-            Transport.packet_hashlist.append(packet.packet_hash)
-            Transport.cache(packet)
+            # By default, remember packet hashes to avoid routing
+            # loops in the network, using the packet filter.
+            remember_packet_hash = True
+
+            # If this packet belongs to a link in our link table,
+            # we'll have to defer adding it to the filter list.
+            # In some cases, we might see a packet over a shared-
+            # medium interface, belonging to a link that transports
+            # or terminates with this instance, but before it would
+            # normally reach us. If the packet is appended to the
+            # filter list at this point, link transport will break.
+            if packet.destination_hash in Transport.link_table:
+                remember_packet_hash = False
+
+            # If this is a link request proof, don't add it until
+            # we are sure it's not actually somewhere else in the
+            # routing chain.
+            if packet.packet_type == RNS.Packet.PROOF and packet.context == RNS.Packet.LRPROOF:
+                remember_packet_hash = False
+
+            if remember_packet_hash:
+                Transport.packet_hashlist.append(packet.packet_hash)
+                # TODO: Enable when caching has been redesigned
+                # Transport.cache(packet)
             
             # Check special conditions for local clients connected
             # through a shared Reticulum instance
             from_local_client         = (packet.receiving_interface in Transport.local_client_interfaces)
             for_local_client          = (packet.packet_type != RNS.Packet.ANNOUNCE) and (packet.destination_hash in Transport.destination_table and Transport.destination_table[packet.destination_hash][2] == 0)
             for_local_client_link     = (packet.packet_type != RNS.Packet.ANNOUNCE) and (packet.destination_hash in Transport.link_table and Transport.link_table[packet.destination_hash][4] in Transport.local_client_interfaces)
             for_local_client_link    |= (packet.packet_type != RNS.Packet.ANNOUNCE) and (packet.destination_hash in Transport.link_table and Transport.link_table[packet.destination_hash][2] in Transport.local_client_interfaces)
@@ -1256,15 +1285,15 @@
                 # Link transport handling. Directs packets according
                 # to entries in the link tables
                 if packet.packet_type != RNS.Packet.ANNOUNCE and packet.packet_type != RNS.Packet.LINKREQUEST and packet.context != RNS.Packet.LRPROOF:
                     if packet.destination_hash in Transport.link_table:
                         link_entry = Transport.link_table[packet.destination_hash]
                         # If receiving and outbound interface is
                         # the same for this link, direction doesn't
-                        # matter, and we simply send the packet on.
+                        # matter, and we simply repeat the packet.
                         outbound_interface = None
                         if link_entry[2] == link_entry[4]:
                             # But check that taken hops matches one
                             # of the expectede values.
                             if packet.hops == link_entry[3] or packet.hops == link_entry[5]:
                                 outbound_interface = link_entry[2]
                         else:
@@ -1277,14 +1306,19 @@
                                     outbound_interface = link_entry[4]
                             elif packet.receiving_interface == link_entry[4]:
                                 # Also check that expected hop count matches
                                 if packet.hops == link_entry[5]:
                                     outbound_interface = link_entry[2]
 
                         if outbound_interface != None:
+                            # Add this packet to the filter hashlist if we
+                            # have determined that it's actually our turn
+                            # to process it.
+                            Transport.packet_hashlist.append(packet.packet_hash)
+
                             new_raw = packet.raw[0:1]
                             new_raw += struct.pack("!B", packet.hops)
                             new_raw += packet.raw[2:]
                             Transport.transmit(outbound_interface, new_raw)
                             Transport.link_table[packet.destination_hash][0] = time.time()
                         else:
                             pass
@@ -1708,15 +1742,32 @@
                         else:
                             RNS.log("Received link request proof with hop mismatch, not transporting it", RNS.LOG_DEBUG)
                     else:
                         # Check if we can deliver it to a local
                         # pending link
                         for link in Transport.pending_links:
                             if link.link_id == packet.destination_hash:
-                                link.validate_proof(packet)
+                                # We need to also allow an expected hops value of
+                                # PATHFINDER_M, since in some cases, the number of hops
+                                # to the destination will be unknown at link creation
+                                # time. The real chance of this occuring is likely to be
+                                # extremely small, and this allowance could probably
+                                # be discarded without major issues, but it is kept
+                                # for now to ensure backwards compatibility.
+
+                                # TODO: Probably reset check back to
+                                # if packet.hops == link.expected_hops:
+                                # within one of the next releases
+
+                                if packet.hops == link.expected_hops or link.expected_hops == RNS.Transport.PATHFINDER_M:
+                                    # Add this packet to the filter hashlist if we
+                                    # have determined that it's actually destined
+                                    # for this system, and then validate the proof
+                                    Transport.packet_hashlist.append(packet.packet_hash)
+                                    link.validate_proof(packet)
 
                 elif packet.context == RNS.Packet.RESOURCE_PRF:
                     for link in Transport.active_links:
                         if link.link_id == packet.destination_hash:
                             link.receive(packet)
                 else:
                     if packet.destination_type == RNS.Destination.LINK:
@@ -1725,15 +1776,15 @@
                                 packet.link = link
                                 
                     if len(packet.data) == RNS.PacketReceipt.EXPL_LENGTH:
                         proof_hash = packet.data[:RNS.Identity.HASHLENGTH//8]
                     else:
                         proof_hash = None
 
-                    # Check if this proof neds to be transported
+                    # Check if this proof needs to be transported
                     if (RNS.Reticulum.transport_enabled() or from_local_client or proof_for_local_client) and packet.destination_hash in Transport.reverse_table:
                         reverse_entry = Transport.reverse_table.pop(packet.destination_hash)
                         if packet.receiving_interface == reverse_entry[1]:
                             RNS.log("Proof received on correct interface, transporting it via "+str(reverse_entry[0]), RNS.LOG_EXTREME)
                             new_raw = packet.raw[0:1]
                             new_raw += struct.pack("!B", packet.hops)
                             new_raw += packet.raw[2:]
@@ -2120,14 +2171,15 @@
     def mark_path_unknown_state(destination_hash):
         if destination_hash in Transport.destination_table:
             Transport.path_states[destination_hash] = Transport.STATE_UNKNOWN
             return True
         else:
             return False
 
+    @staticmethod
     def path_is_unresponsive(destination_hash):
         if destination_hash in Transport.path_states:
             if Transport.path_states[destination_hash] == Transport.STATE_UNRESPONSIVE:
                 return True
 
         return False
 
@@ -2284,16 +2336,26 @@
                     local_rebroadcasts = 0
                     block_rebroadcasts = True
                     announce_hops      = packet.hops
 
                     if is_from_local_client:
                         retransmit_timeout = now
                     else:
-                        # TODO: Look at this timing
-                        retransmit_timeout = now + Transport.PATH_REQUEST_GRACE # + (RNS.rand() * Transport.PATHFINDER_RW)
+                        if Transport.is_local_client_interface(Transport.next_hop_interface(destination_hash)):
+                            RNS.log("Path request destination "+RNS.prettyhexrep(destination_hash)+" is on a local client interface, rebroadcasting immediately", RNS.LOG_EXTREME)
+                            retransmit_timeout = now
+
+                        else:
+                            retransmit_timeout = now + Transport.PATH_REQUEST_GRACE
+
+                            # If we are answering on a roaming-mode interface, wait a
+                            # little longer, to allow potential more well-connected
+                            # peers to answer first.
+                            if attached_interface.mode == RNS.Interfaces.Interface.Interface.MODE_ROAMING:
+                                retransmit_timeout += Transport.PATH_REQUEST_RG
 
                     # This handles an edge case where a peer sends a past
                     # request for a destination just after an announce for
                     # said destination has arrived, but before it has been
                     # rebroadcast locally. In such a case the actual announce
                     # is temporarily held, and then reinserted when the path
                     # request has been served to the peer.
```

### Comparing `rnspure-0.7.3/RNS/Utilities/__init__.py` & `rnspure-0.7.4/RNS/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rncp.py` & `rnspure-0.7.4/RNS/Utilities/rncp.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnid.py` & `rnspure-0.7.4/RNS/Utilities/rnid.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnir.py` & `rnspure-0.7.4/RNS/Utilities/rnir.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnodeconf.py` & `rnspure-0.7.4/RNS/Utilities/rnodeconf.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,21 +145,26 @@
     PRODUCT_T32_20 = 0xB0
     MODEL_B3       = 0xB3
     MODEL_B8       = 0xB8
 
     PRODUCT_T32_21 = 0xB1
     MODEL_B4       = 0xB4
     MODEL_B9       = 0xB9
-    MODEL_B4_TCXO  = 0x04
-    MODEL_B9_TCXO  = 0x09
+    MODEL_B4_TCXO  = 0x04 # The TCXO model codes are only used here to select the
+    MODEL_B9_TCXO  = 0x09 # correct firmware, actual model codes in firmware is
+                          # still 0xB4 and 0xB9.
 
     PRODUCT_H32_V2 = 0xC0
     MODEL_C4       = 0xC4
     MODEL_C9       = 0xC9
 
+    PRODUCT_H32_V3 = 0xC1
+    MODEL_C5       = 0xC5
+    MODEL_CA       = 0xCA
+
     PRODUCT_TBEAM  = 0xE0
     MODEL_E4       = 0xE4
     MODEL_E9       = 0xE9
     MODEL_E3       = 0xE3
     MODEL_E8       = 0xE8
     
     PRODUCT_HMBRW  = 0xF0
@@ -198,14 +203,15 @@
     ROM.PRODUCT_RNODE:  "RNode",
     ROM.PRODUCT_HMBRW:  "Hombrew RNode",
     ROM.PRODUCT_TBEAM:  "LilyGO T-Beam",
     ROM.PRODUCT_T32_10: "LilyGO LoRa32 v1.0",
     ROM.PRODUCT_T32_20: "LilyGO LoRa32 v2.0",
     ROM.PRODUCT_T32_21: "LilyGO LoRa32 v2.1",
     ROM.PRODUCT_H32_V2: "Heltec LoRa32 v2",
+    ROM.PRODUCT_H32_V3: "Heltec LoRa32 v3",
 }
 
 platforms = {
     ROM.PLATFORM_AVR: "AVR",
     ROM.PLATFORM_ESP32:"ESP32",
     ROM.PLATFORM_NRF52:"NRF52",
 }
@@ -232,14 +238,16 @@
     0xB9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v21.zip", "SX1276"],
     0x04: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_lora32v21_tcxo.zip", "SX1278"],
     0x09: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v21_tcxo.zip", "SX1276"],
     0xBA: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_lora32v10.zip", "SX1278"],
     0xBB: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_lora32v10.zip", "SX1276"],
     0xC4: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_heltec32v2.zip", "SX1278"],
     0xC9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_heltec32v2.zip", "SX1276"],
+    0xC5: [470000000, 510000000, 21, "470 - 510 MHz", "rnode_firmware_heltec32v3.zip", "SX1262"],
+    0xCA: [863000000, 928000000, 21, "863 - 928 MHz", "rnode_firmware_heltec32v3.zip", "SX1262"],
     0xE4: [420000000, 520000000, 17, "420 - 520 MHz", "rnode_firmware_tbeam.zip", "SX1278"],
     0xE9: [850000000, 950000000, 17, "850 - 950 MHz", "rnode_firmware_tbeam.zip", "SX1276"],
     0xE3: [420000000, 520000000, 22, "420 - 520 MHz", "rnode_firmware_tbeam_sx1262.zip", "SX1268"],
     0xE8: [850000000, 950000000, 22, "850 - 950 MHz", "rnode_firmware_tbeam_sx1262.zip", "SX1262"],
     0xFE: [100000000, 1100000000, 17, "(Band capabilities unknown)", None, "Unknown"],
     0xFF: [100000000, 1100000000, 14, "(Band capabilities unknown)", None, "Unknown"],
 }
@@ -769,26 +777,21 @@
                 self.product = self.eeprom[ROM.ADDR_PRODUCT]
                 self.model = self.eeprom[ROM.ADDR_MODEL]
                 self.hw_rev = self.eeprom[ROM.ADDR_HW_REV]
                 self.serialno = bytes([self.eeprom[ROM.ADDR_SERIAL], self.eeprom[ROM.ADDR_SERIAL+1], self.eeprom[ROM.ADDR_SERIAL+2], self.eeprom[ROM.ADDR_SERIAL+3]])
                 self.made = bytes([self.eeprom[ROM.ADDR_MADE], self.eeprom[ROM.ADDR_MADE+1], self.eeprom[ROM.ADDR_MADE+2], self.eeprom[ROM.ADDR_MADE+3]])
                 self.checksum = b""
 
-
-                self.min_freq = models[self.model][0]
-                self.max_freq = models[self.model][1]
-                self.max_output = models[self.model][2]
-
                 try:
                     self.min_freq = models[self.model][0]
                     self.max_freq = models[self.model][1]
                     self.max_output = models[self.model][2]
                 except Exception as e:
-                    RNS.log("Exception")
-                    RNS.log(str(e))
+                    RNS.log("Error: Model band and output power capabilities are unknown!")
+                    RNS.log("The contained exception was: "+str(e))
                     self.min_freq = 0
                     self.max_freq = 0
                     self.max_output = 0
 
                 for i in range(0,16):
                     self.checksum = self.checksum+bytes([self.eeprom[ROM.ADDR_CHKSUM+i]])
 
@@ -1552,27 +1555,28 @@
             print("       |    of your own design, or if you are prototyping one.")
             print("")
             print("[3] LilyGO LoRa32 v2.1 (aka T3 v1.6 / T3 v1.6.1)")
             print("[4] LilyGO LoRa32 v2.0")
             print("[5] LilyGO LoRa32 v1.0")
             print("[6] LilyGO T-Beam")
             print("[7] Heltec LoRa32 v2")
-            print("[8] LilyGO LoRa T3S3")
+            print("[8] Heltec LoRa32 v3")
+            #print("[9] LilyGO LoRa T3S3")
             print("       .")
             print("      / \\   Select one of these options if you want to easily turn")
             print("       |    a supported development board into an RNode.")
             print("")
             print("---------------------------------------------------------------------------")
             print("\nEnter the number that matches your device type:\n? ", end="")
 
             selected_product = None
             try:
                 c_dev = int(input())
                 c_mod = False
-                if c_dev < 1 or c_dev > 8:
+                if c_dev < 1 or c_dev > 9:
                     raise ValueError()
                 elif c_dev == 1:
                     selected_product = ROM.PRODUCT_RNODE
                 elif c_dev == 2:
                     selected_product = ROM.PRODUCT_HMBRW
                     clear()
                     print("")
@@ -1664,15 +1668,15 @@
                     print("to USB chips on Heltec LoRa V2 boards, resulting in intermittent USB comms")
                     print("and problems flashing and updating devices.")
                     print("")
                     print("The currently supplied firmware is provided AS-IS as a courtesey to those")
                     print("who would like to experiment with it. Hit enter to continue.")
                     print("---------------------------------------------------------------------------")
                     input()
-                elif c_dev == 8:
+                elif c_dev == 9:
                     selected_product = ROM.PRODUCT_RNODE
                     c_mod = True
                     clear()
                     print("")
                     print("---------------------------------------------------------------------------")
                     print("                     LilyGO LoRa32 T3S3 RNode Installer")
                     print("")
@@ -1681,14 +1685,30 @@
                     print("")
                     print("Please note that Bluetooth is currently not implemented on this board.")
                     print("")
                     print("The currently supplied firmware is provided AS-IS as a courtesey to those")
                     print("who would like to experiment with it. Hit enter to continue.")
                     print("---------------------------------------------------------------------------")
                     input()
+                elif c_dev == 8:
+                    selected_product = ROM.PRODUCT_H32_V3
+                    clear()
+                    print("")
+                    print("---------------------------------------------------------------------------")
+                    print("                     Heltec LoRa32 v3.0 RNode Installer")
+                    print("")
+                    print("Important! Using RNode firmware on Heltec devices should currently be")
+                    print("considered experimental. It is not intended for production or critical use.")
+                    print("")
+                    print("Please note that Bluetooth is currently not implemented on this board.")
+                    print("")
+                    print("The currently supplied firmware is provided AS-IS as a courtesey to those")
+                    print("who would like to experiment with it. Hit enter to continue.")
+                    print("---------------------------------------------------------------------------")
+                    input()
             except Exception as e:
                 print("That device type does not exist, exiting now.")
                 exit()
 
             selected_platform = None
             selected_model = None
             selected_mcu = None
@@ -1744,16 +1764,14 @@
                     print("[2] Handheld v2.1 RNode, 820 - 1020 MHz")
                     print("")
                     print("[3] Original v1.x RNode, 410 - 525 MHz")
                     print("[4] Original v1.x RNode, 820 - 1020 MHz")
                     print("")
                     print("[5] Prototype v2.2 RNode, 410 - 525 MHz")
                     print("[6] Prototype v2.2 RNode, 820 - 1020 MHz")
-                    # print("[5] Prototype v2 RNode, 410 - 525 MHz")
-                    # print("[6] Prototype v2 RNode, 820 - 1020 MHz")
                     print("\n? ", end="")
                     try:
                         c_model = int(input())
                         if c_model < 1 or c_model > 6:
                             raise ValueError()
                         elif c_model == 1:
                             selected_model = ROM.MODEL_A2
@@ -1787,15 +1805,15 @@
                         #     selected_platform = ROM.PLATFORM_ESP32
                     except Exception as e:
                         print("That model does not exist, exiting now.")
                         exit()
                 else:
                     print("\nWhat model is this T3S3?\n")
                     print("[1] 410 - 525 MHz (with SX1268 chip)")
-                    print("[2] 820 - 1020 MHz (with SX1268 chip)")
+                    print("[2] 820 - 1020 MHz (with SX1262 chip)")
                     print("\n? ", end="")
                     try:
                         c_model = int(input())
                         if c_model < 1 or c_model > 2:
                             raise ValueError()
                         elif c_model == 1:
                             selected_model = ROM.MODEL_A1
@@ -1928,14 +1946,36 @@
                     elif c_model > 1:
                         selected_model = ROM.MODEL_C9
                         selected_platform = ROM.PLATFORM_ESP32
                 except Exception as e:
                     print("That band does not exist, exiting now.")
                     exit()
 
+            elif selected_product == ROM.PRODUCT_H32_V3:
+                selected_mcu = ROM.MCU_ESP32
+                print("\nWhat band is this Heltec LoRa32 V3 for?\n")
+                print("[1] 433 MHz")
+                print("[2] 868 MHz")
+                print("[3] 915 MHz")
+                print("[4] 923 MHz")
+                print("\n? ", end="")
+                try:
+                    c_model = int(input())
+                    if c_model < 1 or c_model > 4:
+                        raise ValueError()
+                    elif c_model == 1:
+                        selected_model = ROM.MODEL_C5
+                        selected_platform = ROM.PLATFORM_ESP32
+                    elif c_model > 1:
+                        selected_model = ROM.MODEL_CA
+                        selected_platform = ROM.PLATFORM_ESP32
+                except Exception as e:
+                    print("That band does not exist, exiting now.")
+                    exit()
+
             if selected_model != ROM.MODEL_FF and selected_model != ROM.MODEL_FE:
                 fw_filename = models[selected_model][4]
 
             else:
                 if selected_platform == ROM.PLATFORM_AVR:
                     if selected_mcu == ROM.MCU_1284P:
                         fw_filename = "rnode_firmware.hex"
@@ -2414,14 +2454,31 @@
                                 "--flash_freq", "80m",
                                 "--flash_size", "8MB",
                                 "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.boot_app0",
                                 "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bootloader",
                                 "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.bin",
                                 "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v2.partitions",
                             ]
+                    elif fw_filename == "rnode_firmware_heltec32v3.zip":
+                        return [
+                            sys.executable, flasher,
+                            "--chip", "esp32-s3",
+                            "--port", args.port,
+                            "--baud", args.baud_flash,
+                            "--before", "default_reset",
+                            "--after", "hard_reset",
+                            "write_flash", "-z",
+                            "--flash_mode", "dio",
+                            "--flash_freq", "80m",
+                            "--flash_size", "8MB",
+                            "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v3.boot_app0",
+                            "0x0",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v3.bootloader",
+                            "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v3.bin",
+                            "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_heltec32v3.partitions",
+                        ]
                     elif fw_filename == "rnode_firmware_featheresp32.zip":
                         if numeric_version >= 1.55:
                             return [
                                sys.executable,  flasher,
                                 "--chip", "esp32",
                                 "--port", args.port,
                                 "--baud", args.baud_flash,
@@ -2571,15 +2628,15 @@
                             "--before", "default_reset",
                             "--after", "hard_reset",
                             "write_flash", "-z",
                             "--flash_mode", "dio",
                             "--flash_freq", "80m",
                             "--flash_size", "4MB",
                             "0xe000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_t3s3.boot_app0",
-                            "0x1000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_t3s3.bootloader",
+                            "0x0",  UPD_DIR+"/"+selected_version+"/rnode_firmware_t3s3.bootloader",
                             "0x10000", UPD_DIR+"/"+selected_version+"/rnode_firmware_t3s3.bin",
                             "0x210000",UPD_DIR+"/"+selected_version+"/console_image.bin",
                             "0x8000",  UPD_DIR+"/"+selected_version+"/rnode_firmware_t3s3.partitions",
                         ]
                     elif fw_filename == "extracted_rnode_firmware.zip":
                         return [
                             sys.executable, flasher,
@@ -2711,14 +2768,15 @@
                     rnode.platform = ROM.PLATFORM_AVR
                     rnode.mcu = ROM.MCU_1284P
 
 
             if args.eeprom_wipe:
                 RNS.log("WARNING: EEPROM is being wiped! Power down device NOW if you do not want this!")
                 rnode.wipe_eeprom()
+                rnode.hard_reset()
                 exit()
 
             RNS.log("Reading EEPROM...")
             rnode.download_eeprom()
 
             if rnode.provisioned:
                 if rnode.model != ROM.MODEL_FF:
@@ -3036,18 +3094,21 @@
 
                     serialno = counter+1
                     model = None
                     hwrev = None
                     if args.product != None:
                         if args.product == "03":
                             mapped_product = ROM.PRODUCT_RNODE
-                        if args.product == "f0":
+                        elif args.product == "f0":
                             mapped_product = ROM.PRODUCT_HMBRW
-                        if args.product == "e0":
+                        elif args.product == "e0":
                             mapped_product = ROM.PRODUCT_TBEAM
+                        else:
+                            if len(args.product) == 2:
+                                mapped_product = ord(bytes.fromhex(args.product))
 
                     if mapped_model != None:
                         if mapped_model == ROM.MODEL_B4_TCXO:
                             model = ROM.MODEL_B4
                         elif mapped_model == ROM.MODEL_B9_TCXO:
                             model = ROM.MODEL_B9
                         else:
@@ -3063,14 +3124,17 @@
                             model = ROM.MODEL_A6
                         elif args.model == "e4":
                             model = ROM.MODEL_E4
                         elif args.model == "e9":
                             model = ROM.MODEL_E9
                         elif args.model == "ff":
                             model = ROM.MODEL_FF
+                        else:
+                            if len(args.model) == 2:
+                                model = ord(bytes.fromhex(args.model))
 
 
                     if args.hwrev != None and (args.hwrev > 0 and args.hwrev < 256):
                         hwrev = chr(args.hwrev)
 
                     if serialno > 0 and model != None and hwrev != None:
                         try:
@@ -3120,14 +3184,18 @@
                                 except Exception as e:
                                     RNS.log("Error while signing EEPROM")
                                     RNS.log(str(e))
                             else:
                                 RNS.log("No signing key found")
                                 exit()
 
+                            if model == ROM.MODEL_A1 or model == ROM.MODEL_A6:
+                                rnode.hard_reset()
+                                RNS.log("Waiting for ESP32 reset...")
+                                time.sleep(6.5)
 
                             RNS.log("Bootstrapping device EEPROM...")
 
                             rnode.write_eeprom(ROM.ADDR_PRODUCT, mapped_product)
                             time.sleep(0.006)
                             rnode.write_eeprom(ROM.ADDR_MODEL, model)
                             time.sleep(0.006)
@@ -3172,14 +3240,16 @@
                                     partition_hash = bytes.fromhex(release_info.split()[1])
                                     vf.close()
                                 else:
                                     partition_filename = fw_filename.replace(".zip", ".bin")
                                     partition_hash = get_partition_hash(UPD_DIR+"/"+selected_version+"/"+partition_filename)
 
                                 if partition_hash != None:
+                                    time.sleep(0.75)
+                                    RNS.log("Setting firmware checksum...")
                                     rnode.set_firmware_hash(partition_hash)
 
                             rnode.hard_reset()
                             if rnode.platform == ROM.PLATFORM_ESP32:
                                 RNS.log("Waiting for ESP32 reset...")
                                 time.sleep(6.5)
```

### Comparing `rnspure-0.7.3/RNS/Utilities/rnpath.py` & `rnspure-0.7.4/RNS/Utilities/rnpath.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnprobe.py` & `rnspure-0.7.4/RNS/Utilities/rnprobe.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnsd.py` & `rnspure-0.7.4/RNS/Utilities/rnsd.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnstatus.py` & `rnspure-0.7.4/RNS/Utilities/rnstatus.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/Utilities/rnx.py` & `rnspure-0.7.4/RNS/Utilities/rnx.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/__init__.py` & `rnspure-0.7.4/RNS/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/configobj.py` & `rnspure-0.7.4/RNS/vendor/configobj.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/__init__.py` & `rnspure-0.7.4/RNS/vendor/i2plib/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/aiosam.py` & `rnspure-0.7.4/RNS/vendor/i2plib/aiosam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/exceptions.py` & `rnspure-0.7.4/RNS/vendor/i2plib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/sam.py` & `rnspure-0.7.4/RNS/vendor/i2plib/sam.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/tunnel.py` & `rnspure-0.7.4/RNS/vendor/i2plib/tunnel.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/i2plib/utils.py` & `rnspure-0.7.4/RNS/vendor/i2plib/utils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/ifaddr/__init__.py` & `rnspure-0.7.4/RNS/vendor/ifaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/ifaddr/_posix.py` & `rnspure-0.7.4/RNS/vendor/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/ifaddr/_shared.py` & `rnspure-0.7.4/RNS/vendor/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/ifaddr/_win32.py` & `rnspure-0.7.4/RNS/vendor/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/ifaddr/niwrapper.py` & `rnspure-0.7.4/RNS/vendor/ifaddr/niwrapper.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/platformutils.py` & `rnspure-0.7.4/RNS/vendor/platformutils.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/six.py` & `rnspure-0.7.4/RNS/vendor/six.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/RNS/vendor/umsgpack.py` & `rnspure-0.7.4/RNS/vendor/umsgpack.py`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/rnspure.egg-info/PKG-INFO` & `rnspure-0.7.4/rnspure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnspure
-Version: 0.7.3
+Version: 0.7.4
 Summary: Self-configuring, encrypted and resilient mesh networking stack for LoRa, packet radio, WiFi and everything in between
 Home-page: https://reticulum.network/
 Author: Mark Qvist
 Author-email: mark@unsigned.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rnspure-0.7.3/rnspure.egg-info/SOURCES.txt` & `rnspure-0.7.4/rnspure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rnspure-0.7.3/setup.py` & `rnspure-0.7.4/setup.py`

 * *Files identical despite different names*

