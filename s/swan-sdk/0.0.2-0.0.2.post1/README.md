# Comparing `tmp/swan_sdk-0.0.2.tar.gz` & `tmp/swan_sdk-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swan_sdk-0.0.2.tar", last modified: Fri May  3 21:17:38 2024, max compression
+gzip compressed data, was "swan_sdk-0.0.2.post1.tar", last modified: Sun May  5 21:27:20 2024, max compression
```

## Comparing `swan_sdk-0.0.2.tar` & `swan_sdk-0.0.2.post1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.700455 swan_sdk-0.0.2/
--rw-r--r--   0 zihangchen   (501) staff       (20)     1072 2024-04-27 21:10:50.000000 swan_sdk-0.0.2/LICENSE
--rw-r--r--   0 zihangchen   (501) staff       (20)       32 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/MANIFEST.in
--rw-r--r--   0 zihangchen   (501) staff       (20)     8723 2024-05-03 21:17:38.700163 swan_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)     8184 2024-05-03 21:00:50.000000 swan_sdk-0.0.2/README.md
--rw-r--r--   0 zihangchen   (501) staff       (20)       38 2024-05-03 21:17:38.700505 swan_sdk-0.0.2/setup.cfg
--rw-------   0 zihangchen   (501) staff       (20)     1187 2024-05-03 21:17:23.000000 swan_sdk-0.0.2/setup.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.693312 swan_sdk-0.0.2/swan/
--rw-r--r--   0 zihangchen   (501) staff       (20)      151 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/__init__.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.693920 swan_sdk-0.0.2/swan/api/
--rw-r--r--   0 zihangchen   (501) staff       (20)       25 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/api/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)    12210 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/api/swan_api.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     4279 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/api_client.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.696026 swan_sdk-0.0.2/swan/common/
--rw-r--r--   0 zihangchen   (501) staff       (20)       27 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      922 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/constant.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      327 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/exception.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      447 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/common/file.py
--rw-r--r--   0 zihangchen   (501) staff       (20)       26 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/common/params.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     3256 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/common/utils.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.696565 swan_sdk-0.0.2/swan/contract/
--rw-r--r--   0 zihangchen   (501) staff       (20)       29 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/__init__.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.698196 swan_sdk-0.0.2/swan/contract/abi/
--rw-r--r--   0 zihangchen   (501) staff       (20)     9074 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/ClientPayment.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     9742 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/PaymentContract.json
--rw-r--r--   0 zihangchen   (501) staff       (20)     8855 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/SwanToken.json
--rw-r--r--   0 zihangchen   (501) staff       (20)       33 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/abi/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     8797 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/contract/swan_contract.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.698813 swan_sdk-0.0.2/swan/object/
--rw-r--r--   0 zihangchen   (501) staff       (20)      111 2024-05-03 20:01:42.000000 swan_sdk-0.0.2/swan/object/__init__.py
--rw-r--r--   0 zihangchen   (501) staff       (20)      844 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/object/cp_config.py
--rw-r--r--   0 zihangchen   (501) staff       (20)     1198 2024-04-27 18:03:06.000000 swan_sdk-0.0.2/swan/object/task.py
-drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-03 21:17:38.699834 swan_sdk-0.0.2/swan_sdk.egg-info/
--rw-r--r--   0 zihangchen   (501) staff       (20)     8723 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zihangchen   (501) staff       (20)      676 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        1 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)       69 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/requires.txt
--rw-r--r--   0 zihangchen   (501) staff       (20)        5 2024-05-03 21:17:38.000000 swan_sdk-0.0.2/swan_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.281707 swan_sdk-0.0.2.post1/
+-rw-r--r--   0 zihangchen   (501) staff       (20)     1072 2024-04-27 21:10:50.000000 swan_sdk-0.0.2.post1/LICENSE
+-rw-r--r--   0 zihangchen   (501) staff       (20)       32 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/MANIFEST.in
+-rw-r--r--   0 zihangchen   (501) staff       (20)    10936 2024-05-05 21:27:20.281433 swan_sdk-0.0.2.post1/PKG-INFO
+-rw-r--r--   0 zihangchen   (501) staff       (20)    10391 2024-05-05 21:22:01.000000 swan_sdk-0.0.2.post1/README.md
+-rw-r--r--   0 zihangchen   (501) staff       (20)       38 2024-05-05 21:27:20.281756 swan_sdk-0.0.2.post1/setup.cfg
+-rw-------   0 zihangchen   (501) staff       (20)     1085 2024-05-05 21:23:00.000000 swan_sdk-0.0.2.post1/setup.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.275225 swan_sdk-0.0.2.post1/swan/
+-rw-r--r--   0 zihangchen   (501) staff       (20)      151 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/__init__.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.275874 swan_sdk-0.0.2.post1/swan/api/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       25 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/api/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)    12230 2024-05-05 13:56:09.000000 swan_sdk-0.0.2.post1/swan/api/swan_api.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     4279 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/api_client.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.277801 swan_sdk-0.0.2.post1/swan/common/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       27 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      922 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/constant.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      327 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/exception.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      447 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/common/file.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)       26 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/common/params.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     3256 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/common/utils.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.278228 swan_sdk-0.0.2.post1/swan/contract/
+-rw-r--r--   0 zihangchen   (501) staff       (20)       29 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/__init__.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.279631 swan_sdk-0.0.2.post1/swan/contract/abi/
+-rw-r--r--   0 zihangchen   (501) staff       (20)     9074 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/ClientPayment.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)     9742 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/PaymentContract.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8855 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/SwanToken.json
+-rw-r--r--   0 zihangchen   (501) staff       (20)       33 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/contract/abi/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     8789 2024-05-05 21:22:01.000000 swan_sdk-0.0.2.post1/swan/contract/swan_contract.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.280131 swan_sdk-0.0.2.post1/swan/object/
+-rw-r--r--   0 zihangchen   (501) staff       (20)      111 2024-05-03 20:01:42.000000 swan_sdk-0.0.2.post1/swan/object/__init__.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)      844 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/object/cp_config.py
+-rw-r--r--   0 zihangchen   (501) staff       (20)     1198 2024-04-27 18:03:06.000000 swan_sdk-0.0.2.post1/swan/object/task.py
+drwxr-xr-x   0 zihangchen   (501) staff       (20)        0 2024-05-05 21:27:20.281098 swan_sdk-0.0.2.post1/swan_sdk.egg-info/
+-rw-r--r--   0 zihangchen   (501) staff       (20)    10936 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zihangchen   (501) staff       (20)      676 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)        1 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)       69 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/requires.txt
+-rw-r--r--   0 zihangchen   (501) staff       (20)        5 2024-05-05 21:27:20.000000 swan_sdk-0.0.2.post1/swan_sdk.egg-info/top_level.txt
```

### Comparing `swan_sdk-0.0.2/LICENSE` & `swan_sdk-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/PKG-INFO` & `swan_sdk-0.0.2.post1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swan-sdk
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: A python developer tool kit for Swan Orchestrator services.
 Home-page: https://github.com/swanchain/orchestrator-sdk
 Author: SwanCloud
 Author-email: swan.development@nbai.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,192 +17,225 @@
 
 # PYTHON SWAN SDK
 
 [![Made by FilSwan](https://img.shields.io/badge/made%20by-FilSwan-green.svg)](https://www.filswan.com/) 
 [![Chat on discord](https://img.shields.io/badge/join%20-discord-brightgreen.svg)](https://discord.com/invite/swanchain)
 
 ## Table Of Contents
+
 - [Overview](#overview)
 - [Features](#features)
 - [Installation](#installation)
 - [Use Python dotenv (Optional)](#use-python-dotenv)
 - [Quick Guide](#quick-start-guide-sdk-v2)
-    1. [Get SwanHub API Key](#1-get-swanhub-api-key)
-    2. [Login to SwanHub](#2-login-into-swanhub-through-sdk)
-    3. [Use Swan Payment Contract](#3-connect-to-swan-payment-contract)
-    4. [Retrieve CP Hardware Info](#4-retrieve-avaliable-hardware-informaitons)
-    5. [Get Job Source URI](#5-get-job_source_uri)
-    6. [Esitmate Task Payment](#6-esitmate-payment-amount)
-    7. [Create Task](#7-create-task)
-    8. [Submit Payment](#8-submit-payment)
-    9. [Validate Payment and Delpoy Task](#9-validate-payment-to-deploy-task)
-    10. [Follow Up Deployed Task Status (Optional)](#10-follow-up-task-status-optional)
-- [Executale Example](#examples)
+  1. [Get Orchestrator API Key](#1-get-orchestrator-api-key)
+  2. [Login to Orchestrator](#2-login-into-Orchestrator-through-sdk)
+  3. [Use Swan Payment Contract](#3-connect-to-swan-payment-contract)
+  4. [Retrieve CP Hardware Info](#4-retrieve-available-hardware-information)
+  5. [Get Job Source URI](#5-get-job_source_uri)
+  6. [Esitmate Task Payment](#6-esitmate-payment-amount)
+  7. [Create Task](#7-create-task)
+  8. [Submit Payment](#8-submit-payment)
+  9. [Validate Payment and Deploy Task](#9-validate-payment-to-deploy-task)
+  10. [Follow-Up Deployed Task Status (Optional)](#10-follow-up-task-status-optional)
+- [Executable Example](#examples)
 - [Documentation](#documentation)
 - [Contribution](#contributions)
 - [License](#license)
 
 ## Overview
 
 The PYTHON SWAN SDK is a comprehensive toolkit designed to facilitate seamless interactions with the SwanChain API. Tailored for developers, this SDK simplifies the creation and management of computational tasks (CP tasks), making it an indispensable tool for developers working in various tech domains.
 
-GitHub Link: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2
+GitHub Link: https://github.com/swanchain/python-swan-sdk/tree/main
 
 ## Features
 
 - **API Client Integration**: Streamline your development workflow with our intuitive API client.
 - **Pre-defined Data Models**: Utilize our structured data models for tasks, directories, and source URIs to enhance your application's reliability and scalability.
 - **Service Layer Abstractions**: Access complex functionalities through a simplified high-level interface, improving code maintainability.
-- **Extensive Documentation**: Access a wealth of information through our comprehensive guides and reference materials located in the `docs/` directory on Github.
+- **Extensive Documentation**: Access a wealth of information through our comprehensive guides and reference materials located in the `docs/` directory on GitHub.
 
 ## Installation
 
 Setting up the PYTHON SWAN SDK is straightforward.
 
-To use Python Swan SDK, use Python 3.8 or later. Earlier versions are not supported.
+To use Python Swan SDK, use **Python 3.8 or later** and **web3.py 6.15 or later**. Earlier versions are not supported.
 
-**Install via PyPI testnet:**
+**Install via PyPI:**
 
 ```bash
 pip install swan-sdk==0.0.2
 ```
 
 **Clone from GitHub:**
 
 ```bash
 git clone https://github.com/swanchain/orchestrator-sdk.git
-git checkout release/v0.0.2
+git checkout release/v0.0.2-1
 ```
 
 ## Use Python dotenv
-It is recommanded to store your important person information in configuration or as environmental variables. Python dotenv allows loading environment variable from `.env` files for easier access and better security.
+
+It is recommended to store your important personal information in configuration or as environmental variables. Python dotenv allows loading environment variables from `.env` files for easier access and better security.
 
 python-dotenv package: https://pypi.org/project/python-dotenv/ \
-Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/docs/configuration.md
+Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2-1/docs/configuration.md
 
 ## Quick Start Guide for Swan SDK
+
 Jump into using the SDK with this quick example:
 
-### 1. Get SwanHub API Key
+### 1. Get Orchestrator API Key
 
-To use `swan-sdk` SwanHub API key is required. 
-- Go to Swan Dashboard: https://orchestrator.swanchain.io/provider-status
+To use `swan-sdk`, an Orchestrator API key is required. 
+
+- Go to Orchestrator Dashboard: https://orchestrator.swanchain.io/provider-status
 - Login through MetaMask.
-- Click the user icon on top right.
+- Click the user icon on the top right.
 - Click 'Show API-Key' -> 'New API Key'
 - Store your API Key safely, do not share with others.
 
-### 2. Login into SwanHub Through SDK
+### 2. Login into Orchestrator Through SDK
 
-To use `swan-sdk` you will need to login to SwanHub using API Key. (Wallet login is not supported)
+To use `swan-sdk` you will need to login to Orchestrator using API Key. (Wallet login is not supported)
 
 ```python
 from swan import SwanAPI
 
 swan_api = SwanAPI(api_key="<your_api_key>")
 ```
-
 ### 3. Connect to Swan Payment Contract
 
-Payment of SwanHub deployment is paid through Swan Payment Contract. To navigate the contract ABIs. First create a `SwanContract()` instance:
+Payment of Orchestrator deployment is paid through the Swan Payment Contract. To navigate the contract ABIs. First create a `SwanContract()` instance:
+**Notice: This won't be used until you're trying to Estimate Payment Amount, however, it's still recommended to do this step here to make sure that you can get all contract information before you move on**
+
 ```python
 from swan.contract.swan_contract import SwanContract
 
 contract = SwanContract('<your_private_key>', swan_api.contract_info)
 ```
 
-### 4. Retrieve Avaliable Hardware Informaitons
 
-SwanHub provides selection of Computing Providers with different hardwares.
-Use `SwanAPI().get_hardware_config()` to retrieve all avaliable hardwares on SwanHub.
+### 4. Retrieve available hardware information
+
+Orchestrator provides a selection of Computing Providers with different hardware.
+Use `SwanAPI().get_hardware_config()` to retrieve all available hardware on Orchestrator.
+
+Each hardware is stored as an instance of `HardwareConfig()` object. 
 
-Each hardware is stored in `HardwareConfig()` object.
 ```python
 from swan.object import HardwareConfig
 ```
+Hardware config contains a unique hardware ID, hardware name, description, hardware type (CPU/GPU), price per hour, available region and current status.
 
-Hardware config contains an unique hardware ID, hardware name, description, hardware type (CPU/GPU), price per hour, avaliable region and current status.
+See all available hardware in a Python dictionary:
 
-See all avaliable hardware in a python dictionary:
 ```python
-
 hardwares = swan_api.get_hardware_config()
 hardwares_info = [hardware.to_dict() for hardware in hardwares if hardware.status == "available"] 
-hardwares_info
+print(hardwares_info)
+```
+You can use 
+```python
+from swan.object import HardwareConfig
+```
+to check the hardware information like this:
+- `HardwareConfig().status` shows the availability of the hardware.
+- `HardwareConfig().region` is a list of all regions this hardware is available in.
+- Retrieve individual hardware attributes:
+```python
+print(chosen_hardware.id) # hardware id
+print(chosen_hardware.name) # hardware name
+print(chosen_hardware.description) # hardware description
+print(chosen_hardware.type) # hardware type
+print(chosen_hardware.region) # all avaliable hardware region
+print(chosen_hardware.price) # current hardware price
+print(chosen_hardware.status) # overall hardware avaliablility
 ```
-`HardwareConfig().status` shows the avalibility of the hardware.
-`HardwareConfig().region` is a list of all region this hardware is avaliable in.
 
-Retrieve the hardware with hardware id 0:
+More detials go oject documentation: https://github.com/swanchain/python-swan-sdk/blob/release/v0.0.2.post1/docs/object.md
+
+Useful example: Retrieve the hardware with hardware ID 0:
 ```python
 hardwares = swan_api.get_hardware_config()
-chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0]
-chosen_hardware.to_dict()
+chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0][0]
+print(chosen_hardware.to_dict())
 ```
 
 Sample output:
+
 ```
 {'id': 0,
  'name': 'C1ae.small',
  'description': 'CPU only · 2 vCPU · 2 GiB',
  'type': 'CPU',
  'reigion': ['North Carolina-US', ...],
  'price': '0.0',
  'status': 'available'
 }
 ```
 
+
 ### 5. Get job_source_uri
 
 `job_source_uri` can be create through `SwanAPI().get_source_uri()` API.
 
 Generate a source URI
 A demo tetris docker image on GitHub as repo_uri: 'https://github.com/alphaflows/tetris-docker-image.git'
+
 ```python
 job_source_uri = swan_api.get_source_uri(
     repo_uri='<your_git_hub_link/your_lagrange_space_link>',
     hardware_id=chosen_hardware.id,
     wallet_address='<your_wallet_address>'
 )
 
 job_source_uri = job_source_uri['data']['job_source_uri']
+print(job_source_uri)
 ```
 
-### 6. Esitmate Payment Amount
+### 6. Estimate Payment Amount
+
 To estimate the payment required for the deployment. Use `SwanContract().estiamte_payment()`
+
 ```python
 duration_hour = 1 # or duration you want the deployment to run
 amount = contract.estimate_payment(chosen_hardware.id, duration_hour)
-amount # amount is in wei, 18 decimals
+print(amount) # amount is in wei, 18 decimals
 ```
 
 ### 7. Create Task
 
-Before paying for the task. First create a task on SwanHub using desired task attributes.
+Before paying for the task. First, create a task on Orchestrator using desired task attributes.
+
 ```python
 import json
 
+duration_hour = 1
+# Notice that from here, you need to convert the duration to seconds
 duration = 3600*duration_hour
 cfg_name = chosen_hardware.name
 
 result = swan_api.create_task(
     cfg_name=cfg_name, 
-    region='<region_name>', 
+    region='<region_name>', # e.g. 'North Carolina-US' or chosen_hardware.region[0]
     start_in=300,  # in seconds
     duration=duration, 
     job_source_uri=job_source_uri, #repo.source_uri
     paid=contract._wei_to_swan(amount), # from wei to swan amount/1e18
     wallet_address='<your_wallet_address>',
 )
 task_uuid = result['data']['task']['uuid']
 
 print(json.dumps(result, indent=2)) # Print response
 ```
 
 Sample output:
+
 ```
 {
   "data": {
     "task": {
       "created_at": "1714254304",
       "end_at": "1714257898",
       "leading_job_id": null,
@@ -215,46 +248,89 @@
     }
   },
   "message": "Task_uuid initialized.",
   "status": "success"
 }
 ```
 
-The `task['uuid']` will be used in following operations.
+**The `task['uuid']` will be used in the following operations.**
+
+
 
 ### 8. Submit Payment
 
+- **If you got error about insufficient balance, please make sure you have enough balance in your wallet.**
+- *If you have Error like "to_wei() does not exist", please make sure you have web3.py 6.15 or later.*
+
 Use `SwanContract().submit_payment()` to pay for the task. The TX hash is the receipt for the payment.
+
 ```python
-tx_hash = contract.submit_payment(task_uuid, hardware_id, duration)
+tx_hash = contract.submit_payment(task_uuid, chosen_hardware.id, duration) # duration in seconds
 ```
 
 ### 9. Validate Payment to Deploy Task
 
 Use `SwanAPI().validate_payment()` to validate the payment using TX hash and deploy the task.
+
 ```python
 swan_api.validate_payment(
     tx_hash=tx_hash,
     task_uuid=task_uuid
 )
 ```
 
-### 10. Follow up Task Status (Optional)
+### 10. Follow-up Task Status (Optional)
 
 #### Show results
 
-Get the deploy URI to test your task deployment using `SwanAPI().get_real_uri()`.
+Get the deploy URI to test your deployed task using `SwanAPI().get_real_uri()`.
+
 ```python
 r = swan_api.get_real_url(task_uuid)
 print(r)
 ```
 
+#### Show task details
+Get the task details using `SwanAPI().get_deployment_info()`.
+
+```python
+r = swan_api.get_deployment_info(task_uuid)
+print(r)
+```
+Simple output
+```
+{
+   "data":{
+      "computing_providers":[
+         
+      ],
+      "jobs":[
+         
+      ],
+      "task":{
+         "created_at":"1714877536",
+         "end_at":"1714881125",
+         "leading_job_id":"None",
+         "refund_amount":"None",
+         "status":"accepting_bids",
+         "task_detail_cid":"task_detail_cid",
+         "tx_hash":"None",
+         "updated_at":"1714877801",
+         "uuid":"204cd1be-30b0-4915-a635-4b9dbf1a3b5e"
+      }
+   },
+   "message":"fetch task info for task_uuid='204cd1be-30b0-4915-a635-4b9dbf1a3b5e' successfully",
+   "status":"success"
+}
+```
+
+
 ## Examples
-For executable examples consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/examples
+For executable examples consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2.post1/examples
 
 ## Documentation
 
-For comprehensive documentation, including detailed installation guides, usage examples, and complete API references, please consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/docs
+For comprehensive documentation, including detailed installation guides, usage examples, and complete API references, please consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2.post1/docs
 
 ## License
 
 The PYTHON SWAN SDK is released under the **MIT** license, details of which can be found in the LICENSE file.
```

### Comparing `swan_sdk-0.0.2/setup.py` & `swan_sdk-0.0.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-        name="swan-sdk",
-        version="0.0.2",
-        packages=['swan', 'swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
-        # package_data={'swan.contract.abi': ['swan/contract/abi/PaymentContract.json', 'swan/contract/abi/SwanToken.json']},
-        include_package_data=True,
-        description="A python developer tool kit for Swan Orchestrator services.",
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        url="https://github.com/swanchain/orchestrator-sdk",
-        author="SwanCloud",
-        author_email="swan.development@nbai.io",
-        license="MIT",
-        classifiers=[
-            "License :: OSI Approved :: MIT License",
-            "Programming Language :: Python :: 3",
+    name="swan-sdk",
+    version="0.0.2.post1",
+    packages=['swan', 'swan.api', 'swan.common', 'swan.contract', 'swan.object', 'swan.contract.abi'],
+    # package_data={'swan.contract.abi': ['swan/contract/abi/PaymentContract.json', 'swan/contract/abi/SwanToken.json']},
+    include_package_data=True,
+    description="A python developer tool kit for Swan Orchestrator services.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/swanchain/orchestrator-sdk",
+    author="SwanCloud",
+    author_email="swan.development@nbai.io",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+    ],
+    install_requires=[
+        "requests==2.28.1",
+        "requests-toolbelt==0.10.1",
+        "web3==6.15.1",
+        "tqdm==4.64.1"
         ],
-        install_requires=[
-            "requests==2.28.1",
-            "requests-toolbelt==0.10.1",
-            "web3==6.15.1",
-            "tqdm==4.64.1"
-            ],
-        entry_points={
-            # placeholder
-        },
-        )
+    entry_points={
+        # placeholder
+    },
+)
```

### Comparing `swan_sdk-0.0.2/swan/api/swan_api.py` & `swan_sdk-0.0.2.post1/swan/api/swan_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 class SwanAPI(APIClient):
   
     def __init__(self, api_key: str, login: bool = True, environment: str = None, verification: bool = True):
         """Initialize user configuration and login.
 
         Args:
-            api_key: SwanHub API key, generated through website
-            login: Login into Swanhub or Not
+            api_key: Orchestrator API key, generated through website
+            login: Login into Orchestrator or Not
             environment: Selected server 'production/calibration'
         """
         self.token = None
         self.api_key = api_key
         self.contract_info = None
         self.environment = environment
         if environment == None:
@@ -29,18 +29,18 @@
         else:
             self.swan_url = environment
         if login:
             self.api_key_login()
             self.get_contract_info(verification)
 
     def api_key_login(self):
-        """Login with SwanHub API Key.
+        """Login with Orchestrator API Key.
 
         Returns:
-            A str access token for further SwanHub API access in
+            A str access token for further Orchestrator API access in
             current session.
         """
         params = {"api_key": self.api_key}
         try:
             result = self._request_with_params(
                 POST, SWAN_APIKEY_LOGIN, self.swan_url, params, None, None
             )
```

### Comparing `swan_sdk-0.0.2/swan/api_client.py` & `swan_sdk-0.0.2.post1/swan/api_client.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/common/constant.py` & `swan_sdk-0.0.2.post1/swan/common/constant.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/common/utils.py` & `swan_sdk-0.0.2.post1/swan/common/utils.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/contract/abi/ClientPayment.json` & `swan_sdk-0.0.2.post1/swan/contract/abi/ClientPayment.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/contract/abi/PaymentContract.json` & `swan_sdk-0.0.2.post1/swan/contract/abi/PaymentContract.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/contract/abi/SwanToken.json` & `swan_sdk-0.0.2.post1/swan/contract/abi/SwanToken.json`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/contract/swan_contract.py` & `swan_sdk-0.0.2.post1/swan/contract/swan_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             hardware_id=hardware_id, 
             duration=duration/3600  # duration in estimate_
         ))
         self._approve_payment(amount)
 
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.client_contract.functions.submitPayment(
             task_uuid, 
             hardware_id, 
             duration
@@ -110,27 +110,27 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.to_hex(tx_hash)
+        return self.w3.toHex(tx_hash)
     
 
     def _approve_payment(self, amount):
         """
         called in submit_payment
 
         Args:
             amount: amount in wei
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.token_contract.functions.approve(
             self.client_contract.address,
             amount
         ).build_transaction({
@@ -138,24 +138,24 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.to_hex(tx_hash)
+        return self.w3.toHex(tx_hash)
     
 
     def lock_revenue(self, task_id: str, hardware_id: int, duration: int):
         """
         deprecated
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.payment_contract.functions.lockRevenue(
             task_id, 
             hardware_id, 
             duration
@@ -164,23 +164,23 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.to_hex(tx_hash)
+        return self.w3.toHex(tx_hash)
     
     def _approve_swan_token(self, amount):
         """
         deprecated
         """
         nonce = self.w3.eth.get_transaction_count(self.account.address)
         base_fee = self.w3.eth.get_block('latest')['baseFeePerGas']
-        max_priority_fee_per_gas = self.w3.to_wei(2, 'gwei')
+        max_priority_fee_per_gas = self.w3.toWei(2, 'gwei')
         max_fee_per_gas = base_fee + max_priority_fee_per_gas
         if max_fee_per_gas < max_priority_fee_per_gas:
             max_fee_per_gas = max_priority_fee_per_gas + base_fee
         tx = self.token_contract.functions.approve(
             self.payment_contract.address, 
             amount
         ).build_transaction({
@@ -188,15 +188,15 @@
             'nonce': nonce,
             "maxFeePerGas": max_fee_per_gas,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
         })
         signed_tx = self.w3.eth.account.sign_transaction(tx, self.account._private_key)
         tx_hash = self.w3.eth.send_raw_transaction(signed_tx.rawTransaction)
         self.w3.eth.wait_for_transaction_receipt(tx_hash, timeout=CONTRACT_TIMEOUT)
-        return self.w3.to_hex(tx_hash)
+        return self.w3.toHex(tx_hash)
     
     def _get_swan_balance(self, address=None):
         """Retrieve swan token balance of any wallet from Swan token contract.
 
         Args:
             address: wallet address to check balance. If None, retrieve own token balance.
```

### Comparing `swan_sdk-0.0.2/swan/object/cp_config.py` & `swan_sdk-0.0.2.post1/swan/object/cp_config.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan/object/task.py` & `swan_sdk-0.0.2.post1/swan/object/task.py`

 * *Files identical despite different names*

### Comparing `swan_sdk-0.0.2/swan_sdk.egg-info/PKG-INFO` & `swan_sdk-0.0.2.post1/swan_sdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swan-sdk
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: A python developer tool kit for Swan Orchestrator services.
 Home-page: https://github.com/swanchain/orchestrator-sdk
 Author: SwanCloud
 Author-email: swan.development@nbai.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,192 +17,225 @@
 
 # PYTHON SWAN SDK
 
 [![Made by FilSwan](https://img.shields.io/badge/made%20by-FilSwan-green.svg)](https://www.filswan.com/) 
 [![Chat on discord](https://img.shields.io/badge/join%20-discord-brightgreen.svg)](https://discord.com/invite/swanchain)
 
 ## Table Of Contents
+
 - [Overview](#overview)
 - [Features](#features)
 - [Installation](#installation)
 - [Use Python dotenv (Optional)](#use-python-dotenv)
 - [Quick Guide](#quick-start-guide-sdk-v2)
-    1. [Get SwanHub API Key](#1-get-swanhub-api-key)
-    2. [Login to SwanHub](#2-login-into-swanhub-through-sdk)
-    3. [Use Swan Payment Contract](#3-connect-to-swan-payment-contract)
-    4. [Retrieve CP Hardware Info](#4-retrieve-avaliable-hardware-informaitons)
-    5. [Get Job Source URI](#5-get-job_source_uri)
-    6. [Esitmate Task Payment](#6-esitmate-payment-amount)
-    7. [Create Task](#7-create-task)
-    8. [Submit Payment](#8-submit-payment)
-    9. [Validate Payment and Delpoy Task](#9-validate-payment-to-deploy-task)
-    10. [Follow Up Deployed Task Status (Optional)](#10-follow-up-task-status-optional)
-- [Executale Example](#examples)
+  1. [Get Orchestrator API Key](#1-get-orchestrator-api-key)
+  2. [Login to Orchestrator](#2-login-into-Orchestrator-through-sdk)
+  3. [Use Swan Payment Contract](#3-connect-to-swan-payment-contract)
+  4. [Retrieve CP Hardware Info](#4-retrieve-available-hardware-information)
+  5. [Get Job Source URI](#5-get-job_source_uri)
+  6. [Esitmate Task Payment](#6-esitmate-payment-amount)
+  7. [Create Task](#7-create-task)
+  8. [Submit Payment](#8-submit-payment)
+  9. [Validate Payment and Deploy Task](#9-validate-payment-to-deploy-task)
+  10. [Follow-Up Deployed Task Status (Optional)](#10-follow-up-task-status-optional)
+- [Executable Example](#examples)
 - [Documentation](#documentation)
 - [Contribution](#contributions)
 - [License](#license)
 
 ## Overview
 
 The PYTHON SWAN SDK is a comprehensive toolkit designed to facilitate seamless interactions with the SwanChain API. Tailored for developers, this SDK simplifies the creation and management of computational tasks (CP tasks), making it an indispensable tool for developers working in various tech domains.
 
-GitHub Link: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2
+GitHub Link: https://github.com/swanchain/python-swan-sdk/tree/main
 
 ## Features
 
 - **API Client Integration**: Streamline your development workflow with our intuitive API client.
 - **Pre-defined Data Models**: Utilize our structured data models for tasks, directories, and source URIs to enhance your application's reliability and scalability.
 - **Service Layer Abstractions**: Access complex functionalities through a simplified high-level interface, improving code maintainability.
-- **Extensive Documentation**: Access a wealth of information through our comprehensive guides and reference materials located in the `docs/` directory on Github.
+- **Extensive Documentation**: Access a wealth of information through our comprehensive guides and reference materials located in the `docs/` directory on GitHub.
 
 ## Installation
 
 Setting up the PYTHON SWAN SDK is straightforward.
 
-To use Python Swan SDK, use Python 3.8 or later. Earlier versions are not supported.
+To use Python Swan SDK, use **Python 3.8 or later** and **web3.py 6.15 or later**. Earlier versions are not supported.
 
-**Install via PyPI testnet:**
+**Install via PyPI:**
 
 ```bash
 pip install swan-sdk==0.0.2
 ```
 
 **Clone from GitHub:**
 
 ```bash
 git clone https://github.com/swanchain/orchestrator-sdk.git
-git checkout release/v0.0.2
+git checkout release/v0.0.2-1
 ```
 
 ## Use Python dotenv
-It is recommanded to store your important person information in configuration or as environmental variables. Python dotenv allows loading environment variable from `.env` files for easier access and better security.
+
+It is recommended to store your important personal information in configuration or as environmental variables. Python dotenv allows loading environment variables from `.env` files for easier access and better security.
 
 python-dotenv package: https://pypi.org/project/python-dotenv/ \
-Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/docs/configuration.md
+Detailed instructions: https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2-1/docs/configuration.md
 
 ## Quick Start Guide for Swan SDK
+
 Jump into using the SDK with this quick example:
 
-### 1. Get SwanHub API Key
+### 1. Get Orchestrator API Key
 
-To use `swan-sdk` SwanHub API key is required. 
-- Go to Swan Dashboard: https://orchestrator.swanchain.io/provider-status
+To use `swan-sdk`, an Orchestrator API key is required. 
+
+- Go to Orchestrator Dashboard: https://orchestrator.swanchain.io/provider-status
 - Login through MetaMask.
-- Click the user icon on top right.
+- Click the user icon on the top right.
 - Click 'Show API-Key' -> 'New API Key'
 - Store your API Key safely, do not share with others.
 
-### 2. Login into SwanHub Through SDK
+### 2. Login into Orchestrator Through SDK
 
-To use `swan-sdk` you will need to login to SwanHub using API Key. (Wallet login is not supported)
+To use `swan-sdk` you will need to login to Orchestrator using API Key. (Wallet login is not supported)
 
 ```python
 from swan import SwanAPI
 
 swan_api = SwanAPI(api_key="<your_api_key>")
 ```
-
 ### 3. Connect to Swan Payment Contract
 
-Payment of SwanHub deployment is paid through Swan Payment Contract. To navigate the contract ABIs. First create a `SwanContract()` instance:
+Payment of Orchestrator deployment is paid through the Swan Payment Contract. To navigate the contract ABIs. First create a `SwanContract()` instance:
+**Notice: This won't be used until you're trying to Estimate Payment Amount, however, it's still recommended to do this step here to make sure that you can get all contract information before you move on**
+
 ```python
 from swan.contract.swan_contract import SwanContract
 
 contract = SwanContract('<your_private_key>', swan_api.contract_info)
 ```
 
-### 4. Retrieve Avaliable Hardware Informaitons
 
-SwanHub provides selection of Computing Providers with different hardwares.
-Use `SwanAPI().get_hardware_config()` to retrieve all avaliable hardwares on SwanHub.
+### 4. Retrieve available hardware information
+
+Orchestrator provides a selection of Computing Providers with different hardware.
+Use `SwanAPI().get_hardware_config()` to retrieve all available hardware on Orchestrator.
+
+Each hardware is stored as an instance of `HardwareConfig()` object. 
 
-Each hardware is stored in `HardwareConfig()` object.
 ```python
 from swan.object import HardwareConfig
 ```
+Hardware config contains a unique hardware ID, hardware name, description, hardware type (CPU/GPU), price per hour, available region and current status.
 
-Hardware config contains an unique hardware ID, hardware name, description, hardware type (CPU/GPU), price per hour, avaliable region and current status.
+See all available hardware in a Python dictionary:
 
-See all avaliable hardware in a python dictionary:
 ```python
-
 hardwares = swan_api.get_hardware_config()
 hardwares_info = [hardware.to_dict() for hardware in hardwares if hardware.status == "available"] 
-hardwares_info
+print(hardwares_info)
+```
+You can use 
+```python
+from swan.object import HardwareConfig
+```
+to check the hardware information like this:
+- `HardwareConfig().status` shows the availability of the hardware.
+- `HardwareConfig().region` is a list of all regions this hardware is available in.
+- Retrieve individual hardware attributes:
+```python
+print(chosen_hardware.id) # hardware id
+print(chosen_hardware.name) # hardware name
+print(chosen_hardware.description) # hardware description
+print(chosen_hardware.type) # hardware type
+print(chosen_hardware.region) # all avaliable hardware region
+print(chosen_hardware.price) # current hardware price
+print(chosen_hardware.status) # overall hardware avaliablility
 ```
-`HardwareConfig().status` shows the avalibility of the hardware.
-`HardwareConfig().region` is a list of all region this hardware is avaliable in.
 
-Retrieve the hardware with hardware id 0:
+More detials go oject documentation: https://github.com/swanchain/python-swan-sdk/blob/release/v0.0.2.post1/docs/object.md
+
+Useful example: Retrieve the hardware with hardware ID 0:
 ```python
 hardwares = swan_api.get_hardware_config()
-chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0]
-chosen_hardware.to_dict()
+chosen_hardware = [hardware for hardware in hardwares if hardware.id == 0][0]
+print(chosen_hardware.to_dict())
 ```
 
 Sample output:
+
 ```
 {'id': 0,
  'name': 'C1ae.small',
  'description': 'CPU only · 2 vCPU · 2 GiB',
  'type': 'CPU',
  'reigion': ['North Carolina-US', ...],
  'price': '0.0',
  'status': 'available'
 }
 ```
 
+
 ### 5. Get job_source_uri
 
 `job_source_uri` can be create through `SwanAPI().get_source_uri()` API.
 
 Generate a source URI
 A demo tetris docker image on GitHub as repo_uri: 'https://github.com/alphaflows/tetris-docker-image.git'
+
 ```python
 job_source_uri = swan_api.get_source_uri(
     repo_uri='<your_git_hub_link/your_lagrange_space_link>',
     hardware_id=chosen_hardware.id,
     wallet_address='<your_wallet_address>'
 )
 
 job_source_uri = job_source_uri['data']['job_source_uri']
+print(job_source_uri)
 ```
 
-### 6. Esitmate Payment Amount
+### 6. Estimate Payment Amount
+
 To estimate the payment required for the deployment. Use `SwanContract().estiamte_payment()`
+
 ```python
 duration_hour = 1 # or duration you want the deployment to run
 amount = contract.estimate_payment(chosen_hardware.id, duration_hour)
-amount # amount is in wei, 18 decimals
+print(amount) # amount is in wei, 18 decimals
 ```
 
 ### 7. Create Task
 
-Before paying for the task. First create a task on SwanHub using desired task attributes.
+Before paying for the task. First, create a task on Orchestrator using desired task attributes.
+
 ```python
 import json
 
+duration_hour = 1
+# Notice that from here, you need to convert the duration to seconds
 duration = 3600*duration_hour
 cfg_name = chosen_hardware.name
 
 result = swan_api.create_task(
     cfg_name=cfg_name, 
-    region='<region_name>', 
+    region='<region_name>', # e.g. 'North Carolina-US' or chosen_hardware.region[0]
     start_in=300,  # in seconds
     duration=duration, 
     job_source_uri=job_source_uri, #repo.source_uri
     paid=contract._wei_to_swan(amount), # from wei to swan amount/1e18
     wallet_address='<your_wallet_address>',
 )
 task_uuid = result['data']['task']['uuid']
 
 print(json.dumps(result, indent=2)) # Print response
 ```
 
 Sample output:
+
 ```
 {
   "data": {
     "task": {
       "created_at": "1714254304",
       "end_at": "1714257898",
       "leading_job_id": null,
@@ -215,46 +248,89 @@
     }
   },
   "message": "Task_uuid initialized.",
   "status": "success"
 }
 ```
 
-The `task['uuid']` will be used in following operations.
+**The `task['uuid']` will be used in the following operations.**
+
+
 
 ### 8. Submit Payment
 
+- **If you got error about insufficient balance, please make sure you have enough balance in your wallet.**
+- *If you have Error like "to_wei() does not exist", please make sure you have web3.py 6.15 or later.*
+
 Use `SwanContract().submit_payment()` to pay for the task. The TX hash is the receipt for the payment.
+
 ```python
-tx_hash = contract.submit_payment(task_uuid, hardware_id, duration)
+tx_hash = contract.submit_payment(task_uuid, chosen_hardware.id, duration) # duration in seconds
 ```
 
 ### 9. Validate Payment to Deploy Task
 
 Use `SwanAPI().validate_payment()` to validate the payment using TX hash and deploy the task.
+
 ```python
 swan_api.validate_payment(
     tx_hash=tx_hash,
     task_uuid=task_uuid
 )
 ```
 
-### 10. Follow up Task Status (Optional)
+### 10. Follow-up Task Status (Optional)
 
 #### Show results
 
-Get the deploy URI to test your task deployment using `SwanAPI().get_real_uri()`.
+Get the deploy URI to test your deployed task using `SwanAPI().get_real_uri()`.
+
 ```python
 r = swan_api.get_real_url(task_uuid)
 print(r)
 ```
 
+#### Show task details
+Get the task details using `SwanAPI().get_deployment_info()`.
+
+```python
+r = swan_api.get_deployment_info(task_uuid)
+print(r)
+```
+Simple output
+```
+{
+   "data":{
+      "computing_providers":[
+         
+      ],
+      "jobs":[
+         
+      ],
+      "task":{
+         "created_at":"1714877536",
+         "end_at":"1714881125",
+         "leading_job_id":"None",
+         "refund_amount":"None",
+         "status":"accepting_bids",
+         "task_detail_cid":"task_detail_cid",
+         "tx_hash":"None",
+         "updated_at":"1714877801",
+         "uuid":"204cd1be-30b0-4915-a635-4b9dbf1a3b5e"
+      }
+   },
+   "message":"fetch task info for task_uuid='204cd1be-30b0-4915-a635-4b9dbf1a3b5e' successfully",
+   "status":"success"
+}
+```
+
+
 ## Examples
-For executable examples consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/examples
+For executable examples consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2.post1/examples
 
 ## Documentation
 
-For comprehensive documentation, including detailed installation guides, usage examples, and complete API references, please consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2/docs
+For comprehensive documentation, including detailed installation guides, usage examples, and complete API references, please consult https://github.com/swanchain/python-swan-sdk/tree/release/v0.0.2.post1/docs
 
 ## License
 
 The PYTHON SWAN SDK is released under the **MIT** license, details of which can be found in the LICENSE file.
```

### Comparing `swan_sdk-0.0.2/swan_sdk.egg-info/SOURCES.txt` & `swan_sdk-0.0.2.post1/swan_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

