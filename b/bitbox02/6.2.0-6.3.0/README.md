# Comparing `tmp/bitbox02-6.2.0.tar.gz` & `tmp/bitbox02-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbox02-6.2.0.tar", last modified: Tue May 30 21:24:19 2023, max compression
+gzip compressed data, was "bitbox02-6.3.0.tar", last modified: Sun May  5 08:53:30 2024, max compression
```

## Comparing `bitbox02-6.2.0.tar` & `bitbox02-6.3.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/
--rw-r--r--   0 user      (1000) user      (1000)     1085 2023-05-30 21:24:19.502000 bitbox02-6.2.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      381 2023-01-29 19:30:16.000000 bitbox02-6.2.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/bitbox02/
--rw-r--r--   0 user      (1000) user      (1000)     1642 2023-03-07 13:33:28.000000 bitbox02-6.2.0/bitbox02/bitbox02/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    43686 2023-05-18 09:01:54.000000 bitbox02-6.2.0/bitbox02/bitbox02/bitbox02.py
--rw-r--r--   0 user      (1000) user      (1000)     7373 2023-02-02 14:05:49.000000 bitbox02-6.2.0/bitbox02/bitbox02/bootloader.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/bitbox02/py.typed
--rw-r--r--   0 user      (1000) user      (1000)     2371 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/bitbox02/secp256k1.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/communication/
--rw-r--r--   0 user      (1000) user      (1000)     1030 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    27923 2023-04-28 20:50:57.000000 bitbox02-6.2.0/bitbox02/communication/bitbox_api_protocol.py
--rw-r--r--   0 user      (1000) user      (1000)     1669 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/communication.py
--rw-r--r--   0 user      (1000) user      (1000)     4666 2023-05-29 02:11:48.000000 bitbox02-6.2.0/bitbox02/communication/devices.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/bitbox02/communication/generated/
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1401 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/antiklepto_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     2102 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     3851 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     2699 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     5248 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)    10516 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)    33375 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     6703 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/cardano_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     1664 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     3152 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     6698 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)    19589 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     5757 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)    13514 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     1205 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     1308 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     1386 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     1541 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     1444 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     1990 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)     1186 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.py
--rw-r--r--   0 user      (1000) user      (1000)     1394 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.pyi
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/bitbox02/communication/u2fhid/
--rw-r--r--   0 user      (1000) user      (1000)      709 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/u2fhid/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5800 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/u2fhid/u2fhid.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/py.typed
--rw-r--r--   0 user      (1000) user      (1000)     8023 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1085 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1829 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-02 08:31:34.000000 bitbox02-6.2.0/bitbox02.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)      114 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        9 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 21:24:19.502000 bitbox02-6.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     2895 2023-05-30 21:17:12.000000 bitbox02-6.2.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.703000 bitbox02-6.3.0/
+-rw-r--r--   0 user      (1000) user      (1000)    11432 2023-08-03 09:29:14.000000 bitbox02-6.3.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      923 2024-05-05 08:53:30.702000 bitbox02-6.3.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      381 2023-08-03 09:29:14.000000 bitbox02-6.3.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.699000 bitbox02-6.3.0/bitbox02/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.700000 bitbox02-6.3.0/bitbox02/bitbox02/
+-rw-r--r--   0 user      (1000) user      (1000)     1642 2024-05-05 08:49:54.000000 bitbox02-6.3.0/bitbox02/bitbox02/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    46732 2024-04-22 21:46:32.000000 bitbox02-6.3.0/bitbox02/bitbox02/bitbox02.py
+-rw-r--r--   0 user      (1000) user      (1000)     7373 2023-12-28 11:16:41.000000 bitbox02-6.3.0/bitbox02/bitbox02/bootloader.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/bitbox02/py.typed
+-rw-r--r--   0 user      (1000) user      (1000)     2371 2024-03-04 13:09:47.000000 bitbox02-6.3.0/bitbox02/bitbox02/secp256k1.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.700000 bitbox02-6.3.0/bitbox02/communication/
+-rw-r--r--   0 user      (1000) user      (1000)     1030 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/communication/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    28162 2024-05-02 08:57:40.000000 bitbox02-6.3.0/bitbox02/communication/bitbox_api_protocol.py
+-rw-r--r--   0 user      (1000) user      (1000)     1669 2024-03-04 13:09:47.000000 bitbox02-6.3.0/bitbox02/communication/communication.py
+-rw-r--r--   0 user      (1000) user      (1000)     4642 2024-05-02 08:57:40.000000 bitbox02-6.3.0/bitbox02/communication/devices.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.702000 bitbox02-6.3.0/bitbox02/communication/generated/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1401 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/antiklepto_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2102 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/backup_commands_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     3851 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/backup_commands_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     2699 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/bitbox02_system_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     5248 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)    10831 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/btc_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    34453 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/btc_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     6703 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/cardano_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1912 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/common_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     4119 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/common_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     7406 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/eth_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    22519 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/eth_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     5927 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/hww_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    13940 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/hww_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1986 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/keystore_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     3576 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/keystore_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1386 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/mnemonic_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1541 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/mnemonic_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1444 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/perform_attestation_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1990 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/perform_attestation_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1186 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/system_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1394 2024-05-05 08:29:37.000000 bitbox02-6.3.0/bitbox02/communication/generated/system_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/communication/py.typed
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.702000 bitbox02-6.3.0/bitbox02/communication/u2fhid/
+-rw-r--r--   0 user      (1000) user      (1000)      709 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/communication/u2fhid/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5800 2024-03-04 13:09:47.000000 bitbox02-6.3.0/bitbox02/communication/u2fhid/u2fhid.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/py.typed
+-rw-r--r--   0 user      (1000) user      (1000)     8023 2023-08-03 09:29:14.000000 bitbox02-6.3.0/bitbox02/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-05 08:53:30.699000 bitbox02-6.3.0/bitbox02.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      923 2024-05-05 08:53:30.000000 bitbox02-6.3.0/bitbox02.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1837 2024-05-05 08:53:30.000000 bitbox02-6.3.0/bitbox02.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-05 08:53:30.000000 bitbox02-6.3.0/bitbox02.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-02 08:31:34.000000 bitbox02-6.3.0/bitbox02.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      114 2024-05-05 08:53:30.000000 bitbox02-6.3.0/bitbox02.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2024-05-05 08:53:30.000000 bitbox02-6.3.0/bitbox02.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-05 08:53:30.703000 bitbox02-6.3.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     2895 2024-03-04 13:09:47.000000 bitbox02-6.3.0/setup.py
```

### Comparing `bitbox02-6.2.0/PKG-INFO` & `bitbox02-6.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: bitbox02
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python library for bitbox02 communication
 Home-page: https://github.com/digitalbitbox/bitbox02-firmware
 Author: Shift Crypto
 Author-email: support@shiftcrypto.ch
-License: UNKNOWN
-Description: # BitBox02 python API
-        
-        This repository contains two packages
-        
-        * u2fhid
-        * bitbox02
-        
-        ## u2fhid
-        
-        This is a small package that contains read/write primitives for u2fhid devices such as the
-        bitbox02.
-        
-        ## bitbox02
-        
-        In this folder is the Python API for communicating with the BitBox02 device.
-        
-        The folder `generated` contains files generated by `python-protobuf`. Regenerate with `make`.
-        
 Keywords: digitalbitbox bitbox bitbox02 bitcoin litecoin ethereum erc20 u2f
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BitBox02 python API
+
+This repository contains two packages
+
+* u2fhid
+* bitbox02
+
+## u2fhid
+
+This is a small package that contains read/write primitives for u2fhid devices such as the
+bitbox02.
+
+## bitbox02
+
+In this folder is the Python API for communicating with the BitBox02 device.
+
+The folder `generated` contains files generated by `python-protobuf`. Regenerate with `make`.
```

### Comparing `bitbox02-6.2.0/bitbox02/bitbox02/__init__.py` & `bitbox02-6.3.0/bitbox02/bitbox02/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Library to interact with a BitBox02 device. """
 
 from __future__ import print_function
 import sys
 
-__version__ = "6.2.0"
+__version__ = "6.3.0"
 
 if sys.version_info.major != 3 or sys.version_info.minor < 6:
     print(
         "Python version is {}.{}, but 3.6+ is required by this script.".format(
             sys.version_info.major, sys.version_info.minor
         ),
         file=sys.stderr,
```

### Comparing `bitbox02-6.2.0/bitbox02/bitbox02/bitbox02.py` & `bitbox02-6.3.0/bitbox02/bitbox02/bitbox02.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     from bitbox02.communication.generated import cardano_pb2 as cardano
     from bitbox02.communication.generated import mnemonic_pb2 as mnemonic
     from bitbox02.communication.generated import bitbox02_system_pb2 as bitbox02_system
     from bitbox02.communication.generated import backup_commands_pb2 as backup
     from bitbox02.communication.generated import common_pb2 as common
     from bitbox02.communication.generated import keystore_pb2 as keystore
     from bitbox02.communication.generated import antiklepto_pb2 as antiklepto
+    import google.protobuf.empty_pb2
 
     # pylint: disable=unused-import
     # We export it in __init__.py
     from bitbox02.communication.generated import system_pb2 as system
 except ModuleNotFoundError:
     print("Run `make py` to generate the protobuf messages")
     sys.exit()
@@ -674,14 +675,48 @@
         # pylint: disable=no-member
         request = hww.Request()
         request.electrum_encryption_key.CopyFrom(
             keystore.ElectrumEncryptionKeyRequest(keypath=keypath)
         )
         return self._msg_query(request).electrum_encryption_key.key
 
+    def bip85_bip39(self) -> None:
+        """Invokes the BIP85-BIP39 workflow on the device"""
+        self._require_atleast(semver.VersionInfo(9, 18, 0))
+
+        # pylint: disable=no-member
+        request = hww.Request()
+        request.bip85.CopyFrom(
+            keystore.BIP85Request(
+                bip39=google.protobuf.empty_pb2.Empty(),
+            )
+        )
+        response = self._msg_query(request, expected_response="bip85").bip85
+        assert response.WhichOneof("app") == "bip39"
+
+    def bip85_ln(self) -> bytes:
+        """
+        Generates and returns a mnemonic for a hot Lightning wallet from the device using BIP-85.
+        """
+        self._require_atleast(semver.VersionInfo(9, 17, 0))
+
+        # Only account_number=0 is allowed for now.
+        account_number = 0
+
+        # pylint: disable=no-member
+        request = hww.Request()
+        request.bip85.CopyFrom(
+            keystore.BIP85Request(
+                ln=keystore.BIP85Request.AppLn(account_number=account_number),
+            )
+        )
+        response = self._msg_query(request, expected_response="bip85").bip85
+        assert response.WhichOneof("app") == "ln"
+        return response.ln
+
     def enable_mnemonic_passphrase(self) -> None:
         """
         Enable the bip39 passphrase.
         """
         # pylint: disable=no-member
         request = hww.Request()
         request.set_mnemonic_passphrase_enabled.enabled = True
@@ -753,36 +788,25 @@
         )
         return self._eth_msg_query(request, expected_response="pub").pub.pub
 
     def eth_sign(self, transaction: bytes, keypath: Sequence[int], chain_id: int = 1) -> bytes:
         """
         transaction should be given as a full rlp encoded eth transaction.
         """
-        nonce, gas_price, gas_limit, recipient, value, data, _, _, _ = rlp.decode(transaction)
-        request = eth.ETHRequest()
-        # pylint: disable=no-member
-        request.sign.CopyFrom(
-            eth.ETHSignRequest(
-                coin=self._eth_coin(chain_id),
-                chain_id=chain_id,
-                keypath=keypath,
-                nonce=nonce,
-                gas_price=gas_price,
-                gas_limit=gas_limit,
-                recipient=recipient,
-                value=value,
-                data=data,
-            )
-        )
+        is_eip1559 = transaction.startswith(b"\x02")
 
-        supports_antiklepto = self.version >= semver.VersionInfo(9, 5, 0)
-        if supports_antiklepto:
+        def handle_antiklepto(request: eth.ETHRequest) -> bytes:
             host_nonce = os.urandom(32)
+            if is_eip1559:
+                request.sign_eip1559.host_nonce_commitment.commitment = antiklepto_host_commit(
+                    host_nonce
+                )
+            else:
+                request.sign.host_nonce_commitment.commitment = antiklepto_host_commit(host_nonce)
 
-            request.sign.host_nonce_commitment.commitment = antiklepto_host_commit(host_nonce)
             signer_commitment = self._eth_msg_query(
                 request, expected_response="antiklepto_signer_commitment"
             ).antiklepto_signer_commitment.commitment
 
             request = eth.ETHRequest()
             request.antiklepto_signature.CopyFrom(
                 antiklepto.AntiKleptoSignatureRequest(host_nonce=host_nonce)
@@ -792,14 +816,72 @@
             antiklepto_verify(host_nonce, signer_commitment, signature[:64])
 
             if self.debug:
                 print("Antiklepto nonce verification PASSED")
 
             return signature
 
+        if is_eip1559:
+            self._require_atleast(semver.VersionInfo(9, 16, 0))
+            (
+                decoded_chain_id,
+                nonce,
+                priority_fee,
+                max_fee,
+                gas_limit,
+                recipient,
+                value,
+                data,
+                _,
+                _,
+                _,
+            ) = rlp.decode(transaction[1:])
+            decoded_chain_id_int = int.from_bytes(decoded_chain_id, byteorder="big")
+            if decoded_chain_id_int != chain_id:
+                raise Exception(
+                    f"chainID argument ({chain_id}) does not match chainID encoded in transaction ({decoded_chain_id_int})"
+                )
+            request = eth.ETHRequest()
+            # pylint: disable=no-member
+            request.sign_eip1559.CopyFrom(
+                eth.ETHSignEIP1559Request(
+                    chain_id=chain_id,
+                    keypath=keypath,
+                    nonce=nonce,
+                    max_priority_fee_per_gas=priority_fee,
+                    max_fee_per_gas=max_fee,
+                    gas_limit=gas_limit,
+                    recipient=recipient,
+                    value=value,
+                    data=data,
+                )
+            )
+            return handle_antiklepto(request)
+
+        nonce, gas_price, gas_limit, recipient, value, data, _, _, _ = rlp.decode(transaction)
+        request = eth.ETHRequest()
+        # pylint: disable=no-member
+        request.sign.CopyFrom(
+            eth.ETHSignRequest(
+                coin=self._eth_coin(chain_id),
+                chain_id=chain_id,
+                keypath=keypath,
+                nonce=nonce,
+                gas_price=gas_price,
+                gas_limit=gas_limit,
+                recipient=recipient,
+                value=value,
+                data=data,
+            )
+        )
+
+        supports_antiklepto = self.version >= semver.VersionInfo(9, 5, 0)
+        if supports_antiklepto:
+            return handle_antiklepto(request)
+
         return self._eth_msg_query(request, expected_response="sign").sign.signature
 
     def eth_sign_msg(self, msg: bytes, keypath: Sequence[int], chain_id: int = 1) -> bytes:
         """
         Signs message, the msg will be prefixed with "\x19Ethereum message\n" + len(msg) in the
         hardware. 27 is added to the recID to denote an uncompressed pubkey.
         """
@@ -945,15 +1027,18 @@
                         return b""
                     if value[:2].lower() == "0x":
                         return bytes.fromhex(value[2:])
                 assert isinstance(value, bytes)
                 return value
             if typ.type == eth.ETHSignTypedMessageRequest.DataType.UINT:
                 if isinstance(value, str):
-                    value = int(value)
+                    if value[:2].lower() == "0x":
+                        value = int(value[2:], 16)
+                    else:
+                        value = int(value)
                 assert isinstance(value, int)
                 return value.to_bytes(typ.size, "big")
             if typ.type == eth.ETHSignTypedMessageRequest.DataType.INT:
                 if isinstance(value, str):
                     value = int(value)
                 assert isinstance(value, int)
                 return value.to_bytes(typ.size, "big", signed=True)
```

### Comparing `bitbox02-6.2.0/bitbox02/bitbox02/bootloader.py` & `bitbox02-6.3.0/bitbox02/bitbox02/bootloader.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/bitbox02/secp256k1.py` & `bitbox02-6.3.0/bitbox02/bitbox02/secp256k1.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/__init__.py` & `bitbox02-6.3.0/bitbox02/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/bitbox_api_protocol.py` & `bitbox02-6.3.0/bitbox02/communication/bitbox_api_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,32 +522,42 @@
 
 
 class BitBoxCommonAPI:
     """Class to communicate with a BitBox device"""
 
     # pylint: disable=too-many-public-methods,too-many-arguments
     def __init__(
-        self, transport: TransportLayer, device_info: DeviceInfo, noise_config: BitBoxNoiseConfig
+        self,
+        transport: TransportLayer,
+        device_info: Optional[DeviceInfo],
+        noise_config: BitBoxNoiseConfig,
     ):
         """
         Can raise LibraryVersionOutdatedException. check_min_version() should be called following
         the instantiation.
+        If device_info is None, it is infered using the OP_INFO API call, available since
+        firmware version v5.0.0.
         """
         self.debug = False
-        serial_number = device_info["serial_number"]
 
-        if device_info["product_string"] == BITBOX02MULTI:
-            self.edition = BitBox02Edition.MULTI
-        elif device_info["product_string"] == BITBOX02BTC:
-            self.edition = BitBox02Edition.BTCONLY
-
-        self.version = parse_device_version(serial_number)
-        if self.version is None:
+        if device_info is not None:
+            version = device_info["serial_number"]
+            if device_info["product_string"] == BITBOX02MULTI:
+                edition = BitBox02Edition.MULTI
+            elif device_info["product_string"] == BITBOX02BTC:
+                edition = BitBox02Edition.BTCONLY
+        else:
+            version, _, edition, _ = self.get_info(transport)
+
+        self.edition = edition
+        try:
+            self.version = parse_device_version(version)
+        except:
             transport.close()
-            raise ValueError(f"Could not parse version from {serial_number}")
+            raise
 
         # Delete the prelease part, as it messes with the comparison (e.g. 3.0.0-pre < 3.0.0 is
         # True, but the 3.0.0-pre has already the same API breaking changes like 3.0.0...).
         self.version = semver.VersionInfo(
             self.version.major, self.version.minor, self.version.patch, build=self.version.build
         )
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/communication.py` & `bitbox02-6.3.0/bitbox02/communication/communication.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/devices.py` & `bitbox02-6.3.0/bitbox02/communication/devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,13 +153,13 @@
     if len(devices) > 1:
         raise TooManyFoundException(len(devices))
     if not devices:
         raise NoneFoundException
     return devices[0]
 
 
-def parse_device_version(serial_number: str) -> semver.VersionInfo:
-    match = re.search(r"v([0-9]+\.[0-9]+\.[0-9]+.*)", serial_number)
+def parse_device_version(version: str) -> semver.VersionInfo:
+    match = re.search(r"v([0-9]+\.[0-9]+\.[0-9]+.*)", version)
     if match is None:
-        raise Exception(f"Could not parse version string from serial_number: {serial_number}")
+        raise ValueError(f"Could not parse version string from string: {version}")
 
     return semver.VersionInfo.parse(match.group(1))
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/antiklepto_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/antiklepto_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/backup_commands_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/backup_commands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/bitbox02_system_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/btc_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,71 +11,73 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import antiklepto_pb2 as antiklepto__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tbtc.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xb9\x03\n\x0f\x42TCScriptConfig\x12G\n\x0bsimple_type\x18\x01 \x01(\x0e\x32\x30.shiftcrypto.bitbox02.BTCScriptConfig.SimpleTypeH\x00\x12\x42\n\x08multisig\x18\x02 \x01(\x0b\x32..shiftcrypto.bitbox02.BTCScriptConfig.MultisigH\x00\x1a\xd9\x01\n\x08Multisig\x12\x11\n\tthreshold\x18\x01 \x01(\r\x12)\n\x05xpubs\x18\x02 \x03(\x0b\x32\x1a.shiftcrypto.bitbox02.XPub\x12\x16\n\x0eour_xpub_index\x18\x03 \x01(\r\x12N\n\x0bscript_type\x18\x04 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.BTCScriptConfig.Multisig.ScriptType\"\'\n\nScriptType\x12\t\n\x05P2WSH\x10\x00\x12\x0e\n\nP2WSH_P2SH\x10\x01\"3\n\nSimpleType\x12\x0f\n\x0bP2WPKH_P2SH\x10\x00\x12\n\n\x06P2WPKH\x10\x01\x12\x08\n\x04P2TR\x10\x02\x42\x08\n\x06\x63onfig\"\xfc\x02\n\rBTCPubRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x41\n\txpub_type\x18\x03 \x01(\x0e\x32,.shiftcrypto.bitbox02.BTCPubRequest.XPubTypeH\x00\x12>\n\rscript_config\x18\x04 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfigH\x00\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\x08\"\x8e\x01\n\x08XPubType\x12\x08\n\x04TPUB\x10\x00\x12\x08\n\x04XPUB\x10\x01\x12\x08\n\x04YPUB\x10\x02\x12\x08\n\x04ZPUB\x10\x03\x12\x08\n\x04VPUB\x10\x04\x12\x08\n\x04UPUB\x10\x05\x12\x10\n\x0c\x43\x41PITAL_VPUB\x10\x06\x12\x10\n\x0c\x43\x41PITAL_ZPUB\x10\x07\x12\x10\n\x0c\x43\x41PITAL_UPUB\x10\x08\x12\x10\n\x0c\x43\x41PITAL_YPUB\x10\tB\x08\n\x06output\"k\n\x1a\x42TCScriptConfigWithKeypath\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\xc5\x02\n\x12\x42TCSignInitRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12H\n\x0escript_configs\x18\x02 \x03(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x12\n\nnum_inputs\x18\x05 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x06 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\x12H\n\x0b\x66ormat_unit\x18\x08 \x01(\x0e\x32\x33.shiftcrypto.bitbox02.BTCSignInitRequest.FormatUnit\"\"\n\nFormatUnit\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x07\n\x03SAT\x10\x01\"\xe8\x02\n\x13\x42TCSignNextResponse\x12<\n\x04type\x18\x01 \x01(\x0e\x32..shiftcrypto.bitbox02.BTCSignNextResponse.Type\x12\r\n\x05index\x18\x02 \x01(\r\x12\x15\n\rhas_signature\x18\x03 \x01(\x08\x12\x11\n\tsignature\x18\x04 \x01(\x0c\x12\x12\n\nprev_index\x18\x05 \x01(\r\x12W\n\x1d\x61nti_klepto_signer_commitment\x18\x06 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitment\"m\n\x04Type\x12\t\n\x05INPUT\x10\x00\x12\n\n\x06OUTPUT\x10\x01\x12\x08\n\x04\x44ONE\x10\x02\x12\x0f\n\x0bPREVTX_INIT\x10\x03\x12\x10\n\x0cPREVTX_INPUT\x10\x04\x12\x11\n\rPREVTX_OUTPUT\x10\x05\x12\x0e\n\nHOST_NONCE\x10\x06\"\xea\x01\n\x13\x42TCSignInputRequest\x12\x13\n\x0bprevOutHash\x18\x01 \x01(\x0c\x12\x14\n\x0cprevOutIndex\x18\x02 \x01(\r\x12\x14\n\x0cprevOutValue\x18\x03 \x01(\x04\x12\x10\n\x08sequence\x18\x04 \x01(\r\x12\x0f\n\x07keypath\x18\x06 \x03(\r\x12\x1b\n\x13script_config_index\x18\x07 \x01(\r\x12R\n\x15host_nonce_commitment\x18\x08 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"\xa5\x01\n\x14\x42TCSignOutputRequest\x12\x0c\n\x04ours\x18\x01 \x01(\x08\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.shiftcrypto.bitbox02.BTCOutputType\x12\r\n\x05value\x18\x03 \x01(\x04\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\x12\x0f\n\x07keypath\x18\x05 \x03(\r\x12\x1b\n\x13script_config_index\x18\x06 \x01(\r\"\x99\x01\n\x1b\x42TCScriptConfigRegistration\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\x0c\n\nBTCSuccess\"m\n\"BTCIsScriptConfigRegisteredRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\"<\n#BTCIsScriptConfigRegisteredResponse\x12\x15\n\ris_registered\x18\x01 \x01(\x08\"\xfc\x01\n\x1e\x42TCRegisterScriptConfigRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\x12\x0c\n\x04name\x18\x02 \x01(\t\x12P\n\txpub_type\x18\x03 \x01(\x0e\x32=.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequest.XPubType\"1\n\x08XPubType\x12\x11\n\rAUTO_ELECTRUM\x10\x00\x12\x12\n\x0e\x41UTO_XPUB_TPUB\x10\x01\"b\n\x14\x42TCPrevTxInitRequest\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x12\n\nnum_inputs\x18\x02 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x03 \x01(\r\x12\x10\n\x08locktime\x18\x04 \x01(\r\"r\n\x15\x42TCPrevTxInputRequest\x12\x15\n\rprev_out_hash\x18\x01 \x01(\x0c\x12\x16\n\x0eprev_out_index\x18\x02 \x01(\r\x12\x18\n\x10signature_script\x18\x03 \x01(\x0c\x12\x10\n\x08sequence\x18\x04 \x01(\r\">\n\x16\x42TCPrevTxOutputRequest\x12\r\n\x05value\x18\x01 \x01(\x04\x12\x15\n\rpubkey_script\x18\x02 \x01(\x0c\"\xee\x01\n\x15\x42TCSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12G\n\rscript_config\x18\x02 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"+\n\x16\x42TCSignMessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xb6\x04\n\nBTCRequest\x12_\n\x1bis_script_config_registered\x18\x01 \x01(\x0b\x32\x38.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredRequestH\x00\x12V\n\x16register_script_config\x18\x02 \x01(\x0b\x32\x34.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequestH\x00\x12\x41\n\x0bprevtx_init\x18\x03 \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCPrevTxInitRequestH\x00\x12\x43\n\x0cprevtx_input\x18\x04 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCPrevTxInputRequestH\x00\x12\x45\n\rprevtx_output\x18\x05 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCPrevTxOutputRequestH\x00\x12\x43\n\x0csign_message\x18\x06 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x07 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x42\t\n\x07request\"\x90\x03\n\x0b\x42TCResponse\x12\x33\n\x07success\x18\x01 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCSuccessH\x00\x12`\n\x1bis_script_config_registered\x18\x02 \x01(\x0b\x32\x39.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredResponseH\x00\x12>\n\tsign_next\x18\x03 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x44\n\x0csign_message\x18\x04 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCSignMessageResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x42\n\n\x08response*/\n\x07\x42TCCoin\x12\x07\n\x03\x42TC\x10\x00\x12\x08\n\x04TBTC\x10\x01\x12\x07\n\x03LTC\x10\x02\x12\x08\n\x04TLTC\x10\x03*R\n\rBTCOutputType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05P2PKH\x10\x01\x12\x08\n\x04P2SH\x10\x02\x12\n\n\x06P2WPKH\x10\x03\x12\t\n\x05P2WSH\x10\x04\x12\x08\n\x04P2TR\x10\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tbtc.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xc6\x04\n\x0f\x42TCScriptConfig\x12G\n\x0bsimple_type\x18\x01 \x01(\x0e\x32\x30.shiftcrypto.bitbox02.BTCScriptConfig.SimpleTypeH\x00\x12\x42\n\x08multisig\x18\x02 \x01(\x0b\x32..shiftcrypto.bitbox02.BTCScriptConfig.MultisigH\x00\x12>\n\x06policy\x18\x03 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCScriptConfig.PolicyH\x00\x1a\xd9\x01\n\x08Multisig\x12\x11\n\tthreshold\x18\x01 \x01(\r\x12)\n\x05xpubs\x18\x02 \x03(\x0b\x32\x1a.shiftcrypto.bitbox02.XPub\x12\x16\n\x0eour_xpub_index\x18\x03 \x01(\r\x12N\n\x0bscript_type\x18\x04 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.BTCScriptConfig.Multisig.ScriptType\"\'\n\nScriptType\x12\t\n\x05P2WSH\x10\x00\x12\x0e\n\nP2WSH_P2SH\x10\x01\x1aK\n\x06Policy\x12\x0e\n\x06policy\x18\x01 \x01(\t\x12\x31\n\x04keys\x18\x02 \x03(\x0b\x32#.shiftcrypto.bitbox02.KeyOriginInfo\"3\n\nSimpleType\x12\x0f\n\x0bP2WPKH_P2SH\x10\x00\x12\n\n\x06P2WPKH\x10\x01\x12\x08\n\x04P2TR\x10\x02\x42\x08\n\x06\x63onfig\"\xfc\x02\n\rBTCPubRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x41\n\txpub_type\x18\x03 \x01(\x0e\x32,.shiftcrypto.bitbox02.BTCPubRequest.XPubTypeH\x00\x12>\n\rscript_config\x18\x04 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfigH\x00\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\x08\"\x8e\x01\n\x08XPubType\x12\x08\n\x04TPUB\x10\x00\x12\x08\n\x04XPUB\x10\x01\x12\x08\n\x04YPUB\x10\x02\x12\x08\n\x04ZPUB\x10\x03\x12\x08\n\x04VPUB\x10\x04\x12\x08\n\x04UPUB\x10\x05\x12\x10\n\x0c\x43\x41PITAL_VPUB\x10\x06\x12\x10\n\x0c\x43\x41PITAL_ZPUB\x10\x07\x12\x10\n\x0c\x43\x41PITAL_UPUB\x10\x08\x12\x10\n\x0c\x43\x41PITAL_YPUB\x10\tB\x08\n\x06output\"k\n\x1a\x42TCScriptConfigWithKeypath\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\xc5\x02\n\x12\x42TCSignInitRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12H\n\x0escript_configs\x18\x02 \x03(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x12\n\nnum_inputs\x18\x05 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x06 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\x12H\n\x0b\x66ormat_unit\x18\x08 \x01(\x0e\x32\x33.shiftcrypto.bitbox02.BTCSignInitRequest.FormatUnit\"\"\n\nFormatUnit\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x07\n\x03SAT\x10\x01\"\xe8\x02\n\x13\x42TCSignNextResponse\x12<\n\x04type\x18\x01 \x01(\x0e\x32..shiftcrypto.bitbox02.BTCSignNextResponse.Type\x12\r\n\x05index\x18\x02 \x01(\r\x12\x15\n\rhas_signature\x18\x03 \x01(\x08\x12\x11\n\tsignature\x18\x04 \x01(\x0c\x12\x12\n\nprev_index\x18\x05 \x01(\r\x12W\n\x1d\x61nti_klepto_signer_commitment\x18\x06 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitment\"m\n\x04Type\x12\t\n\x05INPUT\x10\x00\x12\n\n\x06OUTPUT\x10\x01\x12\x08\n\x04\x44ONE\x10\x02\x12\x0f\n\x0bPREVTX_INIT\x10\x03\x12\x10\n\x0cPREVTX_INPUT\x10\x04\x12\x11\n\rPREVTX_OUTPUT\x10\x05\x12\x0e\n\nHOST_NONCE\x10\x06\"\xea\x01\n\x13\x42TCSignInputRequest\x12\x13\n\x0bprevOutHash\x18\x01 \x01(\x0c\x12\x14\n\x0cprevOutIndex\x18\x02 \x01(\r\x12\x14\n\x0cprevOutValue\x18\x03 \x01(\x04\x12\x10\n\x08sequence\x18\x04 \x01(\r\x12\x0f\n\x07keypath\x18\x06 \x03(\r\x12\x1b\n\x13script_config_index\x18\x07 \x01(\r\x12R\n\x15host_nonce_commitment\x18\x08 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"\xa5\x01\n\x14\x42TCSignOutputRequest\x12\x0c\n\x04ours\x18\x01 \x01(\x08\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.shiftcrypto.bitbox02.BTCOutputType\x12\r\n\x05value\x18\x03 \x01(\x04\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\x12\x0f\n\x07keypath\x18\x05 \x03(\r\x12\x1b\n\x13script_config_index\x18\x06 \x01(\r\"\x99\x01\n\x1b\x42TCScriptConfigRegistration\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\x0c\n\nBTCSuccess\"m\n\"BTCIsScriptConfigRegisteredRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\"<\n#BTCIsScriptConfigRegisteredResponse\x12\x15\n\ris_registered\x18\x01 \x01(\x08\"\xfc\x01\n\x1e\x42TCRegisterScriptConfigRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\x12\x0c\n\x04name\x18\x02 \x01(\t\x12P\n\txpub_type\x18\x03 \x01(\x0e\x32=.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequest.XPubType\"1\n\x08XPubType\x12\x11\n\rAUTO_ELECTRUM\x10\x00\x12\x12\n\x0e\x41UTO_XPUB_TPUB\x10\x01\"b\n\x14\x42TCPrevTxInitRequest\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x12\n\nnum_inputs\x18\x02 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x03 \x01(\r\x12\x10\n\x08locktime\x18\x04 \x01(\r\"r\n\x15\x42TCPrevTxInputRequest\x12\x15\n\rprev_out_hash\x18\x01 \x01(\x0c\x12\x16\n\x0eprev_out_index\x18\x02 \x01(\r\x12\x18\n\x10signature_script\x18\x03 \x01(\x0c\x12\x10\n\x08sequence\x18\x04 \x01(\r\">\n\x16\x42TCPrevTxOutputRequest\x12\r\n\x05value\x18\x01 \x01(\x04\x12\x15\n\rpubkey_script\x18\x02 \x01(\x0c\"\xee\x01\n\x15\x42TCSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12G\n\rscript_config\x18\x02 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"+\n\x16\x42TCSignMessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xb6\x04\n\nBTCRequest\x12_\n\x1bis_script_config_registered\x18\x01 \x01(\x0b\x32\x38.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredRequestH\x00\x12V\n\x16register_script_config\x18\x02 \x01(\x0b\x32\x34.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequestH\x00\x12\x41\n\x0bprevtx_init\x18\x03 \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCPrevTxInitRequestH\x00\x12\x43\n\x0cprevtx_input\x18\x04 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCPrevTxInputRequestH\x00\x12\x45\n\rprevtx_output\x18\x05 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCPrevTxOutputRequestH\x00\x12\x43\n\x0csign_message\x18\x06 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x07 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x42\t\n\x07request\"\x90\x03\n\x0b\x42TCResponse\x12\x33\n\x07success\x18\x01 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCSuccessH\x00\x12`\n\x1bis_script_config_registered\x18\x02 \x01(\x0b\x32\x39.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredResponseH\x00\x12>\n\tsign_next\x18\x03 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x44\n\x0csign_message\x18\x04 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCSignMessageResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x42\n\n\x08response*/\n\x07\x42TCCoin\x12\x07\n\x03\x42TC\x10\x00\x12\x08\n\x04TBTC\x10\x01\x12\x07\n\x03LTC\x10\x02\x12\x08\n\x04TLTC\x10\x03*R\n\rBTCOutputType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05P2PKH\x10\x01\x12\x08\n\x04P2SH\x10\x02\x12\n\n\x06P2WPKH\x10\x03\x12\t\n\x05P2WSH\x10\x04\x12\x08\n\x04P2TR\x10\x05\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'btc_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _BTCCOIN._serialized_start=4235
-  _BTCCOIN._serialized_end=4282
-  _BTCOUTPUTTYPE._serialized_start=4284
-  _BTCOUTPUTTYPE._serialized_end=4366
+  _BTCCOIN._serialized_start=4376
+  _BTCCOIN._serialized_end=4423
+  _BTCOUTPUTTYPE._serialized_start=4425
+  _BTCOUTPUTTYPE._serialized_end=4507
   _BTCSCRIPTCONFIG._serialized_start=68
-  _BTCSCRIPTCONFIG._serialized_end=509
-  _BTCSCRIPTCONFIG_MULTISIG._serialized_start=229
-  _BTCSCRIPTCONFIG_MULTISIG._serialized_end=446
-  _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_start=407
-  _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_end=446
-  _BTCSCRIPTCONFIG_SIMPLETYPE._serialized_start=448
-  _BTCSCRIPTCONFIG_SIMPLETYPE._serialized_end=499
-  _BTCPUBREQUEST._serialized_start=512
-  _BTCPUBREQUEST._serialized_end=892
-  _BTCPUBREQUEST_XPUBTYPE._serialized_start=740
-  _BTCPUBREQUEST_XPUBTYPE._serialized_end=882
-  _BTCSCRIPTCONFIGWITHKEYPATH._serialized_start=894
-  _BTCSCRIPTCONFIGWITHKEYPATH._serialized_end=1001
-  _BTCSIGNINITREQUEST._serialized_start=1004
-  _BTCSIGNINITREQUEST._serialized_end=1329
-  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_start=1295
-  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_end=1329
-  _BTCSIGNNEXTRESPONSE._serialized_start=1332
-  _BTCSIGNNEXTRESPONSE._serialized_end=1692
-  _BTCSIGNNEXTRESPONSE_TYPE._serialized_start=1583
-  _BTCSIGNNEXTRESPONSE_TYPE._serialized_end=1692
-  _BTCSIGNINPUTREQUEST._serialized_start=1695
-  _BTCSIGNINPUTREQUEST._serialized_end=1929
-  _BTCSIGNOUTPUTREQUEST._serialized_start=1932
-  _BTCSIGNOUTPUTREQUEST._serialized_end=2097
-  _BTCSCRIPTCONFIGREGISTRATION._serialized_start=2100
-  _BTCSCRIPTCONFIGREGISTRATION._serialized_end=2253
-  _BTCSUCCESS._serialized_start=2255
-  _BTCSUCCESS._serialized_end=2267
-  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_start=2269
-  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_end=2378
-  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_start=2380
-  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_end=2440
-  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_start=2443
-  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_end=2695
-  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_start=2646
-  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_end=2695
-  _BTCPREVTXINITREQUEST._serialized_start=2697
-  _BTCPREVTXINITREQUEST._serialized_end=2795
-  _BTCPREVTXINPUTREQUEST._serialized_start=2797
-  _BTCPREVTXINPUTREQUEST._serialized_end=2911
-  _BTCPREVTXOUTPUTREQUEST._serialized_start=2913
-  _BTCPREVTXOUTPUTREQUEST._serialized_end=2975
-  _BTCSIGNMESSAGEREQUEST._serialized_start=2978
-  _BTCSIGNMESSAGEREQUEST._serialized_end=3216
-  _BTCSIGNMESSAGERESPONSE._serialized_start=3218
-  _BTCSIGNMESSAGERESPONSE._serialized_end=3261
-  _BTCREQUEST._serialized_start=3264
-  _BTCREQUEST._serialized_end=3830
-  _BTCRESPONSE._serialized_start=3833
-  _BTCRESPONSE._serialized_end=4233
+  _BTCSCRIPTCONFIG._serialized_end=650
+  _BTCSCRIPTCONFIG_MULTISIG._serialized_start=293
+  _BTCSCRIPTCONFIG_MULTISIG._serialized_end=510
+  _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_start=471
+  _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_end=510
+  _BTCSCRIPTCONFIG_POLICY._serialized_start=512
+  _BTCSCRIPTCONFIG_POLICY._serialized_end=587
+  _BTCSCRIPTCONFIG_SIMPLETYPE._serialized_start=589
+  _BTCSCRIPTCONFIG_SIMPLETYPE._serialized_end=640
+  _BTCPUBREQUEST._serialized_start=653
+  _BTCPUBREQUEST._serialized_end=1033
+  _BTCPUBREQUEST_XPUBTYPE._serialized_start=881
+  _BTCPUBREQUEST_XPUBTYPE._serialized_end=1023
+  _BTCSCRIPTCONFIGWITHKEYPATH._serialized_start=1035
+  _BTCSCRIPTCONFIGWITHKEYPATH._serialized_end=1142
+  _BTCSIGNINITREQUEST._serialized_start=1145
+  _BTCSIGNINITREQUEST._serialized_end=1470
+  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_start=1436
+  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_end=1470
+  _BTCSIGNNEXTRESPONSE._serialized_start=1473
+  _BTCSIGNNEXTRESPONSE._serialized_end=1833
+  _BTCSIGNNEXTRESPONSE_TYPE._serialized_start=1724
+  _BTCSIGNNEXTRESPONSE_TYPE._serialized_end=1833
+  _BTCSIGNINPUTREQUEST._serialized_start=1836
+  _BTCSIGNINPUTREQUEST._serialized_end=2070
+  _BTCSIGNOUTPUTREQUEST._serialized_start=2073
+  _BTCSIGNOUTPUTREQUEST._serialized_end=2238
+  _BTCSCRIPTCONFIGREGISTRATION._serialized_start=2241
+  _BTCSCRIPTCONFIGREGISTRATION._serialized_end=2394
+  _BTCSUCCESS._serialized_start=2396
+  _BTCSUCCESS._serialized_end=2408
+  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_start=2410
+  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_end=2519
+  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_start=2521
+  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_end=2581
+  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_start=2584
+  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_end=2836
+  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_start=2787
+  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_end=2836
+  _BTCPREVTXINITREQUEST._serialized_start=2838
+  _BTCPREVTXINITREQUEST._serialized_end=2936
+  _BTCPREVTXINPUTREQUEST._serialized_start=2938
+  _BTCPREVTXINPUTREQUEST._serialized_end=3052
+  _BTCPREVTXOUTPUTREQUEST._serialized_start=3054
+  _BTCPREVTXOUTPUTREQUEST._serialized_end=3116
+  _BTCSIGNMESSAGEREQUEST._serialized_start=3119
+  _BTCSIGNMESSAGEREQUEST._serialized_end=3357
+  _BTCSIGNMESSAGERESPONSE._serialized_start=3359
+  _BTCSIGNMESSAGERESPONSE._serialized_end=3402
+  _BTCREQUEST._serialized_start=3405
+  _BTCREQUEST._serialized_end=3971
+  _BTCRESPONSE._serialized_start=3974
+  _BTCRESPONSE._serialized_end=4374
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/btc_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         THRESHOLD_FIELD_NUMBER: builtins.int
         XPUBS_FIELD_NUMBER: builtins.int
         OUR_XPUB_INDEX_FIELD_NUMBER: builtins.int
         SCRIPT_TYPE_FIELD_NUMBER: builtins.int
         threshold: builtins.int
         @property
         def xpubs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[common_pb2.XPub]:
-            """xpubs are acount-level xpubs. Addresses are going to be derived from it using: m/<change>/<receive>.
+            """xpubs are acount-level xpubs. Addresses are going to be derived from it using: `m/<change>/<receive>`.
             The number of xpubs defines the number of cosigners.
             """
             pass
         our_xpub_index: builtins.int
         """Index to the xpub of our keystore in xpubs. The keypath to it is provided via
         BTCPubRequest/BTCSignInit.
         """
@@ -119,27 +119,48 @@
             threshold: builtins.int = ...,
             xpubs: typing.Optional[typing.Iterable[common_pb2.XPub]] = ...,
             our_xpub_index: builtins.int = ...,
             script_type: global___BTCScriptConfig.Multisig.ScriptType.ValueType = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["our_xpub_index",b"our_xpub_index","script_type",b"script_type","threshold",b"threshold","xpubs",b"xpubs"]) -> None: ...
 
+    class Policy(google.protobuf.message.Message):
+        """A policy as specified by 'Wallet policies':
+        https://github.com/bitcoin/bips/pull/1389
+        """
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        POLICY_FIELD_NUMBER: builtins.int
+        KEYS_FIELD_NUMBER: builtins.int
+        policy: typing.Text
+        @property
+        def keys(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[common_pb2.KeyOriginInfo]: ...
+        def __init__(self,
+            *,
+            policy: typing.Text = ...,
+            keys: typing.Optional[typing.Iterable[common_pb2.KeyOriginInfo]] = ...,
+            ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["keys",b"keys","policy",b"policy"]) -> None: ...
+
     SIMPLE_TYPE_FIELD_NUMBER: builtins.int
     MULTISIG_FIELD_NUMBER: builtins.int
+    POLICY_FIELD_NUMBER: builtins.int
     simple_type: global___BTCScriptConfig.SimpleType.ValueType
     @property
     def multisig(self) -> global___BTCScriptConfig.Multisig: ...
+    @property
+    def policy(self) -> global___BTCScriptConfig.Policy: ...
     def __init__(self,
         *,
         simple_type: global___BTCScriptConfig.SimpleType.ValueType = ...,
         multisig: typing.Optional[global___BTCScriptConfig.Multisig] = ...,
+        policy: typing.Optional[global___BTCScriptConfig.Policy] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config",b"config","multisig",b"multisig","simple_type",b"simple_type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config",b"config","multisig",b"multisig","simple_type",b"simple_type"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config",b"config"]) -> typing.Optional[typing_extensions.Literal["simple_type","multisig"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["config",b"config","multisig",b"multisig","policy",b"policy","simple_type",b"simple_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config",b"config","multisig",b"multisig","policy",b"policy","simple_type",b"simple_type"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config",b"config"]) -> typing.Optional[typing_extensions.Literal["simple_type","multisig","policy"]]: ...
 global___BTCScriptConfig = BTCScriptConfig
 
 class BTCPubRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class _XPubType:
         ValueType = typing.NewType('ValueType', builtins.int)
         V: typing_extensions.TypeAlias = ValueType
@@ -435,15 +456,17 @@
     COIN_FIELD_NUMBER: builtins.int
     SCRIPT_CONFIG_FIELD_NUMBER: builtins.int
     KEYPATH_FIELD_NUMBER: builtins.int
     coin: global___BTCCoin.ValueType
     @property
     def script_config(self) -> global___BTCScriptConfig: ...
     @property
-    def keypath(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    def keypath(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Unused for policy registrations."""
+        pass
     def __init__(self,
         *,
         coin: global___BTCCoin.ValueType = ...,
         script_config: typing.Optional[global___BTCScriptConfig] = ...,
         keypath: typing.Optional[typing.Iterable[builtins.int]] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["script_config",b"script_config"]) -> builtins.bool: ...
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/cardano_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/cardano_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/common_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x14shiftcrypto.bitbox02\"\x1a\n\x0bPubResponse\x12\x0b\n\x03pub\x18\x01 \x01(\t\"\x18\n\x16RootFingerprintRequest\".\n\x17RootFingerprintResponse\x12\x13\n\x0b\x66ingerprint\x18\x01 \x01(\x0c\"l\n\x04XPub\x12\r\n\x05\x64\x65pth\x18\x01 \x01(\x0c\x12\x1a\n\x12parent_fingerprint\x18\x02 \x01(\x0c\x12\x11\n\tchild_num\x18\x03 \x01(\r\x12\x12\n\nchain_code\x18\x04 \x01(\x0c\x12\x12\n\npublic_key\x18\x05 \x01(\x0c\"\x1a\n\x07Keypath\x12\x0f\n\x07keypath\x18\x01 \x03(\rb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x14shiftcrypto.bitbox02\"\x1a\n\x0bPubResponse\x12\x0b\n\x03pub\x18\x01 \x01(\t\"\x18\n\x16RootFingerprintRequest\".\n\x17RootFingerprintResponse\x12\x13\n\x0b\x66ingerprint\x18\x01 \x01(\x0c\"l\n\x04XPub\x12\r\n\x05\x64\x65pth\x18\x01 \x01(\x0c\x12\x1a\n\x12parent_fingerprint\x18\x02 \x01(\x0c\x12\x11\n\tchild_num\x18\x03 \x01(\r\x12\x12\n\nchain_code\x18\x04 \x01(\x0c\x12\x12\n\npublic_key\x18\x05 \x01(\x0c\"\x1a\n\x07Keypath\x12\x0f\n\x07keypath\x18\x01 \x03(\r\"d\n\rKeyOriginInfo\x12\x18\n\x10root_fingerprint\x18\x01 \x01(\x0c\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12(\n\x04xpub\x18\x03 \x01(\x0b\x32\x1a.shiftcrypto.bitbox02.XPubb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _PUBRESPONSE._serialized_start=38
@@ -26,8 +26,10 @@
   _ROOTFINGERPRINTREQUEST._serialized_end=90
   _ROOTFINGERPRINTRESPONSE._serialized_start=92
   _ROOTFINGERPRINTRESPONSE._serialized_end=138
   _XPUB._serialized_start=140
   _XPUB._serialized_end=248
   _KEYPATH._serialized_start=250
   _KEYPATH._serialized_end=276
+  _KEYORIGININFO._serialized_start=278
+  _KEYORIGININFO._serialized_end=378
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/perform_attestation_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,48 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
-import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class PubResponse(google.protobuf.message.Message):
+class PerformAttestationRequest(google.protobuf.message.Message):
+    """Deprecated, last used in v1.0.0"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    PUB_FIELD_NUMBER: builtins.int
-    pub: typing.Text
-    def __init__(self,
-        *,
-        pub: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pub",b"pub"]) -> None: ...
-global___PubResponse = PubResponse
-
-class RootFingerprintRequest(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    def __init__(self,
-        ) -> None: ...
-global___RootFingerprintRequest = RootFingerprintRequest
+    CHALLENGE_FIELD_NUMBER: builtins.int
+    challenge: builtins.bytes
+    """32 bytes challenge."""
 
-class RootFingerprintResponse(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    FINGERPRINT_FIELD_NUMBER: builtins.int
-    fingerprint: builtins.bytes
-    def __init__(self,
-        *,
-        fingerprint: builtins.bytes = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fingerprint",b"fingerprint"]) -> None: ...
-global___RootFingerprintResponse = RootFingerprintResponse
-
-class XPub(google.protobuf.message.Message):
-    """See https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki.
-    version field dropped as it will set dynamically based on the context (xpub, ypub, etc.).
-    """
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    DEPTH_FIELD_NUMBER: builtins.int
-    PARENT_FINGERPRINT_FIELD_NUMBER: builtins.int
-    CHILD_NUM_FIELD_NUMBER: builtins.int
-    CHAIN_CODE_FIELD_NUMBER: builtins.int
-    PUBLIC_KEY_FIELD_NUMBER: builtins.int
-    depth: builtins.bytes
-    parent_fingerprint: builtins.bytes
-    child_num: builtins.int
-    chain_code: builtins.bytes
-    public_key: builtins.bytes
     def __init__(self,
         *,
-        depth: builtins.bytes = ...,
-        parent_fingerprint: builtins.bytes = ...,
-        child_num: builtins.int = ...,
-        chain_code: builtins.bytes = ...,
-        public_key: builtins.bytes = ...,
+        challenge: builtins.bytes = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["chain_code",b"chain_code","child_num",b"child_num","depth",b"depth","parent_fingerprint",b"parent_fingerprint","public_key",b"public_key"]) -> None: ...
-global___XPub = XPub
+    def ClearField(self, field_name: typing_extensions.Literal["challenge",b"challenge"]) -> None: ...
+global___PerformAttestationRequest = PerformAttestationRequest
 
-class Keypath(google.protobuf.message.Message):
-    """This message exists for use in oneof or repeated fields, where one can't inline `repeated uint32` due to protobuf rules."""
+class PerformAttestationResponse(google.protobuf.message.Message):
+    """Deprecated, last used in v1.0.0"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
-    KEYPATH_FIELD_NUMBER: builtins.int
-    @property
-    def keypath(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    BOOTLOADER_HASH_FIELD_NUMBER: builtins.int
+    DEVICE_PUBKEY_FIELD_NUMBER: builtins.int
+    CERTIFICATE_FIELD_NUMBER: builtins.int
+    ROOT_PUBKEY_IDENTIFIER_FIELD_NUMBER: builtins.int
+    CHALLENGE_SIGNATURE_FIELD_NUMBER: builtins.int
+    bootloader_hash: builtins.bytes
+    device_pubkey: builtins.bytes
+    certificate: builtins.bytes
+    root_pubkey_identifier: builtins.bytes
+    challenge_signature: builtins.bytes
     def __init__(self,
         *,
-        keypath: typing.Optional[typing.Iterable[builtins.int]] = ...,
+        bootloader_hash: builtins.bytes = ...,
+        device_pubkey: builtins.bytes = ...,
+        certificate: builtins.bytes = ...,
+        root_pubkey_identifier: builtins.bytes = ...,
+        challenge_signature: builtins.bytes = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["keypath",b"keypath"]) -> None: ...
-global___Keypath = Keypath
+    def ClearField(self, field_name: typing_extensions.Literal["bootloader_hash",b"bootloader_hash","certificate",b"certificate","challenge_signature",b"challenge_signature","device_pubkey",b"device_pubkey","root_pubkey_identifier",b"root_pubkey_identifier"]) -> None: ...
+global___PerformAttestationResponse = PerformAttestationResponse
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/eth_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,47 +11,49 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import antiklepto_pb2 as antiklepto__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\teth.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xf4\x01\n\rETHPubRequest\x12\x0f\n\x07keypath\x18\x01 \x03(\r\x12+\n\x04\x63oin\x18\x02 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x43\n\x0boutput_type\x18\x03 \x01(\x0e\x32..shiftcrypto.bitbox02.ETHPubRequest.OutputType\x12\x0f\n\x07\x64isplay\x18\x04 \x01(\x08\x12\x18\n\x10\x63ontract_address\x18\x05 \x01(\x0c\x12\x10\n\x08\x63hain_id\x18\x06 \x01(\x04\"#\n\nOutputType\x12\x0b\n\x07\x41\x44\x44RESS\x10\x00\x12\x08\n\x04XPUB\x10\x01\"\x99\x02\n\x0e\x45THSignRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\r\n\x05nonce\x18\x03 \x01(\x0c\x12\x11\n\tgas_price\x18\x04 \x01(\x0c\x12\x11\n\tgas_limit\x18\x05 \x01(\x0c\x12\x11\n\trecipient\x18\x06 \x01(\x0c\x12\r\n\x05value\x18\x07 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\x08 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\t \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x12\x10\n\x08\x63hain_id\x18\n \x01(\x04\"\xc8\x01\n\x15\x45THSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x12\x10\n\x08\x63hain_id\x18\x05 \x01(\x04\"$\n\x0f\x45THSignResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xfb\x05\n\x1a\x45THSignTypedMessageRequest\x12\x10\n\x08\x63hain_id\x18\x01 \x01(\x04\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12J\n\x05types\x18\x03 \x03(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.StructType\x12\x14\n\x0cprimary_type\x18\x04 \x01(\t\x12R\n\x15host_nonce_commitment\x18\x05 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x1a\xc9\x01\n\nMemberType\x12G\n\x04type\x18\x01 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.DataType\x12\x0c\n\x04size\x18\x02 \x01(\r\x12\x13\n\x0bstruct_name\x18\x03 \x01(\t\x12O\n\narray_type\x18\x04 \x01(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.MemberType\x1a\x61\n\x06Member\x12\x0c\n\x04name\x18\x01 \x01(\t\x12I\n\x04type\x18\x02 \x01(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.MemberType\x1a\x64\n\nStructType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12H\n\x07members\x18\x02 \x03(\x0b\x32\x37.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.Member\"o\n\x08\x44\x61taType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\x08\n\x04UINT\x10\x02\x12\x07\n\x03INT\x10\x03\x12\x08\n\x04\x42OOL\x10\x04\x12\x0b\n\x07\x41\x44\x44RESS\x10\x05\x12\n\n\x06STRING\x10\x06\x12\t\n\x05\x41RRAY\x10\x07\x12\n\n\x06STRUCT\x10\x08\"\xb4\x01\n\x1c\x45THTypedMessageValueResponse\x12R\n\x0broot_object\x18\x01 \x01(\x0e\x32=.shiftcrypto.bitbox02.ETHTypedMessageValueResponse.RootObject\x12\x0c\n\x04path\x18\x02 \x03(\r\"2\n\nRootObject\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\x0b\n\x07MESSAGE\x10\x02\",\n\x1b\x45THTypedMessageValueRequest\x12\r\n\x05value\x18\x01 \x01(\x0c\"\xae\x03\n\nETHRequest\x12\x32\n\x03pub\x18\x01 \x01(\x0b\x32#.shiftcrypto.bitbox02.ETHPubRequestH\x00\x12\x34\n\x04sign\x18\x02 \x01(\x0b\x32$.shiftcrypto.bitbox02.ETHSignRequestH\x00\x12?\n\x08sign_msg\x18\x03 \x01(\x0b\x32+.shiftcrypto.bitbox02.ETHSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x04 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x12J\n\x0esign_typed_msg\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.ETHSignTypedMessageRequestH\x00\x12L\n\x0ftyped_msg_value\x18\x06 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.ETHTypedMessageValueRequestH\x00\x42\t\n\x07request\"\xab\x02\n\x0b\x45THResponse\x12\x30\n\x03pub\x18\x01 \x01(\x0b\x32!.shiftcrypto.bitbox02.PubResponseH\x00\x12\x35\n\x04sign\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.ETHSignResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x03 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x12M\n\x0ftyped_msg_value\x18\x04 \x01(\x0b\x32\x32.shiftcrypto.bitbox02.ETHTypedMessageValueResponseH\x00\x42\n\n\x08response*2\n\x07\x45THCoin\x12\x07\n\x03\x45TH\x10\x00\x12\x0e\n\nRopstenETH\x10\x01\x12\x0e\n\nRinkebyETH\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\teth.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xf4\x01\n\rETHPubRequest\x12\x0f\n\x07keypath\x18\x01 \x03(\r\x12+\n\x04\x63oin\x18\x02 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x43\n\x0boutput_type\x18\x03 \x01(\x0e\x32..shiftcrypto.bitbox02.ETHPubRequest.OutputType\x12\x0f\n\x07\x64isplay\x18\x04 \x01(\x08\x12\x18\n\x10\x63ontract_address\x18\x05 \x01(\x0c\x12\x10\n\x08\x63hain_id\x18\x06 \x01(\x04\"#\n\nOutputType\x12\x0b\n\x07\x41\x44\x44RESS\x10\x00\x12\x08\n\x04XPUB\x10\x01\"\x99\x02\n\x0e\x45THSignRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\r\n\x05nonce\x18\x03 \x01(\x0c\x12\x11\n\tgas_price\x18\x04 \x01(\x0c\x12\x11\n\tgas_limit\x18\x05 \x01(\x0c\x12\x11\n\trecipient\x18\x06 \x01(\x0c\x12\r\n\x05value\x18\x07 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\x08 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\t \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x12\x10\n\x08\x63hain_id\x18\n \x01(\x04\"\x9b\x02\n\x15\x45THSignEIP1559Request\x12\x10\n\x08\x63hain_id\x18\x01 \x01(\x04\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\r\n\x05nonce\x18\x03 \x01(\x0c\x12 \n\x18max_priority_fee_per_gas\x18\x04 \x01(\x0c\x12\x17\n\x0fmax_fee_per_gas\x18\x05 \x01(\x0c\x12\x11\n\tgas_limit\x18\x06 \x01(\x0c\x12\x11\n\trecipient\x18\x07 \x01(\x0c\x12\r\n\x05value\x18\x08 \x01(\x0c\x12\x0c\n\x04\x64\x61ta\x18\t \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\n \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"\xc8\x01\n\x15\x45THSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.ETHCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x12\x10\n\x08\x63hain_id\x18\x05 \x01(\x04\"$\n\x0f\x45THSignResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xfb\x05\n\x1a\x45THSignTypedMessageRequest\x12\x10\n\x08\x63hain_id\x18\x01 \x01(\x04\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12J\n\x05types\x18\x03 \x03(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.StructType\x12\x14\n\x0cprimary_type\x18\x04 \x01(\t\x12R\n\x15host_nonce_commitment\x18\x05 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\x1a\xc9\x01\n\nMemberType\x12G\n\x04type\x18\x01 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.DataType\x12\x0c\n\x04size\x18\x02 \x01(\r\x12\x13\n\x0bstruct_name\x18\x03 \x01(\t\x12O\n\narray_type\x18\x04 \x01(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.MemberType\x1a\x61\n\x06Member\x12\x0c\n\x04name\x18\x01 \x01(\t\x12I\n\x04type\x18\x02 \x01(\x0b\x32;.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.MemberType\x1a\x64\n\nStructType\x12\x0c\n\x04name\x18\x01 \x01(\t\x12H\n\x07members\x18\x02 \x03(\x0b\x32\x37.shiftcrypto.bitbox02.ETHSignTypedMessageRequest.Member\"o\n\x08\x44\x61taType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x42YTES\x10\x01\x12\x08\n\x04UINT\x10\x02\x12\x07\n\x03INT\x10\x03\x12\x08\n\x04\x42OOL\x10\x04\x12\x0b\n\x07\x41\x44\x44RESS\x10\x05\x12\n\n\x06STRING\x10\x06\x12\t\n\x05\x41RRAY\x10\x07\x12\n\n\x06STRUCT\x10\x08\"\xb4\x01\n\x1c\x45THTypedMessageValueResponse\x12R\n\x0broot_object\x18\x01 \x01(\x0e\x32=.shiftcrypto.bitbox02.ETHTypedMessageValueResponse.RootObject\x12\x0c\n\x04path\x18\x02 \x03(\r\"2\n\nRootObject\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\x0b\n\x07MESSAGE\x10\x02\",\n\x1b\x45THTypedMessageValueRequest\x12\r\n\x05value\x18\x01 \x01(\x0c\"\xf3\x03\n\nETHRequest\x12\x32\n\x03pub\x18\x01 \x01(\x0b\x32#.shiftcrypto.bitbox02.ETHPubRequestH\x00\x12\x34\n\x04sign\x18\x02 \x01(\x0b\x32$.shiftcrypto.bitbox02.ETHSignRequestH\x00\x12?\n\x08sign_msg\x18\x03 \x01(\x0b\x32+.shiftcrypto.bitbox02.ETHSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x04 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x12J\n\x0esign_typed_msg\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.ETHSignTypedMessageRequestH\x00\x12L\n\x0ftyped_msg_value\x18\x06 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.ETHTypedMessageValueRequestH\x00\x12\x43\n\x0csign_eip1559\x18\x07 \x01(\x0b\x32+.shiftcrypto.bitbox02.ETHSignEIP1559RequestH\x00\x42\t\n\x07request\"\xab\x02\n\x0b\x45THResponse\x12\x30\n\x03pub\x18\x01 \x01(\x0b\x32!.shiftcrypto.bitbox02.PubResponseH\x00\x12\x35\n\x04sign\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.ETHSignResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x03 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x12M\n\x0ftyped_msg_value\x18\x04 \x01(\x0b\x32\x32.shiftcrypto.bitbox02.ETHTypedMessageValueResponseH\x00\x42\n\n\x08response*2\n\x07\x45THCoin\x12\x07\n\x03\x45TH\x10\x00\x12\x0e\n\nRopstenETH\x10\x01\x12\x0e\n\nRinkebyETH\x10\x02\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eth_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ETHCOIN._serialized_start=2569
-  _ETHCOIN._serialized_end=2619
+  _ETHCOIN._serialized_start=2924
+  _ETHCOIN._serialized_end=2974
   _ETHPUBREQUEST._serialized_start=68
   _ETHPUBREQUEST._serialized_end=312
   _ETHPUBREQUEST_OUTPUTTYPE._serialized_start=277
   _ETHPUBREQUEST_OUTPUTTYPE._serialized_end=312
   _ETHSIGNREQUEST._serialized_start=315
   _ETHSIGNREQUEST._serialized_end=596
-  _ETHSIGNMESSAGEREQUEST._serialized_start=599
-  _ETHSIGNMESSAGEREQUEST._serialized_end=799
-  _ETHSIGNRESPONSE._serialized_start=801
-  _ETHSIGNRESPONSE._serialized_end=837
-  _ETHSIGNTYPEDMESSAGEREQUEST._serialized_start=840
-  _ETHSIGNTYPEDMESSAGEREQUEST._serialized_end=1603
-  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBERTYPE._serialized_start=1088
-  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBERTYPE._serialized_end=1289
-  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBER._serialized_start=1291
-  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBER._serialized_end=1388
-  _ETHSIGNTYPEDMESSAGEREQUEST_STRUCTTYPE._serialized_start=1390
-  _ETHSIGNTYPEDMESSAGEREQUEST_STRUCTTYPE._serialized_end=1490
-  _ETHSIGNTYPEDMESSAGEREQUEST_DATATYPE._serialized_start=1492
-  _ETHSIGNTYPEDMESSAGEREQUEST_DATATYPE._serialized_end=1603
-  _ETHTYPEDMESSAGEVALUERESPONSE._serialized_start=1606
-  _ETHTYPEDMESSAGEVALUERESPONSE._serialized_end=1786
-  _ETHTYPEDMESSAGEVALUERESPONSE_ROOTOBJECT._serialized_start=1736
-  _ETHTYPEDMESSAGEVALUERESPONSE_ROOTOBJECT._serialized_end=1786
-  _ETHTYPEDMESSAGEVALUEREQUEST._serialized_start=1788
-  _ETHTYPEDMESSAGEVALUEREQUEST._serialized_end=1832
-  _ETHREQUEST._serialized_start=1835
-  _ETHREQUEST._serialized_end=2265
-  _ETHRESPONSE._serialized_start=2268
-  _ETHRESPONSE._serialized_end=2567
+  _ETHSIGNEIP1559REQUEST._serialized_start=599
+  _ETHSIGNEIP1559REQUEST._serialized_end=882
+  _ETHSIGNMESSAGEREQUEST._serialized_start=885
+  _ETHSIGNMESSAGEREQUEST._serialized_end=1085
+  _ETHSIGNRESPONSE._serialized_start=1087
+  _ETHSIGNRESPONSE._serialized_end=1123
+  _ETHSIGNTYPEDMESSAGEREQUEST._serialized_start=1126
+  _ETHSIGNTYPEDMESSAGEREQUEST._serialized_end=1889
+  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBERTYPE._serialized_start=1374
+  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBERTYPE._serialized_end=1575
+  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBER._serialized_start=1577
+  _ETHSIGNTYPEDMESSAGEREQUEST_MEMBER._serialized_end=1674
+  _ETHSIGNTYPEDMESSAGEREQUEST_STRUCTTYPE._serialized_start=1676
+  _ETHSIGNTYPEDMESSAGEREQUEST_STRUCTTYPE._serialized_end=1776
+  _ETHSIGNTYPEDMESSAGEREQUEST_DATATYPE._serialized_start=1778
+  _ETHSIGNTYPEDMESSAGEREQUEST_DATATYPE._serialized_end=1889
+  _ETHTYPEDMESSAGEVALUERESPONSE._serialized_start=1892
+  _ETHTYPEDMESSAGEVALUERESPONSE._serialized_end=2072
+  _ETHTYPEDMESSAGEVALUERESPONSE_ROOTOBJECT._serialized_start=2022
+  _ETHTYPEDMESSAGEVALUERESPONSE_ROOTOBJECT._serialized_end=2072
+  _ETHTYPEDMESSAGEVALUEREQUEST._serialized_start=2074
+  _ETHTYPEDMESSAGEVALUEREQUEST._serialized_end=2118
+  _ETHREQUEST._serialized_start=2121
+  _ETHREQUEST._serialized_end=2620
+  _ETHRESPONSE._serialized_start=2623
+  _ETHRESPONSE._serialized_end=2922
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/eth_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         contract_address: builtins.bytes = ...,
         chain_id: builtins.int = ...,
         ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","coin",b"coin","contract_address",b"contract_address","display",b"display","keypath",b"keypath","output_type",b"output_type"]) -> None: ...
 global___ETHPubRequest = ETHPubRequest
 
 class ETHSignRequest(google.protobuf.message.Message):
+    """TX payload for "legacy" (EIP-155) transactions: https://eips.ethereum.org/EIPS/eip-155"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     COIN_FIELD_NUMBER: builtins.int
     KEYPATH_FIELD_NUMBER: builtins.int
     NONCE_FIELD_NUMBER: builtins.int
     GAS_PRICE_FIELD_NUMBER: builtins.int
     GAS_LIMIT_FIELD_NUMBER: builtins.int
     RECIPIENT_FIELD_NUMBER: builtins.int
@@ -135,14 +136,68 @@
         host_nonce_commitment: typing.Optional[antiklepto_pb2.AntiKleptoHostNonceCommitment] = ...,
         chain_id: builtins.int = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["host_nonce_commitment",b"host_nonce_commitment"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","coin",b"coin","data",b"data","gas_limit",b"gas_limit","gas_price",b"gas_price","host_nonce_commitment",b"host_nonce_commitment","keypath",b"keypath","nonce",b"nonce","recipient",b"recipient","value",b"value"]) -> None: ...
 global___ETHSignRequest = ETHSignRequest
 
+class ETHSignEIP1559Request(google.protobuf.message.Message):
+    """TX payload for an EIP-1559 (type 2) transaction: https://eips.ethereum.org/EIPS/eip-1559"""
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    CHAIN_ID_FIELD_NUMBER: builtins.int
+    KEYPATH_FIELD_NUMBER: builtins.int
+    NONCE_FIELD_NUMBER: builtins.int
+    MAX_PRIORITY_FEE_PER_GAS_FIELD_NUMBER: builtins.int
+    MAX_FEE_PER_GAS_FIELD_NUMBER: builtins.int
+    GAS_LIMIT_FIELD_NUMBER: builtins.int
+    RECIPIENT_FIELD_NUMBER: builtins.int
+    VALUE_FIELD_NUMBER: builtins.int
+    DATA_FIELD_NUMBER: builtins.int
+    HOST_NONCE_COMMITMENT_FIELD_NUMBER: builtins.int
+    chain_id: builtins.int
+    @property
+    def keypath(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    nonce: builtins.bytes
+    """smallest big endian serialization, max. 16 bytes"""
+
+    max_priority_fee_per_gas: builtins.bytes
+    """smallest big endian serialization, max. 16 bytes"""
+
+    max_fee_per_gas: builtins.bytes
+    """smallest big endian serialization, max. 16 bytes"""
+
+    gas_limit: builtins.bytes
+    """smallest big endian serialization, max. 16 bytes"""
+
+    recipient: builtins.bytes
+    """20 byte recipient"""
+
+    value: builtins.bytes
+    """smallest big endian serialization, max. 32 bytes"""
+
+    data: builtins.bytes
+    @property
+    def host_nonce_commitment(self) -> antiklepto_pb2.AntiKleptoHostNonceCommitment: ...
+    def __init__(self,
+        *,
+        chain_id: builtins.int = ...,
+        keypath: typing.Optional[typing.Iterable[builtins.int]] = ...,
+        nonce: builtins.bytes = ...,
+        max_priority_fee_per_gas: builtins.bytes = ...,
+        max_fee_per_gas: builtins.bytes = ...,
+        gas_limit: builtins.bytes = ...,
+        recipient: builtins.bytes = ...,
+        value: builtins.bytes = ...,
+        data: builtins.bytes = ...,
+        host_nonce_commitment: typing.Optional[antiklepto_pb2.AntiKleptoHostNonceCommitment] = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["host_nonce_commitment",b"host_nonce_commitment"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["chain_id",b"chain_id","data",b"data","gas_limit",b"gas_limit","host_nonce_commitment",b"host_nonce_commitment","keypath",b"keypath","max_fee_per_gas",b"max_fee_per_gas","max_priority_fee_per_gas",b"max_priority_fee_per_gas","nonce",b"nonce","recipient",b"recipient","value",b"value"]) -> None: ...
+global___ETHSignEIP1559Request = ETHSignEIP1559Request
+
 class ETHSignMessageRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     COIN_FIELD_NUMBER: builtins.int
     KEYPATH_FIELD_NUMBER: builtins.int
     MSG_FIELD_NUMBER: builtins.int
     HOST_NONCE_COMMITMENT_FIELD_NUMBER: builtins.int
     CHAIN_ID_FIELD_NUMBER: builtins.int
@@ -335,38 +390,42 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     PUB_FIELD_NUMBER: builtins.int
     SIGN_FIELD_NUMBER: builtins.int
     SIGN_MSG_FIELD_NUMBER: builtins.int
     ANTIKLEPTO_SIGNATURE_FIELD_NUMBER: builtins.int
     SIGN_TYPED_MSG_FIELD_NUMBER: builtins.int
     TYPED_MSG_VALUE_FIELD_NUMBER: builtins.int
+    SIGN_EIP1559_FIELD_NUMBER: builtins.int
     @property
     def pub(self) -> global___ETHPubRequest: ...
     @property
     def sign(self) -> global___ETHSignRequest: ...
     @property
     def sign_msg(self) -> global___ETHSignMessageRequest: ...
     @property
     def antiklepto_signature(self) -> antiklepto_pb2.AntiKleptoSignatureRequest: ...
     @property
     def sign_typed_msg(self) -> global___ETHSignTypedMessageRequest: ...
     @property
     def typed_msg_value(self) -> global___ETHTypedMessageValueRequest: ...
+    @property
+    def sign_eip1559(self) -> global___ETHSignEIP1559Request: ...
     def __init__(self,
         *,
         pub: typing.Optional[global___ETHPubRequest] = ...,
         sign: typing.Optional[global___ETHSignRequest] = ...,
         sign_msg: typing.Optional[global___ETHSignMessageRequest] = ...,
         antiklepto_signature: typing.Optional[antiklepto_pb2.AntiKleptoSignatureRequest] = ...,
         sign_typed_msg: typing.Optional[global___ETHSignTypedMessageRequest] = ...,
         typed_msg_value: typing.Optional[global___ETHTypedMessageValueRequest] = ...,
+        sign_eip1559: typing.Optional[global___ETHSignEIP1559Request] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["antiklepto_signature",b"antiklepto_signature","pub",b"pub","request",b"request","sign",b"sign","sign_msg",b"sign_msg","sign_typed_msg",b"sign_typed_msg","typed_msg_value",b"typed_msg_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["antiklepto_signature",b"antiklepto_signature","pub",b"pub","request",b"request","sign",b"sign","sign_msg",b"sign_msg","sign_typed_msg",b"sign_typed_msg","typed_msg_value",b"typed_msg_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["request",b"request"]) -> typing.Optional[typing_extensions.Literal["pub","sign","sign_msg","antiklepto_signature","sign_typed_msg","typed_msg_value"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["antiklepto_signature",b"antiklepto_signature","pub",b"pub","request",b"request","sign",b"sign","sign_eip1559",b"sign_eip1559","sign_msg",b"sign_msg","sign_typed_msg",b"sign_typed_msg","typed_msg_value",b"typed_msg_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["antiklepto_signature",b"antiklepto_signature","pub",b"pub","request",b"request","sign",b"sign","sign_eip1559",b"sign_eip1559","sign_msg",b"sign_msg","sign_typed_msg",b"sign_typed_msg","typed_msg_value",b"typed_msg_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["request",b"request"]) -> typing.Optional[typing_extensions.Literal["pub","sign","sign_msg","antiklepto_signature","sign_typed_msg","typed_msg_value","sign_eip1559"]]: ...
 global___ETHRequest = ETHRequest
 
 class ETHResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     PUB_FIELD_NUMBER: builtins.int
     SIGN_FIELD_NUMBER: builtins.int
     ANTIKLEPTO_SIGNER_COMMITMENT_FIELD_NUMBER: builtins.int
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/hww_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 from . import eth_pb2 as eth__pb2
 from . import keystore_pb2 as keystore__pb2
 from . import mnemonic_pb2 as mnemonic__pb2
 from . import system_pb2 as system__pb2
 from . import perform_attestation_pb2 as perform__attestation__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\thww.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x15\x62\x61\x63kup_commands.proto\x1a\x15\x62itbox02_system.proto\x1a\tbtc.proto\x1a\rcardano.proto\x1a\teth.proto\x1a\x0ekeystore.proto\x1a\x0emnemonic.proto\x1a\x0csystem.proto\x1a\x19perform_attestation.proto\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"\t\n\x07Success\"\xc8\r\n\x07Request\x12\x41\n\x0b\x64\x65vice_name\x18\x02 \x01(\x0b\x32*.shiftcrypto.bitbox02.SetDeviceNameRequestH\x00\x12I\n\x0f\x64\x65vice_language\x18\x03 \x01(\x0b\x32..shiftcrypto.bitbox02.SetDeviceLanguageRequestH\x00\x12>\n\x0b\x64\x65vice_info\x18\x04 \x01(\x0b\x32\'.shiftcrypto.bitbox02.DeviceInfoRequestH\x00\x12@\n\x0cset_password\x18\x05 \x01(\x0b\x32(.shiftcrypto.bitbox02.SetPasswordRequestH\x00\x12\x42\n\rcreate_backup\x18\x06 \x01(\x0b\x32).shiftcrypto.bitbox02.CreateBackupRequestH\x00\x12\x42\n\rshow_mnemonic\x18\x07 \x01(\x0b\x32).shiftcrypto.bitbox02.ShowMnemonicRequestH\x00\x12\x36\n\x07\x62tc_pub\x18\x08 \x01(\x0b\x32#.shiftcrypto.bitbox02.BTCPubRequestH\x00\x12\x41\n\rbtc_sign_init\x18\t \x01(\x0b\x32(.shiftcrypto.bitbox02.BTCSignInitRequestH\x00\x12\x43\n\x0e\x62tc_sign_input\x18\n \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignInputRequestH\x00\x12\x45\n\x0f\x62tc_sign_output\x18\x0b \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCSignOutputRequestH\x00\x12O\n\x14insert_remove_sdcard\x18\x0c \x01(\x0b\x32/.shiftcrypto.bitbox02.InsertRemoveSDCardRequestH\x00\x12@\n\x0c\x63heck_sdcard\x18\r \x01(\x0b\x32(.shiftcrypto.bitbox02.CheckSDCardRequestH\x00\x12\x64\n\x1fset_mnemonic_passphrase_enabled\x18\x0e \x01(\x0b\x32\x39.shiftcrypto.bitbox02.SetMnemonicPassphraseEnabledRequestH\x00\x12@\n\x0clist_backups\x18\x0f \x01(\x0b\x32(.shiftcrypto.bitbox02.ListBackupsRequestH\x00\x12\x44\n\x0erestore_backup\x18\x10 \x01(\x0b\x32*.shiftcrypto.bitbox02.RestoreBackupRequestH\x00\x12N\n\x13perform_attestation\x18\x11 \x01(\x0b\x32/.shiftcrypto.bitbox02.PerformAttestationRequestH\x00\x12\x35\n\x06reboot\x18\x12 \x01(\x0b\x32#.shiftcrypto.bitbox02.RebootRequestH\x00\x12@\n\x0c\x63heck_backup\x18\x13 \x01(\x0b\x32(.shiftcrypto.bitbox02.CheckBackupRequestH\x00\x12/\n\x03\x65th\x18\x14 \x01(\x0b\x32 .shiftcrypto.bitbox02.ETHRequestH\x00\x12\x33\n\x05reset\x18\x15 \x01(\x0b\x32\".shiftcrypto.bitbox02.ResetRequestH\x00\x12Q\n\x15restore_from_mnemonic\x18\x16 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.RestoreFromMnemonicRequestH\x00\x12\x43\n\x0b\x66ingerprint\x18\x18 \x01(\x0b\x32,.shiftcrypto.bitbox02.RootFingerprintRequestH\x00\x12/\n\x03\x62tc\x18\x19 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCRequestH\x00\x12U\n\x17\x65lectrum_encryption_key\x18\x1a \x01(\x0b\x32\x32.shiftcrypto.bitbox02.ElectrumEncryptionKeyRequestH\x00\x12\x37\n\x07\x63\x61rdano\x18\x1b \x01(\x0b\x32$.shiftcrypto.bitbox02.CardanoRequestH\x00\x42\t\n\x07requestJ\x04\x08\x01\x10\x02J\x04\x08\x17\x10\x18\"\x89\x07\n\x08Response\x12\x30\n\x07success\x18\x01 \x01(\x0b\x32\x1d.shiftcrypto.bitbox02.SuccessH\x00\x12,\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1b.shiftcrypto.bitbox02.ErrorH\x00\x12?\n\x0b\x64\x65vice_info\x18\x04 \x01(\x0b\x32(.shiftcrypto.bitbox02.DeviceInfoResponseH\x00\x12\x30\n\x03pub\x18\x05 \x01(\x0b\x32!.shiftcrypto.bitbox02.PubResponseH\x00\x12\x42\n\rbtc_sign_next\x18\x06 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x41\n\x0clist_backups\x18\x07 \x01(\x0b\x32).shiftcrypto.bitbox02.ListBackupsResponseH\x00\x12\x41\n\x0c\x63heck_backup\x18\x08 \x01(\x0b\x32).shiftcrypto.bitbox02.CheckBackupResponseH\x00\x12O\n\x13perform_attestation\x18\t \x01(\x0b\x32\x30.shiftcrypto.bitbox02.PerformAttestationResponseH\x00\x12\x41\n\x0c\x63heck_sdcard\x18\n \x01(\x0b\x32).shiftcrypto.bitbox02.CheckSDCardResponseH\x00\x12\x30\n\x03\x65th\x18\x0b \x01(\x0b\x32!.shiftcrypto.bitbox02.ETHResponseH\x00\x12\x44\n\x0b\x66ingerprint\x18\x0c \x01(\x0b\x32-.shiftcrypto.bitbox02.RootFingerprintResponseH\x00\x12\x30\n\x03\x62tc\x18\r \x01(\x0b\x32!.shiftcrypto.bitbox02.BTCResponseH\x00\x12V\n\x17\x65lectrum_encryption_key\x18\x0e \x01(\x0b\x32\x33.shiftcrypto.bitbox02.ElectrumEncryptionKeyResponseH\x00\x12\x38\n\x07\x63\x61rdano\x18\x0f \x01(\x0b\x32%.shiftcrypto.bitbox02.CardanoResponseH\x00\x42\n\n\x08responseJ\x04\x08\x03\x10\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\thww.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x15\x62\x61\x63kup_commands.proto\x1a\x15\x62itbox02_system.proto\x1a\tbtc.proto\x1a\rcardano.proto\x1a\teth.proto\x1a\x0ekeystore.proto\x1a\x0emnemonic.proto\x1a\x0csystem.proto\x1a\x19perform_attestation.proto\"&\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"\t\n\x07Success\"\xfd\r\n\x07Request\x12\x41\n\x0b\x64\x65vice_name\x18\x02 \x01(\x0b\x32*.shiftcrypto.bitbox02.SetDeviceNameRequestH\x00\x12I\n\x0f\x64\x65vice_language\x18\x03 \x01(\x0b\x32..shiftcrypto.bitbox02.SetDeviceLanguageRequestH\x00\x12>\n\x0b\x64\x65vice_info\x18\x04 \x01(\x0b\x32\'.shiftcrypto.bitbox02.DeviceInfoRequestH\x00\x12@\n\x0cset_password\x18\x05 \x01(\x0b\x32(.shiftcrypto.bitbox02.SetPasswordRequestH\x00\x12\x42\n\rcreate_backup\x18\x06 \x01(\x0b\x32).shiftcrypto.bitbox02.CreateBackupRequestH\x00\x12\x42\n\rshow_mnemonic\x18\x07 \x01(\x0b\x32).shiftcrypto.bitbox02.ShowMnemonicRequestH\x00\x12\x36\n\x07\x62tc_pub\x18\x08 \x01(\x0b\x32#.shiftcrypto.bitbox02.BTCPubRequestH\x00\x12\x41\n\rbtc_sign_init\x18\t \x01(\x0b\x32(.shiftcrypto.bitbox02.BTCSignInitRequestH\x00\x12\x43\n\x0e\x62tc_sign_input\x18\n \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignInputRequestH\x00\x12\x45\n\x0f\x62tc_sign_output\x18\x0b \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCSignOutputRequestH\x00\x12O\n\x14insert_remove_sdcard\x18\x0c \x01(\x0b\x32/.shiftcrypto.bitbox02.InsertRemoveSDCardRequestH\x00\x12@\n\x0c\x63heck_sdcard\x18\r \x01(\x0b\x32(.shiftcrypto.bitbox02.CheckSDCardRequestH\x00\x12\x64\n\x1fset_mnemonic_passphrase_enabled\x18\x0e \x01(\x0b\x32\x39.shiftcrypto.bitbox02.SetMnemonicPassphraseEnabledRequestH\x00\x12@\n\x0clist_backups\x18\x0f \x01(\x0b\x32(.shiftcrypto.bitbox02.ListBackupsRequestH\x00\x12\x44\n\x0erestore_backup\x18\x10 \x01(\x0b\x32*.shiftcrypto.bitbox02.RestoreBackupRequestH\x00\x12N\n\x13perform_attestation\x18\x11 \x01(\x0b\x32/.shiftcrypto.bitbox02.PerformAttestationRequestH\x00\x12\x35\n\x06reboot\x18\x12 \x01(\x0b\x32#.shiftcrypto.bitbox02.RebootRequestH\x00\x12@\n\x0c\x63heck_backup\x18\x13 \x01(\x0b\x32(.shiftcrypto.bitbox02.CheckBackupRequestH\x00\x12/\n\x03\x65th\x18\x14 \x01(\x0b\x32 .shiftcrypto.bitbox02.ETHRequestH\x00\x12\x33\n\x05reset\x18\x15 \x01(\x0b\x32\".shiftcrypto.bitbox02.ResetRequestH\x00\x12Q\n\x15restore_from_mnemonic\x18\x16 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.RestoreFromMnemonicRequestH\x00\x12\x43\n\x0b\x66ingerprint\x18\x18 \x01(\x0b\x32,.shiftcrypto.bitbox02.RootFingerprintRequestH\x00\x12/\n\x03\x62tc\x18\x19 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCRequestH\x00\x12U\n\x17\x65lectrum_encryption_key\x18\x1a \x01(\x0b\x32\x32.shiftcrypto.bitbox02.ElectrumEncryptionKeyRequestH\x00\x12\x37\n\x07\x63\x61rdano\x18\x1b \x01(\x0b\x32$.shiftcrypto.bitbox02.CardanoRequestH\x00\x12\x33\n\x05\x62ip85\x18\x1c \x01(\x0b\x32\".shiftcrypto.bitbox02.BIP85RequestH\x00\x42\t\n\x07requestJ\x04\x08\x01\x10\x02J\x04\x08\x17\x10\x18\"\xbf\x07\n\x08Response\x12\x30\n\x07success\x18\x01 \x01(\x0b\x32\x1d.shiftcrypto.bitbox02.SuccessH\x00\x12,\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1b.shiftcrypto.bitbox02.ErrorH\x00\x12?\n\x0b\x64\x65vice_info\x18\x04 \x01(\x0b\x32(.shiftcrypto.bitbox02.DeviceInfoResponseH\x00\x12\x30\n\x03pub\x18\x05 \x01(\x0b\x32!.shiftcrypto.bitbox02.PubResponseH\x00\x12\x42\n\rbtc_sign_next\x18\x06 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x41\n\x0clist_backups\x18\x07 \x01(\x0b\x32).shiftcrypto.bitbox02.ListBackupsResponseH\x00\x12\x41\n\x0c\x63heck_backup\x18\x08 \x01(\x0b\x32).shiftcrypto.bitbox02.CheckBackupResponseH\x00\x12O\n\x13perform_attestation\x18\t \x01(\x0b\x32\x30.shiftcrypto.bitbox02.PerformAttestationResponseH\x00\x12\x41\n\x0c\x63heck_sdcard\x18\n \x01(\x0b\x32).shiftcrypto.bitbox02.CheckSDCardResponseH\x00\x12\x30\n\x03\x65th\x18\x0b \x01(\x0b\x32!.shiftcrypto.bitbox02.ETHResponseH\x00\x12\x44\n\x0b\x66ingerprint\x18\x0c \x01(\x0b\x32-.shiftcrypto.bitbox02.RootFingerprintResponseH\x00\x12\x30\n\x03\x62tc\x18\r \x01(\x0b\x32!.shiftcrypto.bitbox02.BTCResponseH\x00\x12V\n\x17\x65lectrum_encryption_key\x18\x0e \x01(\x0b\x32\x33.shiftcrypto.bitbox02.ElectrumEncryptionKeyResponseH\x00\x12\x38\n\x07\x63\x61rdano\x18\x0f \x01(\x0b\x32%.shiftcrypto.bitbox02.CardanoResponseH\x00\x12\x34\n\x05\x62ip85\x18\x10 \x01(\x0b\x32#.shiftcrypto.bitbox02.BIP85ResponseH\x00\x42\n\n\x08responseJ\x04\x08\x03\x10\x04\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'hww_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _ERROR._serialized_start=205
   _ERROR._serialized_end=243
   _SUCCESS._serialized_start=245
   _SUCCESS._serialized_end=254
   _REQUEST._serialized_start=257
-  _REQUEST._serialized_end=1993
-  _RESPONSE._serialized_start=1996
-  _RESPONSE._serialized_end=2901
+  _REQUEST._serialized_end=2046
+  _RESPONSE._serialized_start=2049
+  _RESPONSE._serialized_end=3008
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/hww_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     ETH_FIELD_NUMBER: builtins.int
     RESET_FIELD_NUMBER: builtins.int
     RESTORE_FROM_MNEMONIC_FIELD_NUMBER: builtins.int
     FINGERPRINT_FIELD_NUMBER: builtins.int
     BTC_FIELD_NUMBER: builtins.int
     ELECTRUM_ENCRYPTION_KEY_FIELD_NUMBER: builtins.int
     CARDANO_FIELD_NUMBER: builtins.int
+    BIP85_FIELD_NUMBER: builtins.int
     @property
     def device_name(self) -> bitbox02_system_pb2.SetDeviceNameRequest:
         """removed: RandomNumberRequest random_number = 1;"""
         pass
     @property
     def device_language(self) -> bitbox02_system_pb2.SetDeviceLanguageRequest: ...
     @property
@@ -117,14 +118,16 @@
         pass
     @property
     def btc(self) -> btc_pb2.BTCRequest: ...
     @property
     def electrum_encryption_key(self) -> keystore_pb2.ElectrumEncryptionKeyRequest: ...
     @property
     def cardano(self) -> cardano_pb2.CardanoRequest: ...
+    @property
+    def bip85(self) -> keystore_pb2.BIP85Request: ...
     def __init__(self,
         *,
         device_name: typing.Optional[bitbox02_system_pb2.SetDeviceNameRequest] = ...,
         device_language: typing.Optional[bitbox02_system_pb2.SetDeviceLanguageRequest] = ...,
         device_info: typing.Optional[bitbox02_system_pb2.DeviceInfoRequest] = ...,
         set_password: typing.Optional[bitbox02_system_pb2.SetPasswordRequest] = ...,
         create_backup: typing.Optional[backup_commands_pb2.CreateBackupRequest] = ...,
@@ -144,18 +147,19 @@
         eth: typing.Optional[eth_pb2.ETHRequest] = ...,
         reset: typing.Optional[bitbox02_system_pb2.ResetRequest] = ...,
         restore_from_mnemonic: typing.Optional[mnemonic_pb2.RestoreFromMnemonicRequest] = ...,
         fingerprint: typing.Optional[common_pb2.RootFingerprintRequest] = ...,
         btc: typing.Optional[btc_pb2.BTCRequest] = ...,
         electrum_encryption_key: typing.Optional[keystore_pb2.ElectrumEncryptionKeyRequest] = ...,
         cardano: typing.Optional[cardano_pb2.CardanoRequest] = ...,
+        bip85: typing.Optional[keystore_pb2.BIP85Request] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["btc",b"btc","btc_pub",b"btc_pub","btc_sign_init",b"btc_sign_init","btc_sign_input",b"btc_sign_input","btc_sign_output",b"btc_sign_output","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","create_backup",b"create_backup","device_info",b"device_info","device_language",b"device_language","device_name",b"device_name","electrum_encryption_key",b"electrum_encryption_key","eth",b"eth","fingerprint",b"fingerprint","insert_remove_sdcard",b"insert_remove_sdcard","list_backups",b"list_backups","perform_attestation",b"perform_attestation","reboot",b"reboot","request",b"request","reset",b"reset","restore_backup",b"restore_backup","restore_from_mnemonic",b"restore_from_mnemonic","set_mnemonic_passphrase_enabled",b"set_mnemonic_passphrase_enabled","set_password",b"set_password","show_mnemonic",b"show_mnemonic"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["btc",b"btc","btc_pub",b"btc_pub","btc_sign_init",b"btc_sign_init","btc_sign_input",b"btc_sign_input","btc_sign_output",b"btc_sign_output","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","create_backup",b"create_backup","device_info",b"device_info","device_language",b"device_language","device_name",b"device_name","electrum_encryption_key",b"electrum_encryption_key","eth",b"eth","fingerprint",b"fingerprint","insert_remove_sdcard",b"insert_remove_sdcard","list_backups",b"list_backups","perform_attestation",b"perform_attestation","reboot",b"reboot","request",b"request","reset",b"reset","restore_backup",b"restore_backup","restore_from_mnemonic",b"restore_from_mnemonic","set_mnemonic_passphrase_enabled",b"set_mnemonic_passphrase_enabled","set_password",b"set_password","show_mnemonic",b"show_mnemonic"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["request",b"request"]) -> typing.Optional[typing_extensions.Literal["device_name","device_language","device_info","set_password","create_backup","show_mnemonic","btc_pub","btc_sign_init","btc_sign_input","btc_sign_output","insert_remove_sdcard","check_sdcard","set_mnemonic_passphrase_enabled","list_backups","restore_backup","perform_attestation","reboot","check_backup","eth","reset","restore_from_mnemonic","fingerprint","btc","electrum_encryption_key","cardano"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["bip85",b"bip85","btc",b"btc","btc_pub",b"btc_pub","btc_sign_init",b"btc_sign_init","btc_sign_input",b"btc_sign_input","btc_sign_output",b"btc_sign_output","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","create_backup",b"create_backup","device_info",b"device_info","device_language",b"device_language","device_name",b"device_name","electrum_encryption_key",b"electrum_encryption_key","eth",b"eth","fingerprint",b"fingerprint","insert_remove_sdcard",b"insert_remove_sdcard","list_backups",b"list_backups","perform_attestation",b"perform_attestation","reboot",b"reboot","request",b"request","reset",b"reset","restore_backup",b"restore_backup","restore_from_mnemonic",b"restore_from_mnemonic","set_mnemonic_passphrase_enabled",b"set_mnemonic_passphrase_enabled","set_password",b"set_password","show_mnemonic",b"show_mnemonic"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bip85",b"bip85","btc",b"btc","btc_pub",b"btc_pub","btc_sign_init",b"btc_sign_init","btc_sign_input",b"btc_sign_input","btc_sign_output",b"btc_sign_output","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","create_backup",b"create_backup","device_info",b"device_info","device_language",b"device_language","device_name",b"device_name","electrum_encryption_key",b"electrum_encryption_key","eth",b"eth","fingerprint",b"fingerprint","insert_remove_sdcard",b"insert_remove_sdcard","list_backups",b"list_backups","perform_attestation",b"perform_attestation","reboot",b"reboot","request",b"request","reset",b"reset","restore_backup",b"restore_backup","restore_from_mnemonic",b"restore_from_mnemonic","set_mnemonic_passphrase_enabled",b"set_mnemonic_passphrase_enabled","set_password",b"set_password","show_mnemonic",b"show_mnemonic"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["request",b"request"]) -> typing.Optional[typing_extensions.Literal["device_name","device_language","device_info","set_password","create_backup","show_mnemonic","btc_pub","btc_sign_init","btc_sign_input","btc_sign_output","insert_remove_sdcard","check_sdcard","set_mnemonic_passphrase_enabled","list_backups","restore_backup","perform_attestation","reboot","check_backup","eth","reset","restore_from_mnemonic","fingerprint","btc","electrum_encryption_key","cardano","bip85"]]: ...
 global___Request = Request
 
 class Response(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     SUCCESS_FIELD_NUMBER: builtins.int
     ERROR_FIELD_NUMBER: builtins.int
     DEVICE_INFO_FIELD_NUMBER: builtins.int
@@ -166,14 +170,15 @@
     PERFORM_ATTESTATION_FIELD_NUMBER: builtins.int
     CHECK_SDCARD_FIELD_NUMBER: builtins.int
     ETH_FIELD_NUMBER: builtins.int
     FINGERPRINT_FIELD_NUMBER: builtins.int
     BTC_FIELD_NUMBER: builtins.int
     ELECTRUM_ENCRYPTION_KEY_FIELD_NUMBER: builtins.int
     CARDANO_FIELD_NUMBER: builtins.int
+    BIP85_FIELD_NUMBER: builtins.int
     @property
     def success(self) -> global___Success: ...
     @property
     def error(self) -> global___Error: ...
     @property
     def device_info(self) -> bitbox02_system_pb2.DeviceInfoResponse:
         """removed: RandomNumberResponse random_number = 3;"""
@@ -196,14 +201,16 @@
     def fingerprint(self) -> common_pb2.RootFingerprintResponse: ...
     @property
     def btc(self) -> btc_pb2.BTCResponse: ...
     @property
     def electrum_encryption_key(self) -> keystore_pb2.ElectrumEncryptionKeyResponse: ...
     @property
     def cardano(self) -> cardano_pb2.CardanoResponse: ...
+    @property
+    def bip85(self) -> keystore_pb2.BIP85Response: ...
     def __init__(self,
         *,
         success: typing.Optional[global___Success] = ...,
         error: typing.Optional[global___Error] = ...,
         device_info: typing.Optional[bitbox02_system_pb2.DeviceInfoResponse] = ...,
         pub: typing.Optional[common_pb2.PubResponse] = ...,
         btc_sign_next: typing.Optional[btc_pb2.BTCSignNextResponse] = ...,
@@ -212,12 +219,13 @@
         perform_attestation: typing.Optional[perform_attestation_pb2.PerformAttestationResponse] = ...,
         check_sdcard: typing.Optional[bitbox02_system_pb2.CheckSDCardResponse] = ...,
         eth: typing.Optional[eth_pb2.ETHResponse] = ...,
         fingerprint: typing.Optional[common_pb2.RootFingerprintResponse] = ...,
         btc: typing.Optional[btc_pb2.BTCResponse] = ...,
         electrum_encryption_key: typing.Optional[keystore_pb2.ElectrumEncryptionKeyResponse] = ...,
         cardano: typing.Optional[cardano_pb2.CardanoResponse] = ...,
+        bip85: typing.Optional[keystore_pb2.BIP85Response] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["btc",b"btc","btc_sign_next",b"btc_sign_next","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","device_info",b"device_info","electrum_encryption_key",b"electrum_encryption_key","error",b"error","eth",b"eth","fingerprint",b"fingerprint","list_backups",b"list_backups","perform_attestation",b"perform_attestation","pub",b"pub","response",b"response","success",b"success"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["btc",b"btc","btc_sign_next",b"btc_sign_next","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","device_info",b"device_info","electrum_encryption_key",b"electrum_encryption_key","error",b"error","eth",b"eth","fingerprint",b"fingerprint","list_backups",b"list_backups","perform_attestation",b"perform_attestation","pub",b"pub","response",b"response","success",b"success"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["response",b"response"]) -> typing.Optional[typing_extensions.Literal["success","error","device_info","pub","btc_sign_next","list_backups","check_backup","perform_attestation","check_sdcard","eth","fingerprint","btc","electrum_encryption_key","cardano"]]: ...
+    def HasField(self, field_name: typing_extensions.Literal["bip85",b"bip85","btc",b"btc","btc_sign_next",b"btc_sign_next","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","device_info",b"device_info","electrum_encryption_key",b"electrum_encryption_key","error",b"error","eth",b"eth","fingerprint",b"fingerprint","list_backups",b"list_backups","perform_attestation",b"perform_attestation","pub",b"pub","response",b"response","success",b"success"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bip85",b"bip85","btc",b"btc","btc_sign_next",b"btc_sign_next","cardano",b"cardano","check_backup",b"check_backup","check_sdcard",b"check_sdcard","device_info",b"device_info","electrum_encryption_key",b"electrum_encryption_key","error",b"error","eth",b"eth","fingerprint",b"fingerprint","list_backups",b"list_backups","perform_attestation",b"perform_attestation","pub",b"pub","response",b"response","success",b"success"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["response",b"response"]) -> typing.Optional[typing_extensions.Literal["success","error","device_info","pub","btc_sign_next","list_backups","check_backup","perform_attestation","check_sdcard","eth","fingerprint","btc","electrum_encryption_key","cardano","bip85"]]: ...
 global___Response = Response
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/mnemonic_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: keystore.proto
+# source: mnemonic.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0ekeystore.proto\x12\x14shiftcrypto.bitbox02\"/\n\x1c\x45lectrumEncryptionKeyRequest\x12\x0f\n\x07keypath\x18\x01 \x03(\r\",\n\x1d\x45lectrumEncryptionKeyResponse\x12\x0b\n\x03key\x18\x01 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0emnemonic.proto\x12\x14shiftcrypto.bitbox02\"\x15\n\x13ShowMnemonicRequest\"H\n\x1aRestoreFromMnemonicRequest\x12\x11\n\ttimestamp\x18\x01 \x01(\r\x12\x17\n\x0ftimezone_offset\x18\x02 \x01(\x05\"6\n#SetMnemonicPassphraseEnabledRequest\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'keystore_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mnemonic_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ELECTRUMENCRYPTIONKEYREQUEST._serialized_start=40
-  _ELECTRUMENCRYPTIONKEYREQUEST._serialized_end=87
-  _ELECTRUMENCRYPTIONKEYRESPONSE._serialized_start=89
-  _ELECTRUMENCRYPTIONKEYRESPONSE._serialized_end=133
+  _SHOWMNEMONICREQUEST._serialized_start=40
+  _SHOWMNEMONICREQUEST._serialized_end=61
+  _RESTOREFROMMNEMONICREQUEST._serialized_start=63
+  _RESTOREFROMMNEMONICREQUEST._serialized_end=135
+  _SETMNEMONICPASSPHRASEENABLEDREQUEST._serialized_start=137
+  _SETMNEMONICPASSPHRASEENABLEDREQUEST._serialized_end=191
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/mnemonic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/perform_attestation_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.py` & `bitbox02-6.3.0/bitbox02/communication/generated/system_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.pyi` & `bitbox02-6.3.0/bitbox02/communication/generated/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/u2fhid/__init__.py` & `bitbox02-6.3.0/bitbox02/communication/u2fhid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/communication/u2fhid/u2fhid.py` & `bitbox02-6.3.0/bitbox02/communication/u2fhid/u2fhid.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02/util.py` & `bitbox02-6.3.0/bitbox02/util.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.2.0/bitbox02.egg-info/PKG-INFO` & `bitbox02-6.3.0/bitbox02.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: bitbox02
-Version: 6.2.0
+Version: 6.3.0
 Summary: Python library for bitbox02 communication
 Home-page: https://github.com/digitalbitbox/bitbox02-firmware
 Author: Shift Crypto
 Author-email: support@shiftcrypto.ch
-License: UNKNOWN
-Description: # BitBox02 python API
-        
-        This repository contains two packages
-        
-        * u2fhid
-        * bitbox02
-        
-        ## u2fhid
-        
-        This is a small package that contains read/write primitives for u2fhid devices such as the
-        bitbox02.
-        
-        ## bitbox02
-        
-        In this folder is the Python API for communicating with the BitBox02 device.
-        
-        The folder `generated` contains files generated by `python-protobuf`. Regenerate with `make`.
-        
 Keywords: digitalbitbox bitbox bitbox02 bitcoin litecoin ethereum erc20 u2f
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# BitBox02 python API
+
+This repository contains two packages
+
+* u2fhid
+* bitbox02
+
+## u2fhid
+
+This is a small package that contains read/write primitives for u2fhid devices such as the
+bitbox02.
+
+## bitbox02
+
+In this folder is the Python API for communicating with the BitBox02 device.
+
+The folder `generated` contains files generated by `python-protobuf`. Regenerate with `make`.
```

### Comparing `bitbox02-6.2.0/bitbox02.egg-info/SOURCES.txt` & `bitbox02-6.3.0/bitbox02.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 bitbox02/__init__.py
 bitbox02/py.typed
 bitbox02/util.py
 bitbox02.egg-info/PKG-INFO
 bitbox02.egg-info/SOURCES.txt
```

### Comparing `bitbox02-6.2.0/setup.py` & `bitbox02-6.3.0/setup.py`

 * *Files identical despite different names*

