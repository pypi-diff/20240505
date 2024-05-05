# Comparing `tmp/dublib-0.6.0.tar.gz` & `tmp/dublib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dublib-0.6.0.tar", last modified: Tue Apr 30 18:08:11 2024, max compression
+gzip compressed data, was "dublib-0.6.1.tar", last modified: Sun May  5 08:40:29 2024, max compression
```

## Comparing `dublib-0.6.0.tar` & `dublib-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 18:08:06.000000 dublib-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 18:08:11.317566 dublib-0.6.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-04-30 18:08:06.000000 dublib-0.6.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-04-30 18:08:06.000000 dublib-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 18:08:11.317566 dublib-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.313566 dublib-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.313566 dublib-0.6.0/src/dublib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/src/dublib/Exceptions/
--rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/TelebotUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/WebRequestor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Exceptions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10447 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Polyglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/StyledPrinter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14733 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/TelebotUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/Terminalyzer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/WebRequestor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:06.000000 dublib-0.6.0/src/dublib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 18:08:11.317566 dublib-0.6.0/src/dublib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 18:08:11.000000 dublib-0.6.0/src/dublib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.146376 dublib-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-05 08:40:20.000000 dublib-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 08:40:29.146376 dublib-0.6.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-05-05 08:40:20.000000 dublib-0.6.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-05 08:40:20.000000 dublib-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 08:40:29.146376 dublib-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.138376 dublib-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib/Exceptions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      624 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      680 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/TelebotUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5427 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      616 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/WebRequestor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Exceptions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10447 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Polyglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/StyledPrinter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15562 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/TelebotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42914 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/Terminalyzer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30855 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/WebRequestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:20.000000 dublib-0.6.1/src/dublib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 08:40:29.142376 dublib-0.6.1/src/dublib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-05 08:40:29.000000 dublib-0.6.1/src/dublib.egg-info/top_level.txt
```

### Comparing `dublib-0.6.0/LICENSE` & `dublib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/PKG-INFO` & `dublib-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `dublib-0.6.0/README.md` & `dublib-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/pyproject.toml` & `dublib-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "cython"]
 
 [project]
 name = "dublib"
-version = "0.6.0"
+version = "0.6.1"
 description = "Коллекция модулей от DUB1401."
 authors = [
 	{name = "DUB1401", email = "vlad.milosta@outlook.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
@@ -35,8 +35,8 @@
     "pyTelegramBotAPI"
 ]
 
 [project.urls]
 Documentation = "https://github.com/DUB1401/dublib/tree/main/docs"
 "Source Code" = "https://github.com/DUB1401/dublib"
 "Bug Tracker" = "https://github.com/DUB1401/dublib/issues"
-Changelog = "https://github.com/DUB1401/dublib/releases"
+Changelog = "https://github.com/DUB1401/dublib/releases"
```

### Comparing `dublib-0.6.0/src/dublib/Exceptions/StyledPrinter.py` & `dublib-0.6.1/src/dublib/Exceptions/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/Exceptions/TelebotUtils.py` & `dublib-0.6.1/src/dublib/Exceptions/TelebotUtils.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/Exceptions/Terminalyzer.py` & `dublib-0.6.1/src/dublib/Exceptions/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/Exceptions/WebRequestor.py` & `dublib-0.6.1/src/dublib/Exceptions/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/Methods.py` & `dublib-0.6.1/src/dublib/Methods.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/Polyglot.py` & `dublib-0.6.1/src/dublib/Polyglot.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/StyledPrinter.py` & `dublib-0.6.1/src/dublib/StyledPrinter.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/TelebotUtils.py` & `dublib-0.6.1/src/dublib/TelebotUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .Methods import ReadJSON, WriteJSON
 from .Exceptions.TelebotUtils import *
 
-from telebot.types import Message, User
+from telebot.types import User
 
 import os
 
 #==========================================================================================#
 # >>>>> УПРАВЛЕНИЕ ПОЛЬЗОВАТЕЛЯМИ <<<<< #
 #==========================================================================================#
 
@@ -56,28 +56,28 @@
 		# Запись локального файла.
 		WriteJSON(self.__StorageDirectory + f"/{self.__ID}.json", self.__Data)
 
 	#==========================================================================================#
 	# >>>>> ПУБЛИЧНЫЕ МЕТОДЫ <<<<< #
 	#==========================================================================================#
 
-	def __init__(self, dir: str, user_id: int, data: dict | None = None):
+	def __init__(self, storage_dir: str, user_id: int, data: dict | None = None):
 		"""
 		Объектное представление данных пользователя.
-			dir – путь к директории хранения данных;
+			storage_dir – путь к директории хранения данных;
 			user_id – ID пользователя;
 			data – словарь с описанием данных пользователя для инициализации (если не передан, данные будут загружены из файла).
 		"""
 
 		#---> Генерация динамических свойств.
 		#==========================================================================================#
 		# ID пользователя.
 		self.__ID = user_id
 		# Директория хранилища.
-		self.__StorageDirectory = dir.replace("\\", "/").rstrip("/")
+		self.__StorageDirectory = storage_dir.replace("\\", "/").rstrip("/")
 		# Словарное представление данных пользователя.
 		self.__Data = {
 			"username": None,
 			"language": None,
 			"is_premium": None,
 			"permissions": [],
 			"data": {}
@@ -125,14 +125,28 @@
 				IsChanged = True
 
 		# Если список разрешений изменён, отсортировать его.
 		if IsChanged: self.__Data["permissions"] = sorted(self.__Data["permissions"])
 		# Сохранение данных.
 		self.__SaveData()
 
+	def create_property(self, key: str, value: any):
+		"""
+		Создаёт свойство пользователя и задаёт ему значение, если такового ещё не существует.
+			key – ключ свойства;
+			value – значение.
+		"""
+		
+		# Если свойства не существует.
+		if key not in self.__Data["data"].keys():
+			# Создание свойства.
+			self.__Data["data"][key] = value
+			# Сохранение данных.
+			self.__SaveData()
+
 	def get_property(self, key: str) -> any:
 		"""
 		Возвращает значение свойства пользователя.
 			key – ключ свойства.
 		"""
 
 		return self.__Data["data"][key]
@@ -178,27 +192,40 @@
 			if Permission in self.__Data["permissions"]:
 				# Удаление разрешения.
 				self.__Data["permissions"].remove(Permission)
 
 		# Сохранение данных.
 		self.__SaveData()
 
+	def remove_property(self, key: str):
+		"""
+		Удаляет свойство пользователя.
+			key – ключ свойства.
+		"""
+
+		# Если свойство существует.
+		if key in self.__Data["data"].keys():
+			# Удаление свойства.
+			del self.__Data["data"][key]
+			# Сохранение данных.
+			self.__SaveData()
+
 	def set_property(self, key: str, value: any):
 		"""
-		Обновляет значение свойства пользователя.
+		Обновляет значение существующего свойства пользователя.
 			key – ключ свойства;
 			value – значение.
 		"""
 		
-		# Если ключа данных не существует, создать его.
-		if "data" not in self.__Data.keys(): self.__Data["data"] = dict()
-		# Помещение данных.
-		self.__Data["data"][key] = value
-		# Сохранение данных.
-		self.__SaveData()
+		# Если свойство существует.
+		if key in self.__Data["data"].keys():
+			# Обновление данных.
+			self.__Data["data"][key] = value
+			# Сохранение данных.
+			self.__SaveData()
 
 	def update(self, user: User):
 		"""
 		Обновляет данные пользователя из параметров, содержащихся в сообщении.
 			user – объект представления пользователя.
 		"""
 
@@ -294,34 +321,34 @@
 		self.__StorageDirectory = dir.replace("\\", "/").rstrip("/")
 
 		# Если директория пользователей не существует, создать её.
 		if not os.path.exists(self.__StorageDirectory): os.makedirs(self.__StorageDirectory)
 		# Загрузка данных пользователей.
 		self.__LoadUsers()
 
-	def auth(self, message: Message) -> UserData:
+	def auth(self, user: User) -> UserData:
 		"""
 		Выполняет идентификацию и обновление данных существующего пользователя или создаёт локальный файл для нового.
-			message – структура описания сообщения.
+			user – структура описания пользователя Telegram.
 		"""
 		
 		# Текущий пользователь.
-		User = None
+		CurrentUser = None
 
 		# Если пользователь ещё не существует.
-		if message.from_user.id not in self.__Users.keys():
+		if user.id not in self.__Users.keys():
 			# Создание нового пользователя.
-			self.__Users[message.from_user.id] = UserData(self.__StorageDirectory, message.from_user.id, message.from_user)
+			self.__Users[user.id] = UserData(self.__StorageDirectory, user.id, user)
 
 		# Обновление данных пользователя.
-		self.__Users[message.from_user.id].update(message.from_user)
+		self.__Users[user.id].update(user)
 		# Установка текущего пользователя.
-		User = self.__Users[message.from_user.id]
+		CurrentUser = self.__Users[user.id]
 
-		return User
+		return CurrentUser
 
 	def get_user(self, user_id: int | str) -> UserData:
 		"""
 		Возвращает объект данных пользователя.
 			user_id – ID пользователя.
 		"""
```

### Comparing `dublib-0.6.0/src/dublib/Terminalyzer.py` & `dublib-0.6.1/src/dublib/Terminalyzer.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib/WebRequestor.py` & `dublib-0.6.1/src/dublib/WebRequestor.py`

 * *Files identical despite different names*

### Comparing `dublib-0.6.0/src/dublib.egg-info/PKG-INFO` & `dublib-0.6.1/src/dublib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dublib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Коллекция модулей от DUB1401.
 Author-email: DUB1401 <vlad.milosta@outlook.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `dublib-0.6.0/src/dublib.egg-info/SOURCES.txt` & `dublib-0.6.1/src/dublib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

