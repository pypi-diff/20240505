# Comparing `tmp/indipyclient-0.1.0.tar.gz` & `tmp/indipyclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.0.tar` & `indipyclient-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.0/LICENSE
--rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.1.0/README.md
--rw-r--r--   0        0        0      416 2024-05-02 12:33:18.000000 indipyclient-0.1.0/indipyclient/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-02 10:21:26.000000 indipyclient-0.1.0/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.0/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    21197 2024-05-02 11:05:08.000000 indipyclient-0.1.0/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.0/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144085 2024-04-28 18:17:36.000000 indipyclient-0.1.0/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.1.0/indipyclient/error.py
--rw-r--r--   0        0        0    26765 2024-05-02 11:52:00.000000 indipyclient-0.1.0/indipyclient/events.py
--rw-r--r--   0        0        0    32116 2024-05-02 11:56:45.000000 indipyclient-0.1.0/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16211 2024-04-28 20:08:14.000000 indipyclient-0.1.0/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27645 2024-04-28 18:21:13.000000 indipyclient-0.1.0/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-02 12:33:02.000000 indipyclient-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.1/README.md
+-rw-r--r--   0        0        0      416 2024-05-05 14:31:43.000000 indipyclient-0.1.1/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-02 10:21:26.000000 indipyclient-0.1.1/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.1/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    21417 2024-05-05 09:36:44.000000 indipyclient-0.1.1/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.1/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.1/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    26738 2024-05-03 13:06:57.000000 indipyclient-0.1.1/indipyclient/events.py
+-rw-r--r--   0        0        0    32617 2024-05-05 09:46:34.000000 indipyclient-0.1.1/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16279 2024-05-03 09:59:43.000000 indipyclient-0.1.1/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.1/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-05 14:31:16.000000 indipyclient-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.1/PKG-INFO
```

### Comparing `indipyclient-0.1.0/LICENSE` & `indipyclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.0/README.md` & `indipyclient-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,21 +25,22 @@
       --host HOST           Hostname/IP of the INDI server (default localhost).
       -b BLOBS, --blobs BLOBS
                             Optional folder where BLOB's will be saved.
       --loglevel LOGLEVEL   Enables logging, value 1, 2, 3 or 4.
       --logfile LOGFILE     File where logs will be saved
       --version             show program's version number and exit
 
-    The BLOB's folder can also be set from within the session. Setting loglevel
-    and logfile should only be used for brief diagnostic purposes, the logfile
-    could grow very big.
+    The BLOB's folder can also be set from within the session.
+    Setting loglevel and logfile should only be used for brief
+    diagnostic purposes, the logfile could grow very big.
     loglevel:1 Information and error messages only,
-    loglevel:2 log vector tags without members or contents,
-    loglevel:3 log vectors and members - but not BLOB contents,
-    loglevel:4 log vectors and all contents
+    loglevel:2 As 1 plus xml vector tags without members or contents,
+    loglevel:3 As 1 plus xml vectors and members - but not BLOB contents,
+    loglevel:4 As 1 plus xml vectors and all contents
+
 
 A typical sesssion would look like:
 
 ![Terminal screenshot](https://github.com/bernie-skipole/indipyclient/raw/main/image.png)
 
 
 This is a companion package to 'indipydriver' which can be used to create INDI drivers.
```

### Comparing `indipyclient-0.1.0/indipyclient/__main__.py` & `indipyclient-0.1.1/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.0/indipyclient/console/consoleclient.py` & `indipyclient-0.1.1/indipyclient/console/consoleclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 logger.setLevel(logging.DEBUG)
                 self.client.debug_verbosity(2)
             elif level == 2:
                 logger.setLevel(logging.DEBUG)
                 self.client.debug_verbosity(1)
             elif level == 1:
                 logger.setLevel(logging.INFO)
-            logfile = pathlib.Path(logfile).expanduser().resolve()
+
             fh = logging.FileHandler(logfile)
             logger.addHandler(fh)
         except:
             return
         return level
 
 
@@ -150,21 +150,25 @@
     def shutdown(self):
         "Sets self._shutdown to True which shuts down the client"
         self._shutdown = True
 
 
     async def _checkshutdown(self):
         "If self._shutdown becomes True, shutdown"
-        while not self._shutdown:
-            await asyncio.sleep(0)
-        await self.client.report("Shutting down client - please wait")
-        self.client.shutdown()
-        while not self.client.stopped:
+        while (not self._shutdown) and (not self.client.stopped):
             await asyncio.sleep(0)
-        # now stop co-routines
+        # so either shutdown has been requested or the ipyclient has stopped for some reason
+        self._shutdown = True
+        if not self.client.stopped:
+            # client is still running, shut it down
+            self.client.report("Shutting down client - please wait")
+            self.client.shutdown()
+            while not self.client.stopped:
+                await asyncio.sleep(0)
+        # so ipyclient has stopped now stop console co-routines
         self.stop = True
         while (not self.updatescreenstopped) and (not self.getinputstopped):
             await asyncio.sleep(0)
         # async tasks finished, clear up the terminal
         curses.nocbreak()
         self.stdscr.keypad(False)
         curses.curs_set(1)
```

### Comparing `indipyclient-0.1.0/indipyclient/console/widgets.py` & `indipyclient-0.1.1/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.0/indipyclient/console/windows.py` & `indipyclient-0.1.1/indipyclient/console/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,17 +268,17 @@
             self.titlewin.addstr(2, 0, "Not Connected")
 
         self.titlewin.noutrefresh()
         self.messwin.noutrefresh()
         curses.doupdate()
 
 
-    async def disableBLOBs(self):
+    def disableBLOBs(self):
         self.control.blobenabled = False
-        await self.client.report("Warning! BLOBs disabled")
+        self.client.report("Warning! BLOBs disabled")
         self.control.send_disableBLOB()
         self.enable_btn.bold = False
         self.disable_btn.bold = True
         self.enable_btn.draw()
         self.disable_btn.draw()
         self.infowin.noutrefresh()
         curses.doupdate()
@@ -317,15 +317,15 @@
             if isinstance(key, tuple):
                 for fld in self.fields:
                     if key in fld:
                         if fld.focus:
                             # focus already set - return the button onclick
                             value = fld.onclick
                             if value == "DisableBLOBs":
-                                await self.disableBLOBs()
+                                self.disableBLOBs()
                                 break
                             else:
                                 return value
                         # focus not set, defocus the one currently
                         # in focus
                         self.defocus()
                         # and set this into focus
@@ -401,15 +401,15 @@
 
             elif key == 10:
                 # Enter has been pressed, check which field has focus
                 for fld in self.fields:
                     if fld.focus:
                         value = fld.onclick
                         if value == "DisableBLOBs":
-                            await self.disableBLOBs()
+                            self.disableBLOBs()
                             break
                         else:
                             return value
 
 
 class EnableBLOBsScreen(ConsoleClientScreen):
 
@@ -488,46 +488,46 @@
         "Only update if global message has changed"
         if isinstance(event, events.Message):
             widgets.drawmessage(self.messwin, self.client.messages[0], maxcols=self.maxcols)
             self.messwin.noutrefresh()
             curses.doupdate()
 
 
-    async def submit(self):
+    def submit(self):
         self._newpath = self.path_txt.text.strip()
         blobfolder = None
         if self._newpath:
             try:
                 blobfolder = pathlib.Path(self._newpath).expanduser().resolve()
             except Exception:
                 self.control.blobenabled = False
                 self.control.send_disableBLOB()
                 self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
-                await self.client.report("Warning! Unable to parse BLOB folder")
+                self.client.report("Warning! Unable to parse BLOB folder")
                 self.submit_btn.focus = False
                 self.messages_btn.focus = True
                 return
             if blobfolder.is_dir():
                 self.control.blobfolder = blobfolder
                 self._newpath = str(blobfolder)
                 self.path_txt.text = self._newpath
                 self.path_txt.draw()
                 self.control.blobenabled = True
                 self.control.send_enableBLOB()
                 self.pathwin.addstr(0, 0, "BLOBs are enabled  ", curses.A_BOLD)
-                await self.client.report("BLOB folder is set")
+                self.client.report("BLOB folder is set")
             else:
                 self.control.blobenabled = False
                 self.control.send_disableBLOB()
                 self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
-                await self.client.report("Warning! BLOB folder is not a directory")
+                self.client.report("Warning! BLOB folder is not a directory")
         else:
             self.control.blobenabled = False
             self.pathwin.addstr(0, 0, "BLOBs are disabled ", curses.A_BOLD)
-            await self.client.report("Warning! BLOB folder is invalid")
+            self.client.report("Warning! BLOB folder is invalid")
             self.control.send_disableBLOB()
         self.submit_btn.focus = False
         self.messages_btn.focus = True
 
 
     async def inputs(self):
         "Gets inputs from the screen"
@@ -546,15 +546,15 @@
             if isinstance(key, tuple):
                 for fld in self.fields:
                     if key in fld:
                         if fld.focus:
                             # focus already set - return the button onclick
                             value = fld.onclick
                             if value == "Submit":
-                                await self.submit()
+                                self.submit()
                                 self.submit_btn.draw()
                                 self.messages_btn.draw()
                                 self.buttwin.noutrefresh()
                                 self.pathwin.noutrefresh()
                                 curses.doupdate()
                                 break
                             else:
@@ -578,15 +578,15 @@
                     curses.doupdate()
                     return "Quit"
                 elif self.messages_btn.focus:
                     return "Messages"
                 elif self.devices_btn.focus:
                     return "Messages"
                 elif self.submit_btn.focus:
-                    await self.submit()
+                    self.submit()
 
             elif key in (32, 9, 261, 338, 258):
                 # go to the next button
                 if self.path_txt.focus:
                     self.path_txt.focus = False
                     self.submit_btn.focus = True
                     self.path_txt.draw()
```

### Comparing `indipyclient-0.1.0/indipyclient/events.py` & `indipyclient-0.1.1/indipyclient/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 from collections import UserDict
 
 import xml.etree.ElementTree as ET
 
 from . import propertyvectors
 
-from . import propertymembers
-
-from .error import ParseException
+from .propertymembers import ParseException, getfloat
 
 
 
 def _parse_timestamp(timestamp_string):
     """Parse a timestamp string and return either None on failure, or a datetime object
        If the given timestamp_string is None, return the datetime for the current time.
        Everything is UTC"""
@@ -576,15 +574,15 @@
                 if not member.text:
                     raise ParseException("Missing value in oneNumber")
                 membervalue = member.text.strip()
                 if not membervalue:
                     raise ParseException("Missing value in oneNumber")
                 # test membervalue ok
                 try:
-                    memberfloat = propertymembers.getfloat(membervalue)
+                    memberfloat = getfloat(membervalue)
                 except TypeError:
                     raise ParseException("Invalid number in setNumberVector")
                 self.data[membername] = membervalue
             else:
                 raise ParseException("Invalid child tag of setNumberVector")
         properties = device.data
         self.vector = properties[self.vectorname]
```

### Comparing `indipyclient-0.1.0/indipyclient/ipyclient.py` & `indipyclient-0.1.1/indipyclient/ipyclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import xml.etree.ElementTree as ET
 
 import logging
 logger = logging.getLogger(__name__)
 
 from . import events
 
-from .error import ParseException, ConnectionTimeOut
+from .propertymembers import ParseException
 
 
 # All xml data received from the driver should be contained in one of the following tags
 TAGS = (b'message',
         b'delProperty',
         b'defSwitchVector',
         b'setSwitchVector',
@@ -160,27 +160,32 @@
         self._verbose = verbose
 
 
     def shutdown(self):
         "Shuts down the client"
         self._stop = True
 
-    async def report(self, message):
+    def report(self, message):
         """This injects a message into the received data, which will be
            picked up by the rxevent method. It is a way to set a message
            on to your client display, in the same way messages come from
            the INDI service. If logging is enabled the message will also
            be logged at level INFO"""
         try:
             timestamp = datetime.now(tz=timezone.utc)
             timestamp = timestamp.replace(tzinfo=None)
             logger.info(message)
             root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
-            event = events.Message(root, None, self)
-            await self.rxevent(event)
+            # and place root into readerque
+            try:
+                self.readerque.put_nowait(root)
+            except asyncio.QueueFull:
+                # The queue is full, something may be wrong
+                # discard this data and continue
+                pass
         except Exception :
             logger.exception("Error in IPyClient.report method")
 
 
     def enabledlen(self):
         "Returns the number of enabled devices"
         return sum(map(lambda x:1 if x.enable else 0, self.data.values()))
@@ -197,35 +202,35 @@
             while not self._stop:
                 self.tx_timer = None
                 self.idle_timer = time.time()
                 try:
                     # start by openning a connection
                     # clear messages
                     self.messages.clear()
-                    await self.report("Attempting to connect")
+                    self.report("Attempting to connect")
                     reader, writer = await asyncio.open_connection(self.indihost, self.indiport)
                     self.connected = True
                     self.messages.clear()
-                    await self.report(f"Connected to {self.indihost}:{self.indiport}")
+                    self.report(f"Connected to {self.indihost}:{self.indiport}")
                     await asyncio.gather(self._run_tx(writer),
                                          self._run_rx(reader),
                                          self._check_alive(writer)
                                          )
                 except ConnectionRefusedError:
-                    await self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
+                    self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
                 except ConnectionResetError:
-                    await self.report("Error: Connection Lost")
+                    self.report("Error: Connection Lost")
                 except Exception:
                     logger.exception("Connection Error")
-                    await self.report("Error: Connection failed")
+                    self.report("Error: Connection failed")
                 self._clear_connection()
                 if self._stop:
                     break
                 else:
-                    await self.report(f"Connection failed, re-trying...")
+                    self.report(f"Connection failed, re-trying...")
 
                 # wait five seconds before re-trying, but keep checking
                 # that self._stop has not been set
                 count = 0
                 while not self._stop:
                     await asyncio.sleep(0.5)
                     count += 1
@@ -271,15 +276,15 @@
                     telapsed = time.time() - self.tx_timer
                     if telapsed > self.respond_timeout:
                         # no response to transmission self.respond_timeout seconds ago
                        writer.close()
                        await writer.wait_closed()
                        self._clear_connection()
                        if not self._stop:
-                           await self.report("Error: Connection timed out")
+                           self.report("Error: Connection timed out")
             if self.connected and self._stop:
                 writer.close()
                 await writer.wait_closed()
                 self._clear_connection()
         except KeyboardInterrupt:
             self.shutdown()
         finally:
@@ -536,24 +541,24 @@
                             # no error has occurred, so add this device to self.data
                             self.data[devicename] = newdevice
                         else:
                             # device not known, not a def, so ignore it
                             continue
                 except ParseException as pe:
                     # if a ParseException is raised, it is because received data is malformed
-                    await self.report(str(pe))
+                    self.report(str(pe))
                     continue
                 finally:
                     self.readerque.task_done()
                 # and to get here, continue has not been called
                 # and an event has been created, call the user event handling function
                 await self.rxevent(event)
         except asyncio.CancelledError:
             raise
-        except Exception as e:
+        except Exception:
             logger.exception("Error in IPyClient._rxhandler method")
         finally:
             self.shutdown()
 
 
     def snapshot(self):
         """Take a snapshot of the devices and returns a dictionary of device
@@ -643,21 +648,21 @@
                                         event = events.VectorTimeOut(device, vector)
                                         await self.rxevent(event)
                     else:
                         # no devices
                         # then send a getProperties, every five seconds, when count is zero
                         if not count:
                             self.send_getProperties()
-                            await self.report("getProperties sent")
+                            self.report("getProperties sent")
                         count += 1
                         if count >= 10:
                             count = 0
         except asyncio.CancelledError:
              raise
-        except Exception as e:
+        except Exception:
             logger.exception("Error in IPyClient._timeout_monitor method")
         finally:
             self.shutdown()
 
 
     def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request. On startup the IPyClient object
@@ -744,40 +749,49 @@
         "Properties are added by being learnt from the driver, they cannot be manually added"
         raise KeyError
 
 
     def rxvector(self, root):
         """Handle received data, sets new propertyvector into self.data,
            or updates existing property vector and returns an event"""
-        if root.tag == "delProperty":
-            return events.delProperty(root, self, self._client)
-        elif root.tag == "message":
-            return events.Message(root, self, self._client)
-        elif root.tag == "defSwitchVector":
-            return events.defSwitchVector(root, self, self._client)
-        elif root.tag == "setSwitchVector":
-            return events.setSwitchVector(root, self, self._client)
-        elif root.tag == "defLightVector":
-            return events.defLightVector(root, self, self._client)
-        elif root.tag == "setLightVector":
-            return events.setLightVector(root, self, self._client)
-        elif root.tag == "defTextVector":
-            return events.defTextVector(root, self, self._client)
-        elif root.tag == "setTextVector":
-            return events.setTextVector(root, self, self._client)
-        elif root.tag == "defNumberVector":
-            return events.defNumberVector(root, self, self._client)
-        elif root.tag == "setNumberVector":
-            return events.setNumberVector(root, self, self._client)
-        elif root.tag == "defBLOBVector":
-            return events.defBLOBVector(root, self, self._client)
-        elif root.tag == "setBLOBVector":
-            return events.setBLOBVector(root, self, self._client)
-        else:
-            raise ParseException("Unrecognised tag received")
+        try:
+            if root.tag == "delProperty":
+                return events.delProperty(root, self, self._client)
+            elif root.tag == "message":
+                return events.Message(root, self, self._client)
+            elif root.tag == "defSwitchVector":
+                return events.defSwitchVector(root, self, self._client)
+            elif root.tag == "setSwitchVector":
+                return events.setSwitchVector(root, self, self._client)
+            elif root.tag == "defLightVector":
+                return events.defLightVector(root, self, self._client)
+            elif root.tag == "setLightVector":
+                return events.setLightVector(root, self, self._client)
+            elif root.tag == "defTextVector":
+                return events.defTextVector(root, self, self._client)
+            elif root.tag == "setTextVector":
+                return events.setTextVector(root, self, self._client)
+            elif root.tag == "defNumberVector":
+                return events.defNumberVector(root, self, self._client)
+            elif root.tag == "setNumberVector":
+                return events.setNumberVector(root, self, self._client)
+            elif root.tag == "defBLOBVector":
+                return events.defBLOBVector(root, self, self._client)
+            elif root.tag == "setBLOBVector":
+                return events.setBLOBVector(root, self, self._client)
+            else:
+                raise ParseException("Unrecognised tag received")
+        except ParseException:
+            raise
+        except KeyboardInterrupt:
+            raise
+        except Exception:
+            logger.exception("Error in IPyClient.rxvector method")
+            raise ParseException("Error while attempting to parse received data")
+
 
     def _snapshot(self):
         "Creates snapshot of this device and its vectors"
         snapdevice = Device(self.devicename)
         for vectorname, vector in self.data:
             snapdevice[vectorname] = vector._snapshot()
         snapdevice.messages = list(self.messages)
```

### Comparing `indipyclient-0.1.0/indipyclient/propertymembers.py` & `indipyclient-0.1.1/indipyclient/propertymembers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 
 import xml.etree.ElementTree as ET
 
 import sys, pathlib
 
-from .error import ParseException
+
+class ParseException(Exception):
+    "Raised if an error occurs when parsing received data"
+    pass
 
 
 def getfloat(value):
     """The INDI spec specifies several different number formats, given a number
        in any of these formats, this returns a float.
        If an error occurs while parsing the number, a TypeError exception is raised."""
     try:
```

### Comparing `indipyclient-0.1.0/indipyclient/propertyvectors.py` & `indipyclient-0.1.1/indipyclient/propertyvectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 from datetime import datetime, timezone
 
 import asyncio
 
 import xml.etree.ElementTree as ET
 
-from .propertymembers import SwitchMember, LightMember, TextMember, NumberMember, BLOBMember
-
-from .error import ParseException
+from .propertymembers import SwitchMember, LightMember, TextMember, NumberMember, BLOBMember, ParseException
 
 
 class Vector(collections.UserDict):
 
     """This class is the parent of the PropertyVector class, which in turn
        is the parent of SwitchVector, LightVector, TextVector, NumberVector
        and BLOBVector classes.
```

### Comparing `indipyclient-0.1.0/pyproject.toml` & `indipyclient-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.0"
+version = "0.1.1"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.0/PKG-INFO` & `indipyclient-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -40,21 +40,22 @@
       --host HOST           Hostname/IP of the INDI server (default localhost).
       -b BLOBS, --blobs BLOBS
                             Optional folder where BLOB's will be saved.
       --loglevel LOGLEVEL   Enables logging, value 1, 2, 3 or 4.
       --logfile LOGFILE     File where logs will be saved
       --version             show program's version number and exit
 
-    The BLOB's folder can also be set from within the session. Setting loglevel
-    and logfile should only be used for brief diagnostic purposes, the logfile
-    could grow very big.
+    The BLOB's folder can also be set from within the session.
+    Setting loglevel and logfile should only be used for brief
+    diagnostic purposes, the logfile could grow very big.
     loglevel:1 Information and error messages only,
-    loglevel:2 log vector tags without members or contents,
-    loglevel:3 log vectors and members - but not BLOB contents,
-    loglevel:4 log vectors and all contents
+    loglevel:2 As 1 plus xml vector tags without members or contents,
+    loglevel:3 As 1 plus xml vectors and members - but not BLOB contents,
+    loglevel:4 As 1 plus xml vectors and all contents
+
 
 A typical sesssion would look like:
 
 ![Terminal screenshot](https://github.com/bernie-skipole/indipyclient/raw/main/image.png)
 
 
 This is a companion package to 'indipydriver' which can be used to create INDI drivers.
```

