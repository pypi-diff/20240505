# Comparing `tmp/ec_slp_lib-1.0.4a2.tar.gz` & `tmp/ec_slp_lib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_slp_lib-1.0.4a2.tar", max compression
+gzip compressed data, was "ec_slp_lib-1.0.5.tar", max compression
```

## Comparing `ec_slp_lib-1.0.4a2.tar` & `ec_slp_lib-1.0.5.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     8266 2023-08-30 15:47:04.977748 ec_slp_lib-1.0.4a2/ec_slp_lib.py
--rw-r--r--   0        0        0      514 2023-08-30 15:47:13.209586 ec_slp_lib-1.0.4a2/pyproject.toml
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 ec_slp_lib-1.0.4a2/PKG-INFO
+-rw-r--r--   0        0        0     8314 2024-05-05 09:06:47.936651 ec_slp_lib-1.0.5/ec_slp_lib.py
+-rw-r--r--   0        0        0      512 2024-05-05 09:06:21.465340 ec_slp_lib-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 ec_slp_lib-1.0.5/PKG-INFO
```

### Comparing `ec_slp_lib-1.0.4a2/ec_slp_lib.py` & `ec_slp_lib-1.0.5/ec_slp_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,244 +9,263 @@
 import random
 import subprocess
 import sys
 import configparser
 import os.path
 import requests
 import os
+import logging
+
+logger = logging.getLogger(__name__)
 
 __author__ = "uak"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2024"
 __credits__ = ["uak"]
 __license__ = "LGPL"
-__version__ = "1.0.4a2"
+__version__ = "1.0.5"
 
 
 class EcSLP:
     """EC SLP class
     """
     def set_rpc_port(self, params, rpc):
         """Set rpc port in Electron Cash config file
         """
         with open(params["ec_config"], 'r+') as f:
             data = json.load(f)
-            data["rpcport"] = rpc["port"] # <--- add `id` value. #FIXME
+            data["rpcport"] = rpc["port"]  # <--- add `id` value. #FIXME
             f.seek(0)        # <--- should reset file position to the beginning.
             json.dump(data, f, indent=4)
             f.truncate()     # remove remaining part
-    
-    
-    def subprocessing(self, cmd, params, capture_output=True, text=True, run=False):
-        """Function to run the wallet commads
-        It checks the network specified in the config file then adds the flag accordingly
+
+    def subprocessing(
+        self,
+        cmd,
+        params,
+        capture_output=True,
+        text=True,
+        run=False
+    ):
+        """Function to run the wallet commads, It checks the network
+        specified in the config file then adds the flag accordingly
         """
         if params["network"] in params["network_options"]:
-            cmd = cmd + (f"--{params['network']}", )
-        elif params["network"] == "mainnet":
-            pass
+            if params["network"] != "mainnet":
+                cmd = cmd + (f"--{params['network']}", )
         else:
             exit("No network specified")
         if params.get("use_custom_dir"):
             cmd = cmd + ("--dir", params.get("custom_dir"), )
         cmd = (params["python_path"], params["electron_cash_path"], *cmd)
-        
-        # ~ # Check configruation option super_user is set so it drop privileges
-        # ~ if super_user:
-            # ~ env = os.environ.copy()
-            # ~ env.update({'HOME': home_dir, 'USER': user_name})
-            # ~ return subprocess.check_output(cmd, preexec_fn=demote(os_uid, os_gid), env=env, text=text)
-        # ~ else:
+
         if run:
             try:
                 return subprocess.run(cmd, text=text)
             except Exception as err:
                 raise
         else:
             try:
                 return subprocess.check_output(cmd, text=text)
             except Exception as err:
                 raise
-    
+
+    # ~ # Check configruation option super_user is set so it drop privileges
+    # ~ if super_user:
+        # ~ env = os.environ.copy()
+        # ~ env.update({'HOME': home_dir, 'USER': user_name})
+        # ~ return subprocess.check_output(
+            # ~ cmd,preexec_fn=demote(os_uid, os_gid),
+            # ~ env=env,
+            # ~ text=text
+        # ~ )
+    # ~ else:
+
     # ~ def demote(os_uid, os_gid):
         # ~ """Pass the function 'set_ids' to preexec_fn, rather than just calling
         # ~ setuid and setgid. This will change the ids for that subprocess only"""
-    
+
         # ~ def set_ids():
             # ~ os.setgid(os_gid)
             # ~ os.setuid(os_uid)
-    
+
         # ~ return set_ids
-    
-    
+
     def get_config_data(self, params, config_option):
         """
         Get config data from Electron Cash wallet configuration file.
         """
         cmd = ("getconfig", config_option)
 
         try:
             return self.subprocessing(cmd, params).rstrip()
         except Exception as err:
             raise
 
-
     def set_config_data(self, params, config_option, value):
         """
         Set config data to Electron Cash wallet configuration file.
         """
         cmd = ("setconfig", config_option, value)
-        
+
         try:
             return self.subprocessing(cmd, params).rstrip()
         except Exception as err:
             raise
 
-    
     def ec_rpc(
                 self,
                 rpc,
-                method, 
+                method,
                 *args
                 ):
         """Use JSON-RPC interface to connect to the EC daemon through RPC
         RPC data is provided from `rpc` dictionary object
         """
-    
+
         data = {
-            "id":random.getrandbits(8), #uniqe number required by json specficiations
-            "method":method,
-            "params":[]
+            "id": random.getrandbits(8),  # uniqe number required by json specficiations
+            "method": method,
+            "params": []
            }
-    
+
         params = list(args)
-        data["params"]=params
+        data["params"] = params
         try:
-            response = requests.post(rpc["url"]+":"+str(rpc["port"]), json=data, auth=(rpc["user"], rpc["password"]))
+            response = requests.post(
+                rpc["url"]+":"+str(rpc["port"]),
+                json=data,
+                auth=(
+                    rpc["user"],
+                    rpc["password"]
+                )
+            )
             response.raise_for_status()
             return json.loads(response.text)
         except requests.exceptions.ConnectionError as err:
             raise Exception("RPC Connection Error")
         except requests.exceptions.HTTPError as err:
             raise Exception("RPC Authentication Error")
         except Exception as err:
-            raise
-    
-        
-        
+            raise err
+
     # Check if daemon is connected
     def check_daemon(self, params):
         """Check daemon running
         Checks if Electron Cash daemon is running
         """
         cmd = ("daemon", "status")
         try:
             daemon_status = self.subprocessing(cmd, params)
             json_output = json.loads(daemon_status)
             return "connected" in json_output
-        except ValueError:  # includes simplejson.decoder.JSONDecodeError
-            raise Exception("daemon is not connected")
-
-
-    def start_daemon(self, params, run=True): # use subprocess run instead of checkout to avoid blocking of other commands
+        except Exception as e:
+            logger.debug(f"Exception: {e}")
+            return False
+
+    def start_daemon(self, params, run=True):
+        # use subprocess run instead of checkout to
+        # avoid blocking of other commands
         """Start the daemon process
         """
         cmd = ("daemon", "start")
-        
+
         try:
             return self.subprocessing(cmd, params, run=run)
         except Exception as err:
             raise err
-            # ~ return False
- 
-    def stop_daemon(self, params, run=True): # use subprocess run instead of checkout to avoid blocking of other commands
-        """Start the daemon process
+
+    def stop_daemon(self, params, run=True):
+        """Stop the daemon process
         """
         cmd = ("daemon", "stop")
-        
+
         try:
             return self.subprocessing(cmd, params, run=run)
         except Exception as err:
             raise err
 
     def load_wallet(self, params, wallet_path):
         """Load the wallet file in the daemon
         """
         cmd = ("daemon", "load_wallet", "-w", wallet_path)
         return self.subprocessing(cmd, params)
-    
-    
+
     # Doesn't support multiple loaded wallet
     def check_wallet_loaded(self, params, wallet_path):
         """Check wallet loaded
         Checks if the wallet is loaded in Electron Cash daemon
         """
         cmd = ("daemon", "status")
         daemon_status = self.subprocessing(cmd, params)
         try:
             json_output = json.loads(daemon_status)
             # Check if wallet is loaded and return True or False
             return (wallet_path, True) in json_output["wallets"].items()
-        except:
-            raise Exception("wallet not loaded")
+        except Exception as e:
+            raise e
 
     # RPC section
 
     def validate_address(self, rpc, address):
         """Validate Address"""
         return self.ec_rpc(rpc, "validateaddress", address)["result"]
-    
+
     def get_unused_bch_address(self, rpc):
         """Get unused BCH address"""
         return self.ec_rpc(rpc, "getunusedaddress")["result"]
-    
-    
+
     def get_unused_slp_address(self, rpc):
         """Get unused SLP address"""
         return self.ec_rpc(rpc, "getunusedaddress_slp")["result"]
-    
-    
+
     def get_bch_balance(self, rpc):
         """Get the total BCH balance in wallet"""
         return self.ec_rpc(rpc, "getbalance")["result"]
-    
-    
+
     def get_address_balance_bch(self, rpc, address):
         """Get the balance of a BCH address"""
-        return self.ec_rpc(rpc, "getaddressbalance",address)["result"]
-    
-    
+        return self.ec_rpc(rpc, "getaddressbalance", address)["result"]
+
     def get_token_balance(self, rpc, token_id_hex):
         """Get the balance of a SLP token in wallet"""
         return self.ec_rpc(rpc, "getbalance_slp", token_id_hex)["result"]
-    
-    
+
     def prepare_bch_transaction(self, rpc, address, bch_amount):
         """Prepare transaction
         Creates the raw transaction data
         """
         try:
             return self.ec_rpc(rpc, "payto", address, bch_amount)["result"]
-        except:
-            raise Exception("Unable to prepare transaction!")
-    
-    
-    def prepare_slp_transaction(self, rpc, token_id_hex, address_slp, token_amount):
+        except Exception as e:
+            raise e
+
+    def prepare_slp_transaction(
+        self,
+        rpc,
+        token_id_hex,
+        address_slp,
+        token_amount
+    ):
         """Prepare SLP transaction
         Creates the raw SLP transaction data
         """
-        return self.ec_rpc(rpc, "payto_slp", token_id_hex, address_slp, token_amount)["result"]
-    
+        return self.ec_rpc(
+            rpc,
+            "payto_slp",
+            token_id_hex,
+            address_slp,
+            token_amount
+            )["result"]
 
     def broadcast_tx(self, rpc, tx_hex):
         """Broadcast transaction
         Send the transaction to the network
         """
         if int(tx_hex, 16):
             return self.ec_rpc(rpc, "broadcast", tx_hex)["result"]
         else:
             raise Exception("error in hex string")
- 
-    
+
     def freeze_address(self, rpc, address):
         """Freeze an address so it can not be used later
         """
         return self.ec_rpc(rpc, "freeze", address)["result"]
```

### Comparing `ec_slp_lib-1.0.4a2/pyproject.toml` & `ec_slp_lib-1.0.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ec_slp_lib"
-version = "1.0.4a2"
+version = "1.0.5"
 description = "Wrapper for Electron Cash commands based on its CLI and RPC commands"
 authors = ["uak <4626956-uak@users.noreply.gitlab.com>"]
 license = "LGPLv3+"
 repository = "https://gitlab.com/uak/electron-cash-slp-basic-lib"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ec_slp_lib-1.0.4a2/PKG-INFO` & `ec_slp_lib-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: ec-slp-lib
-Version: 1.0.4a2
+Name: ec_slp_lib
+Version: 1.0.5
 Summary: Wrapper for Electron Cash commands based on its CLI and RPC commands
 Home-page: https://gitlab.com/uak/electron-cash-slp-basic-lib
 License: LGPLv3+
 Author: uak
 Author-email: 4626956-uak@users.noreply.gitlab.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Project-URL: Repository, https://gitlab.com/uak/electron-cash-slp-basic-lib
```

