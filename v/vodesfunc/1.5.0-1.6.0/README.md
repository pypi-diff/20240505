# Comparing `tmp/vodesfunc-1.5.0.tar.gz` & `tmp/vodesfunc-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vodesfunc-1.5.0.tar", last modified: Tue Oct 31 14:44:44 2023, max compression
+gzip compressed data, was "vodesfunc-1.6.0.tar", last modified: Sun May  5 15:28:14 2024, max compression
```

## Comparing `vodesfunc-1.5.0.tar` & `vodesfunc-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 14:44:44.249182 vodesfunc-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-10-31 14:44:44.245182 vodesfunc-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 14:44:44.249182 vodesfunc-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 14:44:44.245182 vodesfunc-1.5.0/vodesfunc/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/aa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/denoise.py
--rw-r--r--   0 runner    (1001) docker     (127)    15970 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/descale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16973 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2023-10-31 14:44:27.000000 vodesfunc-1.5.0/vodesfunc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 14:44:44.245182 vodesfunc-1.5.0/vodesfunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-10-31 14:44:44.000000 vodesfunc-1.5.0/vodesfunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-31 14:44:44.000000 vodesfunc-1.5.0/vodesfunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 14:44:44.000000 vodesfunc-1.5.0/vodesfunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-31 14:44:44.000000 vodesfunc-1.5.0/vodesfunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-31 14:44:44.000000 vodesfunc-1.5.0/vodesfunc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/vodesfunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/aa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21732 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/descale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/spikefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-05 15:28:06.000000 vodesfunc-1.6.0/vodesfunc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:28:14.735282 vodesfunc-1.6.0/vodesfunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 15:28:14.000000 vodesfunc-1.6.0/vodesfunc.egg-info/top_level.txt
```

### Comparing `vodesfunc-1.5.0/LICENSE` & `vodesfunc-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vodesfunc-1.5.0/PKG-INFO` & `vodesfunc-1.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Vodes' random Vapoursynth Functions.
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -19,20 +19,22 @@
 License-File: LICENSE
 Requires-Dist: Vapoursynth>=61
 Requires-Dist: vsscale>=1.0.1
 Requires-Dist: vsrgtools>=1.3.0
 Requires-Dist: vskernels>=1.2.0
 Requires-Dist: vstools>=1.6.2
 Requires-Dist: vsmasktools>=1.1.0
+Requires-Dist: vsmuxtools>=0.1.0
 
 # vodesfunc
 
-Contains various functions for automation and other stuff I use in my scripts
+Contains various functions for automation and other stuff I use in my scripts.
 
-### This is by no means me trying to be professional and as such, the code will not be treated like it.
-<br>
+Auto generated docs are at https://muxtools.vodes.pw.
+
+#### This is by no means me trying to be professional and as such, the code will not be treated like it.
 
 ## Installation
 
 `pip install vodesfunc` <br>for ~~mostly~~ stable versions
 
 `pip install git+https://github.com/Vodes/vodesfunc.git` <br>for absolutely latest
```

### Comparing `vodesfunc-1.5.0/pyproject.toml` & `vodesfunc-1.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
 [project]
 name = "vodesfunc"
-version = "1.5.0"
+version = "1.6.0"
 description = "Vodes' random Vapoursynth Functions."
 authors = [{ name = "Vodes", email = "vodes.imp@gmail.com" }]
 dependencies = [
     "Vapoursynth>=61",
     "vsscale>=1.0.1",
     "vsrgtools>=1.3.0",
     "vskernels>=1.2.0",
     "vstools>=1.6.2",
     "vsmasktools>=1.1.0",
+    "vsmuxtools>=0.1.0"
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vodesfunc-1.5.0/vodesfunc/aa.py` & `vodesfunc-1.6.0/vodesfunc/aa.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,111 +5,128 @@
 from vsrgtools import unsharp_masked
 from vstools import FrameRangesN, KwargsT, mod2, vs, core, depth, get_y, get_w, join, plane, scale_8bit
 
 from .scale import mod_padding
 
 __all__ = ["pre_aa", "cope_aa", "CopeMode"]
 
+
 def pre_aa(clip: vs.VideoNode, radius: int = 1, strength: float = 100, opencl: bool = True, **nnedi3_args) -> vs.VideoNode:
     """
-        A prefilter to use in conjunction with an AA function.
-        The idea is to fix the luminance uniformity on lineart and make AAing more effective.
+    A prefilter to use in conjunction with an AA function.
+    The idea is to fix the luminance uniformity on lineart and make AAing more effective.
 
-        :param radius:      Radius used for the unsharp function
-        :param strength:    Strength used for the unsharp function
-        :param opencl:      Use nnedi3cl instead of znedi3
-        :param nnedi3_args: Additional args passed to the respective nnedi function
+    :param radius:      Radius used for the unsharp function
+    :param strength:    Strength used for the unsharp function
+    :param opencl:      Use nnedi3cl instead of znedi3
+    :param nnedi3_args: Additional args passed to the respective nnedi function
 
-        :return:            Processed clip
+    :return:            Processed clip
     """
     args = {"qual": 2, "nsize": 0, "nns": 4, "pscrn": 1}
     args.update(**nnedi3_args)
     clip_y = plane(clip, 0)
-    
+
     if opencl:
         (left, right, top, bottom) = mod_padding(clip_y, 2, 2)
         width = clip.width + left + right
         height = clip.height + top + bottom
         clip_y = clip_y.resize.Point(width, height, src_left=-left, src_top=-top, src_width=width, src_height=height)
 
     for i in range(2):
-        bob = clip_y.nnedi3cl.NNEDI3CL(field=3, **nnedi3_args) if opencl else \
-            clip_y.znedi3.nnedi3(field=3, **nnedi3_args)
+        bob = clip_y.nnedi3cl.NNEDI3CL(field=3, **nnedi3_args) if opencl else clip_y.znedi3.nnedi3(field=3, **nnedi3_args)
         sharp = unsharp_masked(clip_y, radius, strength)
         limit = core.std.Expr([sharp, clip_y, bob[::2], bob[1::2]], "x y z a max max min y z a min min max")
         clip_y = limit.std.Transpose()
-    
+
     if opencl:
         clip_y = clip_y.std.Crop(left, right, top, bottom)
         clip_y = clip_y.std.CopyFrameProps(clip)
 
     return clip_y if clip.format.color_family == vs.GRAY else join(clip_y, clip)
 
+
 class CopeMode(IntEnum):
     UpDown = 1
     Descale = 2
     Inverse = 3
 
-def cope_aa(clip: vs.VideoNode, 
-            multiplier: float | None = None, 
-            antialiaser: Antialiaser = Eedi3(0.125, 0.25, gamma=65, vthresh0=40, vthresh1=60, field=1, sclip_aa=None),
-            scaler: KernelT | ScalerT | Sequence[Union[KernelT, ScalerT]] = Lanczos,
-            mode: CopeMode | int = CopeMode.Inverse,
-            mask: bool | vs.VideoNode = True,
-            no_aa_ranges: FrameRangesN = [],
-            **kwargs: KwargsT) -> vs.VideoNode:
+
+def cope_aa(
+    clip: vs.VideoNode,
+    multiplier: float | None = None,
+    antialiaser: Antialiaser = Eedi3(0.125, 0.25, gamma=65, vthresh0=40, vthresh1=60, field=1, sclip_aa=None),
+    scaler: KernelT | ScalerT | Sequence[Union[KernelT, ScalerT]] = Lanczos,
+    mode: CopeMode | int = CopeMode.Inverse,
+    mask: bool | vs.VideoNode = True,
+    no_aa_ranges: FrameRangesN = [],
+    hybrid_cl: bool = False,
+    **kwargs: KwargsT,
+) -> vs.VideoNode:
     """
     Cope and lazy function to AA a doubled clip. Usually while rescaling.
     This is probably overall an awful idea.
 
     :param multiplier:              Basically rfactor. If you're doubling a 720p clip you'll only have a 1440p clip to AA. EEDI3 will fuck it.
                                     Defaults to 1.2 if the input clip is smaller than 1700p. 1 otherwise.
     :param antialiaser:             Antialiaser used for actually doing the stuff. Defaults to EEDI3 with some somewhat conservative settings kindof.
     :param scaler:                  Scaler(s) or rather kernel(s) in this case. Used to up- and downscale for the rfactor.
                                     If you specify a third one it will get used to scale the mask. (Otherwise Bilinear)
     :param mode:                    Method to return back to input res. Available are UpDown (simple downscale), Descale and Inverse (fmtc).
     :param mask:                    Mask for eedi3 possibly save some calculations. Can be a custom one, True for a Kirsch or False to disable.
     :param no_aa_ranges:            Ranges you might not wanna AA for one reason or another.
+    :param hybrid_cl:               Use eedi3cl on one of the two interpolate calls.
+                                    Not sure if this is useful or not. Just wrote it to test.
     """
+
     def fmtc_args(kernel: Kernel) -> KwargsT:
         if isinstance(kernel, Bicubic):
             return KwargsT(kernel="bicubic", a1=kernel.b, a2=kernel.c)
         else:
             return KwargsT(kernel=kernel.__class__.__name__.lower(), taps=kernel.taps if isinstance(kernel, Lanczos) else None)
-        
+
     if not isinstance(scaler, Sequence):
-        scaler = [scaler, scaler] 
-    scalers = [Kernel.ensure_obj(s) if mode != CopeMode.UpDown 
-                else Scaler.ensure_obj(s) for s in scaler]
-    
+        scaler = [scaler, scaler]
+    scalers = [Kernel.ensure_obj(s) if mode != CopeMode.UpDown else Scaler.ensure_obj(s) for s in scaler]
+
     if mask is True:
         from vsmasktools import KirschTCanny
+
         mask = KirschTCanny.edgemask(clip, lthr=60 / 255, hthr=150 / 255, planes=0)
 
     if not multiplier:
         multiplier = 1.2 if clip.height < 1700 else 1.0
     height = mod2(clip.height * multiplier)
     width = get_w(height, mod=None)
     if mask:
         mask = mask.resize.Bilinear(width, height) if len(scalers) < 3 else scalers[2].scale(mask, width, height)
         mask = mask.std.Binarize(scale_8bit(mask, 16))
     wclip = scalers[0].scale(clip, width, height)
     aa = wclip.std.Transpose()
     aa = antialiaser.interpolate(aa, False, sclip=aa, mclip=mask.std.Transpose() if mask else None, **kwargs).std.Transpose()
-    aa = antialiaser.interpolate(aa, False, sclip=aa, mclip=mask if mask else None, **kwargs)
+    if hybrid_cl and isinstance(antialiaser, Eedi3):
+        from copy import deepcopy
+
+        other_antialiaser = deepcopy(antialiaser)
+        other_antialiaser.opencl = True
+        aa = other_antialiaser.interpolate(aa, False, sclip=aa, **kwargs)
+    else:
+        aa = antialiaser.interpolate(aa, False, sclip=aa, mclip=mask if mask else None, **kwargs)
     aa = wclip.std.MaskedMerge(aa, mask)
     match mode:
         case CopeMode.Descale:
             aa = scalers[1].descale(aa, clip.width, clip.height)
         case CopeMode.Inverse:
             aa = aa.fmtc.resample(clip.width, clip.height, invks=True, **fmtc_args(scalers[1]))
         case _:
             aa = scalers[1].scale(aa, clip.width, clip.height)
     if not no_aa_ranges:
         return aa
     else:
         try:
             from jvsfunc import rfs
+
             return rfs(aa, clip, no_aa_ranges)
         except:
             from vstools import replace_ranges as rfs
-            return rfs(aa, clip, no_aa_ranges)
+
+            return rfs(aa, clip, no_aa_ranges)
```

### Comparing `vodesfunc-1.5.0/vodesfunc/denoise.py` & `vodesfunc-1.6.0/vodesfunc/denoise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,141 @@
-from vstools import vs, core, get_y, get_u, get_v, depth, get_depth, join
+from vstools import vs, core, get_y, get_u, get_v, depth, get_depth, join, KwargsT
 from vsrgtools import contrasharpening
 
-__all__ = ['VMDegrain', 'schizo_denoise']
+__all__ = ["VMDegrain", "schizo_denoise"]
 
-def VMDegrain(src: vs.VideoNode, thSAD: int = 60, prefilter: vs.VideoNode | int = 2, 
-    smooth: bool = True, block_size: int = 32, overlap: int = 16, **kwargs) -> vs.VideoNode:
+
+def VMDegrain(
+    src: vs.VideoNode,
+    thSAD: int = 60,
+    prefilter: vs.VideoNode | int = 2,
+    smooth: bool = True,
+    block_size: int = 32,
+    overlap: int = 16,
+    **kwargs: KwargsT,
+) -> vs.VideoNode:
     """
-        Just some convenience function for mvtools with a useable preset and temporal smoothing.
-        Check the MVTools Docs for the params that aren't listed below.
+    Just some convenience function for mvtools with a useable preset and temporal smoothing.
+    Check the MVTools Docs for the params that aren't listed below.
 
 
-        :param src:             Input to denoise
-        :param smooth:          Run TTempsmooth on the denoised clip if True
-        :return:                Denoised clip              
+    :param src:             Input to denoise
+    :param smooth:          Run TTempsmooth on the denoised clip if True
+    :return:                Denoised clip
     """
     from vsdenoise import MVTools, SADMode, SearchMode, MotionMode, PelType, Prefilter
+
     if isinstance(prefilter, int):
         prefilter = Prefilter(prefilter)
     y = depth(get_y(src), 16)
-    d_args = dict(
-        prefilter=prefilter, thSAD=thSAD, block_size=block_size, overlap=overlap,
-        sad_mode=SADMode.SPATIAL.same_recalc, search=SearchMode.DIAMOND, 
-        motion=MotionMode.HIGH_SAD, pel_type=PelType.BICUBIC, rfilter=2, sharp=2,
+    d_args = KwargsT(
+        prefilter=prefilter,
+        thSAD=thSAD,
+        block_size=block_size,
+        overlap=overlap,
+        sad_mode=SADMode.SPATIAL.same_recalc,
+        search=SearchMode.DIAMOND,
+        motion=MotionMode.HIGH_SAD,
+        pel_type=PelType.BICUBIC,
+        rfilter=2,
+        sharp=2,
     )
     d_args.update(**kwargs)
 
     out = MVTools.denoise(y, **d_args)
     if smooth:
         out = out.ttmpsm.TTempSmooth(maxr=1, thresh=1, mdiff=0, strength=1)
 
     out = depth(out, get_depth(src))
-    return out if src.format.color_family == vs.GRAY else join(out, src)
+    return out if src.format.color_family == vs.GRAY else join(out, src)  # type: ignore
 
 
-def schizo_denoise(src: vs.VideoNode, sigma: float | list[float] = [0.8, 0.3], thSAD: int = 60, 
-    radius: int | list[int] = 2, nlm_a: int = 2, prefilter: vs.VideoNode | int = 2, 
-    cuda: bool | list[bool] = True, csharp: int | bool = False, **kwargs) -> vs.VideoNode:
+def schizo_denoise(
+    src: vs.VideoNode,
+    sigma: float | list[float] = [0.8, 0.3],
+    thSAD: int = 60,
+    radius: int | list[int] = 2,
+    nlm_a: int = 2,
+    prefilter: vs.VideoNode | int = 2,
+    cuda: bool | list[bool] = True,
+    csharp: int | bool = False,
+    **kwargs,
+) -> vs.VideoNode:
     """
-        Convenience function for (k)nlm on chroma and mvtools + bm3d(cuda) on luma.
-        Mostly for personal scripts so please don't complain too much unless it's an actual issue.
+    Convenience function for (k)nlm on chroma and mvtools + bm3d(cuda) on luma.
+    Mostly for personal scripts so please don't complain too much unless it's an actual issue.
 
-        :param src:         Input to denoise
-        :param sigma:       Essentially strength for NLMeans and BM3D.
-                            Float or list of floats in this order [bm3d, nlm_uv] or [bm3d, nlm_u, nlm_v]
-        :param thSAD:       Not exactly strength but something like that, for mvtools.
-        :param radius:      Temporal Radius used for NLMeans and BM3D.
-                            Int or list of ints in this order [bm3d, nlm]
-        :param prefilter:   vsdenoise Prefilter or prefiltered clip to use for mvtools.
-                            Defaults to MINBLUR3
-        :param cuda:        Uses NlmCuda and BM3DCuda respectively if available. The latter prefers RTC if available.
-        :param csharp:      Apply contrasharpening after denoising. True defaults to 3 while False obviously disables it.
-        :param kwargs:      Any parameters you might wanna pass to bm3d or mvtools.
+    :param src:         Input to denoise
+    :param sigma:       Essentially strength for NLMeans and BM3D.
+                        Float or list of floats in this order [bm3d, nlm_uv] or [bm3d, nlm_u, nlm_v]
+    :param thSAD:       Not exactly strength but something like that, for mvtools.
+    :param radius:      Temporal Radius used for NLMeans and BM3D.
+                        Int or list of ints in this order [bm3d, nlm]
+    :param prefilter:   vsdenoise Prefilter or prefiltered clip to use for mvtools.
+                        Defaults to MINBLUR3
+    :param cuda:        Uses NlmCuda and BM3DCuda respectively if available. The latter prefers RTC if available.
+                        Will fallback to BM3DHip if installed and no cuda available.
+    :param csharp:      Apply contrasharpening after denoising. True defaults to 3 while False obviously disables it.
+    :param kwargs:      Any parameters you might wanna pass to bm3d or mvtools.
 
-        :return:            Denoised clip
+    :return:            Denoised clip
     """
-    if src.format.color_family != vs.YUV:
+    if src.format.color_family != vs.YUV:  # type: ignore
         raise ValueError("schizo_denoise: This function expects a full YUV clip.")
 
     if not isinstance(radius, list):
         radius = [radius, radius]
 
     if not isinstance(sigma, list):
         sigma = [sigma, sigma]
 
     if not isinstance(cuda, list):
         cuda = [cuda, cuda]
 
     if isinstance(prefilter, int):
         from vsdenoise import Prefilter
+
         prefilter = Prefilter(prefilter)
 
     clip = depth(src, 16)
 
     nlmfunc = core.knlm.KNLMeansCL if not hasattr(core, "nlm_cuda") or not cuda[0] else core.nlm_cuda.NLMeans
 
     if len(sigma) == 3:
-        clip_u = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[1], channels='U')
-        clip_v = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[2], channels='V')
-        nlm = join(get_y(clip), get_u(clip_u), get_v(clip_v))
+        clip_u = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[1], channels="U")
+        clip_v = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[2], channels="V")
+        nlm = join(get_y(clip), get_u(clip_u), get_v(clip_v))  # type: ignore
     else:
-        clip_uv = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[1], channels='UV')
-        nlm = join(clip, clip_uv)
+        clip_uv = nlmfunc(clip, a=nlm_a, d=radius[1], h=sigma[1], channels="UV")
+        nlm = join(clip, clip_uv)  # type: ignore
 
     # 'Extract' possible bm3d args before passing kwargs to mvtools :)
-    bm3dargs = dict(block_step=kwargs.pop("block_step", 8), bm_range=kwargs.pop("bm_range", 9),
-        ps_num=kwargs.pop("ps_num", 2), ps_range=kwargs.pop("ps_range", 4), fast=kwargs.pop("fast", True))
+    bm3dargs = dict(
+        block_step=kwargs.pop("block_step", 8),
+        bm_range=kwargs.pop("bm_range", 9),
+        ps_num=kwargs.pop("ps_num", 2),
+        ps_range=kwargs.pop("ps_range", 4),
+        fast=kwargs.pop("fast", True),
+    )
 
     y = get_y(clip)
     mv = VMDegrain(y, thSAD, prefilter, **kwargs)
 
-    if cuda[1]:
-        bm3dfunc = core.bm3dcuda if not hasattr(core, "bm3dcuda_rtc") else core.bm3dcuda_rtc
+    has_cuda = hasattr(core, "bm3dcuda") or hasattr(core, "bm3dcuda_rtc")
+    has_hip = hasattr(core, "bm3dhip")
+
+    if cuda[1] and (has_cuda or has_hip):
+        if has_cuda:
+            bm3dfunc = core.bm3dcuda if not hasattr(core, "bm3dcuda_rtc") else core.bm3dcuda_rtc
+        else:
+            bm3dfunc = core.bm3dhip
     else:
         bm3dargs.pop("fast")
         bm3dfunc = core.bm3dcpu
 
     bm3d = bm3dfunc.BM3Dv2(depth(y, 32), depth(mv, 32), sigma[0], radius=radius[0], **bm3dargs)
 
-    out = join(depth(bm3d, 16), nlm)
+    out = join(depth(bm3d, 16), nlm)  # type: ignore
     out = depth(out, get_depth(src))
     if csharp != False:
-        out = contrasharpening(out, src, mode = 3 if csharp == True else csharp)
-    return out
+        out = contrasharpening(out, src, mode=3 if csharp == True else csharp)
+    return out
```

### Comparing `vodesfunc-1.5.0/vodesfunc/descale.py` & `vodesfunc-1.6.0/vodesfunc/rescale.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,319 +1,406 @@
-from vstools import vs, core, get_y, depth, iterate, ColorRange, join, get_depth, FieldBased, FieldBasedT
-from vskernels import Scaler, ScalerT, Kernel, KernelT, Catrom
-from vsmasktools import EdgeDetectT, EdgeDetect
-from typing import Callable, Sequence, Union
-from math import floor
-from dataclasses import dataclass
-
-from .scale import Doubler, NNEDI_Doubler
-
-__all__ = ['DescaleTarget', 'MixedRescale', 'DT']
-
-def get_args(clip: vs.VideoNode, base_height: int, height: float, base_width: float = None):
-    base_height = float(base_height)
-    src_width = height * clip.width / clip.height
-    if not base_width:
-        base_width = clip.width
-    cropped_width = base_width - 2 * floor((base_width - src_width) / 2)
-    cropped_height = base_height - 2 * floor((base_height - height) / 2)
-    fractional_args = dict(height = cropped_height, width = cropped_width,
-        src_width = src_width, src_height = height, src_left = (cropped_width - src_width) / 2,
-        src_top = (cropped_height - height) / 2)
-    return fractional_args
-
-class TargetVals():
-    input_clip: vs.VideoNode | None = None
-    descale: vs.VideoNode | None = None
-    rescale: vs.VideoNode | None = None
+from vstools import (
+    vs,
+    core,
+    depth,
+    get_depth,
+    FunctionUtil,
+    get_h,
+    get_lowest_value,
+    padder,
+    KwargsT,
+    get_w,
+    GenericVSFunction,
+    ColorRange,
+    iterate,
+)
+from vskernels import KernelT, Kernel, ScalerT, Bilinear, Hermite
+from vsscale import fdescale_args
+from vsmasktools import EdgeDetectT, KirschTCanny
+from typing import Self, Any
+from math import ceil
+
+from .scale import Doubler
+
+__all__ = ["RescaleBuilder"]
+
+
+class RescaleNumbers:
+    height: float | int
+    width: float | int
+    base_height: int | None
+    base_width: int | None
+
+
+class RescaleClips:
+    descaled: vs.VideoNode
+    rescaled: vs.VideoNode
+    upscaled: vs.VideoNode | None = None
     doubled: vs.VideoNode | None = None
-    upscale: vs.VideoNode | None = None
+    linemask_clip: vs.VideoNode | None = None
+    errormask_clip: vs.VideoNode | None = None
 
-    index: int = 0
 
-@dataclass
-class DescaleTarget(TargetVals):
+class RescaleBuilder(RescaleClips, RescaleNumbers):
     """
-        Basically an entirely self contained rescaling utility class that can do pretty much everything.
+    Proof of concept Builder approach to rescaling.\n
+    Mostly ready for single rescale use. Not entirely sure how to handle multiple properly yet.
 
-        :param height:          Height to be descaled to.
-        :param kernel:          The kernel used for descaling.
-        :param upscaler:        Either a vodesfunc doubler or any scaler from vsscale used to upscale/double the descaled clip.
-        :param downscaler:      Any kernel or scaler used for downscaling the upscaled/doubled clip back to input res.
-        :param base_height:     Needed for fractional descales.
-        :param width:           Width to be descaled to. (will be calculated if None)
-        :param base_width:      Needed for fractional descales. (will be calculated if None)
-        :param shift:           Shifts to apply during the descaling and reupscaling.
-        :param do_post_double:  A function that's called on the doubled clip. Can be used to do sensitive processing on a bigger clip. (e. g. Dehaloing)
-        :param credit_mask:     Can be used to pass a mask that'll be used or False to disable error masking.
-        :param credit_mask_thr: The error threshold of the automatically generated credit mask.
-        :param credit_mask_bh:  Generates an error mask based on a descale using the base_height. For some reason had better results with this on some shows.
-        :param line_mask:       Can be used to pass a mask that'll be used or False to disable line masking.
-                                You can also pass a list containing edgemask function, scaler and thresholds to generate the mask on the doubled clip for potential better results.
-                                If None is passed to the first threshold then the mask won't be binarized. It will also run a Maximum and Inflate call on the mask.
-                                Example: line_mask=(KirschTCanny, Bilinear, 50 / 255, 150 / 255)
-        :param field_based:     Per-field descaling. Must be a FieldBased object. For example, `field_based=FieldBased.TFF`.
-                                This indicates the order the fields get operated in, and whether it needs special attention.
-                                Defaults to checking the input clip for the frameprop.
-        :param bbmod_masks:     Specify rows to be bbmod'ed for a clip to generate the masks on. Will probably be useful for the new border param in descale.
-    """
-    height: float
-    kernel: KernelT = Catrom
-    upscaler: Doubler | ScalerT = NNEDI_Doubler()
-    downscaler: ScalerT = Catrom
-    base_height: int | None = None
-    width: float | None = None
-    base_width: int | None = None
-    shift: tuple[int, int] = (0, 0)
-    do_post_double: Callable[[vs.VideoNode], vs.VideoNode] | None = None
-    credit_mask: vs.VideoNode | bool | None = None
-    credit_mask_thr: float = 0.04
-    credit_mask_bh: bool = False
-    line_mask: vs.VideoNode | bool | Sequence[Union[EdgeDetectT, ScalerT, float | None]] | None = None
-    field_based: FieldBasedT | None = None
-    bbmod_masks: int | list[int] = 0 # Not actually implemented yet lol
-
-    def generate_clips(self, clip: vs.VideoNode) -> 'DescaleTarget':
-        """
-            Generates descaled and rescaled clips of the given input clip
-
-            :param clip:    Clip to descale and rescale
-        """
-        self.kernel = Kernel.ensure_obj(self.kernel)
-        self.input_clip = clip.std.SetFrameProp('Target', self.index + 1)
-        bits, clip = get_depth(clip), get_y(clip)
-        self.height = float(self.height)
-
-        self.field_based = FieldBased.from_param(self.field_based) or FieldBased.from_video(clip)
-
-        if not self.width:
-            self.width = float(self.height * clip.width / clip.height)
-
-        if self.field_based.is_inter:
-            if not self.height.is_integer():
-                raise ValueError("DescaleTarget: `height` must be an integer when descaling an interlaced clip, not float.")
-            if not self.width.is_integer():
-                raise ValueError("DescaleTarget: `width` must be an integer when descaling an interlaced clip, not float.")
-
-            self._descale_fields(clip)
-
-            ref_y = self.rescale
-            clip = FieldBased.PROGRESSIVE.apply(clip)
-            self.line_mask = self.line_mask or False
-        elif self.height.is_integer():
-            self.descale = self.kernel.descale(clip, self.width, self.height, self.shift)
-            self.rescale = self.kernel.scale(self.descale, clip.width, clip.height, self.shift)
-            ref_y = self.rescale
-        else:
-            if self.base_height is None:
-                raise ValueError("DescaleTarget: height cannot be fractional if you don't pass a base_height.")
-            if not float(self.base_height).is_integer():
-                raise ValueError("DescaleTarget: Your base_height has to be an integer.")
-            if self.base_height < self.height:
-                raise ValueError("DescaleTarget: Your base_height has to be bigger than your height.")
-            self.frac_args = get_args(clip, self.base_height, self.height, self.base_width)
-            self.descale = self.kernel.descale(clip, **self.frac_args)  \
-                .std.CopyFrameProps(clip).std.SetFrameProp('Descale', self.index + 1)
-            self.frac_args.pop('width')
-            self.frac_args.pop('height')
-            self.rescale = self.kernel.scale(self.descale, clip.width, clip.height, **self.frac_args) \
-                .std.CopyFrameProps(clip).std.SetFrameProp('Rescale', self.index + 1)
-            if self.credit_mask_bh:
-                base_height_desc = self.kernel.descale(clip, self.base_height * (clip.width / clip.height), self.base_height)
-                ref_y = self.kernel.scale(base_height_desc, clip.width, clip.height)
-            else:
-                ref_y = self.rescale
-
-        if self.line_mask != False and not isinstance(self.line_mask, Sequence):
-            if not isinstance(self.line_mask, vs.VideoNode):
-                try:
-                    from vsmasktools.edge import KirschTCanny
-                    try:
-                        # Scaling was changed so I abuse the new param to check if its the newer version
-                        self.line_mask = KirschTCanny().edgemask(clip, lthr=80 / 255, hthr=150 / 255, planes=(0, True))
-                    except:
-                        self.line_mask = KirschTCanny().edgemask(clip, lthr=80 << 8, hthr=150 << 8)
-                except:
-                    from vsmask.edge import KirschTCanny
-                    self.line_mask = KirschTCanny().edgemask(clip, lthr=80 << 8, hthr=150 << 8)
-
-            if self.do_post_double is not None:
-                self.line_mask = self.line_mask.std.Inflate()
-
-            self.line_mask = depth(self.line_mask, bits)
-
-        if self.credit_mask != False or self.credit_mask_thr <= 0:
-            if not isinstance(self.credit_mask, vs.VideoNode):
-                self.credit_mask = core.std.Expr([depth(clip, 32), depth(ref_y, 32)], f"x y - abs {self.credit_mask_thr} < 0 1 ?")
-                self.credit_mask = depth(self.credit_mask, 16, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
-                self.credit_mask = self.credit_mask.rgvs.RemoveGrain(mode=6)
-                self.credit_mask = iterate(self.credit_mask, core.std.Maximum, 2)
-                self.credit_mask = iterate(self.credit_mask, core.std.Inflate, 2 if self.do_post_double is None else 4)
-
-            self.credit_mask = depth(self.credit_mask, bits)
+    Doesn't handle FieldBased yet.\n
+    (Do I even have to do anything? Pretty sure vskernels does most of the work nowadays)
 
-        return self
+    Example usage:
+    ```py
+    builder, rescaled = (
+        RescaleBuilder(clip)
+        .descale(Bilinear, 843.75, base_height=846)
+        .double()
+        .errormask(0.0975)
+        .linemask()
+        .post_double(lambda x: aa_dehalo(x)) # Or a function like post_double(aa_dehalo)
+        .downscale(Hermite(linear=True))
+        .final()
+    )
+    ```
+    """
 
-    def get_diff(self, clip: vs.VideoNode) -> vs.VideoNode:
+    funcutil: FunctionUtil
+    kernel: Kernel
+    post_crop: KwargsT | None = None
+    rescale_args: KwargsT = KwargsT()
+    shift: tuple[float, float] = (0, 0)
+    border_handling: int = 0
+    border_radius: int | None = None
+
+    def __init__(self, clip: vs.VideoNode):
+        self.funcutil = FunctionUtil(clip, self.__class__.__name__, planes=0, color_family=(vs.YUV, vs.GRAY), bitdepth=(16, 32))
+
+    def descale(
+        self,
+        kernel: KernelT,
+        height: float,
+        width: float | None = None,
+        base_height: int | None = None,
+        base_width: int | None = None,
+        shift: tuple[float, float] = (0, 0),
+        mode: str = "hw",
+        border_handling: int = 0,
+        border_radius: int | None = None,
+    ) -> Self:
         """
-            Returns a clip used for diff measuring ala getnative
+        Performs descale and rescale (with the same kernel).
 
-            :param clip:    Clip to compare the rescaled clip to
-            :return:        Diff clip
-        """
-        clip = depth(get_y(clip), 32)
-        diff = core.std.Expr([depth(self.rescale, 32), clip], ["x y - abs dup 0.015 > swap 0 ?"])
-        return diff.std.Crop(5, 5, 5, 5).std.PlaneStats()
+        :param kernel:              Kernel to descale with
+        :param height:              Height to descale to
+        :param width:               Width to descale to
+        :param base_height:         Padded height used in a "fractional" descale
+        :param base_width:          Padded width used in a "fractional" descale
+                                    Both of these are technically optional but highly recommended to have set for float width/height.
+
+        :param shift:               A custom shift to be applied
+        :param mode:                Whether to descale only height, only width, or both.
+                                    "h" or "w" respectively for the former two.
+
+        :param border_handling:     Adjust the way the clip is padded internally during the scaling process. Accepted values are:\n
+                                    0: Assume the image was resized with mirror padding.\n
+                                    1: Assume the image was resized with zero padding.\n
+                                    2: Assume the image was resized with extend padding, where the outermost row was extended infinitely far.\n
+                                    Defaults to 0.
 
-    def get_upscaled(self, clip: vs.VideoNode, chroma: vs.VideoNode | None = None) -> vs.VideoNode:
+        :param border_radius:       Radius for the border mask. Only used when border_handling is set to 1 or 2.
+                                    Defaults to kernel radius if possible, else 2.
         """
-            Generates and returns the fully upscaled & masked & what not clip
-        """
-        if self.descale == None or self.rescale == None:
-            self.generate_clips(clip)
-
-        bits, y = get_depth(clip), get_y(clip)
-
-        if isinstance(self.upscaler, Doubler):
-            self.doubled = self.upscaler.double(self.descale)
-        else:
-            self.upscaler = Scaler.ensure_obj(self.upscaler)
-            self.doubled = self.upscaler.scale(self.descale, self.descale.width * 2, self.descale.height * 2)
-
-        if self.do_post_double is not None:
-            self.doubled = self.do_post_double(self.doubled)
-
-        self.downscaler = Scaler.ensure_obj(self.downscaler)
-        if hasattr(self, 'frac_args'):
-            # TODO: Figure out how to counteract shift during descaling (if we want to?), maybe additive?
-            self.frac_args.update({key: value * 2 for (key, value) in self.frac_args.items()})
-            self.upscale = self.downscaler.scale(self.doubled, clip.width, clip.height, **self.frac_args)
-            self.upscale = self.upscale.std.CopyFrameProps(self.rescale)
+        clip = self.funcutil.work_clip
+        self.kernel = Kernel.ensure_obj(kernel)
+        self.shift = shift
+        self.border_handling = self.kernel.kwargs.pop("border_handling", border_handling)
+        self.border_radius = border_radius
+
+        if float(height).is_integer():
+            if not width:
+                width = get_w(height, clip)
+            self.width = int(width) if "w" in mode else clip.width
+            self.height = int(height) if "h" in mode else clip.height
+            self.descaled = self.kernel.descale(
+                clip,
+                self.width,
+                self.height,
+                shift=shift,
+                border_handling=self.border_handling,
+            )
+            self.rescaled = perform_rescale(self)
         else:
-            self.upscale = self.downscaler.scale(self.doubled, clip.width, clip.height, tuple(-sh for sh in self.shift))
-
-        self.upscale = depth(self.upscale, bits)
-        self.rescale = depth(self.rescale, bits)
-
-        if self.line_mask != False:
-            if isinstance(self.line_mask, Sequence):
-                if len(self.line_mask) < 4:
-                    raise ValueError("DescaleTarget: line_mask must contain an Edgemask, Downscaler, lthr and hthr if you passed a list.")
-                mask_fun = EdgeDetect.ensure_obj(self.line_mask[0])
-                if self.line_mask[2] is None:
-                    mask = mask_fun.edgemask(self.doubled, planes=0).std.Maximum().std.Inflate()
-                else:
-                    mask = mask_fun.edgemask(self.doubled, self.line_mask[2], self.line_mask[3], planes=0)
-                self.line_mask = Scaler.ensure_obj(self.line_mask[1]).scale(mask, clip.width, clip.height)
-
-            if get_depth(self.line_mask) == 32:
-                self.line_mask = self.line_mask.std.Limiter()
-            self.upscale = y.std.MaskedMerge(self.upscale, self.line_mask)
-
-        if self.credit_mask != False or self.credit_mask_thr <= 0:
-            if get_depth(self.credit_mask) == 32:
-                self.credit_mask = self.credit_mask.std.Limiter()
-            self.upscale = self.upscale.std.MaskedMerge(y, self.credit_mask)
-
-        self.upscale = depth(self.upscale, bits)
-        self.upscale = self.upscale if clip.format.color_family == vs.GRAY else join(self.upscale, clip)
-        return self.upscale if not chroma else join(depth(self.upscale, get_depth(chroma)), depth(chroma, get_depth(chroma)))
-
-    def _return_creditmask(self) -> vs.VideoNode:
-        return core.std.BlankClip(self.input_clip) if self.credit_mask == False else self.credit_mask
-
-    def _return_linemask(self) -> vs.VideoNode:
-        return core.std.BlankClip(self.input_clip) if self.line_mask == False else self.line_mask
-
-    def _return_doubled(self) -> vs.VideoNode:
-        return core.std.BlankClip(self.input_clip, width=self.input_clip * 2) if not self.doubled else self.doubled
-
-    def _descale_fields(self, clip: vs.VideoNode) -> None:
-        wclip = self.field_based.apply(clip)
+            sanitized_shift = (shift[0] if shift[0] else None, shift[1] if shift[1] else None)
+            args, self.post_crop = fdescale_args(clip, height, base_height, base_width, sanitized_shift[0], sanitized_shift[1], width, mode)
+            _, self.rescale_args = fdescale_args(
+                clip, height, base_height, base_width, sanitized_shift[0], sanitized_shift[1], width, mode, up_rate=1
+            )
+            self.height = args.get("src_height", clip.height)
+            self.width = args.get("src_width", clip.width)
+            self.base_height = base_height
+            self.base_width = base_width
 
-        self.descale = self.kernel.descale(wclip, self.width, self.height)
-        self.rescale = self.kernel.scale(self.descale, clip.width, clip.height)
+            self.descaled = self.kernel.descale(clip, border_handling=self.border_handling, **args)
+            self.rescaled = perform_rescale(self, **self.rescale_args)
+        return self
 
-        self.descale = FieldBased.PROGRESSIVE.apply(self.descale)
-        self.rescale = FieldBased.PROGRESSIVE.apply(self.rescale)
+    def post_descale(self, func: GenericVSFunction) -> Self:
+        """
+        A function to apply any arbitrary function on the descaled clip.\n
+        I can't think of a good usecase/example for this but I was asked to add this before.
 
-    @staticmethod
-    def crossconv_shift_calc_irregular(clip: vs.VideoNode, native_height: int) -> float:
-        """Calculate the shift for an irregular cross-conversion."""
-        return 0.25 / (clip.height / native_height)
+        :param func:    This can be any function that takes a videonode input and returns a videonode.
+                        You are responsible for keeping the format the same.
+        """
+        self.descaled = func(self.descaled)
+        return self
 
-DT = DescaleTarget
+    def linemask(
+        self,
+        mask: vs.VideoNode | EdgeDetectT | None = None,
+        downscaler: ScalerT | None = None,
+        maximum_iter: int = 0,
+        inflate_iter: int = 0,
+        expand: int | tuple[int, int | None] = 0,
+        **kwargs,
+    ) -> Self:
+        """
+        A function to apply a linemask to the final output.
 
-class MixedRescale:
-    def __init__(self, src: vs.VideoNode, *targets: DescaleTarget) -> None:
+        :param mask:            This can be a masking function like `KirschTCanny` (also the default if `None`) or a clip.
+        :param downscaler:      Downscaler to use if creating a linemask on the doubled clip. Defaults to `Bilinear` if `None`.
+        :param maximum_iter:    Apply std.Maximum x amount of times
+        :param inflate_iter:    Apply std.inflate x amount of times
+        :param expand:          Apply an ellipse morpho expand with the passed amount.
+                                Can be a tuple of (horizontal, vertical) or a single value for both.
+        :param **kwargs:        Any other params to pass to the edgemask creation. For example `lthr` or `hthr`.
         """
-            A naive per-frame diff approach of trying to get the best descale.
-            Credits to Setsu for most of this class.
+        if isinstance(mask, vs.VideoNode):
+            self.linemask_clip = mask
+            if self.border_handling:
+                self.linemask_clip = self._crop_mask_bord(self.linemask_clip)
+            return self
+        edgemaskFunc = KirschTCanny.ensure_obj(mask)
+
+        # Perform on doubled clip if exists and downscale
+        if self.doubled:
+            scaler = Bilinear.ensure_obj(downscaler)
+            self.linemask_clip = edgemaskFunc.edgemask(self.doubled, **kwargs)
+            self.linemask_clip = scaler.scale(self.linemask_clip, self.funcutil.work_clip.width, self.funcutil.work_clip.height)
+        else:
+            self.linemask_clip = edgemaskFunc.edgemask(self.funcutil.work_clip, **kwargs)
 
+        self.linemask_clip = self._process_mask(self.linemask_clip, maximum_iter, inflate_iter, expand)
 
-            Example usage:
-            ```
-            t1 = DT(847.1, Bilinear(), base_height=848)
-            t2 = DescaleTarget(843.75, Bilinear(), base_height=846)
+        if self.border_handling:
+            self.linemask_clip = self._crop_mask_bord(self.linemask_clip)
 
-            rescaled = MixedRescale(clip, t1, t2)
+        return self
 
-            out(rescaled.final)
-            out(rescaled.line_mask)
-            ```
+    def errormask(
+        self, mask: vs.VideoNode | float = 0.05, maximum_iter: int = 2, inflate_iter: int = 3, expand: int | tuple[int, int | None] = 0
+    ) -> Self:
         """
-        y = get_y(src)
+        A function to apply a basic error mask to the final output.
 
-        for i, d in enumerate(targets):
-            d.index = i
-            d.generate_clips(y)
+        :param mask:            With a float, and by default, will be created internally. Could also pass a clip.
+        :param maximum_iter:    Apply std.Maximum x amount of times
+        :param inflate_iter:    Apply std.inflate x amount of times
+        :param expand:          Apply an ellipse morpho expand with the passed amount.
+                                Can be a tuple of (horizontal, vertical) or a single value for both.
+        """
+        if isinstance(mask, vs.VideoNode):
+            self.errormask_clip = mask
+            return self
+
+        err_mask = core.std.Expr([depth(self.funcutil.work_clip, 32), depth(self.rescaled, 32)], f"x y - abs {mask} < 0 1 ?")
+        err_mask = depth(err_mask, 16, range_out=ColorRange.FULL, range_in=ColorRange.FULL)
+        err_mask = err_mask.rgvs.RemoveGrain(mode=6)
+        err_mask = self._process_mask(err_mask, maximum_iter, inflate_iter, expand)
+        self.errormask_clip = depth(err_mask, get_depth(self.funcutil.work_clip))
 
-        prop_srcs = [d.get_diff(y) for d in targets]
-        targets_idx = tuple(range(len(targets)))
+        if self.border_handling:
+            self.errormask_clip = self._crop_mask_bord(self.errormask_clip)
 
-        blank = core.std.BlankClip(None, 1, 1, vs.GRAY8, src.num_frames, keep=True)
+        return self
 
-        map_prop_srcs = [
-            blank.std.CopyFrameProps(prop_src).akarin.Expr('x.PlaneStatsAverage', vs.GRAYS)
-            for prop_src in prop_srcs
-        ]
+    def double(self, upscaler: Doubler | ScalerT | None = None) -> Self:
+        """
+        Upscales the descaled clip by 2x
 
-        base_frame, idx_frames = blank.get_frame(0), []
+        :param upscaler:        Any kind of vsscale scaler. Defaults to Waifu2x.
+        """
+        if isinstance(upscaler, Doubler):
+            self.doubled = upscaler.double(self.descaled)
+        else:
+            from vsscale import Waifu2x
 
-        for i in targets_idx:
-            fcurr = base_frame.copy()
+            scaler = Waifu2x.ensure_obj(upscaler)  # type: ignore
+            self.doubled = scaler.multi(self.descaled)
+        return self
 
-            fcurr[0][0, 0] = i
+    def post_double(self, func: GenericVSFunction) -> Self:
+        """
+        A function to apply any arbitrary function on the doubled clip.
 
-            idx_frames.append((i, fcurr))
+        :param func:    This can be any function that takes a videonode input and returns a videonode.
+                        You are responsible for keeping the format the same.
+        """
+        if not self.doubled:
+            raise SyntaxError("post_double: Doubled clip has not been generated yet. Please call this after double().")
+        self.doubled = func(self.doubled)
+        return self
 
-        def _select(n: int, f: vs.VideoFrame) -> vs.VideoFrame:
-            return min(idx_frames, key=lambda i: f[i[0]][0][0, 0])[1]
+    def downscale(self, downscaler: ScalerT | None = None) -> Self:
+        """
+        Downscales the clip back the size of the original input clip and applies the masks, if any.
 
-        _select_clip = blank.std.ModifyFrame(map_prop_srcs, _select)
+        :param downscaler:      Any vsscale scaler to use. Defaults to Linear Hermite.
+        """
+        scaler = Hermite(linear=True).ensure_obj(downscaler)
+        if not self.doubled:
+            raise SyntaxError("Downscale/Final is the last one that should be called in a chain!")
+        wclip = self.funcutil.work_clip
+        if self.post_crop:
+            self.upscaled = scaler.scale(self.doubled, wclip.width, wclip.height, **self.post_crop)
+        else:
+            self.upscaled = scaler.scale(self.doubled, wclip.width, wclip.height, (self.shift[0] * 2, self.shift[1] * 2))
 
-        def _selector(clips: list[vs.VideoNode | None]) -> vs.VideoNode:
-            base = next(filter(None, clips), None)
+        if isinstance(self.errormask_clip, vs.VideoNode) and isinstance(self.linemask_clip, vs.VideoNode):
+            self.final_mask = core.std.Expr([self.linemask_clip.std.Limiter(), self.errormask_clip], "x y -")
+            self.upscaled = wclip.std.MaskedMerge(self.upscaled, self.final_mask.std.Limiter())
+        elif isinstance(self.errormask_clip, vs.VideoNode):
+            self.upscaled = self.upscaled.std.MaskedMerge(wclip, self.errormask_clip.std.Limiter())
+        elif isinstance(self.linemask_clip, vs.VideoNode):
+            self.upscaled = wclip.std.MaskedMerge(self.upscaled, self.linemask_clip.std.Limiter())
 
-            if base is None:
-                raise ValueError('Requested clip was None')
+        return self
 
-            base = base.std.BlankClip(keep=True)
-            clips = [c or base for c in clips]
+    def final(self) -> tuple[Self, vs.VideoNode]:
+        """
+        This is the last function in the chain that also returns the final clip.
+        It internally calls `downscale` if you haven't done so before and then merges the resulting clip with the input chroma, if any.
 
-            return core.std.FrameEval(
-                base, lambda n, f: clips[f[0][0, 0]], _select_clip
+        :return: A tuple of this class and the resulting final rescale.
+        """
+        if not self.upscaled:
+            self.downscale()
+        if not self.upscaled:
+            raise TypeError("No downscaled clip has been generated yet!")
+
+        return (self, self.funcutil.return_clip(self.upscaled))
+
+    def _process_mask(
+        self, mask: vs.VideoNode, maximum_iter: int = 0, inflate_iter: int = 0, expand: int | tuple[int, int | None] = 0
+    ) -> vs.VideoNode:
+        if maximum_iter:
+            mask = iterate(mask, core.std.Maximum, maximum_iter)
+
+        if inflate_iter:
+            mask = iterate(mask, core.std.Inflate, inflate_iter)
+
+        if expand:
+            if isinstance(expand, int):
+                expand = (expand, expand)
+            from vsmasktools import Morpho, XxpandMode
+
+            mask = Morpho.expand(mask, expand[0], expand[1], XxpandMode.ELLIPSE)
+
+        return mask
+
+    def _crop_mask_bord(self, mask: vs.VideoNode, color: float = 0.0) -> vs.VideoNode:
+        if not hasattr(self, "_bord_crop_args"):
+            self._bord_crop_args = get_border_crop(self)
+
+        return mask.std.Crop(*self._bord_crop_args).std.AddBorders(*self._bord_crop_args, color=color)
+
+    @property
+    def _kernel_window(self) -> int:
+        if (bord_rad := self.border_radius) is None:
+            try:
+                bord_rad = self.kernel.kernel_radius
+            except (AttributeError, NotImplementedError):
+                bord_rad = 2
+
+        return bord_rad
+
+
+def perform_rescale(builder: RescaleBuilder, **kwargs: Any) -> vs.VideoNode:
+    input_clip = builder.funcutil.work_clip
+    clip = builder.descaled
+    match int(builder.border_handling):
+        case 1:
+            clip = clip.std.AddBorders(
+                *((0, 0) if builder.width == input_clip.width else (10, 10)),
+                *((0, 0) if builder.height == input_clip.height else (10, 10)),
+                get_lowest_value(clip, False, ColorRange.from_video(clip)),
+            )
+        case 2:
+            clip = padder(
+                clip,
+                *((0, 0) if builder.width == input_clip.width else (10, 10)),
+                *((0, 0) if builder.height == input_clip.height else (10, 10)),
+                reflect=False,
             )
+        case _:
+            pass
 
-        self.upscaled = _selector([t.get_upscaled(t.input_clip) if src.format.color_family == vs.GRAY else t.get_upscaled(t.input_clip, src) for t in targets])
-        #self.upscaled = depth(self.upscaled, get_depth(src))
-        self.final = self.upscaled
-
-        self.rescaled = _selector([t.rescale for t in targets])
-        # These two are not working yet because I need to figure out how to make the base clip up there use varres
-        #self.descaled = _selector([t.descale for t in targets])
-        #self.doubled = _selector([t._return_doubled() for t in targets])
-        self.credit_mask = _selector([t._return_creditmask() for t in targets])
-        self.line_mask = _selector([t._return_linemask() for t in targets])
+    shift_top = kwargs.pop("src_top", False) or builder.shift[0]
+    shift_left = kwargs.pop("src_left", False) or builder.shift[1]
 
-    def get_upscaled(self, *_) -> vs.VideoNode:
-        return self.upscaled
+    shift = [
+        shift_top + (builder.height != input_clip.height and builder.border_handling) * 10,
+        shift_left + (builder.width != input_clip.width and builder.border_handling) * 10,
+    ]
+
+    src_width = kwargs.pop("src_width", clip.width)
+    src_height = kwargs.pop("src_height", clip.height)
+
+    return builder.kernel.scale(
+        clip,
+        input_clip.width,
+        input_clip.height,
+        shift,  # type: ignore # Why?
+        src_width=src_width - ((clip.width - builder.width) if float(builder.width).is_integer() else 0),
+        src_height=src_height - ((clip.height - builder.height) if float(builder.width).is_integer() else 0),
+    )
+
+
+def get_border_crop(builder: RescaleBuilder) -> tuple:
+    input_clip = builder.funcutil.work_clip
+    # fmt: off
+    if builder.height == input_clip.height:
+        vertical_crop = (0, 0)
+    else:
+        base_height = builder.base_height or get_h(builder.base_width, builder.descaled) if builder.base_width else builder.height
+        src_top = builder.rescale_args.get("src_top", False) or builder.shift[0]
+        top = max(ceil(
+            (-(builder.height - 1) / 2 + builder._kernel_window - src_top - 1)
+            * input_clip.height / builder.height + (input_clip.height - 1) / 2
+        ), 0)
+
+        bottom = max(ceil(
+            (-(builder.height - 1) / 2 + builder._kernel_window - (base_height - builder.height - src_top) - 1)
+            * input_clip.height / builder.height + (input_clip.height - 1) / 2
+        ), 0)
+
+        vertical_crop = (top, bottom)
+
+    if builder.width == input_clip.width:
+        horizontal_crop = (0, 0)
+    else:
+        base_width = builder.base_width or get_w(builder.base_height, builder.descaled) if builder.base_height else builder.width
+        src_left = builder.rescale_args.get("src_left", False) or builder.shift[1]
+
+        left = max(ceil(
+            (-(builder.width - 1) / 2 + builder._kernel_window - src_left - 1)
+            * input_clip.width / builder.width + (input_clip.width - 1) / 2
+        ), 0)
+
+        right = max(ceil(
+            (-(builder.width - 1) / 2 + builder._kernel_window - (base_width - builder.width - src_left) - 1)
+            * input_clip.width / builder.width + (input_clip.width - 1) / 2
+        ), 0)
+
+        horizontal_crop = (left, right)
+    # fmt: on
+    return horizontal_crop + vertical_crop
```

### Comparing `vodesfunc-1.5.0/vodesfunc/misc.py` & `vodesfunc-1.6.0/vodesfunc/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from vstools import vs, core, depth, get_y
+from typing import Any
 from functools import partial
 
 __all__ = ["dirty_prop_set"]
 
 
 def dirty_prop_set(
     clip: vs.VideoNode,
     threshold: int = 1100,
     luma_scaling: int = 24,
-    prop_name: str = None,
-    src_prop_val: any = None,
-    bbm_prop_val: any = None,
+    prop_name: str | None = None,
+    src_prop_val: Any | None = None,
+    bbm_prop_val: Any | None = None,
     debug_output: bool = False,
 ) -> list[vs.VideoNode]:
     """
     Dirty-edge-based frameprop setting function using bbm, a brightness difference check and a brightness scaling
     (might be a very specific usecase)
 
     Returns both filtered clip and mask in a VideoNode List (0 = clip, 1 = mask)
@@ -24,19 +25,19 @@
 
         dirty_prop_set(.., prop_name = 'Rescale', src_prop_val = 812, bbm_prop_val = 720)
     """
 
     def _select_frame(n: int, f: vs.VideoFrame, clip_a: vs.VideoNode, clip_b: vs.VideoNode) -> vs.VideoNode:
         plane_stats_average = f.props["PlaneStatsAverage"]
         # print(f"Frame {n}: {plane_stats_average:.20f}")
-        return clip_b if plane_stats_average > 0.00010 else clip_a
+        return clip_b if plane_stats_average > 0.00010 else clip_a  # type: ignore
 
     def _get_mask(n: int, f: vs.VideoFrame, clip_a: vs.VideoNode, clip_b: vs.VideoNode) -> vs.VideoNode:
         brightness = f.props["PlaneStatsAverage"]
-        weighted_thr = threshold * (1 - (1 - brightness) ** (brightness**2 * luma_scaling))
+        weighted_thr = threshold * (1 - (1 - brightness) ** (brightness**2 * luma_scaling))  # type: ignore
         if debug_output:
             print(f"Frame {n}: Average Brightness - {brightness:.20f}, Weighted - {weighted_thr:.20f}")
         return core.std.Expr([clip_a, clip_b], [f"y x - {weighted_thr} > 65536 0 ?", ""])
 
     try:
         import awsmfunc as awf
     except:
```

### Comparing `vodesfunc-1.5.0/vodesfunc/noise.py` & `vodesfunc-1.6.0/vodesfunc/noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Sequence, Callable
 from vstools import vs, core, get_depth, scale_value, split, normalize_seq, get_neutral_value, get_peak_value, mod4
-from vskernels import Scaler, Lanczos, BicubicDidee
+from vskernels import Scaler, Lanczos, Bicubic
 
 __all__ = ["adaptive_grain", "grain", "ntype4"]
 
-ntype4 = {"type": 2, "scale": 0.7, "scaler": BicubicDidee()}
-itype4 = {"type": 2, "size": 0.769, "sharp": BicubicDidee(), "protect_chroma": True, "fade_limits": True}
+ntype4 = {"type": 2, "scale": 0.7, "scaler": Bicubic(b=-1 / 2, c=1 / 4)}
+itype4 = {"type": 2, "size": 0.769, "sharp": Bicubic(b=-1 / 2, c=1 / 4), "protect_chroma": True, "fade_limits": True}
 
 
 def adaptive_grain(
     clip: vs.VideoNode,
     strength: float | list[float] = [2.0, 0.5],
     size: float | list[float] = 3,
     type: int = 3,
```

### Comparing `vodesfunc-1.5.0/vodesfunc/scale.py` & `vodesfunc-1.6.0/vodesfunc/scale.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,25 @@
 from typing import Any, Callable
-from vskernels import Catrom, Kernel, Scaler, ScalerT, Lanczos, Point
-from vstools import inject_self, vs, core, depth, get_depth, get_y, Matrix, KwargsT, get_nvidia_version, Transfer
+from vskernels import Catrom, Lanczos
+from vstools import inject_self, vs, core, depth, get_depth, get_y, Matrix, KwargsT, get_nvidia_version
 from vsrgtools.sharp import unsharp_masked
-from .types import PathLike
 from abc import ABC, abstractmethod
+from vsmuxtools import ensure_path_exists, PathLike
 
 
 __all__: list[str] = [
     "NNEDI_Doubler",
     "Clamped_Doubler",
     "Shader_Doubler",
     "Waifu2x_Doubler",
-    "LinearScaler",
     "Lanczos_PreSS",
-    "SigmoidScaler",
 ]
 
 
-class LinearScaler(Scaler):
-    def __init__(self, scaler: ScalerT, **kwargs: KwargsT) -> None:
-        """
-        Simple scaler class to do your scaling business in linear light.
-
-        :params scaler:     Any vsscale scaler class/object
-        """
-        self.scaler = Scaler.ensure_obj(scaler)
-        self.kwargs = kwargs
-
-    def scale(self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs) -> vs.VideoNode:
-        if clip.format.subsampling_h != 0 or clip.format.subsampling_w != 0:
-            print(clip.format.subsampling_h, clip.format.subsampling_w)
-            raise ValueError("LinearScaler: Using linear scaling on a subsampled clip results in very poor output. Please don't do it.")
-
-        trans_in = Transfer.from_video(clip)
-        clip = clip.resize.Point(transfer_in=trans_in, transfer=Transfer.LINEAR)
-        args = KwargsT(clip=clip, width=width, height=height, shift=shift)
-        args.update(**kwargs)
-        args.update(**self.kwargs)
-        scaled = self.scaler.scale(**args)
-        return scaled.resize.Point(transfer_in=Transfer.LINEAR, transfer=trans_in)
-
-
-class SigmoidScaler(Scaler):
-    def __init__(self, scaler: ScalerT, sig_slope: float = 6.5, sig_center: float = 0.75, **kwargs: KwargsT) -> None:
-        """
-        Simple scaler class to do your scaling business in sigmoid light.
-
-        :params scaler:     Any vsscale scaler class/object
-        :param sig_slope:   Curvature value for the sigmoid curve, in range 1-20. The higher the curvature value, the more non-linear the function.
-        :param sig_center:  Inflection point for the sigmoid curve, in range 0-1. The closer to 1, the more the curve looks like a standard power curve.
-        """
-        self.scaler = Scaler.ensure_obj(scaler)
-        self.sig_slope = sig_slope
-        self.sig_center = sig_center
-        self.kwargs = kwargs
-
-    def scale(self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs) -> vs.VideoNode:
-        from math import exp
-        from vsexprtools import norm_expr, ExprOp
-
-        sig_slope = self.sig_slope
-        sig_center = self.sig_center
-        if not 1.0 <= sig_slope <= 20.0:
-            raise ValueError("sig_slope only accepts values from 1.0 to 20.0 inclusive.")
-        if not 0.0 <= sig_center <= 1.0:
-            raise ValueError("sig_center only accepts values from 0.0 to 1.0 inclusive.")
-        if clip.format.subsampling_h != 0 or clip.format.subsampling_w != 0:
-            raise ValueError("SigmoidScaler: Using sigmoid scaling on a subsampled clip results in very poor output. Please don't do it.")
-
-        trans_in = Transfer.from_video(clip)
-        convert_csp = (Matrix.from_transfer(trans_in), clip.format)
-        sig_offset = 1.0 / (1 + exp(sig_slope * sig_center))
-        sig_scale = 1.0 / (1 + exp(sig_slope * (sig_center - 1))) - sig_offset
-
-        bits, clip = get_depth(clip), depth(clip, 32)
-        if clip.format and clip.format.color_family is not vs.RGB:
-            clip = Point.resample(clip, vs.RGBS, None, convert_csp[0])
-        clip = clip.resize.Point(transfer_in=trans_in, transfer=Transfer.LINEAR)
-        expr = f"{sig_center} 1 x {sig_scale} * {sig_offset} + / 1 - log {sig_slope} / -"
-        clip = norm_expr(clip, f"{expr} {ExprOp.clamp(0, 1)}")
-        args = KwargsT(clip=clip, width=width, height=height, shift=shift)
-        args.update(**kwargs)
-        args.update(**self.kwargs)
-        scaled = self.scaler.scale(**args)
-        expr = f"1 1 {sig_slope} {sig_center} x - * exp + / {sig_offset} - {sig_scale} /"
-        scaled = norm_expr(scaled, f"{expr} {ExprOp.clamp(0, 1)}")
-        scaled = Point.resample(scaled, convert_csp[1], convert_csp[0], transfer_in=Transfer.LINEAR, transfer=trans_in)
-        return depth(scaled, bits)
-
-
-class Lanczos_PreSS(Scaler):
+class Lanczos_PreSS(Lanczos):
     """
     Convenience class to pass to a dehalo function.
     This serves the same purpose as NNEDI to double and reverse using point.
     Except it is a quite a bit faster and (if using opencl) takes a lot of load off the GPU.
     """
 
     @inject_self.init_kwargs.clean
@@ -163,28 +89,28 @@
 
     def __init__(self, shaderfile: PathLike = r"C:\FSRCNNX_x2_56-16-4-1.glsl") -> None:
         """
         Simple utility class for doubling a clip using a glsl shader
 
         :param shaderfile:      The glsl shader used to double the resolution
         """
-        self.shaderfile = shaderfile if isinstance(shaderfile, str) else str(shaderfile.resolve())
+        self.shaderfile = str(ensure_path_exists(shaderfile, self))
 
     def double(self, clip: vs.VideoNode) -> vs.VideoNode:
         y = depth(get_y(clip), 16)
         filler_chroma = core.std.BlankClip(y, format=vs.YUV444P16)
         doubled = core.std.ShufflePlanes([y, filler_chroma], [0, 1, 2], vs.YUV).placebo.Shader(
             self.shaderfile, filter="box", width=y.width * 2, height=y.height * 2
         )
         doubled_y = get_y(doubled)
         return depth(doubled_y, get_depth(clip))
 
 
 class Waifu2x_Doubler(Doubler):
-    backend: any
+    backend: Any
     kwargs: KwargsT
     w2xargs: KwargsT = {}
 
     def __init__(
         self,
         cuda: bool | str | None = None,
         fp16: bool = True,
@@ -201,28 +127,31 @@
         :param fp16:            Uses 16 bit floating point internally if True.
         :param num_streams:     Amount of streams to use for Waifu2x; Sacrifices a lot of vram for a speedup.
         :param tiles:           Splits up the upscaling process into multiple tiles.
                                 You will likely have to use atleast `2` if you have less than 16 GB of VRAM.
         :param model:           Model to use from vsmlrt.
         :param kwargs:          Args that get passed to both the Backend and actual scaling function.
         """
-        from vsmlrt import Backend
+        from vsmlrt import Backend, backendT
 
         self.kwargs = {"num_streams": num_streams, "fp16": fp16}
 
+        if "backend" in kwargs.keys():
+            cuda = False
+
         # Partially stolen from setsu but removed useless stuff that is default in mlrt already and added version checks
         if cuda is None:
             nv = get_nvidia_version()
             cuda = nv is not None
             try:
                 if nv is not None and not hasattr(core, "trt") and hasattr(core, "ort"):
                     self.kwargs.update({"use_cuda_graph": True})
                 else:
-                    props: KwargsT = core.trt.DeviceProperties(kwargs.get("device_id", 0))
-                    version_props: KwargsT = core.trt.Version()
+                    props: KwargsT = core.trt.DeviceProperties(kwargs.get("device_id", 0))  # type: ignore
+                    version_props: KwargsT = core.trt.Version()  # type: ignore
 
                     vram = props.get("total_global_memory", 0)
                     trt_version = float(version_props.get("tensorrt_version", 0))
 
                     cuda = "trt"
 
                     presumedArgs = KwargsT(
@@ -250,24 +179,27 @@
             tilesize=kwargs.pop("tilesize", None),
             overlap=kwargs.pop("overlap", None),
         )
 
         self.kwargs.update(kwargs)
 
         if cuda is False:
-            if hasattr(core, "ncnn"):
-                self.backend = Backend.NCNN_VK(**self.kwargs)
+            backend = kwargs.pop("backend", None)
+            if backend and isinstance(backend, backendT):
+                self.backend = backend
             else:
-                self.kwargs.pop("device_id")
-                self.backend = Backend.ORT_CPU(**self.kwargs) if hasattr(core, "ort") else Backend.OV_CPU(**self.kwargs)
+                if hasattr(core, "ncnn"):
+                    self.backend = Backend.NCNN_VK(**self.kwargs)
+                else:
+                    self.kwargs.pop("device_id")
+                    self.backend = Backend.ORT_CPU(**self.kwargs) if hasattr(core, "ort") else Backend.OV_CPU(**self.kwargs)
         elif cuda is True:
             self.backend = Backend.ORT_CUDA(**self.kwargs) if hasattr(core, "ort") else Backend.OV_GPU(**self.kwargs)
         else:
             self.backend = Backend.TRT(**self.kwargs)
-
         self.kwargs = kwargs
         self.model = model
 
     def double(self, clip: vs.VideoNode) -> vs.VideoNode:
         from vsmlrt import Waifu2x
 
         pre = depth(clip, 32).std.Limiter()
@@ -275,15 +207,15 @@
         (left, right, top, bottom) = mod_padding(pre)
         width = pre.width + left + right
         height = pre.height + top + bottom
         pad = pre.resize.Point(width, height, src_left=-left, src_top=-top, src_width=width, src_height=height)
 
         # Model 0 wants a gray input
         needs_gray = self.w2xargs.get("model", 6) == 0
-        was_444 = pre.format.color_family == vs.YUV and pre.format.subsampling_w == 0 and pre.format.subsampling_h == 0 and not needs_gray
+        was_444 = pre.format.color_family == vs.YUV and pre.format.subsampling_w == 0 and pre.format.subsampling_h == 0 and not needs_gray  # type: ignore
 
         if was_444:
             pad = Catrom().resample(pad, format=vs.RGBS, matrix=Matrix.RGB, matrix_in=Matrix.from_video(pre))
         elif needs_gray is True:
             pad = get_y(pad)
         else:
             pad = get_y(pad).std.ShufflePlanes(0, vs.RGB)
@@ -302,20 +234,20 @@
             up = up.std.Expr("x 0.5 255 / +")
 
         return depth(up, get_depth(clip)).std.CopyFrameProps(pre)
 
 
 class Clamped_Doubler(Doubler):
     sharp_doubler: Doubler
-    sharpen_smooth: bool | vs.VideoNode | Callable[[vs.VideoNode], vs.VideoNode] = None
+    sharpen_smooth: bool | vs.VideoNode | Callable[[vs.VideoNode], vs.VideoNode] | None = None
 
     def __init__(
         self,
-        sharpen_smooth: bool | vs.VideoNode | Callable[[vs.VideoNode], vs.VideoNode] = False,
-        sharp_doubler: Doubler | str = Shader_Doubler(),
+        sharpen_smooth: bool | vs.VideoNode | Callable[[vs.VideoNode], vs.VideoNode],
+        sharp_doubler: Doubler | str,
         ratio: int = 100,
         **kwargs,
     ) -> None:
         """
         Simple utility class for doubling a clip using fsrcnnx / any shader clamped to nnedi.
         Using sharpen will be basically the same as the zastin profile in varde's fsrcnnx upscale.
         Not sharpening will on the other hand be the same as the slow profile.
@@ -330,15 +262,15 @@
                                 nnedi params: see `NNEDI_Doubler`
                                 overshoot, undershoot for non-sharpen mode (defaults to ratio / 100)
         """
         self.sharp_doubler = Shader_Doubler(sharp_doubler) if isinstance(sharp_doubler, str) else sharp_doubler
         self.sharpen_smooth = sharpen_smooth
 
         if ratio > 100 or ratio < 1:
-            raise "Clamped_Doubler: ratio should be a value between 1 and 100"
+            raise ValueError("Clamped_Doubler: ratio should be a value between 1 and 100")
         self.ratio = ratio
         self.kwargs = kwargs
 
     def double(self, clip: vs.VideoNode) -> vs.VideoNode:
         y = depth(get_y(clip), 16)
 
         overshoot = self.kwargs.pop("overshoot", self.ratio / 100)
```

### Comparing `vodesfunc-1.5.0/vodesfunc.egg-info/PKG-INFO` & `vodesfunc-1.6.0/vodesfunc.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vodesfunc
-Version: 1.5.0
+Version: 1.6.0
 Summary: Vodes' random Vapoursynth Functions.
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vodesfunc
 Project-URL: Contact, https://discord.gg/Kf94Nv6WVN
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -19,20 +19,22 @@
 License-File: LICENSE
 Requires-Dist: Vapoursynth>=61
 Requires-Dist: vsscale>=1.0.1
 Requires-Dist: vsrgtools>=1.3.0
 Requires-Dist: vskernels>=1.2.0
 Requires-Dist: vstools>=1.6.2
 Requires-Dist: vsmasktools>=1.1.0
+Requires-Dist: vsmuxtools>=0.1.0
 
 # vodesfunc
 
-Contains various functions for automation and other stuff I use in my scripts
+Contains various functions for automation and other stuff I use in my scripts.
 
-### This is by no means me trying to be professional and as such, the code will not be treated like it.
-<br>
+Auto generated docs are at https://muxtools.vodes.pw.
+
+#### This is by no means me trying to be professional and as such, the code will not be treated like it.
 
 ## Installation
 
 `pip install vodesfunc` <br>for ~~mostly~~ stable versions
 
 `pip install git+https://github.com/Vodes/vodesfunc.git` <br>for absolutely latest
```

