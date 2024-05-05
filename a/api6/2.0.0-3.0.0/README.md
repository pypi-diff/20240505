# Comparing `tmp/api6-2.0.0.tar.gz` & `tmp/api6-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api6-2.0.0.tar", last modified: Sun Apr 14 19:41:49 2024, max compression
+gzip compressed data, was "api6-3.0.0.tar", last modified: Sun May  5 09:28:41 2024, max compression
```

## Comparing `api6-2.0.0.tar` & `api6-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.341411 api6-2.0.0/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-04 15:04:40.000000 api6-2.0.0/LICENCE
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-14 19:41:49.341411 api6-2.0.0/PKG-INFO
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-05 07:30:12.000000 api6-2.0.0/README.md
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.340411 api6-2.0.0/api6/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     6823 2024-04-12 12:39:54.000000 api6-2.0.0/api6/Encryption.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       25 2024-04-12 12:38:40.000000 api6-2.0.0/api6/__init__.py
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)    37206 2024-04-14 19:38:10.000000 api6-2.0.0/api6/client.py
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.341411 api6-2.0.0/api6.egg-info/
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/PKG-INFO
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      189 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/SOURCES.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/dependency_links.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        5 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/top_level.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-14 19:41:49.341411 api6-2.0.0/setup.cfg
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      568 2024-04-14 19:37:11.000000 api6-2.0.0/setup.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-05-05 09:28:41.918137 api6-3.0.0/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-04 15:04:40.000000 api6-3.0.0/LICENCE
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-05-05 09:28:41.918137 api6-3.0.0/PKG-INFO
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-05 07:30:12.000000 api6-3.0.0/README.md
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-05-05 09:28:41.917137 api6-3.0.0/api6/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     6823 2024-04-12 12:39:54.000000 api6-3.0.0/api6/Encryption.py
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       25 2024-04-12 12:38:40.000000 api6-3.0.0/api6/__init__.py
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)    45133 2024-05-05 09:21:50.000000 api6-3.0.0/api6/client.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-05-05 09:28:41.918137 api6-3.0.0/api6.egg-info/
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-05-05 09:28:41.000000 api6-3.0.0/api6.egg-info/PKG-INFO
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      189 2024-05-05 09:28:41.000000 api6-3.0.0/api6.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-05-05 09:28:41.000000 api6-3.0.0/api6.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        5 2024-05-05 09:28:41.000000 api6-3.0.0/api6.egg-info/top_level.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-05-05 09:28:41.918137 api6-3.0.0/setup.cfg
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      568 2024-05-05 09:19:52.000000 api6-3.0.0/setup.py
```

### Comparing `api6-2.0.0/LICENCE` & `api6-3.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `api6-2.0.0/PKG-INFO` & `api6-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api6
-Version: 2.0.0
+Version: 3.0.0
 Summary: Luis Rubika Bot to Rubika api 6
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `api6-2.0.0/api6/Encryption.py` & `api6-3.0.0/api6/Encryption.py`

 * *Files identical despite different names*

### Comparing `api6-2.0.0/api6/client.py` & `api6-3.0.0/api6/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,30 +15,38 @@
 from os import system, chmod, remove
 from pathlib import Path
 import time
 from tqdm import tqdm
 import os
 from urllib3 import PoolManager, ProxyManager
 import asyncio
+from termcolor import colored
+import pyfiglet
+font = pyfiglet.Figlet(font='slant')
+ascii_text = font.renderText('Luis api6')
+print(ascii_text)
 class Client:
 	def __init__(self, auth:str,key:str=None,palqform:str='Android',pak:str='app.rbmain.a',v:str="3.4.3",type:str="rubika"):
 		self.palqform = palqform
 		self.v = v
 		self.requ = PoolManager()
 		self.pak = pak
 		self.auth = auth
 		self.auth_send = Encryption.authSet(auth)
 		self.t = "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"
 		if key == None:
 			self.key = None
 		else:
 			privateKey = key.replace('=','')
+			privateKey = privateKey.replace("\n","")
+			privateKey = privateKey.replace("-----BEGIN RSA PRIVATE KEY-----","")
+			privateKey = privateKey.replace("-----END RSA PRIVATE KEY-----","")
 			self.key = privateKey
 		if type == "rubika":
-			self.url = "https://messengerg2c58.iranlms.ir/"
+			self.url = "https://messengerg2c98.iranlms.ir/"
 		else:
 			 if type == "shad":
 			 	self.url = "https://shadmessenger32.iranlms.ir/"
 	def requests(self, input, method):
 	   client = {"app_name": "Main", "package": self.pak, "app_version": self.v, "lang_code": "fa", "platform": self.palqform}
 	   method_payload = {"input": input, "method": method, "client": client}
 	   method_payload = dumps(method_payload)
@@ -71,45 +79,46 @@
 	def getGroupInfo(self, goid:str):
 		return self.requests({"group_guid":goid},"getGroupInfo")
 	def groupPreviewByJoinLink(self, link:str):
 		return self.requests({"hash_link":link},"groupPreviewByJoinLink")
 	def channelPreviewByJoinLink(self, link:str):
 		return self.requests({"hash_link":link},"channelPreviewByJoinLink")
 	def updateUsername(self, id:str):
-		return self.requests({"username":id},updateUsername)
-	def getGroupAllMembers(self, goid:str,start_id=None):
-		return self.requests({"group_guid":goid,"search_text":None,"start_id":start_id},"getGroupAllMembers")
+		return self.requests({"username":id},"updateUsername")
+	def getGroupAllMembers(self, goid:str,start_id=None,text=None):
+		return self.requests({"group_guid":goid,"search_text":text,"start_id":start_id},"getGroupAllMembers")
 	def searchGlobalObjects(self, text):
 		return self.requests({"search_text":text},"searchGlobalObjects")
 	def updateProfile(self,name,bio):
 		return self.requests({"first_name":name,"bio":bio,"updated_parameters":["first_name","bio"]},"updateProfile")
 	def getObjectByUsername(self,user):
 		return self.requests({"username":user},"getObjectByUsername")
 	def getUserInfo(self,user):
 		return self.requests({"user_guid":user},"getUserInfo")
 	def getChats(self,start_id=None):
 		return self.requests({"start_id":start_id},"getChats")
 	def getChannelInfo(self,goid):
 		return self.requests({"channel_guid":goid},"getChannelInfo")
 	def joinChannelByLink(self,link):
 		return self.requests({"hash_link":link},"joinChannelByLink")
-	def setChannelAdmin(self,goid,goidm):
-		return self.requests({"channel_guid":goid,"member_guid":goidm,"action":"SetAdmin","access_list":["ChangeInfo","ViewMembers","ViewAdmins","PinMessages","SendMessages","EditAllMessages","DeleteGlobalAllMessages","AddMember","SetJoinLink","SetAdmin"]},"setChannelAdmin")
+	def setChatAdmin(self,goid,goidm):
+		type = self.getType(goid)
+		return self.requests({f"{type.lower()}_guid":goid,"member_guid":goidm,"action":"SetAdmin","access_list":["ChangeInfo","ViewMembers","ViewAdmins","PinMessages","SendMessages","EditAllMessages","DeleteGlobalAllMessages","AddMember","SetJoinLink","SetAdmin"]},f"set{type}Admin")
 	def requestChangeObjectOwner(self,goid,goidm):
 		return self.requests({"object_guid":goid,"new_owner_user_guid":goidm},"requestChangeObjectOwner")
 	def getMySessions(self):
 		return self.requests({},"getMySessions")
 	def terminateOtherSessions(self):
 		return self.requests({},"terminateOtherSessions")
 	def getLinkFromAppUrl(self,link):
 		return self.requests({"app_url":link},"getLinkFromAppUrl")
 	def forwardMessages(self,goid,togoid,id:list):
 		return self.requests({"from_object_guid":goid,"to_object_guid":togoid,"message_ids":id,"rnd":str(randint(9282873, 102662617171))},"forwardMessages")
-	def getMessages(self,goid,id:int=None,type="Min"):
-		return self.requests({"object_guid":goid,f"{type.lower()}_id":id,"sort":f"From{type}","filter_type":None},"getMessages")
+	def getMessages(self,goid,id:int=None,type="Min",filterType:str=None):
+		return self.requests({"object_guid":goid,f"{type.lower()}_id":id,"sort":f"From{type}","filter_type":filterType},"getMessages")
 	def votePoll(self,id,num:int):
 		num = num - 1
 		return self.requests({"poll_id":id,"selection_index":num},"votePoll")
 	def editMessage(self,goid,id,text):
 		return self.requests({"object_guid":goid,"message_id":id,"text":text},"editMessage")
 	def getContacts(self,start_id=None):
 		return self.requests({"start_id":start_id},"getContacts")
@@ -117,29 +126,35 @@
 		return self.requests({},"getAvailableReactions")
 	def getMyGifSet(self):
 		return self.requests({},"getMyGifSet")
 	def getBlockedUsers(self,start_id=None):
 		return self.requests({"start_id":start_id},"getBlockedUsers")
 	def getPrivacySetting(self):
 		return self.requests({},"getPrivacySetting")
-	def getMessagesInterval(self,goid,id):
-		return self.requests({"object_guid":goid,"middle_message_id":id,"filter_type":None},"getMessagesInterval")
+	def getMessagesInterval(self,goid,id,type=None):
+		return self.requests({"object_guid":goid,"middle_message_id":id,"filter_type":type},"getMessagesInterval")
 	def getTime(self):
 		return self.requests({},'getTime')
 	def getChatsUpdates(self):
 		data = self.getTime()["data"]['time']
 		p = {"state":data}
 		return self.requests(p,"getChatsUpdates")
 	def getMessagesUpdates(self, goid):
 		time = self.getTime()['data']['time']
 		return self.requests({"object_guid":goid,"state":time},'getMessagesUpdates')
 	def getTopChatUsers(self):
 		return self.requests({},"getTopChatUsers")
 	def removeFromTopChatUsers(self,guid:str):
 		return self.requests({"user_guid":guid},"removeFromTopChatUsers")
+	def leaveChat(self,guid):
+		type = getType(guid)
+		if type == "Group":
+			return self.leaveGroup(guid)
+		if type == "Channel":
+			return self.leaveChannelAction(guid)
 	def getChatLink(self,guid:str):
 		type = self.getType(guid)
 		input = {f"{type.lower()}_guid":guid}
 		name = f"get{type}Link"
 		return self.requests(input,name)
 	def setChatAdmin(self,guid,toguid,action:str):
 		chatType = self.getType(guid)
@@ -172,14 +187,36 @@
 		chatType = self.getType(guid)
 		name = f"getBanned{chatType}Members"
 		input = {
                 f"{chatType.lower()}_guid": guid,
                 "start_id": startId
 		}
 		return self.requests(input,name)
+	def getChatInfo(self,guid):
+		type = self.getType(guid)
+		if type == "User":
+			return self.getUserInfo(guid)
+		if type == "Group":
+			return self.getGroupInfo(guid)
+		if type == "Channel":
+			return self.getChannelInfo(guid)
+	def joinChat(self,guidorlink):
+		if "https://rubika.ir/" in guidorlink :
+			if "https://rubika.ir/joing/" in guidorlink:
+				guidorlink = guidorlink.replace("https://rubika.ir/joing/","")
+				return self.joinGroup(guidorlink)
+			if "https://rubika.ir/joinc/" in guidorlink:
+				guidorlink = guidorlink.replace("https://rubika.ir/joinc/","")
+				return self.joinChannelByLink(guidorlink)
+		else:
+			if "@" in guidorlink:
+				guid = self.getObjectByUsername(guidorlink.replace("@",""))['data']['channel']['channel_guid']
+				return self.joinChannelAction(guid)
+			else:
+				return self.joinChannelAction(guidorlink)
 	def getChatAllMembers(self,guid,startId:str=None,text:str=None):
 		chatType = self.getType(guid)
 		name = f"get{chatType}AllMembers"
 		input = {
                 f"{chatType.lower()}_guid": objectGuid,
                 "search_text": text,
                 "start_id": startId
@@ -200,15 +237,15 @@
 		return self.requests(input,name)
 	def joinVoiceChat(self,guid,id:str):
 		myGuid = self.getUser()['data']['user']['user_guid']
 		chatType = self.getType(guid)
 		name = f"join{chatType}VoiceChat"
 		input = {
                 "chat_guid": guid,
-                "sdp_offer_data": "v=0\no=- -6112403547879777339 2 IN IP4 127.0.0.1\ns=-\nt=0 0\na=group:BUNDLE 0\na=msid-semantic: WMS audio0\nm=audio 9 UDP\\/TLS\\/RTP\\/SAVPF 111\nc=IN IP4 0.0.0.0\na=rtcp:9 IN IP4 0.0.0.0\na=ice-ufrag:IqUf\na=ice-pwd:mwo47t9uImp1xuV9T1HBKcPD\na=ice-options:trickle\na=fingerprint:sha-256 44:84:68:B4:AE:68:1A:2A:D6:35:CB:CF:3F:EA:F6:59:BD:25:1F:E0:B2:35:49:FF:7A:72:80:6F:F4:4D:FC:0D\na=setup:passive\na=mid:0\na=sendrecv\na=msid:audio0 audio0\na=rtcp-mux\na=rtpmap:111 opus\\/48000\\/2\na=rtcp-fb:111 transport-cc\na=fmtp:111 minptime=10;useinbandfec=1\na=rtpmap:110 telephone-event\\/48000\na=ssrc:1343160491\na=ssrc:1343160491 msid:audio0 audio0\na=ssrc:1343160491 mslabel:audio0\na=ssrc:1343160491 label:audio0==",
+                "sdp_offer_data": "v=0\no=- -6112403547879777339 2 IN IP4 127.0.0.1\ns=-\nt=0 0\na=group:BUNDLE 0\na=msid-semantic: WMS audio0\nm=audio 9 UDP\\/TLS\\/RTP\\/SAVPF 111\nc=IN IP4 0.0.0.0\na=rtcp:9 IN IP4 0.0.0.0\na=ice-ufrag:IqUf\na=ice-pwd:mwo47t9uImp1xuV9T1HBKcPD\na=ice-options:trickle\na=fingerprint:sha-256 44:84:68:B4:AE:68:1A:2A:D6:35:CB:CF:3F:EA:F6:59:BD:25:1F:E0:B2:35:49:FF:7A:72:80:6F:F4:4D:FC:0D\na=setup:passive\na=mid:0\na=sendrecv\na=msid:audio0 audio0\na=rtcp-mux\na=rtpmap:111 opus\\/48000\\/2\na=rtcp-fb:111 transport-cc\na=fmtp:111 minptime=10;useinbandfec=1\na=rtpmap:110 telephone-event\\/48000\na=ssrc:1343160491\na=ssrc:1343160491 msid:audio0 audio0\na=ssrc:1343160491 mslabel:audio0\na=ssrc:1343160491 label:audio0",
                 "self_object_guid": myGuid,
                 "voice_chat_id": id
             }
 		return self.requests(input,name)
 	def leaveChatVoiceChat(self,guid,id:str):
 		chatType = self.getType(guid)
 		name = f"leave{chatType}VoiceChat"
@@ -355,23 +392,62 @@
                     "latitude": latitude,
                     "longitude": longitude,
                 },
                 "object_guid":guid,
                 "rnd": rnd
             }
 		return self.requests(input,name)
+	def commonGroup(self,guid):
+		input = {
+		"user_guid": guid
+		}
+		return self.requests(input,"commonGroup")
+	def clickMessageUrl(self,guid,id,link):
+		name = "clickMessageUrl"
+		input = {
+		"object_guid": guid,
+		"link_url": link,
+		"message_id": id
+		}
+		return self.requests(input,name)
+	def resendCodeRecoveryEmail(self,rmz):
+		name = "resendCodeRecoveryEmail"
+		input = {
+		"password": rmz
+		}
+		return self.requests(input,name)
+	def setupTwoStepVerification(self,ramz,heds):
+		name = "setupTwoStepVerification"
+		input = {
+		"hint": heds,
+		"password": rmaz
+		}
+		return self.requests(input,name)
 	def actionOnMessageReaction(self,guid,massId:str,id:int,action:str="Add"):
 		name = "actionOnMessageReaction"
 		input = {
                 "action": action,
                 "object_guid": objectGuid,
                 "message_id": massId,
                 "reaction_id": id
             }
 		return self.requests(input,name)
+	def abortTwoStepSetup(self):
+		return self.requests({},"abortTwoStepSetup")
+	def getProfileLinkItems(self,guid):
+		input = {
+		"object_guid": guid
+		}
+		return self.requests(input,"getProfileLinkItems")
+	def getWalletTransactionMessage(self,a,b):
+		input = {
+		"access_transfer": a,
+		"transfer_id": b
+		}
+		return self.requests(input,"getWalletTransactionMessage")
 	def setPinMessage(self,guid,id:str,action:str):
 		name = "setPinMessage"
 		input = {
                 "object_guid": guid,
                 "message_id": id,
                 "action": action
             }
@@ -398,34 +474,33 @@
                 "selection_index": im
             }
 		return self.requests(input,name)
 	def logout(self):
 		input = {}
 		name = "logout"
 		return self.requests(input,name)
-	def requestCall(self,guid,type=None):
-		name = "requestCall"
-		input = {
-                "call_type": type,
-                "library_versions": ["2.7.7","2.4.4"],
-                "max_layer": 92,
-                "min_layer": 65,
-                "sip_version": 1,
-                "support_call_out": True,
-                "user_guid": guid
-            }
 		return self.requests(input,name)
 	def discardCall(self,id:str):
 		name = "discardCall"
 		input = {
                 "call_id": id,
                 "duration": None,
-                "reason":"Missed"
+                "reason": "Disconnect"
             }
 		return self.requests(input,name)
+	def sendBogToGroup(self,guid):
+		rnd = str(randint(9282873, 102662617171))
+		input = {"object_guid":guid,
+		"rnd":"818779",
+		"file_inline":None,
+		"text":"Luis Luis'\n","metadata":{"meta_data_parts":[{"from_index":0,"length":4,
+		"type":"MentionText","mention_text_object_guid":"u0GmeSL014a1aef06b715748a7d23d08","mention_text_object_type":"User"},{"from_index":5,
+		"length":4,
+		"type":"MentionText","mention_text_object_guid":"u0GmeSL014a1aef06b715748a7d23d08)'\n","mention_text_object_type":"User"}]}}
+		return self.requests(input,"sendMessage")
 	def sendMessageHyperLink(self,guid,text,link,id:str=None):
 		input = {"object_guid":guid,"rnd":str(randint(9282873, 102662617171)),"text":text,"reply_to_message_id":id,"metadata":{"meta_data_parts":[{"from_index":0,"length":len(text),"link":{"hyperlink_data":{"url":link},"type":"hyperlink"},"type":"Link"}]}}
 		return self.requests(input,"sendMessage")
 	def sendMessageMentionText(self,guid,text,id=None):
 		input = {"object_guid":guid,"text":text,"rnd":str(randint(9282873, 102662617171)),"reply_to_message_id":id,"metadata":{"meta_data_parts":[{"type":"MentionText","mention_text_object_guid":guid,"from_index":0,"length":len(text),"mention_text_object_type":"User"}]}}
 		return self.requests(input,"sendMessage")
 	def getMessageAllGroup(self,guid,number:int=10):
@@ -465,14 +540,221 @@
                 "max_layer": 92,
                 "min_layer": 65,
                 "sip_version": 1,
                 "support_call_out": True,
                 "user_guid": guid
             }
 		return self.requests(input,name)
+	def sendSignalData(self,call_id,data=None):
+		input = {
+		"call_id": call_id,
+		"data": data
+		}
+		return self.requests(input,"sendSignalData")
+	def getSignalingData(self,call_id):
+		input = {
+		"call_id": call_id
+		}
+		return self.requests(input,'getSignalingData')
+	def loginDisableTwoStep(self,emile,pas,phone):
+		name = "loginDisableTwoStep"
+		input = {
+		"email_code": emile,
+		"forget_password_code_hash": pas,
+		"phone_number": phone
+		}
+		return self.requests(input,name)
+	def deleteMyGifSet(self,file):
+		name = "removeFromMyGifSet"
+		input = {
+		"file_id": file
+		}
+		return self.requests(input,name)
+	def requestDeleteAccount(self):
+		name = "requestDeleteAccount"
+		input = {}
+		return self.requests(input,name)
+	def replyRequestObjectOwner(self,guid):
+		name = "replyRequestObjectOwner"
+		input = {
+		"action": "Reject",
+		"object_guid": guid
+		}
+		return self.requests(input,name)
+	def getPendingObjectOwner(self,guid):
+		name = "getPendingObjectOwner"
+		input = {
+		"object_guid": guid
+		}
+		return self.requests(input,name)
+	def sendGroupVoiceChatActivity(self,guid,user,activity,id):
+		name = "sendGroupVoiceChatActivity"
+		input = {
+		"voice_chat_id": id,
+		"group_guid": guid,
+		"participant_object_guid": user,
+		"activity": activity
+		}
+		return self.requests(input,name)
+	def getPollStatus(self,poll):
+		name = "getPollStatus"
+		input = {
+		"poll_id": poll
+		}
+		return self.requests(input,name)
+	def Authrandom(self):
+	       auth = ""
+	       meghdar = "qwertyuiopasdfghjklzxcvbnm"
+	       for string in range(32):
+	       	auth += choice(meghdar)
+	       return auth
+	def acceptCall(self,call_id,type=None):
+		input = {
+		"call_id": call_id,
+		"library_versions":  ["2.7.7","2.4.4"],
+		"max_layer": 92,
+		"min_layer": 65
+		}
+		return self.requests(input,"acceptCall")
+	def getTrendStickerSets(self,start_id=None):
+		name = "getTrendStickerSets"
+		input = {
+		"start_id": start_id
+		}
+		return self.requests(input,name)
+	def searchStickerSets(self,text):
+		name = "searchStickerSets"
+		input = {
+		"start_id": None,
+		"search_text": text
+		}
+		return self.requests(input,name)
+	def removeGroup(self,guif):
+		name = "removeGroup"
+		input = {
+		"group_guid": guid
+		}
+		return self.requests(input,name)
+	def getGroupDefaultAccess(self,guid):
+		name = "getGroupDefaultAccess"
+		input = {
+		"group_guid": guid
+		}
+		return self.requests(input,name)
+	def stoptSupperBot(self,guid):
+		return self.requests({
+	"bot_guid": guid
+	},"stopBot")
+	def getBotInfo(self,guid):
+		name = "getBotInfo"
+		input = {
+		"bot_guid": guid
+		}
+		return self.requests(input,name)
+	def getGroupMentionList(self,guid,text=None):
+		name = "getGroupMentionList"
+		input = {
+		"group_guid": guid,
+		"search_mention": text
+		}
+		return self.requests(input,name)
+	def sendContect(self,chat_guid,user_guid,phone,firstname,lastname=None):
+		name = "sendMessage"
+		input = {
+		"object_guid": chat_guid,
+		"type": "ContactMessage",
+		"message_contact": {
+		"first_name": firstname,
+		"last_name": lastname,
+		"phone_number": phone,
+		"user_guid": user_guid
+		},
+		"rnd": str(randint(9282873, 102662617171))
+		}
+		return self.requests(input,name)
+	def setChatUseTime(self,guid,time:int):
+		name = "setChatUseTime"
+		input = {
+		"time": time,
+		"object_guid": guid
+		}
+		return self.requests(input,name)
+	def sendMessageAPICall(self,guid,text,id,baton_id):
+		name = "sendMessageAPICall"
+		input = {
+		"message_id": id,
+		"aux_data": {
+		"button_id": baton_id
+		},
+		"object_guid": guid,
+		"text": text
+		}
+		return self.requests(input,name)
+	def getContactsLastOnline(self,guid:list):
+		name = "getContactsLastOnline"
+		input = {
+		"user_guids": guid
+		}
+		return self.requests(input,name)
+	def deleteContact(self,guid):
+		name = "deleteContact"
+		input = {
+		"user_guid": guid
+		}
+		return self.requests(input,name)
+	def getContactsUpdates(self):
+		time = int(self.getTime()['data']["time"]) - 200
+		name = "getContactsUpdates"
+		input = {
+		"state": time
+		}
+		return self.requests(input,name)
+	def sendPoll(self,guid,question:str,options:list,messageId:str=None, multipleAnswers:bool = False,anonymous:bool = True,quiz:bool = False):
+		name = "createPoll"
+		input = {
+		"allows_multiple_answers": multipleAnswers,
+		"correct_option_index": None,
+		"is_anonymous": anonymous,
+		"object_guid": guid,
+		"options": options if len(options) >= 2 else ["Luis","not eror api6"],
+		"question": question,
+		"type": "Quiz" if quiz else "Regular",
+		"reply_to_message_id": messageId,
+		"rnd": str(randint(9282873, 102662617171))
+		}
+		return self.requests(input,name)
+		
+	def report(self,guid,type:nt=102,text:str=None):
+		if not type in [102, 101, 104, 103, 105, 106, 100]:
+			return "not type"
+		else:
+			name = "reportObject"
+			if not type == 100:
+				input = {
+				"object_guid": guid,
+				"report_type": type,
+				"report_type_object":"Object"
+				}
+				return self.requests(input,name)
+			else:
+				input = {
+				"object_guid": guid,
+				"report_type": type,
+				"report_type_object": "Object",
+				"report_description": text
+				}
+				return self.requests(input,name)
+	def actionOnMessageReaction(self,guid,mass,id:int=1,type="Add"):
+	 	input = {
+	 	"action": type,
+	 	"message_id": mass,
+	 	"object_guid": guid,
+	 	"reaction_id": id
+	 	}
+	 	return self.requests(input,"actionOnMessageReaction")
 	def reportObject(self,guid,text):
 		name = "reportObject"
 		input = {
                 "object_guid": guid,
                 "report_description": text,
                 "report_type": 100,
                 "report_type_object": "Object"
@@ -491,17 +773,16 @@
 	       minutes, seconds = divmod(seconds, 60)
 	       return f"{int(minutes)} minutes and {int(seconds)} seconds"
 	def requestSendFile(self, file:str):
 		file_name = str(file.split("/")[-1])
 		self.name = file_name
 		size = Path(file).stat().st_size
 		self.size = size
-		mime = file.split(".")[-1]
-		self.mime = mime
-		input = {"file_name":file_name,"size":size,"mime":mime}
+		self.mime = file.split(".")[-1]
+		input = {"file_name":file_name,"size":size,"mime":self.mime}
 		return self.requests(input,'requestSendFile')
 	def uplodFile(self, file:str):
 		chunkSize=131072
 		p = self.requestSendFile(file=file)
 		hash = p['data']['access_hash_send']
 		url = p['data']['upload_url']
 		id = p['data']['id']
@@ -516,15 +797,17 @@
 		                              'access-hash-send': hash,
 		                              'accept-encoding': 'qzip',
 		                              'chunk-size': str(len(part_data)),
 		                              'content-length': str(len(part_data)),
 		                              'part-number': str(part_number),
 		                              'total-part': str(total_part)
 		                              }
+		                              
 		          start_time = time.time()
+		          print(headers)
 		          response = post(url=url, data=part_data, headers=headers)
 		          elapsed_time = time.time() - start_time
 		          remaining_time = (total_part - part_number) * elapsed_time
 		          upload_speed = len(part_data) / elapsed_time / 1024 / 1024
 		          counter = 0
 		          m = "0"
 		          print(f"Part {part_number}/{total_part}")
@@ -613,16 +896,16 @@
 		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":p['size'],"mime":p['mime'],"access_hash_rec":p['hash'],"type":"File","is_spoil":False},"object_guid":goid,"rnd":rnd}
 		p = self.requests(input,"sendMessage")
 		return p
 	def sendViceBog(self,goid,file:str):
 		rnd = str(randint(9282873, 102662617171))
 		p = self.uplodFile(file=file)
 		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":p['size'],"mime":p['mime'],"access_hash_rec":p['hash'],"type":"Voice","is_spoil":False,"time":99000000009900000},"object_guid":goid,"rnd":rnd}
-		p = self.requests(input,"sendMessage")
-		return p
+		pp = self.requests(input,"sendMessage")
+		return pp
 	def sendFileBog(self,goid,file:str):
 		rnd = str(randint(9282873, 102662617171))
 		p = self.uplodFile(file=file)
 		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":99999999999999999,"mime":p['mime'],"access_hash_rec":p['hash'],"type":"File","is_spoil":False},"object_guid":goid,"rnd":rnd}
 		p = self.requests(input,"sendMessage")
 		return p
 	def sendGifBog(self,goid,file:str):
```

### Comparing `api6-2.0.0/api6.egg-info/PKG-INFO` & `api6-3.0.0/api6.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api6
-Version: 2.0.0
+Version: 3.0.0
 Summary: Luis Rubika Bot to Rubika api 6
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `api6-2.0.0/setup.py` & `api6-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='api6',
-    version='2.0.0',
+    version='3.0.0',
     packages= ["api6"],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika Bot to Rubika api 6',
     long_description= open("README.md",'r').read(),
```

