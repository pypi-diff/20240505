# Comparing `tmp/pdfnaut-0.1.1.tar.gz` & `tmp/pdfnaut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfnaut-0.1.1.tar", last modified: Sun Apr 14 17:48:21 2024, max compression
+gzip compressed data, was "pdfnaut-0.2.0.tar", last modified: Sun May  5 16:54:09 2024, max compression
```

## Comparing `pdfnaut-0.1.1.tar` & `pdfnaut-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.399553 pdfnaut-0.1.1/
--rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    14726 2024-04-14 17:48:21.396545 pdfnaut-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1880 2024-04-03 04:18:41.000000 pdfnaut-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.250544 pdfnaut-0.1.1/pdfnaut/
--rw-rw-rw-   0        0        0      320 2024-04-14 17:40:50.000000 pdfnaut-0.1.1/pdfnaut/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-24 03:14:43.000000 pdfnaut-0.1.1/pdfnaut/exceptions.py
--rw-rw-rw-   0        0        0     6429 2024-03-30 00:18:33.000000 pdfnaut-0.1.1/pdfnaut/filters.py
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.339550 pdfnaut-0.1.1/pdfnaut/objects/
--rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.1.1/pdfnaut/objects/__init__.py
--rw-rw-rw-   0        0        0     1632 2024-03-30 00:16:33.000000 pdfnaut-0.1.1/pdfnaut/objects/base.py
--rw-rw-rw-   0        0        0     1638 2024-03-30 00:18:21.000000 pdfnaut-0.1.1/pdfnaut/objects/stream.py
--rw-rw-rw-   0        0        0     1471 2024-03-30 00:48:56.000000 pdfnaut-0.1.1/pdfnaut/objects/xref.py
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.358544 pdfnaut-0.1.1/pdfnaut/parsers/
--rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.1.1/pdfnaut/parsers/__init__.py
--rw-rw-rw-   0        0        0    21355 2024-04-12 03:48:21.000000 pdfnaut-0.1.1/pdfnaut/parsers/pdf.py
--rw-rw-rw-   0        0        0    12503 2024-04-12 02:41:06.000000 pdfnaut-0.1.1/pdfnaut/parsers/simple.py
--rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.1.1/pdfnaut/py.typed
--rw-rw-rw-   0        0        0     9191 2024-03-30 03:48:10.000000 pdfnaut-0.1.1/pdfnaut/security_handler.py
--rw-rw-rw-   0        0        0     9684 2024-03-30 15:58:40.000000 pdfnaut-0.1.1/pdfnaut/serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.384545 pdfnaut-0.1.1/pdfnaut.egg-info/
--rw-rw-rw-   0        0        0    14726 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 17:48:21.000000 pdfnaut-0.1.1/pdfnaut.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1198 2024-04-14 17:40:42.000000 pdfnaut-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 17:48:21.400546 pdfnaut-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 17:48:21.377548 pdfnaut-0.1.1/tests/
--rw-rw-rw-   0        0        0     1857 2024-03-27 21:59:14.000000 pdfnaut-0.1.1/tests/test_encryption.py
--rw-rw-rw-   0        0        0     3726 2024-04-12 02:42:40.000000 pdfnaut-0.1.1/tests/test_object_parsing.py
--rw-rw-rw-   0        0        0     2673 2024-04-11 22:31:30.000000 pdfnaut-0.1.1/tests/test_parsing_files.py
--rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.1.1/tests/test_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/
+-rw-rw-rw-   0        0        0    10315 2024-01-02 18:49:05.000000 pdfnaut-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    14726 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1880 2024-04-03 04:18:41.000000 pdfnaut-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.507081 pdfnaut-0.2.0/pdfnaut/
+-rw-rw-rw-   0        0        0      320 2024-05-05 02:30:46.000000 pdfnaut-0.2.0/pdfnaut/__init__.py
+-rw-rw-rw-   0        0        0      329 2024-04-23 00:33:36.000000 pdfnaut-0.2.0/pdfnaut/exceptions.py
+-rw-rw-rw-   0        0        0    11422 2024-04-25 03:11:59.000000 pdfnaut-0.2.0/pdfnaut/filters.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.625120 pdfnaut-0.2.0/pdfnaut/objects/
+-rw-rw-rw-   0        0        0      551 2024-03-29 21:44:31.000000 pdfnaut-0.2.0/pdfnaut/objects/__init__.py
+-rw-rw-rw-   0        0        0     1632 2024-03-30 00:16:33.000000 pdfnaut-0.2.0/pdfnaut/objects/base.py
+-rw-rw-rw-   0        0        0     1638 2024-03-30 00:18:21.000000 pdfnaut-0.2.0/pdfnaut/objects/stream.py
+-rw-rw-rw-   0        0        0     1471 2024-03-30 00:48:56.000000 pdfnaut-0.2.0/pdfnaut/objects/xref.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.680202 pdfnaut-0.2.0/pdfnaut/parsers/
+-rw-rw-rw-   0        0        0      105 2024-03-29 21:48:59.000000 pdfnaut-0.2.0/pdfnaut/parsers/__init__.py
+-rw-rw-rw-   0        0        0    21582 2024-05-05 04:21:54.000000 pdfnaut-0.2.0/pdfnaut/parsers/pdf.py
+-rw-rw-rw-   0        0        0    12503 2024-04-12 02:41:06.000000 pdfnaut-0.2.0/pdfnaut/parsers/simple.py
+-rw-rw-rw-   0        0        0        0 2023-12-28 16:38:46.000000 pdfnaut-0.2.0/pdfnaut/py.typed
+-rw-rw-rw-   0        0        0    13542 2024-05-05 04:00:09.000000 pdfnaut-0.2.0/pdfnaut/security_handler.py
+-rw-rw-rw-   0        0        0     9684 2024-03-30 15:58:40.000000 pdfnaut-0.2.0/pdfnaut/serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.794336 pdfnaut-0.2.0/pdfnaut.egg-info/
+-rw-rw-rw-   0        0        0    14726 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-05 16:54:09.000000 pdfnaut-0.2.0/pdfnaut.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1275 2024-05-05 02:30:26.000000 pdfnaut-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 16:54:09.803774 pdfnaut-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 16:54:09.784201 pdfnaut-0.2.0/tests/
+-rw-rw-rw-   0        0        0     2864 2024-05-05 15:19:17.000000 pdfnaut-0.2.0/tests/test_encryption.py
+-rw-rw-rw-   0        0        0      936 2024-05-05 16:43:43.000000 pdfnaut-0.2.0/tests/test_filters.py
+-rw-rw-rw-   0        0        0     3726 2024-04-12 02:42:40.000000 pdfnaut-0.2.0/tests/test_object_parsing.py
+-rw-rw-rw-   0        0        0     2673 2024-04-11 22:31:30.000000 pdfnaut-0.2.0/tests/test_parsing_files.py
+-rw-rw-rw-   0        0        0     3719 2024-03-27 21:43:26.000000 pdfnaut-0.2.0/tests/test_serializer.py
```

### Comparing `pdfnaut-0.1.1/LICENSE` & `pdfnaut-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/PKG-INFO` & `pdfnaut-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.1.1
+Version: 0.2.0
 Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pdfnaut-0.1.1/README.md` & `pdfnaut-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/objects/__init__.py` & `pdfnaut-0.2.0/pdfnaut/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/objects/base.py` & `pdfnaut-0.2.0/pdfnaut/objects/base.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/objects/stream.py` & `pdfnaut-0.2.0/pdfnaut/objects/stream.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/objects/xref.py` & `pdfnaut-0.2.0/pdfnaut/objects/xref.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/parsers/pdf.py` & `pdfnaut-0.2.0/pdfnaut/parsers/pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,14 +367,18 @@
         elif isinstance(pdf_object, bytes):
             return self.security_handler.decrypt_object(
                 self._encryption_key, pdf_object, reference
             )
         elif isinstance(pdf_object, list):
             return [self._get_decrypted(obj, reference) for obj in pdf_object]
         elif isinstance(pdf_object, dict):
+            # make a special exception if the dictionary is the Encrypt key in the trailer
+            # we do not need to decrypt them
+            if reference == self.trailer["Encrypt"]:
+                return pdf_object
             return {name: self._get_decrypted(value, reference) for name, value in pdf_object.items()}         
 
         # Why would a number be encrypted?
         return pdf_object
 
     def parse_stream(self, xref_entry: InUseXRefEntry, extent: int) -> bytes:
         """Parses a PDF stream of length ``extent``"""
```

### Comparing `pdfnaut-0.1.1/pdfnaut/parsers/simple.py` & `pdfnaut-0.2.0/pdfnaut/parsers/simple.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut/security_handler.py` & `pdfnaut-0.2.0/pdfnaut/security_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 from __future__ import annotations
 
 from hashlib import md5
-from typing import Any, Union, Protocol, cast
+from typing import Any, Union, Protocol, Literal, cast
 
 from .objects import PdfHexString, PdfIndirectRef, PdfName, PdfStream
 
 
 class CryptProvider(Protocol):
     key: bytes
 
     def __init__(self, key: bytes) -> None:
         self.key = key
     
     def encrypt(self, contents: bytes) -> bytes: ...
     def decrypt(self, contents: bytes) -> bytes: ...
 
 
+class _IdentityProvider(CryptProvider):
+    def encrypt(self, contents: bytes) -> bytes:
+        return contents
+
+    def decrypt(self, contents: bytes) -> bytes:
+        return contents
+
 try:
     from Crypto.Cipher import ARC4, AES
     from Crypto.Util import Padding
 
     class _DomeARC4Provider(CryptProvider):
         def decrypt(self, contents: bytes) -> bytes:
             return ARC4.new(self.key).decrypt(contents)
         
         def encrypt(self, contents: bytes) -> bytes:
             return ARC4.new(self.key).encrypt(contents)
         
-    class _DomeAESCBCProvider(CryptProvider):
+    class _DomeAES128Provider(CryptProvider):
         def decrypt(self, contents: bytes) -> bytes:
             iv = contents[:16]
             encrypted = contents[16:]
 
             decrypted = AES.new(self.key, AES.MODE_CBC, iv).decrypt(encrypted)
             # last byte of decrypted indicates amount of trailing padding
             return decrypted[:-decrypted[-1]]
         
         def encrypt(self, contents: bytes) -> bytes:
             padded = Padding.pad(contents, 16, style="pkcs7")
 
             encryptor = AES.new(self.key, AES.MODE_CBC)
             return encryptor.iv + encryptor.encrypt(padded)
         
-    CRYPT_PROVIDERS = { "ARC4": _DomeARC4Provider, "AES_CBC": _DomeAESCBCProvider }
+    CRYPT_PROVIDERS = { "ARC4": _DomeARC4Provider, "AESV2": _DomeAES128Provider, 
+                        "Identity": _IdentityProvider }
 except ImportError:
-    CRYPT_PROVIDERS = { "ARC4": None, "AES_CBC": None }
+    CRYPT_PROVIDERS = { "ARC4": None, "AESV2": None, "Identity": _IdentityProvider }
 
 
 PASSWORD_PADDING = b'(\xbfN^Nu\x8aAd\x00NV\xff\xfa\x01\x08..\x00\xb6\xd0h>\x80/\x0c\xa9\xfedSiz'
 
+def pad_password(password: bytes) -> bytes:
+    return password[:32] + PASSWORD_PADDING[:32 - len(password)]
+
 
 class StandardSecurityHandler:
     def __init__(self, encryption: dict[str, Any], ids: list[PdfHexString]) -> None:
         self.encryption = encryption
         self.ids = ids
 
     @property
     def key_length(self) -> int:
         return self.encryption.get("Length", 40) // 8
 
     def compute_encryption_key(self, password: bytes) -> bytes:  
         """Computes an encryption key as defined in ``§ 7.6.3.3 Encryption Key Algorithm > 
         Algorithm 2: Computing an encryption key`` in the PDF spec."""      
-        padded_password = password[:32] + PASSWORD_PADDING[:32 - len(password)]
+        padded_password = pad_password(password)
 
         psw_hash = md5(padded_password)
         psw_hash.update(_O.value if isinstance(_O := self.encryption["O"], PdfHexString) else _O)
         psw_hash.update(self.encryption["P"].to_bytes(4, "little", signed=True))
         psw_hash.update(self.ids[0].value)
 
         if self.encryption.get("V", 0) >= 4 and not self.encryption.get("EncryptMetadata", True):
@@ -74,14 +85,54 @@
 
         if self.encryption["R"] >= 3:
             for _ in range(50):
                 psw_hash = md5(psw_hash.digest()[:self.key_length])
 
         return psw_hash.digest()[:self.key_length]
     
+    def compute_owner_password(self, owner_password: bytes, user_password: bytes) -> bytes:
+        """Computes the O (owner password) value in the Encrypt dictionary
+        as defined in ``§ 7.6.3.3 Encryption Key Algorithm > Algorithm 3``"""   
+
+        padded = pad_password(owner_password or user_password)
+        owner_digest = md5(padded).digest()
+        if self.encryption["R"] >= 3:
+            for _ in range(50):
+                owner_digest = md5(owner_digest).digest()
+
+        owner_cipher = owner_digest[:self.key_length]
+        
+        padded_user_psw = pad_password(user_password)
+        arc4 = self._get_provider("ARC4")
+        owner_crypt = arc4(owner_cipher).encrypt(padded_user_psw)
+
+        if self.encryption["R"] >= 3:
+            for i in range(1, 20):
+                owner_crypt = arc4(bytearray(b ^ i for b in owner_cipher)).encrypt(owner_crypt)
+
+        return owner_crypt
+    
+    def compute_user_password(self, password: bytes) -> bytes:
+        """Computes the U (owner password) value in the Encrypt dictionary
+        as defined in ``§ 7.6.3.3 Encryption Key Algorithm > Algorithms 4 and 5``"""   
+
+        encr_key = self.compute_encryption_key(password)
+        arc4 = self._get_provider("ARC4")
+        if self.encryption["R"] == 2:
+            padding_crypt = arc4(encr_key).encrypt(PASSWORD_PADDING)
+            return padding_crypt
+        else: # rev 3
+            padded_id_hash = md5(PASSWORD_PADDING + self.ids[0].value)
+            user_cipher = arc4(encr_key).encrypt(padded_id_hash.digest())
+
+            for i in range(1, 20):
+                user_cipher = arc4(bytearray(b ^ i for b in encr_key)).encrypt(user_cipher)
+
+            return pad_password(user_cipher)
+         
     def authenticate_user_password(self, password: bytes) -> tuple[bytes, bool]:  
         """Authenticates the provided user ``password`` according to Algorithm 4, 5, and 6 in 
         ``§ 7.6.3.4 Password Algorithms`` of the PDF spec.
         
         Returns:
             If the password was correct, a tuple of two values: the encryption key that should 
             decrypt the document and True. Otherwise, ``(b"", False)`` is returned."""
@@ -109,15 +160,15 @@
         """Authenticates the provided owner ``password`` (or user password if none) 
         according to Algorithms 3 and 7 in ``§ 7.6.3.4 Password Algorithms`` of the PDF spec.
         
         Returns:
             If the password was correct, a tuple of two values: the encryption key that should 
             decrypt the document and True. Otherwise, ``(b"", False)`` is returned."""
         # (a) to (d) in Algorithm 3
-        padded_password = password[:32] + PASSWORD_PADDING[:32 - len(password)]
+        padded_password = pad_password(password)
         digest = md5(padded_password).digest()
         if self.encryption["R"] >= 3:
             for _ in range(50):
                 digest = md5(digest).digest()
 
         cipher_key = digest[:self.key_length]
         user_cipher = _O.value if isinstance(_O := self.encryption["O"], PdfHexString) else _O
@@ -129,80 +180,122 @@
         else:
             for i in range(19, -1, -1):
                 user_cipher = make_provider(bytearray(b ^ i for b in cipher_key)).encrypt(user_cipher)
 
         return self.authenticate_user_password(user_cipher)
 
     _Encryptable = Union[PdfStream, PdfHexString, bytes]
-    def decrypt_object(self, encryption_key: bytes, contents: _Encryptable, reference: PdfIndirectRef, *, crypt_filter: dict[str, Any] | None = None) -> bytes:
-        """Decrypts the specified `contents` object according to Algorithm 1 in ``§ 7.6.2 General Encryption Algorithm``
+    def compute_object_crypt(self, encryption_key: bytes, contents: _Encryptable, 
+                             reference: PdfIndirectRef, *, 
+                             crypt_filter: dict[str, Any] | None = None) -> tuple[CryptMethod, bytes, bytes]:
+        """Computes all needed parameters to encrypt or decrypt ``contents`` according to 
+        Algorithm 1 in ``§ 7.6.2 General Encryption Algorithm``
         
         Arguments:
             encryption_key (bytes):
-                An encryption key generated by :meth:``.compute_encryption_key``
+                An encryption key generated by :meth:`.compute_encryption_key`
 
             contents (`PdfStream | PdfHexString | bytes`):
-                The contents to decrypt. The type of object to decrypt will determine what crypt filter
-                will be used for decryption (StmF for streams, StrF for hex and literal strings).
+                The contents to encrypt/decrypt. The type of object will determine what 
+                crypt filter will be used for decryption (StmF for streams, StrF for 
+                hex and literal strings).
 
             reference (`PdfIndirectRef`):
-                The reference of either the object itself (in the case of a stream) or the object 
-                containing it (in the case of a string)
+                The reference of either the object itself (in the case of a stream) or 
+                the object containing it (in the case of a string)
 
             crypt_filter (`dict[str, Any]`, optional):
                 The specific crypt filter to be referenced when decrypting the document.
                 If not specified, the default for this type of ``contents`` will be used.
 
         Returns:
-            A decrypted bytes representation of ``contents``
+            A tuple of 3 values: the crypt method to apply (AES CBC or ARC4), 
+            the key to use with this method, and the data to encrypt/decrypt.
         """
         generation = reference.generation.to_bytes(4, "little")
         object_number = reference.object_number.to_bytes(4, "little")
 
         extended_key = encryption_key + object_number[:3] + generation[:2]
 
-        is_aes = self._is_aes_filter(crypt_filter or {}) or self._aes_applies_for(contents)
-        if is_aes:
+        method = self._get_cfm_method(crypt_filter) if crypt_filter else self._get_crypt_method(contents)
+        if method == "AESV2":
             extended_key += bytes([0x73, 0x41, 0x6C, 0x54])
 
-        decryption_key = md5(extended_key).digest()[:self.key_length][:16]
+        crypt_key = md5(extended_key).digest()[:self.key_length + 5][:16]
 
         if isinstance(contents, PdfStream):
-            encrypted = contents.raw
+            data = contents.raw
         elif isinstance(contents, PdfHexString):
-            encrypted = contents.value
+            data = contents.value
         elif isinstance(contents, bytes):
-            encrypted = contents
+            data = contents
         else:
             raise TypeError("contents arg not a stream or string object")
 
-        if is_aes:
-            return self._get_provider("AES_CBC")(decryption_key).decrypt(encrypted)
-        return self._get_provider("ARC4")(decryption_key).decrypt(encrypted)
+        return (method, crypt_key, data)
+
+    def encrypt_object(self, encryption_key: bytes, contents: _Encryptable, 
+                       reference: PdfIndirectRef, *, 
+                       crypt_filter: dict[str, Any] | None = None) -> bytes:
+        """Encrypts the specified ``contents`` according to Algorithm 1 in 
+        ``§ 7.6.2 General Encryption Algorithm``.
+        
+        For details on arguments, please see :meth:`.compute_object_crypt`"""
+        
+        crypt_method, key, decrypted = self.compute_object_crypt(encryption_key, 
+                                                                 contents, reference, 
+                                                                 crypt_filter=crypt_filter)
+
+        return self._get_provider(crypt_method)(key).encrypt(decrypted)
+
+    def decrypt_object(self, encryption_key: bytes, contents: _Encryptable, 
+                       reference: PdfIndirectRef, *, 
+                       crypt_filter: dict[str, Any] | None = None) -> bytes:
+        """Decrypts the specified ``contents`` according to Algorithm 1 in 
+        ``§ 7.6.2 General Encryption Algorithm``.
+        
+        For details on arguments, please see :meth:`.compute_object_crypt`"""
+        
+        crypt_method, key, encrypted = self.compute_object_crypt(encryption_key, 
+                                                                 contents, reference,
+                                                                 crypt_filter=crypt_filter)
+
+        return self._get_provider(crypt_method)(key).decrypt(encrypted)
 
     def _get_provider(self, name: str) -> type[CryptProvider]:
         provider = CRYPT_PROVIDERS.get(name)
         if provider is None:
             raise NotImplementedError(f"Missing crypt provider for {name}. Register in CRYPT_PROVIDERS or install a compatible module.")
         return provider
 
-    def _aes_applies_for(self, contents: _Encryptable) -> bool:
+    CryptMethod = Literal["Identity", "ARC4", "AESV2"]
+    def _get_crypt_method(self, contents: _Encryptable) -> CryptMethod:
         if self.encryption["V"] != 4:
-            return False
-        
+            # ARC4 is assumed given that can only be specified if V = 4. It is definitely
+            # not Identity because the document wouldn't be encrypted in that case.
+            return "ARC4"            
+
         if isinstance(contents, PdfStream):
             cf_name = cast(PdfName, self.encryption.get("StmF", PdfName(b"Identity")))
         elif isinstance(contents, (bytes, PdfHexString)):
             cf_name = cast(PdfName, self.encryption.get("StrF", PdfName(b"Identity")))
         else:
             raise TypeError("contents arg not a stream or string object")
-        
+
         if cf_name.value == b"Identity":
-            return False
-            
-        crypt_filters = cast("dict[str, Any]", self.encryption.get("CF", {}))
+            return "Identity" # No processing needed
         
+        crypt_filters = cast("dict[str, Any]", self.encryption.get("CF", {}))
         crypter = crypt_filters.get(cf_name.value.decode(), {})
-        return self._is_aes_filter(crypter)
-    
-    def _is_aes_filter(self, crypt_filter: dict[str, Any]) -> bool:
-        return crypt_filter.get("CFM", PdfName(b"Identity")).value == b"AESV2"
+        
+        return self._get_cfm_method(crypter)
+
+    def _get_cfm_method(self, crypt_filter: dict[str, Any]) -> CryptMethod:
+        cf_name = crypt_filter.get("CFM", PdfName(b"Identity"))
+        if cf_name.value == b"Identity":
+            return "Identity"
+        elif cf_name.value == b"AESV2":
+            return "AESV2"
+        elif cf_name.value == b"V2":
+            return "ARC4"
+
+        raise NotImplementedError(f"{cf_name} not a supported crypt filter for the Standard security handler")
```

### Comparing `pdfnaut-0.1.1/pdfnaut/serializer.py` & `pdfnaut-0.2.0/pdfnaut/serializer.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/pdfnaut.egg-info/PKG-INFO` & `pdfnaut-0.2.0/pdfnaut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfnaut
-Version: 0.1.1
+Version: 0.2.0
 Summary: Explore PDFs with ease
 Author: Angel Carias
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pdfnaut-0.1.1/pdfnaut.egg-info/SOURCES.txt` & `pdfnaut-0.2.0/pdfnaut.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -16,10 +16,11 @@
 pdfnaut/objects/base.py
 pdfnaut/objects/stream.py
 pdfnaut/objects/xref.py
 pdfnaut/parsers/__init__.py
 pdfnaut/parsers/pdf.py
 pdfnaut/parsers/simple.py
 tests/test_encryption.py
+tests/test_filters.py
 tests/test_object_parsing.py
 tests/test_parsing_files.py
 tests/test_serializer.py
```

### Comparing `pdfnaut-0.1.1/pyproject.toml` & `pdfnaut-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [project]
 name = "pdfnaut"
-version = "0.1.1"
 description = "Explore PDFs with ease"
 authors = [
     { name = "Angel Carias" }
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
@@ -17,14 +16,15 @@
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11", 
     "Programming Language :: Python :: 3.12"    
 ]
+dynamic = ["version"]
 dependencies = []
 
 [project.urls]
 homepage = "https://github.com/aescarias/pdfnaut"
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov"]
@@ -34,10 +34,13 @@
 testpaths = ["tests"]
 pythonpath = ["."]
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["pdfnaut*"]
 
+[tool.setuptools.dynamic]
+version = { attr = "pdfnaut.__version__" }
+
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `pdfnaut-0.1.1/tests/test_encryption.py` & `pdfnaut-0.2.0/tests/test_encryption.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,7 +45,30 @@
     with open("tests/docs/encrypted-aes128.pdf", "rb") as fp:
         parser = PdfParser(fp.read())
         parser.parse()
 
         parser.decrypt("nil")
         metadata = cast("dict[str, Any]", parser.resolve_reference(parser.trailer["Info"]))
         assert metadata["Producer"].value == b"pypdf"
+
+def test_rc4_aes_password_values():
+    with open("tests/docs/encrypted-arc4.pdf", "rb") as fp:
+        parser = PdfParser(fp.read())
+        parser.parse()
+
+        encr_metadata = cast("dict[str, Any]", parser.resolve_reference(parser.trailer["Info"]))
+        
+        encrypt_dict = parser.resolve_reference(parser.trailer["Encrypt"])
+        assert parser.security_handler is not None
+
+        # Passwords
+        o_value = parser.security_handler.compute_owner_password(b"null", b"nil")
+        assert o_value.hex().lower().encode() == encrypt_dict["O"].raw.lower()
+
+        u_value = parser.security_handler.compute_user_password(b"nil")
+        assert u_value.hex().lower().encode() == encrypt_dict["U"].raw.lower()
+
+        # Encryption with passwords
+        encr_key = parser.security_handler.compute_encryption_key(b"nil")
+
+        assert encr_metadata["Producer"].value == parser.security_handler.encrypt_object(
+            encr_key, b"pypdf", parser.trailer["Info"])
```

### Comparing `pdfnaut-0.1.1/tests/test_object_parsing.py` & `pdfnaut-0.2.0/tests/test_object_parsing.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/tests/test_parsing_files.py` & `pdfnaut-0.2.0/tests/test_parsing_files.py`

 * *Files identical despite different names*

### Comparing `pdfnaut-0.1.1/tests/test_serializer.py` & `pdfnaut-0.2.0/tests/test_serializer.py`

 * *Files identical despite different names*

