# Comparing `tmp/keras-vision-0.4.tar.gz` & `tmp/keras-vision-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-vision-0.4.tar", last modified: Fri May  3 19:10:00 2024, max compression
+gzip compressed data, was "keras-vision-0.4.1.tar", last modified: Sun May  5 18:31:55 2024, max compression
```

## Comparing `keras-vision-0.4.tar` & `keras-vision-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.813512 keras-vision-0.4/
--rw-rw-rw-   0        0        0     1142 2024-05-03 19:10:00.811506 keras-vision-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.794632 keras-vision-0.4/keras_vision/
-drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.810491 keras-vision-0.4/keras_vision/MobileViT_v1/
--rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4/keras_vision/MobileViT_v1/__init__.py
--rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4/keras_vision/MobileViT_v1/base_layers.py
--rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4/keras_vision/MobileViT_v1/configs.py
--rw-rw-rw-   0        0        0     6761 2024-05-03 18:40:51.000000 keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1.py
--rw-rw-rw-   0        0        0    16065 2024-05-03 18:38:33.000000 keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
--rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
--rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4/keras_vision/MobileViT_v1/utils.py
--rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4/keras_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 19:10:00.801633 keras-vision-0.4/keras_vision.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-03 19:10:00.000000 keras-vision-0.4/keras_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 19:10:00.813512 keras-vision-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1823 2024-05-03 19:09:15.000000 keras-vision-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.745030 keras-vision-0.4.1/
+-rw-rw-rw-   0        0        0     1389 2024-05-05 18:31:55.743518 keras-vision-0.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.727505 keras-vision-0.4.1/keras_vision/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.742520 keras-vision-0.4.1/keras_vision/MobileViT_v1/
+-rw-rw-rw-   0        0        0      501 2024-05-03 18:35:52.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/__init__.py
+-rw-rw-rw-   0        0        0     4516 2024-05-03 18:38:00.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/base_layers.py
+-rw-rw-rw-   0        0        0     2428 2024-05-03 18:38:07.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/configs.py
+-rw-rw-rw-   0        0        0     8176 2024-05-05 18:29:05.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1.py
+-rw-rw-rw-   0        0        0    13452 2024-05-05 15:29:51.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1_block.py
+-rw-rw-rw-   0        0        0     2529 2024-05-03 18:37:13.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/multihead_self_attention_2D.py
+-rw-rw-rw-   0        0        0      523 2024-04-17 10:55:18.000000 keras-vision-0.4.1/keras_vision/MobileViT_v1/utils.py
+-rw-rw-rw-   0        0        0       39 2024-04-17 11:28:04.000000 keras-vision-0.4.1/keras_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:31:55.734528 keras-vision-0.4.1/keras_vision.egg-info/
+-rw-rw-rw-   0        0        0     1389 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 18:31:55.000000 keras-vision-0.4.1/keras_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:31:55.746038 keras-vision-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-05 18:30:00.000000 keras-vision-0.4.1/setup.py
```

### Comparing `keras-vision-0.4/PKG-INFO` & `keras-vision-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4
+Version: 0.4.1
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,13 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras
 
 Porting all models from everywhere to Keras for leveraging multi-backend support.
 
 Cause why not?🤷🏻‍♂️
+
+### Updates
+
+1. [2024-05-04] Converted MobileViT to Keras 3 and released weights of all 3 variants.
+   1. Jax backend currently not working, I'm working on a fix.
+   2. Release: <https://github.com/veb-101/keras-vision/releases/tag/v0.4>
```

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/base_layers.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/base_layers.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/configs.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/configs.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+import warnings
 from typing import Optional
 
+
 import keras.ops as kops
 from keras import Model, Input
 from keras.layers import GlobalAveragePooling2D, Dropout, Dense
+from keras.utils import get_file
 
 from .configs import get_mobile_vit_v1_configs
 from .base_layers import ConvLayer, InvertedResidualBlock
 from .mobile_vit_v1_block import MobileViT_v1_Block
 
+VERSION = 0.4
+WEIGHTS_URL = "https://github.com/veb-101/keras-vision/releases/download/{version}/keras_MobileVIT_v1_model_{model_type}.weights.h5"
+
 
 def MobileViT_v1(
     configs,
     dropout: float = 0.1,
     linear_drop: float = 0.0,
     attention_drop: float = 0.0,
-    num_classes: int = 1000,
+    num_classes: int | None = 1000,
     input_shape: tuple[int, int, int] = (256, 256, 3),
     model_name: str = f"MobileViT_v1-S",
 ):
     """
     Arguments
     --------
 
@@ -132,67 +138,89 @@
         transformer_repeats=configs.tf_block_5_repeats,
         name="MobileViTBlock-3",
         dropout=dropout,
         attention_drop=attention_drop,
         linear_drop=linear_drop,
     )(out)
 
-    out = ConvLayer(num_filters=configs.final_conv_dims, kernel_size=1, strides=1)(out)
+    out = ConvLayer(num_filters=configs.final_conv_dims, kernel_size=1, strides=1, name="final_conv")(out)
 
-    # Output layer
-    out = GlobalAveragePooling2D()(out)
+    if num_classes:
+        # Output layer
+        out = GlobalAveragePooling2D()(out)
 
-    if linear_drop > 0.0:
-        out = Dropout(rate=dropout)(out)
+        if linear_drop > 0.0:
+            out = Dropout(rate=dropout)(out)
 
-    out = Dense(units=num_classes)(out)
+        out = Dense(units=num_classes)(out)
 
     model = Model(inputs=input_layer, outputs=out, name=model_name)
 
     return model
 
 
 def build_MobileViT_v1(
     model_type: str = "S",
     num_classes: int = 1000,
     input_shape: tuple = (256, 256, 3),
+    include_top: bool = True,  # Whether to include the classification layer in the model
+    pretrained: bool = False,  # Whether to load pretrained weights
+    cache_dir: Optional[str] = None,  # Local cache directory for weights
     updates: Optional[dict] = None,
     **kwargs,
 ):
     """
-    Create MobileViT-v1 Classification models
+    Create MobileViT-v1 Classification models or feature extractors with optional pretrained weights.
 
-    Arguments
-    --------
-        model_type: (str)   MobileViT version to create. Options: S, XS, XSS
+    Arguments:
+    ---------
+        model_type: (str)   MobileViT version to create. Options: S, XS, XXS
         num_classes: (int)   Number of output classes
         input_shape: (tuple) Input shape -> H, W, C
+        include_top: (bool) Whether to include the classification layers
+        pretrained: (bool) Whether to load pretrained weights
+        cache_dir: (str) Local directory to cache the downloaded weights
         updates: (dict) a key-value pair indicating the changes to be made to the base model.
 
     Additional arguments:
     ---------------------
         linear_drop: (float) Dropout rate for Dense layers
         attention_drop: (float) Dropout rate for the attention matrix
-
     """
     model_type = model_type.upper()
-
     if model_type not in ("S", "XS", "XXS"):
-        raise ValueError("Bad Input. 'model_type' should one of ['S', 'XS', 'XXS']")
+        raise ValueError("Bad Input. 'model_type' should be one of ['S', 'XS', 'XXS']")
 
     updated_configs = get_mobile_vit_v1_configs(model_type, updates=updates)
 
+    # Build the base model
     model = MobileViT_v1(
         configs=updated_configs,
-        num_classes=num_classes,
+        num_classes=num_classes if include_top else None,
         input_shape=input_shape,
         model_name=f"MobileViT_v1-{model_type}",
         **kwargs,
     )
-    # model.summary()
+
+    if pretrained:
+
+        weights_path = get_file(
+            fname=f"keras_MobileVIT_v1_model_{model_type}.weights.h5",
+            origin=WEIGHTS_URL.format(version=VERSION, model_type=model_type),
+            cache_subdir="models",
+            hash_algorithm="auto",
+            extract=False,
+            archive_format="auto",
+            cache_dir=cache_dir,
+        )
+
+        with warnings.catch_warnings():
+            # Ignore UserWarnings within this block
+            warnings.simplefilter("ignore", UserWarning)
+            model.load_weights(weights_path, skip_mismatch=True)
 
     return model
 
 
 if __name__ == "__main__":
     model = build_MobileViT_v1(
         model_type="S",  # "XS", "XXS"
```

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/mobile_vit_v1_block.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/mobile_vit_v1_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -116,77 +116,14 @@
 
 #     # [B, N, P, D] --> [B, P, N, D]
 #     transposed_fm = kops.transpose(reshaped_fm, axes=[0, 2, 1, 3])
 
 #     return transposed_fm
 
 
-# def unfolding(feature_map, patch_w, patch_h):
-#     # Initially convert channel-last to channel-first for processing
-#     feature_map = kops.transpose(feature_map, [0, 3, 1, 2])  # [B, H, W, C] -> [B, C, H, W]
-
-#     patch_area = patch_w * patch_h
-
-#     # batch_size, in_channels, orig_h, orig_w = feature_map.shape
-#     shape = kops.shape(feature_map)
-#     batch_size, in_channels, orig_h, orig_w = shape[0], shape[1], shape[2], shape[3]
-
-#     orig_h, orig_w = kops.cast(orig_h, dtype="int32"), kops.cast(orig_w, dtype="int32")
-
-#     a = kops.ceil(orig_h / patch_h)
-#     b = kops.ceil(orig_w / patch_w)
-
-#     new_h = kops.cast(a * kops.cast(patch_h, dtype=a.dtype), dtype="int32")
-#     new_w = kops.cast(b * kops.cast(patch_w, dtype=a.dtype), dtype="int32")
-
-#     def resize_image():
-#         feature_map = kops.image.resize(feature_map.transpose(0, 2, 3, 1), [new_h, new_w], data_format="channels_last")
-#         return feature_map.transpose(0, 3, 1, 2)
-
-#     def return_original():
-#         return feature_map
-
-#     # feature_map = kops.image.resize(feature_map, [new_h, new_w], data_format="channels_first")
-
-#     # Condition to decide if resizing is necessary
-#     feature_map = kops.cond(
-#         kops.logical_or(kops.not_equal(new_w, orig_w), kops.not_equal(new_h, orig_h)),
-#         true_fn=resize_image,
-#         false_fn=return_original,
-#     )
-
-#     num_patch_w = new_w // patch_w
-#     num_patch_h = new_h // patch_h
-#     num_patches = num_patch_h * num_patch_w
-
-#     # Handle dynamic shape multiplication
-#     dynamic_shape_mul = kops.prod([batch_size, in_channels * num_patch_h])
-
-#     # Reshape and transpose to create patches
-#     reshaped_fm = kops.reshape(feature_map, [dynamic_shape_mul, patch_h, num_patch_w, patch_w])
-#     print("hereeee")
-#     transposed_fm = kops.transpose(reshaped_fm, [0, 2, 1, 3])
-#     reshaped_fm = kops.reshape(transposed_fm, [batch_size, in_channels, num_patches, patch_area])
-#     transposed_fm = kops.transpose(reshaped_fm, [0, 3, 2, 1])
-#     patches = kops.reshape(transposed_fm, [batch_size * patch_area, num_patches, in_channels])
-
-#     info_dict = {
-#         "orig_size": (orig_h, orig_w),
-#         "batch_size": batch_size,
-#         "interpolate": kops.logical_or(kops.not_equal(new_w, orig_w), kops.not_equal(new_h, orig_h)),
-#         # "interpolat": True,
-#         "total_patches": num_patches,
-#         "num_patches_w": num_patch_w,
-#         "num_patches_h": num_patch_h,
-#         "patch_area": patch_area,
-#     }
-
-#     return patches, info_dict
-
-
 class MobileViT_v1_Block(Layer):
     def __init__(
         self,
         out_filters: int = 64,
         embedding_dim: int = 90,
         patch_size: Union[int, tuple] = 2,
         transformer_repeats: int = 2,
```

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/multihead_self_attention_2D.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/multihead_self_attention_2D.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4/keras_vision/MobileViT_v1/utils.py` & `keras-vision-0.4.1/keras_vision/MobileViT_v1/utils.py`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4/keras_vision.egg-info/PKG-INFO` & `keras-vision-0.4.1/keras_vision.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-vision
-Version: 0.4
+Version: 0.4.1
 Summary: Building Vision models in Keras3 for framework agnostic training and inference.
 Home-page: https://github.com/veb-101/keras-vision
 Author: Vaibhav Singh
 Author-email: vaibhav.singh.3001@gmail.com
 License: Apache 2.0
 Keywords: keras3 tensorflow Jax PyTorch Vision
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,13 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras
 
 Porting all models from everywhere to Keras for leveraging multi-backend support.
 
 Cause why not?🤷🏻‍♂️
+
+### Updates
+
+1. [2024-05-04] Converted MobileViT to Keras 3 and released weights of all 3 variants.
+   1. Jax backend currently not working, I'm working on a fix.
+   2. Release: <https://github.com/veb-101/keras-vision/releases/tag/v0.4>
```

### Comparing `keras-vision-0.4/keras_vision.egg-info/SOURCES.txt` & `keras-vision-0.4.1/keras_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-vision-0.4/setup.py` & `keras-vision-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
-__version__ = "0.4"
+__version__ = "0.4.1"
 DESCRIPTION = "Building Vision models in Keras3 for framework agnostic training and inference."
 
 # Setting up
 setup(
     name="keras-vision",
     version=__version__,
     author="Vaibhav Singh",
```

