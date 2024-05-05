# Comparing `tmp/soundtools-0.2.1.0.tar.gz` & `tmp/soundtools-0.2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.2.1.0.tar", last modified: Sat May  4 02:18:36 2024, max compression
+gzip compressed data, was "soundtools-0.2.2.0.tar", last modified: Sun May  5 01:33:55 2024, max compression
```

## Comparing `soundtools-0.2.1.0.tar` & `soundtools-0.2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/
--rw-rw-rw-   0        0        0      701 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 02:18:36.542690 soundtools-0.2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      789 2024-05-04 02:18:14.000000 soundtools-0.2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.538703 soundtools-0.2.1.0/soundtools/
--rw-rw-rw-   0        0        0      399 2024-05-04 02:16:57.000000 soundtools-0.2.1.0/soundtools/__init__.py
--rw-rw-rw-   0        0        0    37676 2024-05-04 02:16:50.000000 soundtools-0.2.1.0/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-05-04 02:18:36.541693 soundtools-0.2.1.0/soundtools.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 02:18:36.000000 soundtools-0.2.1.0/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/
+-rw-rw-rw-   0        0        0      701 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-10 02:26:25.000000 soundtools-0.2.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-05 01:33:55.540721 soundtools-0.2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      789 2024-05-05 01:33:25.000000 soundtools-0.2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.536722 soundtools-0.2.2.0/soundtools/
+-rw-rw-rw-   0        0        0      399 2024-05-05 01:33:20.000000 soundtools-0.2.2.0/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    33899 2024-05-05 01:31:59.000000 soundtools-0.2.2.0/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-05-05 01:33:55.539722 soundtools-0.2.2.0/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-05 01:33:55.000000 soundtools-0.2.2.0/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.2.1.0/PKG-INFO` & `soundtools-0.2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.1.0
+Version: 0.2.2.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.1.0
+version: 0.2.2.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

### Comparing `soundtools-0.2.1.0/setup.py` & `soundtools-0.2.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 setup(
 name='soundtools',
-version='0.2.1.0',
+version='0.2.2.0',
 description="used to work with sounds waves",
 long_description="""made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.1.0
+version: 0.2.2.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves""",
 author='Mohammad Erfan Karami',
```

### Comparing `soundtools-0.2.1.0/soundtools/soundtools.py` & `soundtools-0.2.2.0/soundtools/soundtools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """### made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-### version: 0.2.1.0
+### version: 0.2.2.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves"""
 
@@ -40,15 +40,15 @@
     def __setitem__(self, __key: str, __value: float) -> None:
         return super().__setitem__(__key.upper(), __value)
 
 
 #-- sound waves --#
 class Sounds:
     """has some basic sound waves and also caches the result of the functions for faster output"""
-    def __init__(self, sample_rate: int=48000, dtype:np.float32|np.int16|np.uint8=np.float32) -> None:
+    def __init__(self, sample_rate: int=48000, dtype:Dtype=np.float32) -> None:
         self.default_sample_rate: int = sample_rate
         self.existed_notes: dict[str, tuple] = {}
         
         self.tau = 2*np.pi
         self.rev_pi = 1/np.pi
         self.two_oper_pi = 2/np.pi
         self.four_over_pi = 4/np.pi
@@ -74,14 +74,18 @@
     def cache_wave(wave_type: str) -> SoundBuffer:
         """caches the waves so if you had to generate a note multiple times it's gonna use the cached wave. 
         you can't use the lru_cache from the functools module because waves are stored as numpy arrays and numpy arrays are not hashable, 
         so this decorator will store the numpy array as a tuple in "self.existed_notes" and convert it back to a numpy array each time you want to use that wave
         \nreturns the cached value if available, otherwise caches the returned wave"""
         def decorator(func: Wave) -> SoundBuffer:
             def wrapper(self, freq:float, dur:float, vol: float):
+                # Error if frequency is negative
+                if freq < 0:
+                    raise f"frequency must be positive number, given frequency: {freq}"
+                
                 name = f"{wave_type}|{freq}|{dur}"
                 if name in self.existed_notes.keys():
                     wave = vol * np.array(self.existed_notes[name], dtype=self.dtype)
                     return wave
                 
                 temp = func(self, freq, dur, self.max_amp)
                 result: SoundBuffer = func(self, freq, dur, vol)
@@ -104,40 +108,39 @@
     def square_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a square wave based on the given frequency, duration and amplitude or volume\n
         a square wave is typically generated by adding all the odd harmonics (3, 5, 7, 9...) to a fundamental frequency\n
         each harmonic is added with a little bit less volume which causes the amplitude to change a bit so at the end the amplitude is multiplied by 4/pi to fix it
         returns a numpy array"""
         
         # -- creating the fundumental note --#
-        buf = np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(3, 1000, 2):
-            f = freq*h
-            #-- break if the frequency is greater than 20,000 because human ear can' hear it and the arent many headphones that can play more than this anyways --#
-            if f > 20_000:
-                break
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = np.sin(fund)
+        
+        n = np.ceil(20_000 / freq).astype(np.int16)
+        for h in range(3, n, 2):
             #-- adding the harmonics --#
-            buf += np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h
+            buf += np.sin(fund*h) / h
         
         wave = ((self.four_over_pi)*vol*buf).astype(self.dtype)
         return wave
     
     @cache_wave("tri")
     def triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a triangle wave based on the given frequency, duration and amplitude or volume\n
         a triangle wave is typically generated by adding every second odd harmonic (5, 9, 13...) to a fundamental frequency\n
         each harmonic is added with a less volume which causes the amplitude to change a bit so at the end the amplitude is multiplied by '8/pi^2' to fix it\n
         returns a numpy array"""
         
-        buf = np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(1, 500):
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = np.sin(fund)
+        
+        n = np.ceil(10_000 / freq).astype(np.int16)
+        for h in range(1, n):
             harmonic = (2*h+1)
-            f = freq*harmonic
-            if f > 20000:
-                break
-            buf += (-1)**h * harmonic**(-2) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)
+            buf += (-1)**h * np.sin(fund * harmonic) / (harmonic*harmonic)
         
         wave = ((self.eight_over_pi_sqr)*vol*buf).astype(self.dtype)
         return wave
     
     @cache_wave("fast_tri")
     def fast_triangle_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         return (self.two_oper_pi * vol * np.arcsin(np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate))).astype(self.dtype)
@@ -146,130 +149,76 @@
     def sawtooth_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """returns a numpy array,
         creates a sawtooth wave based on the given frequency, duration and amplitude or volume\n
         a sawtooth wave is typically generated by adding every harmonic to a fundamental frequency with the odd harmonics being negative (2, -3, 4, -5...)\n
         each harmonic is added with less volume which causes the amplitude to change a bit so at the end we do this
         >>> (vol * (0.5 - self.rev_pi*buf))"""
         
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h)
-        
-        wave = (vol * ((-self.two_oper_pi)*buf)).astype(np.float32)
-        return wave
-    
-    @cache_wave("revsaw")
-    def reversed_sawtooth_wave(self, freq:float, dur:float, vol: float) -> SoundBuffer:
-        """creates a reversed sawtooth wave based on the given frequency, duration and amplitude or volume\n
-        a reversed sawtooth wave is typically generated by adding every harmonic to a fundamental frequency with the odd harmonics being negative (2, -3, 4, -5...)\n
-        each harmonic is added with less volume which causes the amplitude to change a bit so at the end we do this
-        >>> ((2*vol/np.pi) * (0.5 - self.rev_pi*buf))"""
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = np.sin(fund) * -1
         
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h)
+        n = np.ceil(20_000 / freq).astype(np.int16)
+        for h in range(2, n):
+            buf += (-1)**h * (np.sin(fund * h) / h)
         
-        wave = (vol * self.two_oper_pi * buf).astype(np.float32)
+        wave = (vol * ((-self.two_oper_pi)*buf)).astype(np.float32)
         return wave
     
-    @cache_wave("smoothsaw")
-    def smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=1.25) -> SoundBuffer:
+    def smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=2.5) -> SoundBuffer:
         """creates a wave like saw wave but without the sharp points"""
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**smoothness)
         
-        wave = (vol * -self.two_oper_pi * buf).astype(self.dtype)
-        return wave
-    
-    @cache_wave("revsmoothsaw")
-    def rev_smooth_saw_wave(self, freq:float, dur:float, vol: float, smoothness: float=1.25) -> SoundBuffer:
-        """creates a wave like reversed saw wave but without the sharp points"""
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**smoothness)
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = np.sin(fund) * -1
         
-        wave = (vol * self.two_oper_pi * buf).astype(self.dtype)
-        return wave
-    
-    @cache_wave("wavy")
-    def wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=1.25) -> SoundBuffer:
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**wavyness)
+        n = np.ceil(20_000 / freq).astype(np.int16)
+        for h in range(2, n):
+            buf += (-1)**h * (np.sin(fund * h) / h**smoothness)
         
         wave = (vol * -self.two_oper_pi * buf).astype(self.dtype)
         return wave
     
-    @cache_wave("revwavy")
-    def rev_wavy_wave(self, freq:float, dur:float, vol: float, wavyness: int=1.25) -> SoundBuffer:
-        buf = (-1) * np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
-        for h in range(2, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * f * np.arange(self.default_sample_rate * dur) / self.default_sample_rate)/h**wavyness)
-        
-        wave = (vol * self.two_oper_pi * buf).astype(self.dtype)
-        return wave
-    
     @cache_wave("organ")
     def organ(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates an organ like sound based on the given frequency, duration and amplitude or volume"""
         
-        pi_2_samples_num = self.tau * np.arange(self.default_sample_rate * dur)
-        buf = vol * np.sin(pi_2_samples_num * freq / self.default_sample_rate)
-        buf += vol*0.9 * np.sin(pi_2_samples_num * freq*2 / self.default_sample_rate)
-        buf += vol * np.sin(pi_2_samples_num * freq*4 / self.default_sample_rate)
-        buf += vol*0.6 * np.sin(pi_2_samples_num * freq*6 / self.default_sample_rate)
-        buf += vol*0.7 * np.sin(pi_2_samples_num * freq*16 / self.default_sample_rate)
-        buf += vol*0.5 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
-        buf += vol*0.3 * np.sin(pi_2_samples_num * freq*24 / self.default_sample_rate)
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = vol * np.sin(fund)
+        buf += vol*0.9 * np.sin(fund * 2)
+        buf += vol * np.sin(fund * 4)
+        buf += vol*0.6 * np.sin(fund * 6)
+        buf += vol*0.7 * np.sin(fund* 16)
+        buf += vol*0.5 * np.sin(fund * 20)
+        buf += vol*0.3 * np.sin(fund* 24)
 
         wave = (buf/7*2.424).astype(self.dtype)
         # wave = (buf/7*2.4247).astype(self.dtype) # for better percision (might cause quality issues on high volumes)
         return wave
     
     @cache_wave("marimb")
     def marimba(self, freq:float, dur:float, vol: float) -> SoundBuffer:
         """creates a "not even close to marimba" sound based on the given frequency, duration and amplitude or volume\n
         warning!: very annoying sound"""
         
-        pi_2_samples_num = self.tau * np.arange(self.default_sample_rate * dur)
-        buf = vol * np.sin(pi_2_samples_num * freq / self.default_sample_rate)
-        buf += vol*0.75 * np.sin(pi_2_samples_num * freq*10 / self.default_sample_rate)
-        buf += vol/2 * np.sin(pi_2_samples_num * freq*20 / self.default_sample_rate)
-        buf += vol/4 * np.sin(pi_2_samples_num * freq*30 / self.default_sample_rate)
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = vol * np.sin(fund)
+        buf += vol*0.75 * np.sin(fund * 10)
+        buf += vol/2 * np.sin(fund * 20)
+        buf += vol/4 * np.sin(fund * 30)
         
         wave = (buf/4).astype(self.dtype)
         return self.fade_out(wave, wave.size)
     
     @cache_wave("tst")
     def test(self, freq:float, dur:float, vol: float) -> SoundBuffer:
-        buf = np.sin(self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate)
+        fund = self.tau * np.arange(self.default_sample_rate * dur) * freq / self.default_sample_rate
+        buf = np.sin(fund)
+        
+        n = np.ceil(20_000 / freq).astype(np.int16)
         for h in range(1, 1000):
-            f = freq*h
-            if f > 20000:
-                break
-            buf += (-1)**h * (np.sin(self.tau * np.arange(self.default_sample_rate * dur) * f / self.default_sample_rate)/h)
+            buf += (-1)**h * (np.sin(fund * h) / h)
         
         wave = (vol * (0.5 - self.rev_pi*buf)).astype(self.dtype)
         return wave
     
     
     def _fix_amp(self, wave: SoundBuffer) -> SoundBuffer:
         wave[wave > self.max_amp] = self.max_amp
@@ -333,28 +282,25 @@
 
         i = np.iinfo(dtype)
         abs_max: int = 2 ** (i.bits - 1)
         offset = i.min + abs_max
         return (sig * abs_max + offset).clip(i.min, i.max).astype(dtype)
     
     # converts an int type array to a float32
-    def pcm2float(self, sig: np.ndarray, dtype: Literal["float32"]="float32") -> SoundBuffer:
+    def pcm2float(self, sig: np.ndarray) -> SoundBuffer:
         """gets an int dtype array as input, converts it to float and returns the converted array"""
         
         sig = np.asarray(sig)
         if sig.dtype.kind not in 'iu':
             raise TypeError("'sig' must be an array of integers")
-        dtype = np.dtype(dtype)
-        if dtype.kind != 'f':
-            raise TypeError("'dtype' must be a floating point type")
 
-        i = np.iinfo(sig.dtype)
+        i = np.finfo(np.float32)
         abs_max: int = 2 ** (i.bits - 1)
         offset = i.min + abs_max
-        return (sig.astype(dtype) - offset) / abs_max
+        return (sig.astype(np.float32) - offset) / abs_max
         
     # exports to .erfan file which is completely useless but you can play them with the app.py file adn you can convert them to wav file which is actualy useful
     def export_to_erfan(self, file_name:str, buffer: np.ndarray|bytes, sample_rate: int, dtype, channels: int) -> None:
         """exports to \".erfan\" file which can be played with the app in my github https://github.com/erfan-ops"""
         
         if type(buffer) != bytes:
             dtype = buffer.dtype
@@ -513,15 +459,18 @@
             sample_rate = self.sample_rate
         
         self.stream = self.config_stream(samp_width=samp_width,
                                          channels=n_channels,
                                          sample_rate=sample_rate)
     
     
-    def init_input_stream(self, samp_width: int|str="float32", n_channels: int=1, sample_rate: int|None=None, chunk:int=3200) -> None:
+    def init_input_stream(self, samp_width: int|str="float32",
+                          n_channels: int=1,
+                          sample_rate: int|None=None,
+                          chunk:int=3200) -> None:
         if not sample_rate:
             sample_rate = self.sample_rate
         
         if type(samp_width) == str:
             samp_width = self.get_sampwidth_from_str(dtype=samp_width)
         
         self.input_stream = self.AUDIO_OBJECT.open(format=self.AUDIO_OBJECT.get_format_from_width(samp_width),
@@ -776,15 +725,15 @@
             self.stream.write(b)
         
         b = wave[(i+1)*chunk : ].data.tobytes()
         self.stream.write(b)
     
     
     # created a chord sound buffer and plays it
-    def play_chord(self, notes: Iterable, wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
+    def play_chord(self, notes: Iterable[Note], wave_type: Wave, duration:str|float=0, volume:float=0) -> None:
         """generates then plays a chord with the given arguments"""
         buf = self.generate_chord_buffer(notes, wave_type, duration, volume).tobytes()
         
         self.play_buffer(buf)
     
     
     def play_erfan(self, file_name: str) -> None:
```

### Comparing `soundtools-0.2.1.0/soundtools.egg-info/PKG-INFO` & `soundtools-0.2.2.0/soundtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: soundtools
-Version: 0.2.1.0
+Version: 0.2.2.0
 Summary: used to work with sounds waves
 Author: Mohammad Erfan Karami
 Author-email: erfan012amir016@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 made by Mohammad Erfan Karami
 github: https://github.com/erfan-ops
 
-version: 0.2.1.0
+version: 0.2.2.0
 
 this package is used to create, play and save sound files
 it has some basic sound waves although you can add your own and modify the package.
 
 it stores the sound waves as numpy arrays and uses pyaudio for playback
 and uses matplotlib to visualize the waves
```

