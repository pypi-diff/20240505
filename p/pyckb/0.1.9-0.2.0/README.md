# Comparing `tmp/pyckb-0.1.9.tar.gz` & `tmp/pyckb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckb-0.1.9.tar", last modified: Mon Apr 29 09:21:17 2024, max compression
+gzip compressed data, was "pyckb-0.2.0.tar", last modified: Sun May  5 01:43:59 2024, max compression
```

## Comparing `pyckb-0.1.9.tar` & `pyckb-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.1.9/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-29 09:21:17.949677 pyckb-0.1.9/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.1.9/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.945677 pyckb-0.1.9/ckb/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-29 09:12:52.000000 pyckb-0.1.9/ckb/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4637 2024-04-19 12:01:42.000000 pyckb-0.1.9/ckb/bech32m.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-26 09:57:50.000000 pyckb-0.1.9/ckb/config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17328 2024-04-29 09:13:36.000000 pyckb-0.1.9/ckb/core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2024-04-29 09:13:08.000000 pyckb-0.1.9/ckb/denomination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2024-01-22 07:26:45.000000 pyckb-0.1.9/ckb/ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3833 2024-01-22 11:27:41.000000 pyckb-0.1.9/ckb/molecule.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2373 2024-04-23 08:43:17.000000 pyckb-0.1.9/ckb/rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4285 2024-04-26 12:19:31.000000 pyckb-0.1.9/ckb/secp256k1.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23940 2024-04-29 09:14:31.000000 pyckb-0.1.9/ckb/wallet.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/pyckb.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-04-29 09:21:17.000000 pyckb-0.1.9/pyckb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-04-29 09:19:50.000000 pyckb-0.1.9/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-29 09:21:17.949677 pyckb-0.1.9/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 09:21:17.949677 pyckb-0.1.9/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2254 2024-03-21 07:26:46.000000 pyckb-0.1.9/test/test_core.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.1.9/test/test_ecdsa.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1245 2024-04-23 08:21:35.000000 pyckb-0.1.9/test/test_rpc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2024-04-29 09:17:31.000000 pyckb-0.1.9/test/test_wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.690624 pyckb-0.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-12-30 04:14:24.000000 pyckb-0.2.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-05 01:43:59.686623 pyckb-0.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2722 2024-04-10 03:25:41.000000 pyckb-0.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/ckb/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2024-04-29 09:12:52.000000 pyckb-0.2.0/ckb/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4637 2024-04-19 12:01:42.000000 pyckb-0.2.0/ckb/bech32m.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4149 2024-04-26 09:57:50.000000 pyckb-0.2.0/ckb/config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17860 2024-05-05 01:35:59.000000 pyckb-0.2.0/ckb/core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2024-04-29 09:13:08.000000 pyckb-0.2.0/ckb/denomination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1565 2024-05-02 03:14:12.000000 pyckb-0.2.0/ckb/ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2024-05-05 01:36:48.000000 pyckb-0.2.0/ckb/molecule.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2373 2024-04-23 08:43:17.000000 pyckb-0.2.0/ckb/rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2024-04-30 05:58:44.000000 pyckb-0.2.0/ckb/secp256k1.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23980 2024-05-05 01:39:01.000000 pyckb-0.2.0/ckb/wallet.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/pyckb.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4232 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      398 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2024-05-05 01:43:59.000000 pyckb-0.2.0/pyckb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2024-05-05 01:43:14.000000 pyckb-0.2.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-05 01:43:59.690624 pyckb-0.2.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-05 01:43:59.686623 pyckb-0.2.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2237 2024-05-05 01:31:03.000000 pyckb-0.2.0/test/test_core.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      586 2024-01-12 02:25:22.000000 pyckb-0.2.0/test/test_ecdsa.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-05-05 01:28:02.000000 pyckb-0.2.0/test/test_rpc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2024-04-29 09:17:31.000000 pyckb-0.2.0/test/test_wallet.py
```

### Comparing `pyckb-0.1.9/LICENSE` & `pyckb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/PKG-INFO` & `pyckb-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.1.9/README.md` & `pyckb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/ckb/bech32m.py` & `pyckb-0.2.0/ckb/bech32m.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/ckb/config.py` & `pyckb-0.2.0/ckb/config.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/ckb/ecdsa.py` & `pyckb-0.2.0/ckb/ecdsa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ckb.secp256k1
 import itertools
 import random
+import typing
 
 
-def sign(prikey: ckb.secp256k1.Fr, m: ckb.secp256k1.Fr) -> tuple[ckb.secp256k1.Fr, ckb.secp256k1.Fr, int]:
+def sign(prikey: ckb.secp256k1.Fr, m: ckb.secp256k1.Fr) -> typing.Tuple[ckb.secp256k1.Fr, ckb.secp256k1.Fr, int]:
     # https://www.secg.org/sec1-v2.pdf
     # 4.1.3 Signing Operation
     for _ in itertools.repeat(0):
         k = ckb.secp256k1.Fr(random.randint(0, ckb.secp256k1.N - 1))
         R = ckb.secp256k1.G * k
         r = ckb.secp256k1.Fr(R.x.x)
         if r.x == 0:
```

### Comparing `pyckb-0.1.9/ckb/molecule.py` & `pyckb-0.2.0/ckb/molecule.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,105 +66,100 @@
 
 class Byte:
     def __init__(self, data: int):
         assert 0 <= data and data <= 0xff
         self.data = data
 
     def __eq__(self, other):
-        a = self.data == other.data
-        return a
+        return self.data == other.data
+
+    def molecule(self):
+        return bytearray([self.data])
 
     @staticmethod
-    def molecule_read(data: bytearray):
+    def molecule_decode(data: bytearray):
         assert len(data) == 1
         return data[0]
 
     @staticmethod
     def molecule_size():
         return 1
 
-    def molecule(self):
-        return bytearray([self.data])
-
 
 class Byte32:
     def __init__(self, data: bytearray):
         assert len(data) == 32
         self.data = data
 
     def __eq__(self, other):
-        a = self.data == other.data
-        return a
+        return self.data == other.data
+
+    def molecule(self):
+        return self.data
 
     @staticmethod
-    def molecule_read(data: bytearray):
+    def molecule_decode(data: bytearray):
         return data
 
     @staticmethod
     def molecule_size():
         return 32
 
-    def molecule(self):
-        return self.data
-
 
 class Bytes:
     def __init__(self, data: bytearray):
         self.data = data
 
     def __eq__(self, other):
-        a = self.data == other.data
-        return a
-
-    @staticmethod
-    def molecule_read(data: bytearray):
-        l = int.from_bytes(data[:4], 'little')
-        assert l == len(data) - 4
-        return data[4:]
+        return self.data == other.data
 
     def molecule(self):
         r = bytearray()
         r.extend(len(self.data).to_bytes(4, 'little'))
         r.extend(self.data)
         return r
 
+    @staticmethod
+    def molecule_decode(data: bytearray):
+        l = int.from_bytes(data[:4], 'little')
+        assert l == len(data) - 4
+        return data[4:]
+
 
 class U32:
     def __init__(self, data: int):
         assert 0 <= data and data <= 0xffffffff
         self.data = data
 
     def __eq__(self, other):
-        a = self.data == other.data
-        return a
+        return self.data == other.data
+
+    def molecule(self):
+        return self.data.to_bytes(4, 'little')
 
     @staticmethod
-    def molecule_read(data: bytearray):
+    def molecule_decode(data: bytearray):
         return int.from_bytes(data, 'little')
 
     @staticmethod
     def molecule_size():
         return 4
 
-    def molecule(self):
-        return self.data.to_bytes(4, 'little')
-
 
 class U64:
     def __init__(self, data: int):
         assert 0 <= data and data <= 0xffffffffffffffff
         self.data = data
 
     def __eq__(self, other):
-        a = self.data == other.data
-        return a
+        return self.data == other.data
+
+    def molecule(self):
+        return self.data.to_bytes(8, 'little')
 
     @staticmethod
-    def molecule_read(data: bytearray):
+    def molecule_decode(data: bytearray):
         return int.from_bytes(data, 'little')
 
     @staticmethod
     def molecule_size():
         return 8
-
-    def molecule(self):
-        return self.data.to_bytes(8, 'little')
```

### Comparing `pyckb-0.1.9/ckb/rpc.py` & `pyckb-0.2.0/ckb/rpc.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/ckb/secp256k1.py` & `pyckb-0.2.0/ckb/secp256k1.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,18 @@
         self.x = x
         self.y = y
 
     def __repr__(self):
         return f'Pt({self.x}, {self.y})'
 
     def __eq__(self, data):
-        return self.x == data.x and self.y == data.y
+        return all([
+            self.x == data.x,
+            self.y == data.y,
+        ])
 
     def __add__(self, data):
         # https://www.cs.miami.edu/home/burt/learning/Csc609.142/ecdsa-cert.pdf
         # Don Johnson, Alfred Menezes and Scott Vanstone, The Elliptic Curve Digital Signature Algorithm (ECDSA)
         # 4.1 Elliptic Curves Over Fp
         if self.x == Fq(0) and self.y == Fq(0):
             return data
```

### Comparing `pyckb-0.1.9/ckb/wallet.py` & `pyckb-0.2.0/ckb/wallet.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def analyze_mining_fee(self):
         # Make sure the transaction fee is less than 1 CKB. This is a rough check, but works well in most cases.
         sender_capacity = 0
         output_capacity = 0
         for e in self.tx.raw.inputs:
             out_point = e.previous_output
             result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
-            origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
+            origin = ckb.core.CellOutput.json_decode(result['transaction']['outputs'][out_point.index])
             sender_capacity += origin.capacity
         for e in self.tx.raw.outputs:
             output_capacity += e.capacity
         assert sender_capacity - output_capacity <= 1 * ckb.denomination.ckbytes
 
     def analyze_outputs_data(self):
         assert len(self.tx.raw.outputs) == len(self.tx.raw.outputs_data)
@@ -59,27 +59,28 @@
 class Wallet:
     def __init__(self, prikey: int):
         self.prikey = ckb.core.PriKey(prikey)
         self.pubkey = self.prikey.pubkey()
         self.script = ckb.core.Script(
             ckb.config.current.script.secp256k1_blake160.code_hash,
             ckb.config.current.script.secp256k1_blake160.hash_type,
-            ckb.core.hash(self.pubkey.molecule())[:20]
+            ckb.core.hash(self.pubkey.sec())[:20]
         )
         self.addr = ckb.core.address_encode(self.script)
 
     def __repr__(self):
         return json.dumps(self.json())
 
     def __eq__(self, other):
-        a = self.prikey == other.prikey
-        b = self.pubkey == other.pubkey
-        c = self.script == other.script
-        d = self.addr == other.addr
-        return a and b and c and d
+        return all([
+            self.prikey == other.prikey,
+            self.pubkey == other.pubkey,
+            self.script == other.script,
+            self.addr == other.addr,
+        ])
 
     def json(self):
         return {
             'prikey': self.prikey.json(),
             'pubkey': self.pubkey.json(),
             'script': self.script.json(),
             'addr': self.addr,
@@ -108,22 +109,22 @@
         assert self.capacity() > capacity
         sender_capacity = 0
         accept_capacity = capacity
         accept_script = script
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, None))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(bytearray())
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 256):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -143,20 +144,20 @@
 
     def transfer_all(self, script: ckb.core.Script):
         assert self.capacity() > 0
         sender_capacity = 0
         accept_capacity = 0
         accept_script = script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, None))
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 256):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
         accept_capacity = sender_capacity - len(tx.molecule()) - 4
         tx.raw.outputs[0].capacity = accept_capacity
         sign_data = bytearray()
@@ -174,22 +175,22 @@
     def script_deploy(self, script: ckb.core.Script, data: bytearray):
         sender_capacity = 0
         accept_capacity = (61 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, None))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(data)
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 256):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -211,22 +212,22 @@
         sender_capacity = 0
         accept_capacity = (126 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         accept_typeid = ckb.core.Script(ckb.core.type_id_code_hash, ckb.core.type_id_hash_type, bytearray([0] * 32))
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, accept_typeid))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(data)
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 256):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -244,33 +245,33 @@
         tx.witnesses[0] = ckb.core.WitnessArgs(sign, None, None).molecule()
         WalletTransactionAnalyzer(tx).analyze()
         hash = ckb.rpc.send_transaction(tx.json())
         return bytearray.fromhex(hash[2:])
 
     def script_update_type_id(self, script: ckb.core.Script, data: bytearray, out_point: ckb.core.OutPoint):
         result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
-        origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
+        origin = ckb.core.CellOutput.json_decode(result['transaction']['outputs'][out_point.index])
         assert origin.type.code_hash == ckb.core.type_id_code_hash
         assert origin.type.hash_type == ckb.core.type_id_hash_type
         sender_capacity = origin.capacity
         accept_capacity = (126 + len(data)) * ckb.denomination.ckbytes
         accept_script = script
         accept_typeid = origin.type
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
         tx.raw.inputs.append(ckb.core.CellInput(0, out_point))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, accept_typeid))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(data)
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 255):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -299,23 +300,23 @@
             ckb.config.current.script.dao.code_hash,
             ckb.config.current.script.dao.hash_type,
             bytearray()
         )
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.dao.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.dao.cell_dep))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, accept_typeid))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(bytearray([0] * 8))
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 256):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -333,36 +334,36 @@
         hash = ckb.rpc.send_transaction(tx.json())
         return bytearray.fromhex(hash[2:])
 
     def dao_prepare(self, out_point: ckb.core.OutPoint):
         # https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0023-dao-deposit-withdraw/0023-dao-deposit-withdraw.md#withdraw-phase-1
         result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
         number = int(ckb.rpc.get_header(result['tx_status']['block_hash'])['number'], 16)
-        origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
+        origin = ckb.core.CellOutput.json_decode(result['transaction']['outputs'][out_point.index])
         assert origin.type.code_hash == ckb.config.current.script.dao.code_hash
         assert origin.type.hash_type == ckb.config.current.script.dao.hash_type
         assert origin.type.args == bytearray()
         sender_capacity = origin.capacity
         accept_capacity = origin.capacity
         accept_script = origin.lock
         accept_typeid = origin.type
         change_capacity = 0
         change_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.dao.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.dao.cell_dep))
         tx.raw.header_deps.append(bytearray.fromhex(result['tx_status']['block_hash'][2:]))
         tx.raw.inputs.append(ckb.core.CellInput(0, out_point))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, accept_typeid))
         tx.raw.outputs.append(ckb.core.CellOutput(change_capacity, change_script, None))
         tx.raw.outputs_data.append(number.to_bytes(8, 'little'))
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), None, None).molecule())
         for cell in itertools.islice(self.livecell(), 255):
-            cell_out_point = ckb.core.OutPoint.json_read(cell['out_point'])
+            cell_out_point = ckb.core.OutPoint.json_decode(cell['out_point'])
             cell_capacity = int(cell['output']['capacity'], 16)
             cell_input = ckb.core.CellInput(0, cell_out_point)
             sender_capacity += cell_capacity
             tx.raw.inputs.append(cell_input)
             change_capacity = sender_capacity - accept_capacity - len(tx.molecule()) - 4
             if change_capacity >= 61 * ckb.denomination.ckbytes:
                 break
@@ -379,15 +380,15 @@
         WalletTransactionAnalyzer(tx).analyze()
         hash = ckb.rpc.send_transaction(tx.json())
         return bytearray.fromhex(hash[2:])
 
     def dao_extract(self, out_point: ckb.core.OutPoint):
         # https://github.com/nervosnetwork/rfcs/blob/master/rfcs/0023-dao-deposit-withdraw/0023-dao-deposit-withdraw.md#withdraw-phase-2
         result = ckb.rpc.get_transaction('0x' + out_point.tx_hash.hex())
-        origin = ckb.core.CellOutput.json_read(result['transaction']['outputs'][out_point.index])
+        origin = ckb.core.CellOutput.json_decode(result['transaction']['outputs'][out_point.index])
         assert origin.type.code_hash == ckb.config.current.script.dao.code_hash
         assert origin.type.hash_type == ckb.config.current.script.dao.hash_type
         assert origin.type.args == bytearray()
         deposit_block_number_byte = bytearray.fromhex(result['transaction']['outputs_data'][out_point.index][2:])
         deposit_block_number = int.from_bytes(deposit_block_number_byte, 'little')
         deposit_block_header = ckb.rpc.get_header_by_number(hex(deposit_block_number))
         deposit_block_hash = bytearray.fromhex(deposit_block_header['hash'][2:])
@@ -407,16 +408,16 @@
         )
         extract_since = 0x2000000000000000 + extract_since_epoch
         occupy_capacity = 102 * ckb.denomination.ckbytes
         sender_capacity = (origin.capacity - occupy_capacity) * prepare_dao_ar // deposit_dao_ar + occupy_capacity
         accept_capacity = 0
         accept_script = self.script
         tx = ckb.core.Transaction(ckb.core.TransactionRaw(0, [], [], [], [], []), [])
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.secp256k1_blake160.cell_dep))
-        tx.raw.cell_deps.append(ckb.core.CellDep.conf_read(ckb.config.current.script.dao.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.secp256k1_blake160.cell_dep))
+        tx.raw.cell_deps.append(ckb.core.CellDep.conf_decode(ckb.config.current.script.dao.cell_dep))
         tx.raw.header_deps.append(deposit_block_hash)
         tx.raw.header_deps.append(prepare_block_hash)
         tx.raw.inputs.append(ckb.core.CellInput(extract_since, out_point))
         tx.raw.outputs.append(ckb.core.CellOutput(accept_capacity, accept_script, None))
         tx.raw.outputs_data.append(bytearray())
         tx.witnesses.append(ckb.core.WitnessArgs(bytearray([0] * 65), bytearray([0] * 8), None).molecule())
         accept_capacity = sender_capacity - len(tx.molecule()) - 4
```

### Comparing `pyckb-0.1.9/pyckb.egg-info/PKG-INFO` & `pyckb-0.2.0/pyckb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckb
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python SDK for CKB
 Author-email: Mohanson <mohanson@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Mohanson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyckb-0.1.9/test/test_core.py` & `pyckb-0.2.0/test/test_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import ckb
 
 
 def test_addr():
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
-    args = ckb.core.hash(pubkey.molecule())[:20]
+    args = ckb.core.hash(pubkey.sec())[:20]
     script = ckb.core.Script(
         ckb.config.current.script.secp256k1_blake160.code_hash,
         ckb.config.current.script.secp256k1_blake160.hash_type,
         args
     )
     addr = ckb.core.address_encode(script)
     assert addr == 'ckt1qzda0cr08m85hc8jlnfp3zer7xulejywt49kt2rr0vthywaa50xwsqt4z78ng4yutl5u6xsv27ht6q08mhujf8s2r0n40'
     assert ckb.core.address_decode(addr) == script
     assert script.hash().hex() == '0b1bae4beaf456349c63c3ce67491fc75a1276d7f9eedd7ea84d6a77f9f3f5f7'
-    assert ckb.core.Script.molecule_read(script.molecule()) == script
+    assert ckb.core.Script.molecule_decode(script.molecule()) == script
 
 
 def test_epoch():
     assert ckb.core.epoch_decode(0x3690138000093) == (147, 312, 873)
     assert ckb.core.epoch_encode(147, 312, 873) == 0x3690138000093
 
 
 def test_pubkey():
     # Double checked by https://ckb.tools/generator
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
     assert pubkey.x == 0x79be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798
     assert pubkey.y == 0x483ada7726a3c4655da4fbfc0e1108a8fd17b448a68554199c47d08ffb10d4b8
-    assert pubkey.molecule().hex() == '0279be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798'
-    assert ckb.core.PubKey.molecule_read(pubkey.molecule()) == pubkey
+    assert pubkey.sec().hex() == '0279be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798'
+    assert ckb.core.PubKey.sec_decode(pubkey.sec()) == pubkey
 
 
 def test_pubkey_hash():
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
-    assert ckb.core.hash(pubkey.molecule())[:20].hex() == '75178f34549c5fe9cd1a0c57aebd01e7ddf9249e'
+    assert ckb.core.hash(pubkey.sec())[:20].hex() == '75178f34549c5fe9cd1a0c57aebd01e7ddf9249e'
 
 
 def test_script():
     script = ckb.core.Script(
         ckb.config.current.script.secp256k1_blake160.code_hash,
         ckb.config.current.script.secp256k1_blake160.hash_type,
         bytearray([0x00, 0x01, 0x02, 0x03])
     )
-    assert ckb.core.Script.molecule_read(script.molecule()) == script
+    assert ckb.core.Script.molecule_decode(script.molecule()) == script
 
 
 def test_sign():
     prikey = ckb.core.PriKey(1)
     prikey.sign(bytearray.fromhex('9bd7e06f3ecf4be0f2fcd2188b23f1b9fcc88e5d4b65a8637b17723bbda3cce8'))
 
 
 def test_witness_args():
     witness_args = ckb.core.WitnessArgs(
         bytearray([0x00, 0x01, 0x02, 0x03]),
         bytearray([0x00, 0x01, 0x02, 0x03]),
         None,
     )
-    assert ckb.core.WitnessArgs.molecule_read(witness_args.molecule()) == witness_args
+    assert ckb.core.WitnessArgs.molecule_decode(witness_args.molecule()) == witness_args
```

### Comparing `pyckb-0.1.9/test/test_ecdsa.py` & `pyckb-0.2.0/test/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `pyckb-0.1.9/test/test_rpc.py` & `pyckb-0.2.0/test/test_rpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import ckb
 
 
 def test_get_cells():
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
-    args = ckb.core.hash(pubkey.molecule())[:20].hex()
+    args = ckb.core.hash(pubkey.sec())[:20].hex()
     script = ckb.core.Script(
         ckb.config.current.script.secp256k1_blake160.code_hash,
         ckb.config.current.script.secp256k1_blake160.hash_type,
         bytearray.fromhex(args)
     )
     search = {'script': script.json(), 'script_type': 'lock'}
     assert ckb.rpc.get_cells(search, 'asc', '0xff', None)['objects'] != []
 
 
 def test_get_cells_capacity():
     prikey = ckb.core.PriKey(1)
     pubkey = prikey.pubkey()
-    args = ckb.core.hash(pubkey.molecule())[:20].hex()
+    args = ckb.core.hash(pubkey.sec())[:20].hex()
     script = ckb.core.Script(
         ckb.config.current.script.secp256k1_blake160.code_hash,
         ckb.config.current.script.secp256k1_blake160.hash_type,
         bytearray.fromhex(args)
     )
     search = {'script': script.json(), 'script_type': 'lock'}
     assert int(ckb.rpc.get_cells_capacity(search)['capacity'], 16) >= 0
```

### Comparing `pyckb-0.1.9/test/test_wallet.py` & `pyckb-0.2.0/test/test_wallet.py`

 * *Files identical despite different names*

