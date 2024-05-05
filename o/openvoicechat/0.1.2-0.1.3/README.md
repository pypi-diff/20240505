# Comparing `tmp/openvoicechat-0.1.2.tar.gz` & `tmp/openvoicechat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvoicechat-0.1.2.tar", last modified: Fri May  3 21:40:11 2024, max compression
+gzip compressed data, was "openvoicechat-0.1.3.tar", last modified: Sun May  5 20:53:29 2024, max compression
```

## Comparing `openvoicechat-0.1.2.tar` & `openvoicechat-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:40:11.701192 openvoicechat-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-03 21:40:07.000000 openvoicechat-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 21:40:11.701192 openvoicechat-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-03 21:40:07.000000 openvoicechat-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:40:11.701192 openvoicechat-0.1.2/openvoicechat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-03 21:40:11.000000 openvoicechat-0.1.2/openvoicechat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-03 21:40:11.000000 openvoicechat-0.1.2/openvoicechat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:40:11.000000 openvoicechat-0.1.2/openvoicechat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-03 21:40:11.000000 openvoicechat-0.1.2/openvoicechat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:40:11.000000 openvoicechat-0.1.2/openvoicechat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:40:11.701192 openvoicechat-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-03 21:40:07.000000 openvoicechat-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.372341 openvoicechat-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-05 20:53:29.372341 openvoicechat-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.364341 openvoicechat-0.1.3/openvoicechat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.368341 openvoicechat-0.1.3/openvoicechat/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/llm_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/llm_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/llm_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/llm/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.368341 openvoicechat-0.1.3/openvoicechat/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/stt_deepgram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/stt_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/stt_vosk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/stt/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.368341 openvoicechat-0.1.3/openvoicechat/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_parler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_piper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_tortoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/tts/tts_xtts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/openvoicechat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:53:29.368341 openvoicechat-0.1.3/openvoicechat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-05 20:53:29.000000 openvoicechat-0.1.3/openvoicechat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-05 20:53:29.000000 openvoicechat-0.1.3/openvoicechat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:53:29.000000 openvoicechat-0.1.3/openvoicechat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 20:53:29.000000 openvoicechat-0.1.3/openvoicechat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 20:53:29.000000 openvoicechat-0.1.3/openvoicechat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:53:29.372341 openvoicechat-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-05 20:53:25.000000 openvoicechat-0.1.3/setup.py
```

### Comparing `openvoicechat-0.1.2/LICENSE` & `openvoicechat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.2/PKG-INFO` & `openvoicechat-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: openvoicechat
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenVoiceChat is an opensource library that allows you to have a natural voice conversation with your LLM agent.
 Home-page: http://www.fakhirali.pk/OpenVoiceChat/
 Author: Fakhir Ali
 Author-email: ali.fakhir33@gmail.com
 License-File: LICENSE
 Requires-Dist: sounddevice
-Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: pygame
 Requires-Dist: pyaudio
 Requires-Dist: librosa
 Requires-Dist: pydub
 Requires-Dist: python-dotenv
-Requires-Dist: phonemizer
 Requires-Dist: websockets
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Provides-Extra: piper
 Requires-Dist: piper-tts; extra == "piper"
 Requires-Dist: piper-phonemize; extra == "piper"
 Provides-Extra: vosk
 Requires-Dist: vosk; extra == "vosk"
-Provides-Extra: llama
-Requires-Dist: llama-cpp-python; extra == "llama"
 Provides-Extra: open-ai
 Requires-Dist: openai; extra == "open-ai"
 Provides-Extra: tortoise
 Requires-Dist: tortoise-tts; extra == "tortoise"
 Provides-Extra: xtts
 Requires-Dist: TTS; extra == "xtts"
```

### Comparing `openvoicechat-0.1.2/README.md` & `openvoicechat-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 https://github.com/fakhirali/OpenVoiceChat/assets/32309516/88b7973d-a362-46f3-ab18-232bb59a188e
 
 
 Supports all kinds of stt, tts and llm [models](notes/Models.md).
 
 Supports interruptions.
 
-Well [abstracted](/tts) apis, easy to use and [extend](notes/Adding_models.md).
-
-Runs locally on a [consumer GPU](https://www.nvidia.com/en-us/geforce/graphics-cards/30-series/rtx-3080-3080ti/).
+Well [abstracted](/openvoicechat/tts) apis, easy to use and [extend](notes/Adding_models.md).
 
 The goal is to be the open source alternative to [closed commercial implementations](notes/Competition.md)
 
 Some ideas are [here](notes/Ideas.md). 
 
 [TODO](notes/TODO.md).
 
@@ -38,25 +36,25 @@
 ```shell 
 python main.py
 ```
 
 [Discord](https://discord.gg/M5S2JksapH)
 
 ## Installing Required Packages
-### TO install only the base packages
+### To install only the base packages
 ```shell
-pip install -e git+https://github.com/fakhirali/OpenVoiceChat.git#egg=OpenVoiceChat
+pip install openvoicechat
 ```
 
-### TO install base and functionality specific packages
+### To install base and functionality specific packages
 ```shell
-pip install -e git+https://github.com/fakhirali/OpenVoiceChat.git#egg=OpenVoiceChat[piper]
+pip install openvoicechat[piper,xtts]
 ```
 
-Similary "piper" can be replaced by any of the following
+similarly "piper" and "xtts" can be replaced by any of the following
 - piper
 - vosk
 - llama
 - open_ai
 - tortoise
 - xtts
 - transformers
```

### Comparing `openvoicechat-0.1.2/openvoicechat.egg-info/PKG-INFO` & `openvoicechat-0.1.3/openvoicechat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: openvoicechat
-Version: 0.1.2
+Version: 0.1.3
 Summary: OpenVoiceChat is an opensource library that allows you to have a natural voice conversation with your LLM agent.
 Home-page: http://www.fakhirali.pk/OpenVoiceChat/
 Author: Fakhir Ali
 Author-email: ali.fakhir33@gmail.com
 License-File: LICENSE
 Requires-Dist: sounddevice
-Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: pygame
 Requires-Dist: pyaudio
 Requires-Dist: librosa
 Requires-Dist: pydub
 Requires-Dist: python-dotenv
-Requires-Dist: phonemizer
 Requires-Dist: websockets
 Provides-Extra: transformers
 Requires-Dist: transformers; extra == "transformers"
 Provides-Extra: piper
 Requires-Dist: piper-tts; extra == "piper"
 Requires-Dist: piper-phonemize; extra == "piper"
 Provides-Extra: vosk
 Requires-Dist: vosk; extra == "vosk"
-Provides-Extra: llama
-Requires-Dist: llama-cpp-python; extra == "llama"
 Provides-Extra: open-ai
 Requires-Dist: openai; extra == "open-ai"
 Provides-Extra: tortoise
 Requires-Dist: tortoise-tts; extra == "tortoise"
 Provides-Extra: xtts
 Requires-Dist: TTS; extra == "xtts"
```

### Comparing `openvoicechat-0.1.2/setup.py` & `openvoicechat-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,32 +6,29 @@
     description='OpenVoiceChat is an opensource library that allows you to have a natural voice conversation with '
                 'your LLM agent.',
     long_description='If you plan on making an LLM agent and want to have your users be able to talk to it like a '
                      'person (low latency, handles interruptions), this library is for you. It aims to be the '
                      'opensource, highly extensible and easy to use alternative to the proprietary solutions.',
     url='http://www.fakhirali.pk/OpenVoiceChat/',
     name='openvoicechat',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'sounddevice',
-        'torch',
         'torchaudio',
         'pygame',
         'pyaudio',
         'librosa',
         'pydub',
         'python-dotenv',
-        'phonemizer',
         'websockets'
     ],
     extras_require={
         'transformers' : ['transformers'],
         'piper': ['piper-tts','piper-phonemize'],
         'vosk': ['vosk'],
-        'llama': ['llama-cpp-python'],
         'open_ai': ['openai'],
         'tortoise': ['tortoise-tts'],
         'xtts': ['TTS'],
     },
     dependency_links=[],
 )
```

