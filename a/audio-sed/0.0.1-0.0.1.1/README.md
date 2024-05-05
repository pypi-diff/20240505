# Comparing `tmp/audio_sed-0.0.1.tar.gz` & `tmp/audio_sed-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\audio_sed-0.0.1.tar", last modified: Sun Apr  7 16:49:27 2024, max compression
+gzip compressed data, was "audio_sed-0.0.1.1.tar", last modified: Sun May  5 18:34:13 2024, max compression
```

## Comparing `audio_sed-0.0.1.tar` & `audio_sed-0.0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 16:49:27.114873 audio_sed-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-12-29 13:20:56.000000 audio_sed-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     5107 2024-04-07 16:49:27.112871 audio_sed-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4482 2023-12-30 00:32:25.000000 audio_sed-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 16:49:27.005783 audio_sed-0.0.1/audio_sed/
-drwxrwxrwx   0        0        0        0 2024-04-07 16:49:27.078843 audio_sed-0.0.1/audio_sed/pytorch/
--rw-rw-rw-   0        0        0      894 2023-12-29 13:20:56.000000 audio_sed-0.0.1/audio_sed/pytorch/audio_augmentations.py
--rw-rw-rw-   0        0        0     5301 2023-12-29 13:20:56.000000 audio_sed-0.0.1/audio_sed/pytorch/sed_block.py
--rw-rw-rw-   0        0        0     6816 2024-04-07 14:39:12.000000 audio_sed-0.0.1/audio_sed/pytorch/sed_models.py
--rw-rw-rw-   0        0        0      666 2023-12-29 13:20:56.000000 audio_sed-0.0.1/audio_sed/sed_config.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:49:27.101862 audio_sed-0.0.1/audio_sed/tensorflow/
--rw-rw-rw-   0        0        0     5177 2023-12-29 13:20:56.000000 audio_sed-0.0.1/audio_sed/tensorflow/sed_block.py
--rw-rw-rw-   0        0        0     7224 2023-12-29 13:20:56.000000 audio_sed-0.0.1/audio_sed/tensorflow/sed_models.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:49:27.012789 audio_sed-0.0.1/audio_sed.egg-info/
--rw-rw-rw-   0        0        0     5107 2024-04-07 16:49:26.000000 audio_sed-0.0.1/audio_sed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-04-07 16:49:26.000000 audio_sed-0.0.1/audio_sed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 16:49:26.000000 audio_sed-0.0.1/audio_sed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 16:49:26.000000 audio_sed-0.0.1/audio_sed.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-07 16:49:26.000000 audio_sed-0.0.1/audio_sed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 16:49:27.114873 audio_sed-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-12-29 13:20:56.000000 audio_sed-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:34:13.067110 audio_sed-0.0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5088 2024-05-05 18:34:13.065108 audio_sed-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4482 2023-12-30 00:32:25.000000 audio_sed-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:34:13.053099 audio_sed-0.0.1.1/audio_sed/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:34:13.062106 audio_sed-0.0.1.1/audio_sed/pytorch/
+-rw-rw-rw-   0        0        0      894 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/audio_sed/pytorch/audio_augmentations.py
+-rw-rw-rw-   0        0        0     5301 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/audio_sed/pytorch/sed_block.py
+-rw-rw-rw-   0        0        0     7241 2024-05-05 18:33:51.000000 audio_sed-0.0.1.1/audio_sed/pytorch/sed_models.py
+-rw-rw-rw-   0        0        0      666 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/audio_sed/sed_config.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:34:13.064108 audio_sed-0.0.1.1/audio_sed/tensorflow/
+-rw-rw-rw-   0        0        0     5177 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/audio_sed/tensorflow/sed_block.py
+-rw-rw-rw-   0        0        0     7224 2023-12-29 13:20:56.000000 audio_sed-0.0.1.1/audio_sed/tensorflow/sed_models.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:34:13.059103 audio_sed-0.0.1.1/audio_sed.egg-info/
+-rw-rw-rw-   0        0        0     5088 2024-05-05 18:34:12.000000 audio_sed-0.0.1.1/audio_sed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-05 18:34:12.000000 audio_sed-0.0.1.1/audio_sed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:34:12.000000 audio_sed-0.0.1.1/audio_sed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-05 18:34:12.000000 audio_sed-0.0.1.1/audio_sed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-05 18:34:12.000000 audio_sed-0.0.1.1/audio_sed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:34:13.067110 audio_sed-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-05-05 18:17:44.000000 audio_sed-0.0.1.1/setup.py
```

### Comparing `audio_sed-0.0.1/LICENSE` & `audio_sed-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/PKG-INFO` & `audio_sed-0.0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: audio_sed
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Implementation of audio SED architecture for tensorflow and pytorch.
 Home-page: https://github.com/Shiro-LK/SoundEventDetection
+Download-URL: https://github.com/Shiro-LK/SoundEventDetection.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
-Download-URL: https://github.com/Shiro-LK/SoundEventDetection.git
 Keywords: torch,tensorflow,audio_sed
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sound Event Detection
@@ -114,8 +113,7 @@
 
 
 # Citation 
 
 - [PANNs: Large-Scale Pretrained Audio Neural Networks for Audio Pattern Recognition](https://arxiv.org/abs/1912.10211)
 - PANNs model: https://github.com/qiuqiangkong/audioset_tagging_cnn
 - https://github.com/Shiro-LK/tflibrosa
-
```

### Comparing `audio_sed-0.0.1/README.md` & `audio_sed-0.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed/pytorch/audio_augmentations.py` & `audio_sed-0.0.1.1/audio_sed/pytorch/audio_augmentations.py`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed/pytorch/sed_block.py` & `audio_sed-0.0.1.1/audio_sed/pytorch/sed_block.py`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed/pytorch/sed_models.py` & `audio_sed-0.0.1.1/audio_sed/pytorch/sed_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             features[i]["output"], features[i]["attention_global"] = global_attn(features[i]["clipwise"])
             
 
         return features
 
 class AudioSED(nn.Module):
     def __init__(self, backbone, num_classes:list, in_features:int, in_channel:int=3, hidden_size=1024, activation= 'sigmoid', use_logmel=True, 
-                spectrogram_augmentation = None, apply_attention="step", drop_rate = [0.5, 0.5], config_sed:dict = ConfigSED().__dict__):
+                spectrogram_augmentation = None, apply_attention="step", drop_rate = [0.5, 0.5], config_sed:dict = ConfigSED().__dict__, wav_2_spectrogram=False):
         """
             Classifier for a new task using pretrained CNN as a sub module.
         """
         super(AudioSED, self).__init__()    
         self.num_classes = num_classes
         self.in_channel = in_channel
         self.use_logmel = use_logmel
@@ -118,50 +118,57 @@
         self.amin = config_sed["amin"]
         self.top_db = config_sed["top_db"]
         self.spectrogram_augmentation = spectrogram_augmentation
         self.bn = nn.BatchNorm2d(self.mel_bins)
         # Spectrogram extractor 
         self.spectrogram_extractor = Spectrogram(n_fft=self.window_size, hop_length=self.hop_size, 
             win_length=self.window_size, window=self.window, center=self.center, pad_mode=self.pad_mode, 
-            freeze_parameters=True)
+            freeze_parameters=True) if wav_2_spectrogram else nn.Identity()
 
         # Logmel feature extractor
         self.logmel_extractor = LogmelFilterBank(sr=self.sample_rate, n_fft=self.window_size, 
             n_mels=self.mel_bins, fmin=self.fmin, fmax=self.fmax, ref=self.ref, amin=self.amin, 
-            top_db=self.top_db, freeze_parameters=True)
+            top_db=self.top_db, freeze_parameters=True) if  wav_2_spectrogram else nn.Identity()
 
         self.backbone =  backbone 
    
         self.sed_block = SED_Block(num_classes=num_classes, in_features=in_features, hidden_size=hidden_size, 
                 activation = activation, drop_rate = drop_rate,   apply_attention=apply_attention)
-                
+        self.wav_2_spectrogram = wav_2_spectrogram
     def forward(self, input, mixup_fn=None ):
         """Input: (batch_size, length, data_length)
+        # Spectrogram should be: (batch size, c, mel_bins, time_steps)
         """
-        with torch.no_grad():
-            x = self.spectrogram_extractor(input)   # (batch_size, 1, time_steps, freq_bins)
-            #print("sepctrogram :", x.shape)
-            if self.use_logmel:
-                with autocast(False):
-                    x = self.logmel_extractor(x) # (batch_size, 1, time_steps, mel_bins)
+        x = input
+        if self.wav_2_spectrogram:
+            with torch.no_grad():
+                x = self.spectrogram_extractor(x)   # (batch_size, 1, time_steps, freq_bins)
+                #print("sepctrogram :", x.shape)
+                if self.use_logmel:
+                    with autocast(False):
+                        x = self.logmel_extractor(x) # (batch_size, 1, time_steps, mel_bins)
+                x = torch.permute(x, (0,1,3,2))
 
         if self.training and self.spectrogram_augmentation:
             x = self.spectrogram_augmentation(x)
 
         # Mixup on spectrogram
         if self.training and mixup_fn is not None:
             x = mixup_fn(x)  
 
         # (BS, C=1, H, W)
         frames_num = x.shape[2]   
-        x = x.transpose(1, 3)
+        x = x.transpose(1, 2)
         x = self.bn(x) # BN applied on melbins
-        x = x.transpose(1, 3)
+        x = x.transpose(1, 2)
         
         if x.shape[1] == 1 and self.in_channel > 1:        
             x = torch.cat([x for _ in range(self.in_channel)], dim=1)
         
-        x = self.backbone(x) # (batch size, channels, steps, freq)
-        
+        x = self.backbone(x)
+        # (batch size, channels, freq, steps)
+        x = torch.permute(x, (0,1,3,2))
+
+        # (batch size, channels, steps, freq)
         outputs = self.sed_block(x)
 
         return outputs
```

### Comparing `audio_sed-0.0.1/audio_sed/sed_config.py` & `audio_sed-0.0.1.1/audio_sed/sed_config.py`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed/tensorflow/sed_block.py` & `audio_sed-0.0.1.1/audio_sed/tensorflow/sed_block.py`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed/tensorflow/sed_models.py` & `audio_sed-0.0.1.1/audio_sed/tensorflow/sed_models.py`

 * *Files identical despite different names*

### Comparing `audio_sed-0.0.1/audio_sed.egg-info/PKG-INFO` & `audio_sed-0.0.1.1/audio_sed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: audio-sed
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Implementation of audio SED architecture for tensorflow and pytorch.
 Home-page: https://github.com/Shiro-LK/SoundEventDetection
+Download-URL: https://github.com/Shiro-LK/SoundEventDetection.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
-Download-URL: https://github.com/Shiro-LK/SoundEventDetection.git
 Keywords: torch,tensorflow,audio_sed
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sound Event Detection
@@ -114,8 +113,7 @@
 
 
 # Citation 
 
 - [PANNs: Large-Scale Pretrained Audio Neural Networks for Audio Pattern Recognition](https://arxiv.org/abs/1912.10211)
 - PANNs model: https://github.com/qiuqiangkong/audioset_tagging_cnn
 - https://github.com/Shiro-LK/tflibrosa
-
```

### Comparing `audio_sed-0.0.1/setup.py` & `audio_sed-0.0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md', encoding="utf-8-sig") as f:
         README = f.read()
     return README
 
 
 setup(
     name='audio_sed',
-    version='0.0.1',    
+    version='0.0.1.1',    
     description='Implementation of audio SED architecture for tensorflow and pytorch.',
     author='Shiro-LK',
     author_email='shirosaki94@gmail.com',
     license='MIT License',
     packages=['audio_sed', 'audio_sed.pytorch', 'audio_sed.tensorflow'],
     long_description=readme(),
     long_description_content_type="text/markdown",
```

