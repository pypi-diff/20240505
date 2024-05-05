# Comparing `tmp/pyreqwest_impersonate-0.4.1.tar.gz` & `tmp/pyreqwest_impersonate-0.4.2.tar.gz`

## Comparing `pyreqwest_impersonate-0.4.1.tar` & `pyreqwest_impersonate-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.1/Cargo.toml
--rw-r--r--   0     1001      127     7988 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      766 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/.gitignore
--rw-r--r--   0     1001      127     7518 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/README.md
--rw-r--r--   0     1001      127      343 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark/README.md
--rw-r--r--   0     1001      127     3484 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark/benchmark.py
--rw-r--r--   0     1001      127     3179 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark/generate_image.py
--rw-r--r--   0     1001      127       94 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark/requirements.txt
--rw-r--r--   0     1001      127      990 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark/server.py
--rw-r--r--   0     1001      127    85794 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/benchmark.jpg
--rw-r--r--   0     1001      127    26340 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/src/response.rs
--rw-r--r--   0     1001      127     3830 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/tests/test_client.py
--rw-r--r--   0     1001      127     5370 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/tests/test_defs.py
--rw-r--r--   0     1001      127    43175 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-05-02 16:05:50.000000 pyreqwest_impersonate-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8587 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.2/Cargo.toml
+-rw-r--r--   0     1001      127     7984 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      766 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/.gitignore
+-rw-r--r--   0     1001      127     7989 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/README.md
+-rw-r--r--   0     1001      127      343 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/README.md
+-rw-r--r--   0     1001      127     3484 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/benchmark.py
+-rw-r--r--   0     1001      127     3719 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/generate_image.py
+-rw-r--r--   0     1001      127      144 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      990 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark/server.py
+-rw-r--r--   0     1001      127    84789 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/benchmark.jpg
+-rw-r--r--   0     1001      127    26365 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/src/response.rs
+-rw-r--r--   0     1001      127     3830 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/tests/test_client.py
+-rw-r--r--   0     1001      127     5370 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/tests/test_defs.py
+-rw-r--r--   0     1001      127    41269 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-05-05 16:43:38.000000 pyreqwest_impersonate-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     9058 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.4.2/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.4.1/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.4.2/.github/workflows/CI.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
-          rust-toolchain: nightly
+          rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist --zig
           sccache: 'true'
           manylinux: 2_28
         env:
           CFLAGS_aarch64_unknown_linux_gnu: "-D__ARM_ARCH=8"
       - name: Upload wheels
@@ -85,15 +85,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
-          rust-toolchain: nightly
+          rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist --zig
           sccache: 'true'
           manylinux: musllinux_1_2
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
@@ -141,15 +141,15 @@
           python-version: '3.12'
           architecture: ${{ matrix.platform.target }}
       - name: Install nasm
         run: choco install nasm
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
-          rust-toolchain: nightly
+          rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-windows-${{ matrix.platform.target }}
@@ -176,15 +176,15 @@
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: '3.12'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
-          rust-toolchain: nightly
+          rust-toolchain: stable
           target: ${{ matrix.platform.target }}
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
```

### Comparing `pyreqwest_impersonate-0.4.1/.gitignore` & `pyreqwest_impersonate-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/README.md` & `pyreqwest_impersonate-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,23 @@
  - [II. AsyncClient](#ii-asyncclient)
 
 ## Installation
 
 ```python
 pip install -U pyreqwest_impersonate
 ```
+To improve the performance of the library for your particular processor, you can build the library yourself using Rust. Install Rust: https://www.rust-lang.org/tools/install
+```python
+git clone https://github.com/deedy5/pyreqwest_impersonate.git
+cd pyreqwest_impersonate
+python3 -m venv .venv
+source .venv/bin/activate
+pip install maturin
+RUSTFLAGS="-C target-cpu=native" maturin develop --release  # Compiled library will be here: .venv/lib/python3.1x/site-packages
+```
 
 ## Key Features
 - Impersonate: The Client offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and TLS/JA3/JA4/HTTP2 fingerprints.
 - Thread-safe: The Client is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
 - Automatic Character Encoding Detection: The encoding is taken from the "Content-Type" header, but if not specified, "UTF-8". If encoding does not match the content, the package automatically detects and uses the correct encoding to decode the text.
 - Small Size: The compiled library is about 5.8MB in size.
 - High Performance: The library is designed for a large number of threads, uses all processors, and releases the GIL. All operations like accessing headers, decoding text, or parsing JSON are executed in Rust.
```

### Comparing `pyreqwest_impersonate-0.4.1/benchmark/benchmark.py` & `pyreqwest_impersonate-0.4.2/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/benchmark/generate_image.py` & `pyreqwest_impersonate-0.4.2/benchmark/generate_image.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,40 +45,55 @@
     # Plot CPU time for 200k requests
     rects = ax.bar(x + 5*width, cpu_time_200k, width, label='CPU Time 200k')
     ax.bar_label(rects, padding=3, fontsize=7) 
 
     return x, width, names
 
 # Create a figure with two subplots
-fig, (ax1, ax2) = plt.subplots(2, 1, figsize=(10, 6), layout='constrained')
+fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=(10, 6), layout='constrained')
 
 # Plot data for 1 thread in the first subplot
 x1, width, names = plot_data('1_threads.csv', ax1, 0)
 
+# Plot data for 5 threads in the second subplot
+x2, _, _ = plot_data('5_threads.csv', ax2, 0)
+
 # Plot data for 32 threads in the second subplot
-x2, _, _ = plot_data('32_threads.csv', ax2, 0) # Offset is 0 for the second plot
+x3, _, _ = plot_data('32_threads.csv', ax3, 0)
+
 
 # Adjust the y-axis limits for the first subplot
 y_min, y_max = ax1.get_ylim()
 new_y_max = y_max + 1
 ax1.set_ylim(y_min, new_y_max)
 
 # Adjust the y-axis limits for the second subplot
 y_min, y_max = ax2.get_ylim()
 new_y_max = y_max + 1
 ax2.set_ylim(y_min, new_y_max)
 
+# Adjust the y-axis limits for the third subplot
+y_min, y_max = ax3.get_ylim()
+new_y_max = y_max + 1
+ax3.set_ylim(y_min, new_y_max)
+
 # Add some text for labels, title and custom x-axis tick labels, etc.
 ax1.set_ylabel('Time (s)')
 ax1.set_title('Performance comparison. Threads: 1. Requests: 2000. Response: gzip, utf-8, size 5Kb|50Kb|200Kb')
 ax1.set_xticks(x1 + 3*width - width/2) # Adjust the x-ticks to be after the 3rd bar, moved 0.5 bar width to the left
 ax1.set_xticklabels(names)
 ax1.legend(loc='upper left', ncols=6, prop={'size': 8})
 
 ax2.set_ylabel('Time (s)')
-ax2.set_title('Performance comparison. Threads: 32. Requests: 2000. Response: gzip, utf-8, size 5Kb|50Kb|200Kb')
+ax2.set_title('Performance comparison. Threads: 5. Requests: 2000. Response: gzip, utf-8, size 5Kb|50Kb|200Kb')
 ax2.set_xticks(x2 + 3*width - width/2) # Adjust the x-ticks to be after the 3rd bar, moved 0.5 bar width to the left
 ax2.set_xticklabels(names)
 ax2.legend(loc='upper left', ncols=6, prop={'size': 8})
 
+ax3.set_ylabel('Time (s)')
+ax3.set_title('Performance comparison. Threads: 32. Requests: 2000. Response: gzip, utf-8, size 5Kb|50Kb|200Kb')
+ax3.set_xticks(x3 + 3*width - width/2) # Adjust the x-ticks to be after the 3rd bar, moved 0.5 bar width to the left
+ax3.set_xticklabels(names)
+ax3.legend(loc='upper left', ncols=6, prop={'size': 8})
+
 # Save the plot to a file
 plt.savefig('benchmark.jpg', format='jpg')
```

### Comparing `pyreqwest_impersonate-0.4.1/benchmark/server.py` & `pyreqwest_impersonate-0.4.2/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/benchmark.jpg` & `pyreqwest_impersonate-0.4.2/benchmark.jpg`

 * *Files 16% similar despite different names*

#### Image content

```diff
@@ -1,21 +1,21 @@
    .;:;8888@8@888888X888X@88888X8@X8@88888S8@S888@8X8@@@S;::
- .%XX@%SS:XXSSX:XXtS%X.88XSS%;;8tX%SX;X8tSS%X% .   ..  :S: %
-  SX                  .:.    .            .       .8.  8;@ t
-  .S . . . .     . .       .    . .    .    .  .   8 ; 8S8 %
- @.X         .          .     .     .   :@.   .    88  88S t
- 8:@ .  .  .     . :%X   .  .   .  .  . :@%  8%    8 : 8t8.%
- ;.@   . t@   .   .@8:  8S;   S8   t..;8X8@ :@   tX8X :@8@ t
-   % ...%@8 . SS %X8@ :t;8t..%:X  :X;8X.888@:88:%X88 :.%8@.%
-  :X. 8S@88%%8S8888 :%t:8:S%..;8X8@t S8 888%X88S888t8@@88@ t
-  :S;;8S X@%%8% ; tX:8XX:%X:t S8%:X@8@S8X;S 8  t :SXXXXS 8;%
-  .   :%88@888%S;%%X8X88;88@@XXX@S8888S@888X@@St;8888888X   
- .:;X@X@8X@8888@8@8@S88X888@8@@888888X8X@88888%StX@tS@@X@t;t
- :%X;;;;::;:;;t:;t:;;t:%S;:::::;:;;;;:;%:;;:;: .  .   .8@S %
- ;SX  .  .    .       .   .    .      . .  .      ..   88S.t
-;;XX.  .    .  .    .  .    .    .  .  .    .:t  .  . .88X.%
-8 ;%      .      .    . 8 ;   .    .     .    8    .  .88S t
-8 ;X .      . 88.  .   .:8: .   .     . .% . 88. .   .;%.@ %
-  S@   .  .  .88:   %X@@X8t:  .   .:.  :X.X.888 . .:X X@:@ t
- .%@  ..;8 :Xt:@:SX888t@@8t...:; .;@SS:8@@;8888:.;;@8%.8:@.t
-  ;%. @X888t@888S88.88%;88;%.@t8S%%S t88S88tS.8t:S8888888%.t
-  %:;;:%X%S888%%  %8XX%8 X888SX@88888X.888%S@S%;;8S8@S8;.;;:
+ .%XX@%SS:XXSSX:XXtS%X.88XSS%;;8tX%SX;X8tSS%X% .       ;S: %
+  tX                  .:.    .            .       .t8. 8t8 t
+  :% . . . .     . .       .    . .    .    .  .   @S  8%8 t
+ @:@         .          .     .     .    .    .  . X t 88S %
+ 8:@ .  .  .     . .X;   .  .   .  .  . 88%  ;t    @@. 8t8.t
+ ;.@  .  :%   .    X8 . 8;;   ;t   ;:  t @S  :8. :;8 t.88@ %
+   %.  .;t%t. 88 t8S8; t;SS .%8;. :8%S%t8X8S888 :% XS X;8S.%
+  :X  8;88%:%8S8S@88t@S:@tS8:@8: 8@t t8.8888888%S888@8.88@.t
+  :X;;8@:X:: X% %  XS@8SS X: St.8.@X%8S8X;8 tS %  .SXXSS 8;%
+       S88@88@%S;tS88@8@;88@8X8@8t888@%8@8X888St.8888888X   
+ t%SX@S8@X8888888@8XS8XS888888@88888888X@88888SX%8X%X8XX8t;t
+ ;SX;;:;:.ttttt:;;:;:;.%%;:;;::%;t;;t:t%:;ttt;   .. .  88X %
+ :tS     .       .       .         .  .     .      . . 88X t
+;:;S . .     . .    . .   .  .  .      .  .   . .     .88t.%
+8;SX      .       .     :%    .   . . . .   .S@  .   ..88@.t
+8 SX.  .   . .tt    .  .;;% .             .  @8t   .  .8t8 t
+  S@    .     8@ .  ;;%8 8;   . .  .. . % . %88    .8 8:8:.t
+ .tX. . :X8 SX X.XtS888888%.. .: .;t8%%S88@SS88  :t@8. 8.X %
+  tS  8:8@8 ;88@%88.88;SS%X8%S @@;S% %88%S%;S88S t @8X88.8 t
+  t;;:;;SS@88XXt..%8XS%8.X888XS888@88%;X@@XSXSS::@@8@8%%tt;:
```

#### Image metadata

```diff
@@ -10,10 +10,10 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 100
 Y resolution: 100
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 17089
+Number of unique colors: 17485
 Comment: 
 EXIF data:
```

### Comparing `pyreqwest_impersonate-0.4.1/src/response.rs` & `pyreqwest_impersonate-0.4.2/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/tests/test_client.py` & `pyreqwest_impersonate-0.4.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/tests/test_defs.py` & `pyreqwest_impersonate-0.4.2/tests/test_defs.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/Cargo.lock` & `pyreqwest_impersonate-0.4.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -44,23 +44,14 @@
 [[package]]
 name = "antidote"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34fde25430d87a9388dadbe6e34d7f72a462c8b43ac8d309b42b0a8505d7e2a5"
 
 [[package]]
-name = "any_all_workaround"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88fea40735f2cc320a5133ce772d39c571bd6c9b0d4c1a326926eecdd5af2e86"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "async-compression"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e9eabd7a98fe442131a17c316bd9349c43695e49e730c3c8e12cfb5f4da2693"
 dependencies = [
  "brotli 5.0.0",
  "flate2",
@@ -68,17 +59,17 @@
  "memchr",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -299,39 +290,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "crossbeam-deque"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
-dependencies = [
- "crossbeam-epoch",
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-epoch"
-version = "0.9.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
-dependencies = [
- "crossbeam-utils",
-]
-
-[[package]]
-name = "crossbeam-utils"
-version = "0.8.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
-
-[[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
@@ -344,15 +310,14 @@
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
- "any_all_workaround",
  "cfg-if",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -489,20 +454,14 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
-name = "hermit-abi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
-
-[[package]]
 name = "http"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
@@ -768,24 +727,14 @@
 [[package]]
 name = "num-conv"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
 
 [[package]]
-name = "num_cpus"
-version = "1.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
-dependencies = [
- "hermit-abi",
- "libc",
-]
-
-[[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
@@ -935,20 +884,19 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.4.1"
+version = "0.4.2"
 dependencies = [
  "encoding_rs",
  "pyo3",
  "pythonize",
- "rayon",
  "reqwest-impersonate",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "pythonize"
@@ -966,34 +914,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "rayon"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
-dependencies = [
- "either",
- "rayon-core",
-]
-
-[[package]]
-name = "rayon-core"
-version = "1.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
-dependencies = [
- "crossbeam-deque",
- "crossbeam-utils",
-]
-
-[[package]]
 name = "redox_syscall"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags 2.5.0",
 ]
@@ -1281,15 +1209,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
- "num_cpus",
  "pin-project-lite",
  "socket2",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-boring-imp"
@@ -1312,24 +1239,23 @@
  "futures-util",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
```

### Comparing `pyreqwest_impersonate-0.4.1/pyproject.toml` & `pyreqwest_impersonate-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.4.1/PKG-INFO` & `pyreqwest_impersonate-0.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.4.1
+Version: 0.4.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -42,14 +42,23 @@
  - [II. AsyncClient](#ii-asyncclient)
 
 ## Installation
 
 ```python
 pip install -U pyreqwest_impersonate
 ```
+To improve the performance of the library for your particular processor, you can build the library yourself using Rust. Install Rust: https://www.rust-lang.org/tools/install
+```python
+git clone https://github.com/deedy5/pyreqwest_impersonate.git
+cd pyreqwest_impersonate
+python3 -m venv .venv
+source .venv/bin/activate
+pip install maturin
+RUSTFLAGS="-C target-cpu=native" maturin develop --release  # Compiled library will be here: .venv/lib/python3.1x/site-packages
+```
 
 ## Key Features
 - Impersonate: The Client offers an `impersonate` option, enabling it to mimic web browsers by replicating their headers and TLS/JA3/JA4/HTTP2 fingerprints.
 - Thread-safe: The Client is designed to be thread-safe, allowing it to be safely used in multithreaded environments.
 - Automatic Character Encoding Detection: The encoding is taken from the "Content-Type" header, but if not specified, "UTF-8". If encoding does not match the content, the package automatically detects and uses the correct encoding to decode the text.
 - Small Size: The compiled library is about 5.8MB in size.
 - High Performance: The library is designed for a large number of threads, uses all processors, and releases the GIL. All operations like accessing headers, decoding text, or parsing JSON are executed in Rust.
```

