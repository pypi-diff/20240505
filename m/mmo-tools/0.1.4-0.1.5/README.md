# Comparing `tmp/mmo_tools-0.1.4.tar.gz` & `tmp/mmo_tools-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmo_tools-0.1.4.tar", last modified: Sat May  4 13:27:08 2024, max compression
+gzip compressed data, was "mmo_tools-0.1.5.tar", last modified: Sun May  5 08:50:31 2024, max compression
```

## Comparing `mmo_tools-0.1.4.tar` & `mmo_tools-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.943275 mmo_tools-0.1.4/
--rw-rw-rw-   0        0        0     2481 2024-05-04 13:27:08.942276 mmo_tools-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1455 2024-05-04 13:23:51.000000 mmo_tools-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 13:27:08.943275 mmo_tools-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1235 2024-05-04 13:26:57.000000 mmo_tools-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.921276 mmo_tools-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.932276 mmo_tools-0.1.4/src/mmo_tools/
--rw-rw-rw-   0        0        0      183 2024-05-04 13:04:59.000000 mmo_tools-0.1.4/src/mmo_tools/__init__.py
--rw-rw-rw-   0        0        0     2667 2024-05-04 13:26:49.000000 mmo_tools-0.1.4/src/mmo_tools/core.py
--rw-rw-rw-   0        0        0     1836 2024-05-04 13:02:48.000000 mmo_tools-0.1.4/src/mmo_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:27:08.942276 mmo_tools-0.1.4/src/mmo_tools.egg-info/
--rw-rw-rw-   0        0        0     2481 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 13:27:08.000000 mmo_tools-0.1.4/src/mmo_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 08:50:31.360558 mmo_tools-0.1.5/
+-rw-rw-rw-   0        0        0     6191 2024-05-05 08:50:31.360558 mmo_tools-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4757 2024-05-05 08:50:07.000000 mmo_tools-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 08:50:31.360558 mmo_tools-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1235 2024-05-05 08:47:37.000000 mmo_tools-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:50:31.339558 mmo_tools-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 08:50:31.344559 mmo_tools-0.1.5/src/mmo_tools/
+-rw-rw-rw-   0        0        0      304 2024-05-05 08:46:45.000000 mmo_tools-0.1.5/src/mmo_tools/__init__.py
+-rw-rw-rw-   0        0        0     4010 2024-05-05 08:43:47.000000 mmo_tools-0.1.5/src/mmo_tools/core.py
+-rw-rw-rw-   0        0        0     1852 2024-05-05 08:47:13.000000 mmo_tools-0.1.5/src/mmo_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 08:50:31.358562 mmo_tools-0.1.5/src/mmo_tools.egg-info/
+-rw-rw-rw-   0        0        0     6191 2024-05-05 08:50:31.000000 mmo_tools-0.1.5/src/mmo_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-05 08:50:31.000000 mmo_tools-0.1.5/src/mmo_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 08:50:31.000000 mmo_tools-0.1.5/src/mmo_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 08:50:31.000000 mmo_tools-0.1.5/src/mmo_tools.egg-info/top_level.txt
```

### Comparing `mmo_tools-0.1.4/setup.py` & `mmo_tools-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
     name='mmo_tools',  # Tên thư viện của bạn
-    version='0.1.4',  # Phiên bản đầu tiên
+    version='0.1.5',  # Phiên bản đầu tiên
     packages=find_packages('src'),  # Tìm tất cả các packages trong thư mục src
     package_dir={'': 'src'},  # Chỉ định thư mục chứa các packages
     author='Lam Dinh',
     author_email='ldl.contact.booking@gmail.com',
     description='Thư Viện Hỗ Trợ Viết Tool Facebook Nhanh',
     long_description=open('README.md','r',encoding='utf-8').read(),  # Đọc nội dung README nếu có
     long_description_content_type='text/markdown',  # Định dạng của long description
```

### Comparing `mmo_tools-0.1.4/src/mmo_tools/core.py` & `mmo_tools-0.1.5/src/mmo_tools/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
    
     try:
         data_r =  [key.strip("\n") for key in open(file , "r",encoding="UTF-8").readlines()]
     except Exception as error:
         return error
     data   = []
     for r in data_r:
+        if r == "":continue
         rp = utils.dict_typ()
         r = r + "||"
         if ("c_user" in r) and ("i_user" not in r):user =  r.split("c_user=")[1].split(";")[0]
         elif "i_user" in r:user =  r.split("i_user=")[1].split(";")[0]
         else:user = ""
         
         rp.update({"c_user":user}) # => user id
@@ -34,14 +35,53 @@
                     pass_mail = utils.type_pwemail(value=r , valuemail=rtip.strip("\n"))
                     if pass_mail:rp.update({'passemail':pass_mail})
             except Exception:
                 continue
         data.append(rp)
     return data
 
+def convert_headers_web(headers_text: str) -> str:
+
+    """
+        return headers {key : value}
+    """
+    headers , check , name = {} , 0 , str()
+    if "\n" not in headers_text:
+        print("""
+        Headers are not in the correct format.
+              Example 1: 
+
+                   Accept:
+*/*
+              Content-Type:
+application/x-www-form-urlencoded
+              
+
+              Example 2 :
+
+                   Accept:*/*,
+                   Content-Type:application/x-www-form-urlencoded
+              
+            
+
+              
+""")
+    try:
+        for temp in headers_text:
+            if temp[-1:] in ':':
+                name = temp[:-1].replace('\n','|').replace('`','"').replace('(^)','://')
+                headers.update({name:""})
+                check = 1
+            if temp[-1:] not in ':' and check:
+                headers.update({name:temp.replace('\n','|').replace('`','"').replace('(^)','://')})
+                check = 0
+    except Exception as error:
+        print(error)
+        return headers
+    return headers
 def convert_proxy(proxy) -> str:
     https = {}
     if len(proxy.split(":")) == 2:
         https = {
             "https":f"http://{proxy}",
             "http":f"http://{proxy}"
             }
@@ -54,11 +94,16 @@
         ip , port , user , pass_proxy = map(str,proxy.split(":"))
         https = {
             "https":f"http://{user}:{pass_proxy}@{ip}:{ port}",
             "http":f"http://{user}:{pass_proxy}@{ip}:{ port}"
             }
     return https
 
-def checklive(fbid):
-    if len(requests.get(f'https://graph.facebook.com/{str(fbid)}/picture?redirect=0').json()['data']['url']) >= 150: return 1
-    return 0
-
+def check_facebook_account(fbid):
+    try:
+        response = requests.get(f'https://graph.facebook.com/{str(fbid)}/picture?redirect=0')
+        data = response.json()
+        url = data['data']['url']
+        return len(url) >= 150
+    except (requests.RequestException, KeyError) as e:
+        print(f"Lỗi khi kiểm tra tài khoản Facebook: {e}")
+        return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmo_tools-0.1.4/src/mmo_tools/utils.py` & `mmo_tools-0.1.5/src/mmo_tools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 def type_pw(value,valueid):
     value =  value + "|"
     for index , x in enumerate(value.split("|")):
         try:
             if valueid == x and len(value.split("|")) >  1:
                 return value.split("|")[index + 1]
-        except:pass
+        except Exception:pass
 def type_pwemail(value,valuemail):
     value =  value + "|"
     for index , x in enumerate(value.split("|")):
-        # try:
+        try:
             if valuemail == x and len(value.split("|")) >  1:
                 return value.split("|")[index + 1]
-        # except:pass
+        except Exception:pass
 
 
 def headers():
     return {
             "accept":"*/*",
             "accept-encoding":"gzip, deflate, br",
             "accept-language":"en-US,en;q=0.9",
```

