# Comparing `tmp/satorisynapse-0.0.9.tar.gz` & `tmp/satorisynapse-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.0.9.tar", last modified: Thu Apr 18 21:52:42 2024, max compression
+gzip compressed data, was "satorisynapse-0.1.0.tar", last modified: Sun May  5 15:53:08 2024, max compression
```

## Comparing `satorisynapse-0.0.9.tar` & `satorisynapse-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.318185 satorisynapse-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:52:42.314185 satorisynapse-0.0.9/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 21:52:42.000000 satorisynapse-0.0.9/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 21:52:42.318185 satorisynapse-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-18 21:52:29.000000 satorisynapse-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/setup.py
```

### Comparing `satorisynapse-0.0.9/LICENSE` & `satorisynapse-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.9/PKG-INFO` & `satorisynapse-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.9
+Version: 0.1.0
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.9/satorisynapse/lib/requests.py` & `satorisynapse-0.1.0/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.0.9/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.1.0/satorisynapse/synapse/asynchronous.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,44 +2,53 @@
 we discovered that udp hole punching inside docker containers is not always
 possible because of the way the docker nat works. we thought it was.
 this host script is meant to run on the host machine.
 it will establish a sse connection with the flask server running inside
 the container. it will handle the UDP hole punching, passing data between the
 flask server and the remote peers.
 '''
-
+import os
+import sys
 import time
-import typing as t
 import socket
 import asyncio
-import requests  # ==2.31.0
+import platform
+import subprocess
+import typing as t
 import aiohttp  # ==3.8.4
+import requests  # ==2.31.0
 from satorisynapse.lib.error import SseTimeoutFailure
-from satorisynapse.lib.domain import Envelope, Ping, SYNAPSE_PORT
-from satorisynapse.lib.requests import requests
-from satorisynapse.lib.utils import greyPrint
+from satorisynapse.lib.domain import Envelope, Ping, Signal, SYNAPSE_PORT
+from satorisynapse.lib.utils import greyPrint, satoriUrl
+
+keepRunning = True
 
 
 class Synapse():
     ''' go-between for the flask server and the remote peers '''
 
-    def __init__(self, port: int = None):
+    def __init__(
+        self,
+        port: int = None,
+        version: str = None,
+        restartPath: str = None,
+        installDir: str = None,
+    ):
         self.port = port or SYNAPSE_PORT
+        self.version = version or 'v1',
+        self.restartPath = restartPath
+        self.installDir = installDir
         self.socketListener = None
         self.neuronListener = None
         self.peers: t.List[str] = []
         self.session = aiohttp.ClientSession()
         self.socket: socket.socket = self.createSocket()
         self.loop = asyncio.get_event_loop()
         self.broke = asyncio.Event()
 
-    @staticmethod
-    def satoriUrl(endpoint='') -> str:
-        return 'http://localhost:24601/synapse' + endpoint
-
     ### INIT ###
 
     async def run(self):
         ''' runs forever '''
         await self.initNeuronListener()
         await self.initSocketListener()
 
@@ -51,15 +60,15 @@
         await self.cancelSocketListener()
         self.socketListener = asyncio.create_task(self.listenToSocket())
 
     async def createNeuronListener(self):
         timeout = aiohttp.ClientTimeout(total=None, sock_read=None)
         async with aiohttp.ClientSession(timeout=timeout) as session:
             try:
-                async with session.get(Synapse.satoriUrl('/stream')) as response:
+                async with session.get(satoriUrl('/stream')) as response:
                     async for line in response.content:
                         if line.startswith(b'data:'):
                             asyncio.create_task(
                                 self.handleNeuronMessage(
                                     line.decode('utf-8')[5:].strip()))
             except asyncio.TimeoutError:
                 greyPrint('Neuron connection timed out...')
@@ -119,15 +128,74 @@
     async def addPeer(self, ip: str):
         await self.speak(ip, self.port, data=Ping().toJson)
         self.peers.append(ip)
 
     ### HANDLERS ###
 
     async def handleNeuronMessage(self, message: str):
+
+        async def handleSignal(signal: Signal):
+            global keepRunning
+            if msg.vesicle.restart:
+                greyPrint('restarting Satori Neuron...')
+                subprocess.Popen('docker stop satorineuron')
+                time.sleep(30)
+                if self.restartPath not in [None, '', 'none', 'null', 'None']:
+                    if platform.system() == "Windows" and (
+                        self.restartPath.endswith('.exe') or
+                        self.restartPath.endswith('.bat') or
+                        self.restartPath.endswith('.lnk')
+                    ):
+                        subprocess.Popen(
+                            f'start cmd.exe /k "{self.restartPath}"',
+                            shell=True)
+                    else:
+                        if platform.system() == "Windows":
+                            subprocess.Popen(
+                                f'start cmd.exe /k {sys.executable} "{self.restartPath}"',
+                                shell=True)
+                        elif platform.system() == "Darwin":
+                            # osascript -e 'tell application "Terminal" to do script "python3 /path/to/your_script.py"'
+                            escapedExecutable = sys.executable.replace(
+                                " ", "\\ ")
+                            escapedRestartPath = self.restartPath.replace(
+                                " ", "\\ ")
+                            subprocess.Popen(
+                                f"""osascript -e 'tell application "Terminal" to do script "{escapedExecutable} {escapedRestartPath}"'""",
+                                shell=True)
+                        elif platform.system() == "Linux":
+                            subprocess.Popen(
+                                ["gnome-terminal", "--", sys.executable, self.restartPath])
+                    self.broke.set()
+                    # exit()
+                    keepRunning = False
+                elif self.installDir not in [None, '', 'none', 'null', 'None']:
+                    subprocess.Popen(
+                        f'docker pull satorinet/satorineuron:{self.version}')
+                    time.sleep(60)
+                    subprocess.Popen((
+                        'docker run --rm -it --name satorineuron '
+                        '-p 24601:24601 '
+                        f'-v {os.path.join(self.installDir, "wallet")}:/Satori/Neuron/wallet '
+                        f'-v {os.path.join(self.installDir, "config")}:/Satori/Neuron/config '
+                        f'-v {os.path.join(self.installDir, "data")}:/Satori/Neuron/data '
+                        f'-v {os.path.join(self.installDir, "models")}:/Satori/Neuron/models '
+                        '--env SATORI_RUN_MODE=prod '
+                        f'satorinet/satorineuron:{self.version} ./start.sh'),)
+            if msg.vesicle.shutdown:
+                greyPrint('shutting down Satori Neuron...')
+                self.broke.set()
+                subprocess.Popen('docker stop satorineuron')
+                time.sleep(30)
+                # exit()
+                keepRunning = False
+
         msg = Envelope.fromJson(message)
+        if msg.vesicle.className == 'Signal':
+            return await handleSignal(msg.vesicle)
         await self.maybeAddPeer(msg.ip)
         await self.speak(
             remoteIp=msg.ip,
             remotePort=self.port,
             data=msg.vesicle.toJson)
 
     async def handlePeerMessage(self, data: bytes, address: t.Tuple[str, int]):
@@ -150,15 +218,15 @@
         #        greyPrint(f'connection to {address[0]} established!')
         #        return
         await self.relayToNeuron(data=data, ip=address[0], port=address[1])
 
     async def relayToNeuron(self, data: bytes, ip: str, port: int):
         try:
             async with self.session.post(
-                    Synapse.satoriUrl('/message'),
+                    satoriUrl('/message'),
                     data=data,
                     headers={
                         'Content-Type': 'application/octet-stream',
                         'remoteIp': ip
                     },
             ) as response:
                 if response.status != 200:
@@ -193,65 +261,113 @@
                 greyPrint('Neuron listener task cancelled successfully.')
 
     async def shutdown(self):
         await self.session.close()
         await self.cancelSocketListener()
         await self.cancelNeuronListener()
         self.socket.close()
-        greyPrint('Synapse shutdown complete.')
+        greyPrint('Satori Synapse shutdown complete.')
 
 
 def silentlyWaitForNeuron():
     while True:
         try:
-            r = requests.get(Synapse.satoriUrl('/ping'))
+            r = requests.get(satoriUrl('/ping'))
             if r.status_code == 200:
                 return
         except Exception as _:
             pass
-        time.sleep(1)
+        time.sleep(10)
 
 
-async def main(port: int = None):
+async def main(
+    port: int = None,
+    version: str = None,
+    restartPath: str = None,
+    installDir: str = None,
+):
 
     async def waitForNeuron():
         notified = False
         while True:
             try:
-                r = requests.get(Synapse.satoriUrl('/ping'))
-                if r.status_code == 200:
+                r = requests.get(satoriUrl('/ping'))
+                if r.text == 'ready':
                     if notified:
-                        greyPrint('established connection to Satori Neuron')
+                        greyPrint(
+                            'established connection to Satori Neuron')
                     return
+                if r.text == 'ok' and not notified:
+                    greyPrint('waiting for Satori Neuron...')
             except Exception as _:
                 if not notified:
-                    greyPrint('waiting for Satori Neuron to start')
+                    greyPrint('waiting for Satori Neuron...')
                     notified = True
             await asyncio.sleep(1)
 
-    while True:
+    while keepRunning:
         await waitForNeuron()
-        synapse = Synapse(port)
+        synapse = Synapse(
+            port=port,
+            version=version,
+            restartPath=restartPath,
+            installDir=installDir)
         await synapse.run()
-        greyPrint("Satori P2P Relay is running. Press Ctrl+C to stop.")
+        greyPrint("Satori Synapse is running. Press Ctrl+C to stop.")
         try:
             await synapse.broke.wait()
             raise Exception('synapse not running')
         except KeyboardInterrupt:
             pass
         except SseTimeoutFailure:
             pass
         except Exception as _:
             pass
         finally:
             await synapse.shutdown()
+    await synapse.shutdown()
 
 
-def runSynapse(port: int = None):
+def runSynapse(
+    port: int = None,
+    version: str = None,
+    restartPath: str = None,
+    installDir: str = None,
+):
     try:
-        asyncio.run(main(port))
+        greyPrint('Synapse started (async version)')
+        asyncio.run(main(
+            port=int(port) if isinstance(port, str) else port,
+            version=version,
+            restartPath=restartPath,
+            installDir=installDir))
     except KeyboardInterrupt:
-        print('Interrupted by user')
+        print('Synapse exited by user')
 
 
 if __name__ == '__main__':
-    runSynapse()
+    if len(sys.argv) == 5:
+        runSynapse(
+            port=sys.argv[1],
+            version=sys.argv[2],
+            restartPath=sys.argv[3],
+            installDir=sys.argv[4],)
+        exit(0)
+    elif len(sys.argv) == 4:
+        runSynapse(
+            port=sys.argv[1],
+            version=sys.argv[2],
+            restartPath=sys.argv[3])
+        exit(0)
+    elif len(sys.argv) == 3:
+        runSynapse(port=sys.argv[1], version=sys.argv[2])
+        exit(0)
+    elif len(sys.argv) == 2:
+        if sys.argv[1] == 'help':
+            print(
+                'Usage: python3 runSynapse.py [port] [version (docker image version)] [restartPath]')
+        else:
+            runSynapse(port=sys.argv[1])
+        exit(0)
+    else:
+        runSynapse()
+        exit(0)
```

### Comparing `satorisynapse-0.0.9/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.1.0/satorisynapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.0.9
+Version: 0.1.0
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.0.9/setup.py` & `satorisynapse-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.0.9'
+    return '0.1.0'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
```

