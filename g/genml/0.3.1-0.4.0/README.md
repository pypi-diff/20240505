# Comparing `tmp/genml-0.3.1.tar.gz` & `tmp/genml-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\genml-0.3.1.tar", last modified: Tue Mar 12 03:02:21 2024, max compression
+gzip compressed data, was "dist\genml-0.4.0.tar", last modified: Sun May  5 15:49:35 2024, max compression
```

## Comparing `genml-0.3.1.tar` & `genml-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 03:02:21.000000 genml-0.3.1/
--rw-rw-rw-   0        0        0     2958 2024-03-12 03:02:21.000000 genml-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2024-03-11 17:06:57.000000 genml-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 03:02:21.000000 genml-0.3.1/genml/
--rw-rw-rw-   0        0        0      513 2024-03-10 20:44:58.000000 genml-0.3.1/genml/__init__.py
--rw-rw-rw-   0        0        0     9157 2024-03-12 02:59:57.000000 genml-0.3.1/genml/genml.py
--rw-rw-rw-   0        0        0    11485 2024-03-10 20:44:58.000000 genml-0.3.1/genml/mittag_leffler.py
-drwxrwxrwx   0        0        0        0 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/
--rw-rw-rw-   0        0        0     2958 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-12 03:02:21.000000 genml-0.3.1/genml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-12 03:02:21.000000 genml-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      563 2024-03-12 03:02:13.000000 genml-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:49:34.000000 genml-0.4.0/
+-rw-rw-rw-   0        0        0     1507 2024-05-05 15:34:35.000000 genml-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     2559 2024-05-05 15:49:34.000000 genml-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2281 2024-05-05 15:34:35.000000 genml-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:49:34.000000 genml-0.4.0/genml/
+-rw-rw-rw-   0        0        0      513 2024-05-05 15:34:38.000000 genml-0.4.0/genml/__init__.py
+-rw-rw-rw-   0        0        0     9892 2024-05-05 15:34:38.000000 genml-0.4.0/genml/genml.py
+-rw-rw-rw-   0        0        0    11485 2024-05-05 15:34:38.000000 genml-0.4.0/genml/mittag_leffler.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/
+-rw-rw-rw-   0        0        0     2559 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-05 15:49:34.000000 genml-0.4.0/genml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:49:34.000000 genml-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      597 2024-05-05 15:34:35.000000 genml-0.4.0/setup.py
```

### Comparing `genml-0.3.1/README.md` & `genml-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 *School of Physics and Electronics, Hunan University, Changsha 410082, China*
 
 E-mail: huangzih@hnu.edu.cn
 
 GenML is a Python library designed for generating Mittag-Leffler correlated noise, which is crucial for modeling a wide range of phenomena in complex systems. This document provides a brief overview of how to install and use GenML to generate M-L noise and compute its autocorrelation functions.
 
+##### Documentation website: [https://genml.readthedocs.io](https://genml.readthedocs.io)
+
 ## Installation
 
 To install GenML, simply run the following command in your Python environment:
 
 ```bash
 pip install -U genml
 ```
@@ -29,27 +31,28 @@
 
 # Parameters
 N = 10  # Number of sequences
 T = 500  # Length of each sequence
 C = 1.0  # Amplitude coefficient
 lamda = 0.5  # Mittag-Leffler exponent
 tau = 10  # Characteristic memory time
-nc = 4  # Number of CPU cores for parallel processing
+seed = 42 # Random seed
 
 # Generate M-L noise sequences
-xi = genml.mln(N, T, C, lamda, tau, nc)
+xi = genml.mln(N, T, C, lamda, tau, seed)
 ```
 
 ### Calculating Autocorrelation Function
 
 To calculate the autocorrelation function (ACF) values of the generated noise sequences, you can use the `acf` function for actual ACF values and the `acft` function for theoretical ACF values:
 
 ```python
 tmax = 100  # Max lag for ACF calculation
 dt = 1  # Step size between lags
+nc = 4  # Number of CPU cores for parallel processing
 
 # Calculate actual ACF values
 acfv = genml.acf(xi, tmax, dt, nc)
 
 # Calculate theoretical ACF values
 acftv = genml.acft(tmax, dt, C, lamda, tau)
 ```
```

### Comparing `genml-0.3.1/genml/__init__.py` & `genml-0.4.0/genml/__init__.py`

 * *Files identical despite different names*

### Comparing `genml-0.3.1/genml/genml.py` & `genml-0.4.0/genml/genml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,83 +1,105 @@
-import numpy as np
+import sys
+import time
 import warnings
-import random
+import numpy as np
+import multiprocessing as mp
 from tqdm import tqdm
 from .mittag_leffler import ml
-import multiprocessing
-from multiprocessing import Pool, current_process
+from multiprocess import Pool as Pool1
+from multiprocessing import Pool as Pool2
 
 
 class MLN(object):
     """
-    Implements the generation of Mittag-Leffler correlated noise.
+    Implement the generation of Mittag-Leffler correlated noise.
 
     This class is dedicated to producing sequences of Mittag-Leffler correlated noise, characterized by its unique
-    autocorrelation properties. It is initialized with parameters: T (the sequence length), C (the amplitude coefficient),
-    lamda (the Mittag-Leffler exponent), and tau (the characteristic memory time).
+    autocorrelation properties. It is initialized with parameters: N (number of noise sequences), T (the sequence length), 
+    C (the amplitude coefficient), lamda (the Mittag-Leffler exponent), tau (the characteristic memory time) and seed (random seed).
     """
-    def __init__(self, T, C, lamda, tau, A=None):
+    
+    A = None
+    params = None
+   
+    def __init__(self, N, T, C, lamda, tau, seed=None):
         """
-        Initializes the MLN class.
+        Initialize the MLN class.
 
         Parameters:
-        - T: Total length of the noise trajectory (int).
+        - N: Number of noise sequences to generate (int).
+        - T: Total length of single noise sequence (int).
         - C: Amplitude coefficient (float).
         - lamda: Mittag-Leffler exponent (0 < lamda < 2).
         - tau: Characteristic memory time (0 < tau <= 10000).
+        - seed: Random seed (default: None).
         """
         if not isinstance(T, int) or T <= 0:
             raise TypeError("Length of noise must be a positive int.")
         if lamda <= 0 or lamda >= 2:
             raise ValueError("Lamda parameter must be in interval (0, 2).")
         if tau > 10000 or tau <= 0:
             raise ValueError("Tau parameter must be in interval (0, 10000].")
+        self.N = N
         self.T = T
         self.Topt = T
         self.C = C
         self.lamda = lamda
         self.tau = tau
-        self.A = A
+        self.seed = seed
         self.acvs = []
-
+        
 
     def _mln(self):
         """
         Sample the Mittag-Leffler correlated noise.
 
-        Returns an array of noise sequence.
+        Return an array of noise sequences.
         """
-        Z = np.random.normal(0.0, 1.0, 2 * self.T)
+        np.random.seed(self.seed)
+        Z = np.random.normal(0.0, 1.0, (self.N, 2 * self.T))
         return self.syn_mln(Z)
 
 
     def cal_acft(self, lag):
         """
         Calculate the theoretical autocorrelation function for Mittag-Leffler correlated noise.
 
         Parameters:
         - lag (int or array): The time lag(s).
 
-        Returns:
+        Return:
         - The calculated autocorrelation function value(s) at the specified lag(s).
         """
         lag = -(abs(lag) / self.tau) ** self.lamda
         return self.C * ml(lag, alpha=self.lamda) / (self.tau ** self.lamda)
 
 
+    def update_A(self):
+        '''
+        Update the matrix of non-negative eigenvalues based on current parameters or availability.
+
+        Check if MLN.A is unavailable or parameters have changed. If conditions are met, trigger the 
+        generation of a new MLN.A using 'gen_A'.
+        '''
+        if MLN.A is None or MLN.params != (self.T, self.C, self.lamda, self.tau):
+            MLN.A = self.gen_A()
+            MLN.params = (self.T, self.C, self.lamda, self.tau)            
+
+    
     def gen_A(self):
         """
-        Computes the eigenvalues of a circulant matrix with optimal length, ensuring non-negativity.
+        Compute the eigenvalues of a circulant matrix with optimal length, ensuring non-negativity.
 
         This function identifies the optimal sequence length and computes the eigenvalues of the associated circulant matrix
         derived from the autocorrelation function. The process ensures the non-negativity condition. 
         
         The 'ls' list serves as a sorted waiting list of potential sequence lengths.
 
-        Returns:
+        Return:
         - An array of non-negative eigenvalues corresponding to the optimal length circulant matrix.
         """
         ls0 = [int(25 * i) for i in range(4, 40)]
         ls = list(range(1, 10)) + [int(2.5 * i) for i in range(4, 40)] + ls0 + list(np.array(ls0) * 10)\
             + list(np.array(ls0) * 100) + list(np.array(ls0) * 1000) + list(np.array(ls0) * 10000) + list(np.array(ls0) * 100000)\
             + list(np.array(ls0) * 1000000) + list(np.array(ls0) * 10000000) + list(np.array(ls0) * 100000000) + list(np.array(ls0) * 1000000000)
         self.acvs = self.cal_acft(np.array(range(self.T))).tolist()
@@ -99,144 +121,137 @@
             return None
         else:
             return A0
 
 
     def syn_mln(self, Z):
         """
-        Synthesizes Mittag-Leffler correlated noise leveraging Fourier techniques.
+        Synthesize Mittag-Leffler correlated noise leveraging Fourier techniques.
 
         This function transforms a sequence of normal random variables into Mittag-Leffler correlated noise, based on Fourier techniques.
 
         Parameters:
-        - Z (array): A sequence of normal random variables.
+        - Z (array): Sequences of normal random variables.
 
-        Returns:
+        Return:
         - An array representing the synthesized Mittag-Leffler correlated noise.
         """
-        A = self.gen_A()
-        Z = np.random.normal(0.0, 1.0, 2 * self.T)
-        Y = np.zeros(2 * self.T, dtype=complex)
-        for i in range(2 * self.T):
-            A_sqrt = np.sqrt(A[i] * self.T)
-            if i == 0:
-                Y[i] = A_sqrt * np.sqrt(2) * Z[i]
-            elif i < self.T:
-                Y[i] = A_sqrt * (Z[2 * i - 1] + 1j * Z[2 * i])
-            elif i == self.T:
-                Y[i] = A_sqrt * np.sqrt(2) * Z[2 * self.T - 1]
-            else:
-                Y[i] = Y[2 * self.T - i].conjugate()
-        # Fourier transform of the combined noise sequence
+        A = MLN.A
+        Y = np.zeros((self.N, 2 * self.T), dtype=complex)
+        A_sqrt = np.sqrt(A * self.T)
+        Y[:, 0] = A_sqrt[0] * np.sqrt(2) * Z[:, 0]
+        Y[:, 1:self.T] = A_sqrt[1:self.T] * (Z[:, 1:2*self.T-1:2] + 1j * Z[:, 2:2*self.T:2])
+        Y[:, self.T] = A_sqrt[self.T] * np.sqrt(2) * Z[:, 2 * self.T - 1]
+        Y[:, self.T+1:] = Y[:, self.T-1:0:-1].conjugate()
         X = np.fft.ifft(Y)
-        return X[:self.T].real
-
+        return X[:, :self.T].real
 
 
 def cal_mln(args):
     """
-    Instantiate the MLN class to generate a single noise sequence.
+    Instantiate the MLN class to generate noise sequences.
     """
-    T, C, lamda, tau, A = args
-    return MLN(T, C, lamda, tau, A)._mln()
+    N, T, C, lamda, tau, seed = args
+    return MLN(N, T, C, lamda, tau, seed)._mln()
 
 
 def cal_acf(args):
     """
-    Computes the actual autocorrelation function of Mittag-Leffler correlated noise at a specific lag.
+    Compute the actual autocorrelation function of Mittag-Leffler correlated noise at a specific lag.
     """
     xi, T, i = args
     if i == 0:
         corr = np.sum(xi[:, :] * xi[:, :], axis=1) / T
     else:
         corr = np.sum(xi[:, :-i] * xi[:, i:], axis=1) / (T - i)
     return corr.mean()
 
 
-
-
-def mln(N, T, C, lamda, tau, nc=1):
+def mln(N, T, C, lamda, tau, seed=None):
     """
-    Generates N Mittag-Leffler correlated noise sequences of length T in parallel.
+    Generate N Mittag-Leffler correlated noise sequences of length T.
     Adjusts noise length to match the target length if required.
 
     Parameters:
-    - N: Number of trajectories to generate (int).
-    - T: Total length of the noise trajectory (int).
+    - N: Number of noise sequences to generate (int).
+    - T: Total length of single noise sequence (int).
     - C: Amplitude coefficient (float).
     - lamda: Mittag-Leffler exponent (0 < lamda < 2).
     - tau: Characteristic memory time (0 < tau <= 10000).
-    - nc: Number of parallel cores (int).
+    - seed: Random seed (default: None).
 
-    Returns:
-    A 2D array of size (N, T) containing the generated Mittag-Leffler correlated noise trajectories.
+    Return:
+    A 2D array of size (N, T) containing the generated Mittag-Leffler correlated noise sequences.
     """
     if not isinstance(N, int) or N <= 0:
-        raise TypeError("Number of trajectories must be a positive int.")
-    if current_process().name == 'MainProcess':
-        pbar = tqdm(total=N, desc='Generating M-L noise', position=0)
+        raise TypeError("Number of sequences must be a positive int.")
+    start_time = time.time()
     xi = np.zeros((N, T))
-    A = MLN(T, C, lamda, tau).gen_A()
-    Topt = A.shape[0] // 2
-    args_ls = [(Topt, C, lamda, tau, A) for _ in range(N)]
-    npc = multiprocessing.cpu_count() // 2
-    nc = min(N, npc) if nc > N else min(nc, npc)
-    with Pool(processes=nc) as pool:
-        for i, tmp in enumerate(pool.imap(cal_mln, args_ls)):
-            rd = random.randint(0, Topt - T)
-            xi[i, :] = tmp[rd:rd + T]
-            if pbar: pbar.update(1)
-    if pbar: pbar.close()
+    MLN(N, T, C, lamda, tau).update_A()
+    Topt = MLN.A.shape[0] // 2
+    np.random.seed(seed)
+    rd = np.random.randint(0, Topt - T + 1, N)
+    idx = np.arange(T) + rd[:, np.newaxis]
+    args = N, Topt, C, lamda, tau, seed
+    xi = cal_mln(args)[np.arange(N)[:, np.newaxis], idx]
+    end_time = time.time()
+    execution_time = end_time - start_time
+    print("M-L Noise Generation Time: ", execution_time, "s")
     return xi
 
 
 def acf(xi, tmax, dt, nc=1):
     """
     Parallel computation of the actual autocorrelation function for specified lags for Mittag-Leffler correlated noise sequences.
 
     Parameters:
     - xi: 2D numpy array containing noise sequences generated by `genml.mln`.
     - tmax: Maximum lag to compute the autocorrelation function for (int).
     - dt: Step size between lags (int).
     - nc: Number of parallel cores (int).
 
-    Returns:
+    Return:
     A 1D numpy array containing the acf values.
     """
     if not isinstance(xi, np.ndarray):
         raise TypeError("xi must be a numpy ndarray")
     if not isinstance(tmax, int) or not isinstance(dt, int) or not isinstance(nc, int):
         raise TypeError("tmax, dt, and nc must be integers")
     if np.any(xi.shape) <= 0:
         raise ValueError("The number and length of the noise must be greater than 0.")
     T = xi.shape[1]
     if tmax > T - 1:
         raise ValueError("The max lag must be lower than T.")
     if not (1 <= dt < tmax):
         raise ValueError("The sampling interval must be within the range [1, tmax).")
-    npc = multiprocessing.cpu_count() // 2
+    npc = mp.cpu_count()
     nc = min(tmax, npc) if nc > tmax else min(nc, npc)
     ls = list(range(0, tmax + 1, dt))
     args_ls = [(xi, T, i) for i in ls]
-    with Pool(processes=nc) as pool:
-        acfv = list(tqdm(pool.imap(cal_acf, args_ls), total=len(args_ls), desc='Calculating ACF', position=0))
+    if sys.platform.startswith('darwin'):
+        print("macOS detected, employing the multiprocess library")
+        with Pool1(processes=nc) as pool:
+            acfv = list(tqdm(pool.imap(cal_acf, args_ls), total=len(args_ls), desc='Calculating ACF', position=0))
+    else:
+        with Pool2(processes=nc) as pool:
+            acfv = list(tqdm(pool.imap(cal_acf, args_ls), total=len(args_ls), desc='Calculating ACF', position=0))
     return np.array(acfv)
 
 
 def acft(tmax, dt, C, lamda, tau):
     """
     Calculate the theoretical autocorrelation function for Mittag-Leffler correlated noise.
 
     Parameters:
     - tmax: Maximum lag to compute the acft for (int).
     - dt: Step size between lags (int).
     - C: Amplitude coefficient (float).
     - lamda: Mittag-Leffler exponent (0 < lamda < 2).
     - tau: Characteristic memory time (0 < tau <= 10000).
 
-    Returns:
+    Return:
     A 1D numpy array containing the theoretical acf.
     """
     if not (1 <= dt < tmax):
         raise ValueError("The sampling interval must be within the range [1, tmax).")
-    acftv = MLN(tmax, C, lamda, tau).cal_acft(np.array(range(0, tmax + 1, dt)))
+    acftv = MLN(1, tmax, C, lamda, tau).cal_acft(np.array(range(0, tmax + 1, dt)))
     return acftv
```

### Comparing `genml-0.3.1/genml/mittag_leffler.py` & `genml-0.4.0/genml/mittag_leffler.py`

 * *Files identical despite different names*

### Comparing `genml-0.3.1/setup.py` & `genml-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='genml',
-    version='0.3.1',
+    version='0.4.0',
     description='A Python package for generating Mittag-Leffler correlated noise',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'numpy>=1.16.0',
         'tqdm>=4.29.1',
         'scipy>=1.2.0',
-        'matplotlib>=3.0.2'
+        'matplotlib>=3.0.2',
+        'multiprocess>=0.70.12'
     ],
     python_requires='>=3.6',
 )
```

