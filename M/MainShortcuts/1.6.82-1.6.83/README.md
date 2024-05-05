# Comparing `tmp/mainshortcuts-1.6.82.tar.gz` & `tmp/mainshortcuts-1.6.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.82.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.83.tar", max compression
```

## Comparing `mainshortcuts-1.6.82.tar` & `mainshortcuts-1.6.83.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.82/README.md
--rwxr-xr-x   0        0        0      696 2024-04-26 04:58:29.000000 mainshortcuts-1.6.82/pyproject.toml
--rwxr-xr-x   0        0        0     6027 2024-03-18 12:04:56.000000 mainshortcuts-1.6.82/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0      937 2024-04-26 04:58:23.000000 mainshortcuts-1.6.82/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      456 2024-01-13 08:00:52.000000 mainshortcuts-1.6.82/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     6649 2024-03-18 10:53:54.000000 mainshortcuts-1.6.82/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0      890 2024-03-18 10:58:02.000000 mainshortcuts-1.6.82/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1467 2024-03-18 11:02:06.000000 mainshortcuts-1.6.82/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     3230 2024-04-25 01:47:08.000000 mainshortcuts-1.6.82/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     2852 2024-03-18 11:17:08.000000 mainshortcuts-1.6.82/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     5877 2024-03-18 11:35:14.000000 mainshortcuts-1.6.82/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     2672 2024-04-26 04:58:16.000000 mainshortcuts-1.6.82/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3649 2024-04-12 17:48:30.000000 mainshortcuts-1.6.82/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2120 2024-03-18 11:57:28.000000 mainshortcuts-1.6.82/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.82/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.82/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6163 2024-03-18 12:10:52.000000 mainshortcuts-1.6.82/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      783 2024-03-18 12:11:44.000000 mainshortcuts-1.6.82/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.82/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0      937 2024-03-18 12:15:06.000000 mainshortcuts-1.6.82/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    14794 2024-03-18 12:16:26.000000 mainshortcuts-1.6.82/src/MainShortcuts/values.py
--rwxr-xr-x   0        0        0     1194 2024-04-26 04:58:07.000000 mainshortcuts-1.6.82/src/MainShortcuts/win.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.82/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.83/README.md
+-rwxr-xr-x   0        0        0      696 2024-05-05 16:39:22.000000 mainshortcuts-1.6.83/pyproject.toml
+-rwxr-xr-x   0        0        0     6053 2024-04-28 12:31:10.000000 mainshortcuts-1.6.83/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0      937 2024-05-05 16:39:15.000000 mainshortcuts-1.6.83/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      465 2024-04-28 11:33:14.000000 mainshortcuts-1.6.83/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     4772 2024-04-28 11:54:48.000000 mainshortcuts-1.6.83/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0     1003 2024-05-01 01:56:58.000000 mainshortcuts-1.6.83/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1472 2024-04-28 11:59:24.000000 mainshortcuts-1.6.83/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     3345 2024-04-28 12:07:16.000000 mainshortcuts-1.6.83/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     2923 2024-04-28 12:09:32.000000 mainshortcuts-1.6.83/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     5925 2024-04-28 12:17:10.000000 mainshortcuts-1.6.83/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     2672 2024-05-05 16:39:08.000000 mainshortcuts-1.6.83/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3603 2024-04-28 12:27:24.000000 mainshortcuts-1.6.83/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2174 2024-04-28 12:29:34.000000 mainshortcuts-1.6.83/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.83/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.83/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6265 2024-04-28 12:35:16.000000 mainshortcuts-1.6.83/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      789 2024-04-28 12:36:52.000000 mainshortcuts-1.6.83/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.83/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0      983 2024-04-28 12:40:04.000000 mainshortcuts-1.6.83/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    14818 2024-04-28 12:41:38.000000 mainshortcuts-1.6.83/src/MainShortcuts/values.py
+-rwxr-xr-x   0        0        0     1194 2024-04-26 04:58:06.000000 mainshortcuts-1.6.83/src/MainShortcuts/win.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.83/PKG-INFO
```

### Comparing `mainshortcuts-1.6.82/README.md` & `mainshortcuts-1.6.83/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.82/pyproject.toml` & `mainshortcuts-1.6.83/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
-version = "1.6.82"
-name = "mainshortcuts"
+version = "1.6.83"
+name = "MainShortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
 ]
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.83/src/MainShortcuts/MainCore.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class _MainCore:
   """Переменные:
   .args - то же самое, что и sys.argv
   .dir - папка с текущей программой (использует __file__)
   .execdir - если программа находится в папке "_internal", указана родительская папка
   .embed - тексты для всраивания MainCore в программу
   .run - запущена ли программа или её импортируют? (использует __name__)"""
-  def __init__(self,color=True,*,__name__,__file__):
+  def __init__(self,color:bool=True,*,__name__,__file__):
     self.args=sys.argv
     self.core_name="MainCore"
     self.core_version=5
     self.dir=os.path.dirname(__file__) # Папка, в которой находится программа
     self.execdir=self.dir # Если программа собрана через "pyinstaller --onedir", указывает папку с исполняемым файлом
     try:
       tmp=os.path.split(self.dir)
@@ -106,27 +106,27 @@
         self.colors["RESET"]=clr.Style.RESET_ALL
         self.colors["WHITE"]=clr.Fore.WHITE
         self.colors["YELLOW"]=clr.Fore.YELLOW
       except:
         color=False
   def __repr__(self):
     return ms.json.encode({"name":self.core_name,"version":self.core_version},mode="c")
-  def cprint(self,a,start="",**kwargs): # Вывести цветной текст | cprint("Обычный текст, {BLUE}Синий текст")
+  def cprint(self,a:str,start:str="",**kwargs): # Вывести цветной текст | cprint("Обычный текст, {BLUE}Синий текст")
     try:
       b=str(a).rstrip().format(**self.colors)
     except KeyError:
       b=str(a).rstrip()
       for k,v in self.colors.items():
         try:
           arg={k:v}
           b=b.format(**arg)
         except KeyError:
           pass
     print(self.colors["RESET"]+self.colors[start]+b.rstrip()+self.colors["RESET"],**kwargs)
-  def cformat(self,a,start=""): # Аналогично cprint, но вывод в return, и нет strip
+  def cformat(self,a:str,start:str="")->str: # Аналогично cprint, но вывод в return, и нет strip
     try:
       b=str(a).format(**self.colors)
     except KeyError:
       b=str(a).rstrip()
       for k,v in self.colors.items():
         try:
           arg={k:v}
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.83/src/MainShortcuts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__=(1,6,82)
+__version_tuple__=(1,6,83)
 __depends__={
   "required":[
     "json",
     "os",
     "platform",
     "shutil",
     "subprocess",
@@ -26,9 +26,9 @@
   "MS-jsonC",
   "MS-jsonP",
   "MS-mkdir",
   ]
 from MainShortcuts.imports import *
 __all__=imports_all.copy()
 __import_errors__=imports_import_errors.copy()
-__version__="{}.{}.{}".format(*__version_tuple__)
 del imports_all,imports_import_errors
+__version__="{}.{}.{}".format(*__version_tuple__)
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.83/src/MainShortcuts/dictplus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class dictplus:
   """Улучшенный словарь
   Можно получить элементы и через dictplus["key"], и через dictplus.key
   Вариант использования через аттрибуты может работать не на все ключи"""
-  def __init__(self,data=None):
+  def __init__(self,data:dict=None):
     """Без аргументов создаётся {}
     Аргументом можно указать любой словарь"""
     if data==None:
       self.__data__={}
     else:
       self.__data__=data.copy()
   def __getattr__(self,k):
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.83/src/MainShortcuts/dir.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,76 @@
+from typing import Union
 import MainShortcuts.path as m_path
 import os as _os
 import shutil as _shutil
-def create(path,force=False):
+def create(path:str,force:bool=False)->bool:
   """Создать папку
   Если путь существует, ничего не делает
   force - принудительно создать папку (удалит файл, который находится на её месте)"""
   if m_path.exists(path):
     type=m_path.info(path)["type"]
     if type=="dir":
       return True
     elif force:
       m_path.delete(path)
     else:
       raise Exception("The object exists and is not a folder")
   _os.makedirs(path)
   return True
 mk=create
-def delete(path):
+def delete(path:str):
   """Удалить папку с содержимым
   Если в назначении файл, выдаст ошибку"""
   type=m_path.info(path)["type"]
   if type=="dir":
     _shutil.rmtree(path)
   else:
     raise Exception("Unknown type: "+type)
 rm=delete
-def copy(fr,to,force=False):
+def copy(fr:str,to:str,force:bool=False):
   """Копировать папку с содержимым
   force - принудительно копировать"""
   type=m_path.info(fr)["dir"]
   if type=="dir":
     if m_path.info(to)["type"]!="dir" and force:
       try:
         m_path.delete(to)
       except:
         pass
     _shutil.copytree(fr,to)
   else:
     raise Exception("Unknown type: "+type)
 cp=copy
-def move(fr,to,force=False):
+def move(fr:str,to:str,force:bool=False):
   """Переместить папку с содержимым
   force - принудительно переместить"""
   type=m_path.info(fr)["dir"]
   if type=="dir":
     if m_path.info(to)["type"]!="dir" and force:
       try:
         m_path.delete(to)
       except:
         pass
     _shutil.move(fr,to)
   else:
     raise Exception("Unknown type: "+type)
-def rename(fr,to,force=False):
+def rename(fr:str,to:str,force:bool=False):
   """Переименовать папку
   force - принудительно переименовать"""
   t=m_path.info(fr)["dir"]
   if t=="dir":
     if m_path.info(to)["type"]!="dir" and force:
       try:
         m_path.delete(to)
       except:
         pass
     _os.rename(fr,to)
   else:
     raise Exception("Unknown type: "+t)
-def list(path,files=True,dirs=True,links=None):
+def list(path:str,files:bool=True,dirs:bool=True,links:Union[bool,None]=None):
   """Получить список содержимого папки
   files - True: включать файлы в список
           False: не показывать файлы в списке
   dirs  - True: включать папки в список
           False: не показывать папки в списке
   links - None: показывать всё
           True: показывать только ссылки
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/file.py` & `mainshortcuts-1.6.83/src/MainShortcuts/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 import MainShortcuts.path as m_path
 import os as _os
 import shutil as _shutil
 _open=open
-def read(path,encoding="utf-8"):
+def read(path:str,encoding:str="utf-8"):
   """Прочитать файл как текст
   encoding - кодировка
   Если файла нет, возвращает пустую строку"""
   if _os.path.isfile(path):
     with _open(path,"rb") as f:
       text=f.read().decode(encoding)
   else:
     text=""
   return text
-def write(path,text="",encoding="utf-8",force=False):
+def write(path:str,text:str="",encoding:str="utf-8",force=False):
   """Записать текст в файл
   text - текст для записи
   encoding - кодировка
   force - принудительно создать файл"""
   if _os.path.isdir(path) and force:
     m_path.rm(path)
   with _open(path,"wb") as f:
     f.write(str(text).encode(encoding))
   return True
-def open(path):
+def open(path:str):
   """Прочитать файл как байты
   Если файла нет, возвращает пустые байты"""
   if _os.path.isfile(path):
     with _open(path,"rb") as f:
       content=f.read()
   else:
     content=b""
   return content
 load=open
-def save(path,content=b"",force=False):
+def save(path:str,content=b"",force=False):
   """Записать байты в файл
   content - байты для записи
   force - принудительно создать файл"""
   if _os.path.isdir(path) and force:
     m_path.rm(path)
   with _open(path,"wb") as f:
     f.write(content)
   return True
-def delete(path):
+def delete(path:str):
   """Удалить файл
   Если он не существует, ничего не изменится
   Если на месте папка, выдаст ошибку"""
   type=m_path.info(path)["type"]
   if type=="file":
     m_path.rm(path)
   elif not _os.path.exists(path):
     pass
   else:
     raise Exception("Unknown type: "+type)
-def copy(fr,to,force=False):
+def copy(fr:str,to:str,force:bool=False):
   """Копировать файл
   force - если в месте назначения папка, удалить её"""
   type=m_path.info(fr)["type"]
   if type=="file":
     if m_path.exists(to) and force:
       m_path.delete(to)
     _shutil.copy(fr,to)
   else:
     raise Exception("Unknown type: "+type)
-def move(fr,to,force=False):
+def move(fr:str,to:str,force:bool=False):
   """Переместить файл
   force - если в месте назначения папка, удалить её"""
   type=m_path.info(fr)["type"]
   if type=="file":
     if m_path.exists(to) and force:
       m_path.delete(to)
     _shutil.move(fr,to)
   else:
     raise Exception("Unknown type: "+type)
-def rename(fr,to,force=False):
+def rename(fr:str,to:str,force:bool=False):
   """Переименовать файл
   force - если в месте назначения папка, удалить её"""
   type=m_path.info(fr)["type"]
   if type=="file":
     if m_path.exists(to) and force:
       m_path.delete(to)
     _os.rename(fr,to)
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.83/src/MainShortcuts/fileobj.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   import hashlib as hl
   hl_err=False
 except Exception as e:
   hl_err=e
 class hash:
   """Получить контрольные суммы и размер файла
   Может зависнуть при больших файлах"""
-  def __init__(self,path):
+  def __init__(self,path:str):
     if hl_err!=False:
       raise hl_err
     algs=[
       "blake2b",
       "blake2s",
       "md5",
       "sha1",
@@ -22,29 +22,30 @@
       "sha3_256",
       "sha3_384",
       "sha3_512",
       "sha512",
       ]
     self.size=os.path.getsize(path)
     with open(path,"rb") as f:
+      b=f.read()
       for i in algs:
-        self[i]=getattr(hl,i)(f.read()).hexdigest()
+        self[i]=getattr(hl,i)(b).hexdigest()
   def __getitem__(self,k):
     return getattr(self,k)
   def __setitem__(self,k,v):
     setattr(self,k,v)
 class fileobj:
   """Улучшенная работа с файлом
   Переменные класса:
     .content / .data / .bytes - байты файла (получить/записать)
     .text / .str - текст файла (получить/записать)
     .lines - текстовые линии файла (получить/записать)
     .size - размер файла в байтах. Если force=True и файл отсутствует, возвращает 0
     .exists - существует ли файл?"""
-  def __init__(self,p,encoding="utf-8",force=False,short_names=True):
+  def __init__(self,p:str,encoding:str="utf-8",force:bool=False):
     """
     p - путь к файлу
     encoding - кодировка (при работе с текстом)
     force - принудительно выполнять"""
     if os.path.isdir(p) and not force:
       raise IsADirectoryError("Can't work with folder")
     self.encoding=encoding
@@ -64,26 +65,26 @@
     elif k=="exists":
       return os.path.exists(self.path)
     elif k=="__dict__":
       return self.__dict__
     else:
       return self.__dict__[k]
   def __setattr__(self,k,v):
-    nochange=[
-      "checksum",
-      "copy",
-      "delete",
-      "exists",
-      "link",
-      "move",
-      "open",
-      "read",
-      "save",
-      "size",
-      "write",
+    nochange=[
+      "checksum",
+      "copy",
+      "delete",
+      "exists",
+      "link",
+      "move",
+      "open",
+      "read",
+      "save",
+      "size",
+      "write",
       ]
     if k in ["content","data","bytes"]:
       self.save(v)
     elif k in ["text","str"]:
       self.write(v)
     elif k=="lines":
       self.write("\n".join(list(v)))
@@ -129,87 +130,87 @@
       "size",
       "str",
       "text",
       ]
     return v+f+f2
   def __repr__(self):
     return f"ms.fileobj('{self.path}',encoding='{self.encoding}',force={self.force})"
-  def open(self):
+  def open(self)->bytes:
     """Получить байты из файла"""
     if self.force:
       try:
         with open(self.path,"rb") as f:
           a=f.read()
       except:
         a=b""
     else:
       with open(self.path,"rb") as f:
         a=f.read()
     return a
-  def save(self,v):
+  def save(self,v:bytes):
     """Записать байты в файл"""
     if self.force:
       if os.path.isdir(self.path):
         shutil.rmtree(self.path)
       if type(v)!=bytes:
         v=str(v).encode(self.encoding)
     with open(self.path,"wb") as f:
       a=f.write(v)
     return a
-  def read(self):
+  def read(self)->str:
     """Получить текст из файла"""
     return self.open().decode(self.encoding)
-  def write(self,v):
+  def write(self,v:str):
     """Записать текст в файл"""
     return self.save(v.encode(self.encoding))
   def delete(self):
     """Удалить файл"""
     if os.path.islink(self.path):
       os.unlink(self.path)
     elif os.path.isfile(self.path):
       os.remove(self.path)
     elif os.path.isdir(self.path):
       shutil.rmtree(self.path)
-  def move(self,dest,follow=True):
+  def move(self,dest:str,follow:bool=True):
     """Переместить файл
     follow - следовать за файлом"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
     shutil.move(self.path,dest)
     if follow:
       self.path=dest
-  def copy(self,dest,follow=False):
+  def copy(self,dest:str,follow:bool=False):
     """Копировать файл
     follow - следовать за файлом"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
     shutil.copy(self.path,dest)
     if follow:
       self.path=dest
-  def link(self,dest):
+  def link(self,dest:str):
     """Сделать символическую ссылку на файл"""
     if os.path.exists(dest) and self.force:
       if os.path.islink(dest):
         os.unlink(dest)
       elif os.path.isfile(dest):
         os.remove(dest)
       elif os.path.isdir(dest):
         shutil.rmtree(dest)
     os.symlink(self.path,dest)
-  def checksum(self):
+  def checksum(self)->hash:
     """Получить контрольные суммы и размер файла"""
     return hash(self.path)
   cp=copy
   hash=checksum
   ln=link
   load=open
   mv=move
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.83/src/MainShortcuts/imports.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/json.py` & `mainshortcuts-1.6.83/src/MainShortcuts/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import MainShortcuts.file as m_file
 import MainShortcuts.path as m_path
 import json as _json
 import sys as _sys
 _print=print
-def _obj_encoder(obj,recurse=2,func=lambda k:not k.startswith("_")):
+def _obj_encoder(obj,recurse=2,func=lambda k:not k.startswith("_"))->dict:
   """Преобразование объекта в словарь
   obj - сам объект
   recurse - глубина рекурсивной обработки
   func - фильтр атрибутов"""
   if hasattr(obj,"to_dict"):
     to_dict=getattr(obj,"to_dict")
     if callable(to_dict):
@@ -29,67 +29,63 @@
       v=getattr(obj,k)
       if callable(v):continue
       if type(v) in types:
         d[k]=v
       elif recurse>0:
         d[k]=_obj_encoder(v,recurse=recurse-1)
   return d
-def encode(data,mode="c",indent=2,sort=True,force=True,**kwargs):
+def encode(data,mode:str="c",indent:int=2,sort:bool=True,force:bool=True,**kwargs)->str:
   """Данные в текст JSON
   data - данные для кодирования
   mode - c/compress/min/zip: сжатый JSON
          p/pretty/max/print: развёрнутый JSON
   indent - кол-во отступов в развёрнутом JSON
   sort - сортировка словарей
   force - преобразовывать объекты в словари
   остальные аргументы как в json.dumps"""
   if force:
     kwargs["default"]=_obj_encoder
   kwargs["sort_keys"]=sort
   if mode in ["c","compress","min","zip"]: # Сжатый
     kwargs["separators"]=[",",":"]
-    t=_json.dumps(data,**kwargs)
   elif mode in ["pretty","p","print","max"]: # Развёрнутый
     kwargs["indent"]=int(indent)
-    t=_json.dumps(data,**kwargs)
-  else: # Без параметров
-    t=_json.dumps(data,**kwargs)
-  return t
-def decode(text,**kwargs):
+  return _json.dumps(data,**kwargs)
+def decode(text:str,**kwargs):
   """Текст JSON в данные
   text - текст для декодирования
   остальные аргументы как в json.loads"""
   return _json.loads(str(text),**kwargs)
-def write(path,data,encoding="utf-8",force=False,**kwargs):
+def write(path:str,data,encoding:str="utf-8",force:bool=False,**kwargs):
   """Записать данные в файл JSON
   path - путь к файлу
   data - данные
   encoding - кодировка
   force - если в месте назначения папка, удалить её
   остальные аргументы как в ms.json.encode"""
   if m_path.info(path)["type"]=="dir" and force:
     m_path.rm(path)
   return m_file.write(path,encode(data,**kwargs),encoding=encoding)
-def read(path,encoding="utf-8",**kwargs):
+def read(path:str,encoding:str="utf-8",**kwargs):
   """Прочитать данные из JSON файла
   path - путь к файлу
   encoding - кодировка
   остальные аргументы как в ms.json.decode"""
   return decode(m_file.read(path,encoding=encoding),**kwargs)
-def print(data,file=_sys.stdout,mode="p",**kwargs):
+def print(data,file=_sys.stdout,mode:str="p",**kwargs):
   """Вывести данные в stdout в виде JSON
   mode - как в ms.json.encode
   file - как в print"""
   kwargs["mode"]=mode
   _print(encode(data,**kwargs),file=file)
-def rebuild(text,**kwargs):
+def rebuild(text:str,**kwargs):
   """Перестроить текст JSON
   text - сам текст
   остальные аргументы как в ms.json.encode"""
   return encode(decode(text),**kwargs)
-def rewrite(path,encoding="utf-8",**kwargs):
+def rewrite(path:str,encoding:str="utf-8",**kwargs):
   """Перестроить JSON в файле
   path - путь к файлу
   encoding - кодировка
   остальные аргументы как в ms.json.write"""
   kwargs["encoding"]=encoding
   return write(path,read(path,encoding=encoding),**kwargs)
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/list.py` & `mainshortcuts-1.6.83/src/MainShortcuts/list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
-def filter(a,whitelist=None,blacklist=[],regex=False,begin=None,end=None):
+def filter(a:list,whitelist:list=None,blacklist:list=[],regex:str=False,begin:str=None,end:str=None):
   """Фильтровать список
   whitelist - удалить всё, чего нет в этом списке
   blacklist - удалить всё, что есть в этом списке
   regex - сортировка с регулярным выражением (строки)"""
+  a=list(a)
   if whitelist==None:
     whitelist=a
   if type(whitelist)==str:
     whitelist=[whitelist]
   if type(blacklist)==str:
     blacklist=[blacklist]
   b=[]
@@ -42,15 +43,15 @@
       if (i in whitelist) and (not i in blacklist):
         add=True
       else:
         add=False
     if add:
       b.append(i)
   return b
-def rm_duplicates(a,trim=False,case=False,func=lambda i:i):
+def rm_duplicates(a:list,trim:bool=False,case:bool=False,func=lambda i:i):
   """Удалить дублирующиеся элементы
   trim - True: использовать strip()
          l: использовать lstrip()
          r: использовать rstrip()
   case - lower/upper/capitalize
   func - обработать каждый элемент этой функцией"""
   b=[]
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/main.py` & `mainshortcuts-1.6.83/src/MainShortcuts/main.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/path.py` & `mainshortcuts-1.6.83/src/MainShortcuts/path.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 sep=_os.sep # Разделитель в пути файла
 extsep=_os.extsep # Разделитель в расширении файла
 pathsep=sep
 separator=sep
 pwd=_os.getcwd
 cd=_os.chdir
 exists=_os.path.exists
-def merge(array,sep=pathsep):
+def merge(array:list,sep:str=pathsep):
   """Собрать путь к объекту из массива"""
   return sep.join(array)
-def split(path,sep=pathsep):
+def split(path:str):
   """Разложить путь к объекту на массив"""
-  return path.split(sep)
-def info(path=_os.getcwd(),listdir=False,listlinks=False):
+  return path.replace("\\","/").split("/")
+def info(path:str=_os.getcwd(),listdir:bool=False,listlinks:bool=False)->dict:
   """Информация о файле/папке
   path - путь к объекту
   listdir - если папка, то рекурсивно создать список содержимого и суммарный размер
   listlinks - проверять ссылки при рекурсии?"""
   path=path.replace("\\","/")
   i={
     "dir":None, # Папка, в которой находится объект
@@ -86,15 +86,15 @@
     else:
       i["type"]="unknown"
   i["errors"]=errors
   return i
 class recurse_info:
   """Рекурсивная информация о папке
   В разработке"""
-  def __init__(self,p=_os.getcwd(),links=False):
+  def __init__(self,p:str=_os.getcwd(),links:bool=False):
     self.path=p
     for k,v in info(p,listdir=True,listlinks=links).items():
       self[k]=v
     if self.type=="dir":
       f={}
       d={}
       for i in self.files:
@@ -122,51 +122,51 @@
           myD[k]=self[k]
       for k in dir(other):
         if not k.startswith("_"):
           otD[k]=other[k]
       return myD==otD
     except:
       return False
-def delete(path):
+def delete(path:str):
   """Удалить папку или файл, если существует"""
   if _os.path.exists(path):
     if _os.path.islink(path):
       _os.unlink(path)
     elif _os.path.isfile(path):
       _os.remove(path)
     elif _os.path.isdir(path):
       _shutil.rmtree(path)
     else:
       raise Exception("Unknown type")
 rm=delete
 # del=delete
-def copy(fr,to):
+def copy(fr:str,to:str):
   """Копировать"""
   if _os.path.isfile(fr):
     _shutil.copy(fr,to)
   elif _os.path.isdir(fr):
     _shutil.copytree(fr,to)
   else:
     raise Exception("Unknown type")
 cp=copy
-def move(fr,to):
+def move(fr:str,to:str):
   """Переместить"""
   _shutil.move(fr,to)
 mv=move
-def rename(fr,to):
+def rename(fr:str,to:str):
   """Переименовать"""
   _os.rename(fr,to)
 rn=rename
-def link(fr,to,force=False):
+def link(fr:str,to:str,force:bool=False):
   """Сделать символическую ссылку"""
   if exists(to) and force:
     delete(to)
   _os.symlink(fr,to)
 ln=link
-def format(path,replace_to=None,sep=pathsep):
+def format(path:str,replace_to:str=None,sep=pathsep)->str:
   """Форматировать путь к файлу (изменить разделитель, удалить недопустимые символы)
   replace_to - заменить недопустимые символы на указанный"""
   for i in ["/","\\"]:
     path=path.replace(i,sep)
   if replace_to!=None:
     for i in ["\n",":","*","?","\"","<",">","|","+","%","!","@"]:
       path=path.replace(i,replace_to)
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.83/src/MainShortcuts/proc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 var=_os.environ # Переменные всего процесса
 sp_kwargs={
   "text":True,
   "stdin":_subprocess.PIPE,
   "stdout":_subprocess.PIPE,
   "stderr":_subprocess.PIPE,
   }
-def run(a,*args,**kwargs):
+def run(a,*args,**kwargs)->dict:
   """Запустить процесс (упрощённый subprocess.Popen)"""
   kw=sp_kwargs
   kw.update(kwargs)
   p=_subprocess.Popen(a,*args,**kw)
   code=p.wait()
   out,err=p.communicate()
   r={
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/script.py` & `mainshortcuts-1.6.83/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/str.py` & `mainshortcuts-1.6.83/src/MainShortcuts/str.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-def array2str(a):
+from typing import Union
+def array2str(a:Union[list,tuple])->list:
   """Преобразовать каждый элемент в строку"""
   b=[]
   for i in a:
     b.append(str(i))
   return b
 list2str=array2str
-def dict2str(a):
+def dict2str(a:dict)->dict:
   """Преобразовать каждое значение в строку"""
   b={}
   for key,value in a.items():
     b[key]=str(value)
   return b
 class replace:
-  def multi(text=None,dict=None):
+  def multi(text:str,d:dict)->str:
     """Мульти-замена {"что заменить":"чем заменить"}"""
     t=str(text)
-    for key,value in dict.items():
-      t=t.replace(key,str(value))
+    for k,v in d.items():
+      t=t.replace(k,str(v))
     return t
-  def all(text=None,fr=None,to=None):
+  def all(text:str,fr:str,to:str)->str:
     """Замена пока заменяемый текст не исчезнет"""
     t=str(text)
     a=str(fr)
     b=str(to)
     if a in b:
-      raise endlessCycle('"{0}" is contained in "{1}", this causes an infinite loop'.format(a,b))
+      raise Exception('"{0}" is contained in "{1}", this causes an infinite loop'.format(a,b))
     while a in t:
       t=t.replace(a,b)
     return t
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/values.py` & `mainshortcuts-1.6.83/src/MainShortcuts/values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Модифицированные версии встроенных значений"""
 import builtins,json
 class int:
-  def __init__(self,data=0):
+  def __init__(self,data:int=0):
     self.data=builtins.int(data)
   def __repr__(self):
     return f"ms.values.int({json.dumps(self.data)})"
   def __str__(self):
     return builtins.str(self.data)
   def __neg__(self):
     return self.data.__neg__(self)
@@ -174,15 +174,15 @@
       return self.data.__truediv__(other)
   def __xor__(self,other):
     if type(self)==type(other):
       return self.data.__xor__(other.data)
     else:
       return self.data.__xor__(other)
 class float:
-  def __init__(self,data=0.0):
+  def __init__(self,data:float=0.0):
     self.data=builtins.float(data)
   def __repr__(self):
     return f"ms.values.float({json.dumps(self.data)})"
   def __str__(self):
     return builtins.str(self.data)
   def __neg__(self):
     return self.data.__neg__(self)
@@ -297,15 +297,15 @@
       return self.data.__sub__(other)
   def __truediv__(self,other):
     if type(self)==type(other):
       return self.data.__truediv__(other.data)
     else:
       return self.data.__truediv__(other)
 class str:
-  def __init__(self,data=""):
+  def __init__(self,data:str=""):
     self.data=builtins.str(data)
   def __repr__(self):
     return f"ms.values.str({json.dumps(self.data)})"
   def __str__(self):
     return builtins.str(self.data)
   def __getitem__(self,k):
     return self.data[k]
@@ -363,15 +363,15 @@
       return self.data.__rmod__(other)
   def __rmul__(self,other):
     if type(self)==type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
 class list:
-  def __init__(self,data=[]):
+  def __init__(self,data:list=[]):
     self.data=builtins.list(data)
   def __repr__(self):
     return f"ms.values.list({json.dumps(self.data)})"
   def __str__(self):
     return builtins.str(self.data)
   def __getitem__(self,k):
     return self.data[k]
@@ -429,15 +429,15 @@
       return self.data.__ne__(other)
   def __rmul__(self,other):
     if type(self)==type(other):
       return self.data.__rmul__(other.data)
     else:
       return self.data.__rmul__(other)
 class dict:
-  def __init__(self,data={}):
+  def __init__(self,data:dict={}):
     self.data=builtins.dict(data)
   def __repr__(self):
     return f"ms.values.dict({json.dumps(self.data)})"
   def __str__(self):
     return builtins.str(self.data)
   def __getitem__(self,k):
     return self.data[k]
```

### Comparing `mainshortcuts-1.6.82/src/MainShortcuts/win.py` & `mainshortcuts-1.6.83/src/MainShortcuts/win.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.82/PKG-INFO` & `mainshortcuts-1.6.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mainshortcuts
-Version: 1.6.82
+Name: MainShortcuts
+Version: 1.6.83
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

