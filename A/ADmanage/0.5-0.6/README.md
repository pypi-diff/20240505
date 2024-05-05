# Comparing `tmp/ADmanage-0.5.tar.gz` & `tmp/admanage-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADmanage-0.5.tar", last modified: Tue Feb 27 21:19:43 2024, max compression
+gzip compressed data, was "admanage-0.6.tar", last modified: Sun May  5 15:20:03 2024, max compression
```

## Comparing `ADmanage-0.5.tar` & `admanage-0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-02-27 21:19:43.696666 ADmanage-0.5/
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-02-27 21:19:43.692175 ADmanage-0.5/ADmanage/
--rw-r--r--   0 jack       (501) staff       (20)    11863 2024-02-27 20:59:13.000000 ADmanage-0.5/ADmanage/__init__.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2024-02-27 21:19:43.694784 ADmanage-0.5/ADmanage.egg-info/
--rw-r--r--   0 jack       (501) staff       (20)     7457 2024-02-27 21:19:43.000000 ADmanage-0.5/ADmanage.egg-info/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)      198 2024-02-27 21:19:43.000000 ADmanage-0.5/ADmanage.egg-info/SOURCES.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2024-02-27 21:19:43.000000 ADmanage-0.5/ADmanage.egg-info/dependency_links.txt
--rw-r--r--   0 jack       (501) staff       (20)       15 2024-02-27 21:19:43.000000 ADmanage-0.5/ADmanage.egg-info/requires.txt
--rw-r--r--   0 jack       (501) staff       (20)        9 2024-02-27 21:19:43.000000 ADmanage-0.5/ADmanage.egg-info/top_level.txt
--rw-r--r--   0 jack       (501) staff       (20)     7457 2024-02-27 21:19:43.695662 ADmanage-0.5/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)     7557 2024-02-27 21:18:19.000000 ADmanage-0.5/README.md
--rw-r--r--   0 jack       (501) staff       (20)       38 2024-02-27 21:19:43.696915 ADmanage-0.5/setup.cfg
--rw-r--r--   0 jack       (501) staff       (20)      363 2024-02-27 21:19:19.000000 ADmanage-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.597107 admanage-0.6/
+drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.570706 admanage-0.6/ADmanage/
+-rw-rw-rw-   0        0        0    12012 2024-04-12 09:20:05.000000 admanage-0.6/ADmanage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:20:03.595087 admanage-0.6/ADmanage.egg-info/
+-rw-rw-rw-   0        0        0     7702 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 15:20:03.000000 admanage-0.6/ADmanage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7702 2024-05-05 15:20:03.596087 admanage-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7557 2024-05-05 15:14:58.000000 admanage-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:20:03.597107 admanage-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-05-05 15:17:39.000000 admanage-0.6/setup.py
```

### Comparing `ADmanage-0.5/ADmanage/__init__.py` & `admanage-0.6/ADmanage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,17 +151,19 @@
         # Add a null record
         record = self.new_record(0)
         record['Data'] = self.DNS_RPC_RECORD_TS()
         record['Data']['entombedTime'] = tstime
         self.conn.modify(targetentry['dn'], {'dnsRecord': [(MODIFY_REPLACE, [record.getData()])],'dNSTombstoned': [(MODIFY_REPLACE, True)]})
 
     # List all user, group and computer objects
-    def get_ADobjects(self):
-        search_filter = f"(|(objectClass=user)(objectClass=group)(objectClass=computer))"
-        self.conn.search(self.base_dn, search_filter, attributes=['*'])
+    def get_ADobjects(self, custom_base_dn=None, custom_filter=None, custom_attributes=None):
+        base_dn = custom_base_dn or self.base_dn
+        search_filter = custom_filter or "(|(objectClass=user)(objectClass=group)(objectClass=computer))"
+        attributes = custom_attributes or ['*']
+        self.conn.search(base_dn, search_filter=search_filter,  attributes=attributes, search_scope=SUBTREE)
 
         if self.conn.entries:
             return self.conn.entries
 
     # Search for user, group, or computer objects with sAMAccountName value
     def get_ADobject(self, _object):
         search_filter = f"(&(|(objectClass=user)(objectClass=group)(objectClass=computer))(sAMAccountName={_object}))"
@@ -185,16 +187,15 @@
             attributes['cn'] = cn
             attributes['userPrincipalName'] = f"{sam}@{self.domain}"
 
             self.conn.add(f"cn={cn},{ou}", attributes=attributes)
 
             self.reset_password(sam, password)
             self.modify_ADobject_attributes(sam, attributes={'userAccountControl': '512'})
-            
-    
+
         if attributes['objectClass'] == 'computer':
             sam = f"{attributes['cn'].lower()}$"
             cn = attributes['cn']
             attributes['sAMAccountName'] = sam
 
             self.conn.add(f"cn={cn},{ou}", attributes=attributes)
 
@@ -206,22 +207,22 @@
 
             changes = {
                 'primaryGroupID': '515',
                 'userAccountControl': '4096'
             }
 
             self.modify_ADobject_attributes(sam, changes)
-        
+
         if attributes['objectClass'] == 'group':
             sam = f"{attributes['cn'].lower()}"
             cn = attributes['cn']
             attributes['sAMAccountName'] = sam
 
             self.conn.add(f"cn={cn},{ou}", attributes=attributes)
-        
+
         return self.get_ADobject(sam)
 
     # Removing users, computers or groups
     def del_ADobject(self, _object):
         _object_dn = self.get_ADobject(_object).distinguishedName
         if self.conn.delete(_object_dn[0]):
             return 200
@@ -231,15 +232,15 @@
     # List members of group
     def get_member(self, group_name):
         search_filter = f"(&(objectClass=group)(sAMAccountName={group_name}))"
         self.conn.search(self.base_dn, search_filter, attributes=['member'])
 
         if self.conn.entries:
             return self.conn.entries[0].member
-        
+
 
     # List groups of users
     def get_memberOf(self, username):
         search_filter = f"(&(objectClass=user)(sAMAccountName={username}))"
         self.conn.search(self.base_dn, search_filter, attributes=['memberOf'])
 
         if self.conn.entries:
@@ -248,34 +249,34 @@
 
     # Adding users, computers, or groups to groups
     def add_ADobject_to_group(self, _object, group):
         _object_dn = self.get_ADobject(_object).distinguishedName
         group_dn = self.get_ADobject(group).distinguishedName
 
         self.conn.modify(group_dn[0], {'member': [(MODIFY_ADD, [_object_dn[0]])]})
-        
+
         return self.get_ADobject(group).member
 
 
     # Removing users, computers, or groups from groups
     def del_ADobject_from_group(self, _object, group):
         _object_dn = self.get_ADobject(_object).distinguishedName
         group_dn = self.get_ADobject(group).distinguishedName
 
         self.conn.modify(group_dn[0], {'member': [(MODIFY_DELETE, _object_dn[0])]})
-        
+
         return self.get_ADobject(group).member
 
     # Updating user, computer, or group attributes.
     def modify_ADobject_attributes(self, _object, attributes):
         _object_dn = self.get_ADobject(_object).distinguishedName
 
         for key, value in attributes.items():
             self.conn.modify(_object_dn[0], {key: [(MODIFY_REPLACE, [value])]})
-        
+
         return self.get_ADobject(_object)
 
 
     # Reset password (Only work with ssl bind)
     def reset_password(self, username, password):
         user_dn = self.get_ADobject(username).distinguishedName
 
@@ -309,8 +310,8 @@
         new_uac = int(str(old_uac)) | uacFlag
 
         attributes = {
             'userAccountControl': new_uac
         }
 
         self.modify_ADobject_attributes(_object, attributes)
-        return self.get_ADobject(_object)
+        return self.get_ADobject(_object)
```

### Comparing `ADmanage-0.5/ADmanage.egg-info/PKG-INFO` & `admanage-0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,198 +1,193 @@
-Metadata-Version: 2.1
-Name: ADmanage
-Version: 0.5
-Description-Content-Type: text/markdown
-
-# ADmanage
-
-The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
-
-#### get_DNSentries
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_DNSentries()
-ad_client.disconnect()
-print(result)
-```
-#### get_DNSentry
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_DNSentry('quad9')
-ad_client.disconnect()
-print(result)
-```
-#### add_DNSentry
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.add_DNSentry('quad9', '149.112.112.112')
-ad_client.disconnect()
-print(result)
-```
-#### modify_DNSentry
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.modify_DNSentry('quad9', '9.9.9.9')
-ad_client.disconnect()
-print(result)
-```
-#### del_DNSentry
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.del_DNSentry('quad9')
-ad_client.disconnect()
-print(result)
-```
-#### get_ADobjects
-Searches for and returns all user, group, and computer objects.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_ADobjects()
-ad_client.disconnect()
-print(result)
-```
-#### get_ADobject
-Searches for and returns a specific AD object based on its sAMAccountName value.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_ADobject('Administrator')
-ad_client.disconnect()
-print(result)
-```
-#### add_ADobject
-Adds users, computers, or groups to the AD server.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'user', 'givenName': 'Jack', 'sn': 'Bower', 'password': 'Password1'})
-ad_client.disconnect()
-print(result)
-```
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'computer', 'cn': 'jbower-pc'})
-ad_client.disconnect()
-print(result)
-```
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'group', 'cn': '24hChrono'})
-ad_client.disconnect()
-print(result)
-```
-#### del_ADobject
-Deletes a specified AD object.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.del_ADobject('jbower')
-ad_client.disconnect()
-print(result)
-```
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.del_ADobject('jbower-pc$')
-ad_client.disconnect()
-print(result)
-```
-#### get_member
-Retrieves the members of a specified group.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_member('Administrators')
-ad_client.disconnect()
-print(result)
-```
-#### get_memberOf
-Retrieves the groups to which a user belongs.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.get_memberOf('Administrator')
-ad_client.disconnect()
-print(result)
-```
-#### add_ADobject_to_group
-Adds an AD object to a group.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.add_ADobject_to_group('jbower', 'test')
-ad_client.disconnect()
-print(result)
-```
-#### del_ADobject_from_group
-Removes an AD object from a group.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.del_ADobject_from_group('jbower', 'test')
-ad_client.disconnect()
-print(result)
-```
-#### modify_ADobject_attributes
-Modifies attributes of a specified AD object.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.modify_ADobject_attributes('jbower', {'mail': 'jack.bower@cobblepot59.int'})
-ad_client.disconnect()
-print(result)
-```
-#### reset_password
-Resets the password of a user (works with SSL bind).
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.reset_password('jbower', 'Password2')
-ad_client.disconnect()
-print(result)
-```
-#### enable_ADobject
-Enables a user or computer account.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.enable_ADobject('jbower')
-ad_client.disconnect()
-print(result)
-```
-#### disable_ADobject
-Disables a user or computer account.
-```sh
-from ADmanage import ADclient
-
-ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
-result = ad_client.disable_ADobject('jbower-pc$')
-ad_client.disconnect()
-print(result)
-```
+# ADmanage
+
+The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
+
+#### get_DNSentries
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_DNSentries()
+ad_client.disconnect()
+print(result)
+```
+#### get_DNSentry
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_DNSentry('quad9')
+ad_client.disconnect()
+print(result)
+```
+#### add_DNSentry
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.add_DNSentry('quad9', '149.112.112.112')
+ad_client.disconnect()
+print(result)
+```
+#### modify_DNSentry
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.modify_DNSentry('quad9', '9.9.9.9')
+ad_client.disconnect()
+print(result)
+```
+#### del_DNSentry
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.del_DNSentry('quad9')
+ad_client.disconnect()
+print(result)
+```
+#### get_ADobjects
+Searches for and returns all user, group, and computer objects.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_ADobjects()
+ad_client.disconnect()
+print(result)
+```
+#### get_ADobject
+Searches for and returns a specific AD object based on its sAMAccountName value.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_ADobject('Administrator')
+ad_client.disconnect()
+print(result)
+```
+#### add_ADobject
+Adds users, computers, or groups to the AD server.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'user', 'givenName': 'Jack', 'sn': 'Bower', 'password': 'Password1'})
+ad_client.disconnect()
+print(result)
+```
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'computer', 'cn': 'jbower-pc'})
+ad_client.disconnect()
+print(result)
+```
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.add_ADobject('OU=test,DC=cobblepot59,DC=int', {'objectClass': 'group', 'cn': '24hChrono'})
+ad_client.disconnect()
+print(result)
+```
+#### del_ADobject
+Deletes a specified AD object.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.del_ADobject('jbower')
+ad_client.disconnect()
+print(result)
+```
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.del_ADobject('jbower-pc$')
+ad_client.disconnect()
+print(result)
+```
+#### get_member
+Retrieves the members of a specified group.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_member('Administrators')
+ad_client.disconnect()
+print(result)
+```
+#### get_memberOf
+Retrieves the groups to which a user belongs.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.get_memberOf('Administrator')
+ad_client.disconnect()
+print(result)
+```
+#### add_ADobject_to_group
+Adds an AD object to a group.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.add_ADobject_to_group('jbower', 'test')
+ad_client.disconnect()
+print(result)
+```
+#### del_ADobject_from_group
+Removes an AD object from a group.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.del_ADobject_from_group('jbower', 'test')
+ad_client.disconnect()
+print(result)
+```
+#### modify_ADobject_attributes
+Modifies attributes of a specified AD object.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.modify_ADobject_attributes('jbower', {'mail': 'jack.bower@cobblepot59.int'})
+ad_client.disconnect()
+print(result)
+```
+#### reset_password
+Resets the password of a user (works with SSL bind).
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.reset_password('jbower', 'Password2')
+ad_client.disconnect()
+print(result)
+```
+#### enable_ADobject
+Enables a user or computer account.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.enable_ADobject('jbower')
+ad_client.disconnect()
+print(result)
+```
+#### disable_ADobject
+Disables a user or computer account.
+```sh
+from ADmanage import ADclient
+
+ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
+result = ad_client.disable_ADobject('jbower-pc$')
+ad_client.disconnect()
+print(result)
+```
```

### Comparing `ADmanage-0.5/README.md` & `admanage-0.6/ADmanage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: ADmanage
+Version: 0.6
+Description-Content-Type: text/markdown
+Requires-Dist: ldap3
+Requires-Dist: impacket
+
 # ADmanage
 
 The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
 
 #### get_DNSentries
 ```sh
 from ADmanage import ADclient
@@ -186,8 +193,8 @@
 ```sh
 from ADmanage import ADclient
 
 ad_client = ADclient(domain='cobblepot59.int', username='Administrator', password='Password1', dc_ip='ldap.cobblepot59.int', base_dn='DC=cobblepot59,DC=int', secure=True)
 result = ad_client.disable_ADobject('jbower-pc$')
 ad_client.disconnect()
 print(result)
-```
+```
```

