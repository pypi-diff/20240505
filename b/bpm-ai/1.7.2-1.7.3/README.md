# Comparing `tmp/bpm_ai-1.7.2.tar.gz` & `tmp/bpm_ai-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.7.2.tar", max compression
+gzip compressed data, was "bpm_ai-1.7.3.tar", max compression
```

## Comparing `bpm_ai-1.7.2.tar` & `bpm_ai-1.7.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      726 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/README.md
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      195 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1961 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1595 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     1699 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.prompt
--rw-r--r--   0        0        0     3644 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      950 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     8786 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     8181 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     8459 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.prompt
--rw-r--r--   0        0        0     6247 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     3044 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     1466 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.prompt
--rw-r--r--   0        0        0     7565 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0     2578 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/extract/util.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      690 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0      738 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.prompt
--rw-r--r--   0        0        0     1631 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      632 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0      688 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.prompt
--rw-r--r--   0        0        0     3164 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0      680 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/bpm_ai/translate/util.py
--rw-r--r--   0        0        0      900 2024-05-03 21:42:35.046613 bpm_ai-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1961 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     1699 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/compose.prompt
+-rw-r--r--   0        0        0     3644 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      950 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     8786 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     8181 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     8459 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/decide.prompt
+-rw-r--r--   0        0        0     6247 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     3044 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     1466 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/extract.prompt
+-rw-r--r--   0        0        0     7565 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0     2578 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/extract/util.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      690 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0      738 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/generic/generic.prompt
+-rw-r--r--   0        0        0     1631 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      632 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0      688 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/translate.prompt
+-rw-r--r--   0        0        0     3170 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0      680 2024-05-05 11:46:17.239679 bpm_ai-1.7.3/bpm_ai/translate/util.py
+-rw-r--r--   0        0        0      900 2024-05-05 11:46:17.243679 bpm_ai-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 bpm_ai-1.7.3/PKG-INFO
```

### Comparing `bpm_ai-1.7.2/README.md` & `bpm_ai-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/common/multimodal.py` & `bpm_ai-1.7.3/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.7.3/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.7.3/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/compose/compose.prompt` & `bpm_ai-1.7.3/bpm_ai/compose/compose.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/compose/compose.py` & `bpm_ai-1.7.3/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/compose/util.py` & `bpm_ai-1.7.3/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.7.3/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.7.3/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/decide/decide.prompt` & `bpm_ai-1.7.3/bpm_ai/decide/decide.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/decide/decide.py` & `bpm_ai-1.7.3/bpm_ai/decide/decide.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/decide/schema.py` & `bpm_ai-1.7.3/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.7.3/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.7.3/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/extract/extract.prompt` & `bpm_ai-1.7.3/bpm_ai/extract/extract.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/extract/extract.py` & `bpm_ai-1.7.3/bpm_ai/extract/extract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/extract/util.py` & `bpm_ai-1.7.3/bpm_ai/extract/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.7.3/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.7.3/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/generic/generic.prompt` & `bpm_ai-1.7.3/bpm_ai/generic/generic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/generic/generic.py` & `bpm_ai-1.7.3/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.7.3/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.7.3/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/translate/translate.prompt` & `bpm_ai-1.7.3/bpm_ai/translate/translate.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/bpm_ai/translate/translate.py` & `bpm_ai-1.7.3/bpm_ai/translate/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         raise MissingParameterError("target language is required")
 
     if not ocr and llm.supports_images():
         input_items = prepare_images_for_llm_prompt(input_items)
     else:
         input_items = await ocr_documents(input_items, ocr)
     input_items = await transcribe_audio(input_items, asr)
-    input_data = prepare_text_blobs(input_data)
-    assert_all_files_processed(input_data)
+    input_items = prepare_text_blobs(input_items)
+    assert_all_files_processed(input_items)
 
     prompt = Prompt.from_file(
         "translate",
         input=input_items,
         lang=target_language
     )
 
@@ -65,16 +65,16 @@
         return input_data
 
     if not target_language or target_language.isspace():
         raise MissingParameterError("target language is required")
 
     input_items = await ocr_documents(input_items, ocr)
     input_items = await transcribe_audio(input_items, asr)
-    input_data = await replace_text_blobs(input_data)
-    assert_all_files_processed(input_data)
+    input_items = await replace_text_blobs(input_items)
+    assert_all_files_processed(input_items)
 
     try:
         target_language_code = get_lang_code(target_language)
     except LookupError:
         raise LanguageNotFoundError(f"Could not identify target language '{target_language}'.")
 
     texts_to_translate = list(input_items.values())
```

### Comparing `bpm_ai-1.7.2/bpm_ai/translate/util.py` & `bpm_ai-1.7.3/bpm_ai/translate/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.7.2/pyproject.toml` & `bpm_ai-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.7.2"
+version = "1.7.3"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `bpm_ai-1.7.2/PKG-INFO` & `bpm_ai-1.7.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.7.2
+Version: 1.7.3
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

