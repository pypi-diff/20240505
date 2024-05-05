# Comparing `tmp/aec6s-1.0.0.tar.gz` & `tmp/aec6s-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aec6s-1.0.0.tar", last modified: Sun Apr 21 20:58:08 2024, max compression
+gzip compressed data, was "aec6s-1.0.1.tar", last modified: Sun May  5 20:25:31 2024, max compression
```

## Comparing `aec6s-1.0.0.tar` & `aec6s-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-21 20:58:08.038716 aec6s-1.0.0/
--rw-r--r--   0 yw         (501) staff       (20)    35129 2024-04-20 17:56:35.000000 aec6s-1.0.0/LICENSE
--rw-r--r--   0 yw         (501) staff       (20)     1020 2024-04-21 20:58:08.038512 aec6s-1.0.0/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)      595 2024-04-21 16:13:56.000000 aec6s-1.0.0/README.md
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-21 20:58:08.037391 aec6s-1.0.0/aec6s/
--rw-r--r--   0 yw         (501) staff       (20)     1514 2024-04-21 20:52:40.000000 aec6s-1.0.0/aec6s/AEC.py
--rw-r--r--   0 yw         (501) staff       (20)       26 2024-04-20 19:44:10.000000 aec6s-1.0.0/aec6s/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     1830 2024-04-20 20:56:46.000000 aec6s-1.0.0/aec6s/anci_download.py
--rw-r--r--   0 yw         (501) staff       (20)     3596 2024-04-21 16:00:05.000000 aec6s-1.0.0/aec6s/anci_get_AER.py
--rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 aec6s-1.0.0/aec6s/anci_get_OWV.py
--rw-r--r--   0 yw         (501) staff       (20)     1660 2024-04-20 20:51:25.000000 aec6s-1.0.0/aec6s/anci_list_files.py
--rw-r--r--   0 yw         (501) staff       (20)      338 2024-04-21 20:52:35.000000 aec6s-1.0.0/aec6s/fillnan.py
--rw-r--r--   0 yw         (501) staff       (20)     1722 2024-04-20 20:56:46.000000 aec6s-1.0.0/aec6s/get_ancillary.py
--rw-r--r--   0 yw         (501) staff       (20)     4375 2024-04-21 20:54:14.000000 aec6s-1.0.0/aec6s/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)    11081 2024-04-21 20:53:29.000000 aec6s-1.0.0/aec6s/read_metadata.py
--rw-r--r--   0 yw         (501) staff       (20)     2460 2024-04-21 20:52:31.000000 aec6s-1.0.0/aec6s/run.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-21 20:58:08.037950 aec6s-1.0.0/aec6s.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     1020 2024-04-21 20:58:07.000000 aec6s-1.0.0/aec6s.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)      429 2024-04-21 20:58:08.000000 aec6s-1.0.0/aec6s.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2024-04-21 20:58:07.000000 aec6s-1.0.0/aec6s.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       36 2024-04-21 20:58:07.000000 aec6s-1.0.0/aec6s.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2024-04-21 20:58:07.000000 aec6s-1.0.0/aec6s.egg-info/top_level.txt
--rw-r--r--   0 yw         (501) staff       (20)       38 2024-04-21 20:58:08.038757 aec6s-1.0.0/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)      668 2024-04-21 20:56:41.000000 aec6s-1.0.0/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-04-21 20:58:08.038173 aec6s-1.0.0/tests/
--rw-r--r--   0 yw         (501) staff       (20)      414 2024-04-21 20:51:48.000000 aec6s-1.0.0/tests/test.py
--rw-r--r--   0 yw         (501) staff       (20)     1259 2024-04-21 20:48:14.000000 aec6s-1.0.0/tests/test_private.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-05 20:25:31.683319 aec6s-1.0.1/
+-rw-r--r--   0 yw         (501) staff       (20)    35129 2024-04-20 17:56:35.000000 aec6s-1.0.1/LICENSE
+-rw-r--r--   0 yw         (501) staff       (20)     2264 2024-05-05 20:25:31.683075 aec6s-1.0.1/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     1840 2024-05-05 20:22:32.000000 aec6s-1.0.1/README.md
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-05 20:25:31.681640 aec6s-1.0.1/aec6s/
+-rw-r--r--   0 yw         (501) staff       (20)     1578 2024-04-23 01:46:40.000000 aec6s-1.0.1/aec6s/AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)       26 2024-04-20 19:44:10.000000 aec6s-1.0.1/aec6s/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     1830 2024-04-20 20:56:46.000000 aec6s-1.0.1/aec6s/anci_download.py
+-rw-r--r--   0 yw         (501) staff       (20)     3596 2024-04-21 16:00:05.000000 aec6s-1.0.1/aec6s/anci_get_AER.py
+-rw-r--r--   0 yw         (501) staff       (20)     2383 2024-03-10 16:16:52.000000 aec6s-1.0.1/aec6s/anci_get_OWV.py
+-rw-r--r--   0 yw         (501) staff       (20)     1660 2024-04-20 20:51:25.000000 aec6s-1.0.1/aec6s/anci_list_files.py
+-rw-r--r--   0 yw         (501) staff       (20)      338 2024-04-21 20:52:35.000000 aec6s-1.0.1/aec6s/fillnan.py
+-rw-r--r--   0 yw         (501) staff       (20)     1722 2024-04-20 20:56:46.000000 aec6s-1.0.1/aec6s/get_ancillary.py
+-rw-r--r--   0 yw         (501) staff       (20)     4912 2024-05-05 20:07:16.000000 aec6s-1.0.1/aec6s/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)    11171 2024-05-05 20:21:03.000000 aec6s-1.0.1/aec6s/read_metadata.py
+-rw-r--r--   0 yw         (501) staff       (20)     2460 2024-05-05 20:25:06.000000 aec6s-1.0.1/aec6s/run.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-05 20:25:31.682312 aec6s-1.0.1/aec6s.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     2264 2024-05-05 20:25:31.000000 aec6s-1.0.1/aec6s.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)      429 2024-05-05 20:25:31.000000 aec6s-1.0.1/aec6s.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2024-05-05 20:25:31.000000 aec6s-1.0.1/aec6s.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       36 2024-05-05 20:25:31.000000 aec6s-1.0.1/aec6s.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2024-05-05 20:25:31.000000 aec6s-1.0.1/aec6s.egg-info/top_level.txt
+-rw-r--r--   0 yw         (501) staff       (20)       38 2024-05-05 20:25:31.683422 aec6s-1.0.1/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)      668 2024-05-05 20:23:57.000000 aec6s-1.0.1/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2024-05-05 20:25:31.682707 aec6s-1.0.1/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      565 2024-04-21 21:01:28.000000 aec6s-1.0.1/tests/test.py
+-rw-r--r--   0 yw         (501) staff       (20)     1376 2024-05-05 20:16:19.000000 aec6s-1.0.1/tests/test_private.py
```

### Comparing `aec6s-1.0.0/LICENSE` & `aec6s-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/AEC.py` & `aec6s-1.0.1/aec6s/AEC.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,13 +37,16 @@
         start_time = time.time()
         print("\nConvolution started ")
         image_conv = scipy.signal.convolve2d(image, PSF, mode='same', boundary='fill', fillvalue=image.mean())
         print("Convolution completed: %s seconds " % (time.time() - start_time))
         
         output = image + dif2dir * (image - image_conv)
         
+        # add nan back
+        output[is_nan] = np.nan
+        
         # Modify L2R NC file 
         dset[ACOLITE_band][:] = output
         
     # Close file 
     dset.close()
```

### Comparing `aec6s-1.0.0/aec6s/anci_download.py` & `aec6s-1.0.1/aec6s/anci_download.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/anci_get_AER.py` & `aec6s-1.0.1/aec6s/anci_get_AER.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/anci_get_OWV.py` & `aec6s-1.0.1/aec6s/anci_get_OWV.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/anci_list_files.py` & `aec6s-1.0.1/aec6s/anci_list_files.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/get_ancillary.py` & `aec6s-1.0.1/aec6s/get_ancillary.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/aec6s/get_parameters.py` & `aec6s-1.0.1/aec6s/get_parameters.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,19 +55,35 @@
 
     # Calculate the distance from the center for each pixel
     distances = np.sqrt((xx - center)**2 + (yy - center)**2) * pixel_size
     clipped_distances = np.clip(distances, np.min(r_values), np.max(r_values)) # make sure no extrapolation 
 
     # Apply interpolation to distances to get weights for each pixel
     interpolated_weights = interpolator(clipped_distances)
-
-    # Normalize to 1
-    PSF = interpolated_weights / np.sum(interpolated_weights)
     
-    AEC_parameters = {'PSF':PSF,
+    ### Normalize to 1
+    PSF = interpolated_weights.copy()
+    
+    # Find the central pixel coordinates
+    center_row = PSF.shape[0] // 2
+    center_col = PSF.shape[1] // 2
+    
+    # Store the value of the central pixel
+    center_value = PSF[center_row, center_col]
+    
+    # Calculate the sum of all elements in the array and subtract the central pixel value
+    adjusted_sum = PSF.sum() - center_value
+    
+    # Normalize the array
+    normalized_array = PSF / adjusted_sum * (1-center_value)
+    
+    # Add back the central pixel value
+    normalized_array[center_row, center_col] = center_value
+
+    AEC_parameters = {'PSF':normalized_array,
                       'dif2dir':dif2dir}
 
     return AEC_parameters
 
 # Define the function F_r(r)
 def F_r(radius, t_Rayleigh, t_Aerosol):
     import numpy as np
```

### Comparing `aec6s-1.0.0/aec6s/read_metadata.py` & `aec6s-1.0.1/aec6s/read_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     elif sensor == 'L9_OLI':
         
         # source: https://landsat.gsfc.nasa.gov/satellites/landsat-9/landsat-9-instruments/oli-2-design/oli-2-relative-spectral-response/
         metadata['AEC_bands_6S'] = _L9_RSR()
         metadata['AEC_bands_wl'] = [442.81, 481.89, 560.95, 654.32, 864.64, 1608.15, 2200.12]
         
         # Add ACOLITE_bands!!! 
+        sys.exit('Missing L9 OLI bands for ACOLITE, contact Yulun at yulunwu8@gmail.com')
         
     else:
         sys.exit('Unknown sensor.')
         
     metadata['ACOLITE_bands'] =  [f'rhos_{band}' for band in ACOLITE_bands]
         
     return metadata
```

### Comparing `aec6s-1.0.0/aec6s/run.py` & `aec6s-1.0.1/aec6s/run.py`

 * *Files identical despite different names*

### Comparing `aec6s-1.0.0/setup.py` & `aec6s-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='aec6s',
-    version='1.0.0',
+    version='1.0.1',
     author='Yulun Wu',
     author_email='yulunwu8@gmail.com',
     description='Adjacency-effect correction following the Vermote et al. 1997 approach',
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `aec6s-1.0.0/tests/test_private.py` & `aec6s-1.0.1/tests/test_private.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,27 @@
 import aec6s
 
 
 
 
 # S2
 file = '/Users/yw/Local_storage/GLORIA/240420 Vermote approach/S2A_MSI_2015_09_12_10_17_24_T32TPR_L2R_copy.nc'
+file = '/Users/yw/Local_storage/GLORIA/240420 Vermote approach/S2B_MSI_2021_01_19_00_07_00_T55HFV_L2R_copy.nc'
+
+
+
+
 
 # test no data 
 
 # file = '/Users/yw/Local_storage/temp_OSD_test/ACed/20230928/S2B_MSI_2023_09_28_15_44_58_T17MNP_L2R.nc'
 
 
 # L8
-file = '/Users/yw/Local_storage/GLORIA/240420 Vermote approach/L8_OLI_2018_07_03_15_25_47_012030_L2R_copy.nc'
+# file = '/Users/yw/Local_storage/GLORIA/240420 Vermote approach/L8_OLI_2018_07_03_15_25_47_012030_L2R_copy.nc'
 
 
 
 
 anci_folder = '/Users/yw/Local_storage/GLORIA/240420 Vermote approach/anci' 
 
 username = 'Isa1990'
```

