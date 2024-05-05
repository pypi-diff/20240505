# Comparing `tmp/cbor_diag-1.0.1.tar.gz` & `tmp/cbor_diag-1.0.2.tar.gz`

## Comparing `cbor_diag-1.0.1.tar` & `cbor_diag-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 cbor_diag-1.0.1/Cargo.toml
--rw-r--r--   0     1001      123     5842 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      755 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.gitignore
--rw-r--r--   0     1001      123      345 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/.readthedocs.yaml
--rw-r--r--   0     1001      123     2171 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/README.rst
--rw-r--r--   0     1001      123      130 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doc/conf.py
--rw-r--r--   0     1001      123      318 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doc/index.rst
--rw-r--r--   0     1001      123      501 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/doctest.txt
--rw-r--r--   0     1001      123      579 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/pyproject.toml
--rw-r--r--   0     1001      123       40 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/pytest.ini
--rw-r--r--   0     1001      123       85 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/python/cbor_diag/__init__.py
--rw-r--r--   0     1001      123     2132 2023-05-27 20:12:38.000000 cbor_diag-1.0.1/src/lib.rs
--rw-r--r--   0     1001      123    12905 2023-05-27 20:14:12.000000 cbor_diag-1.0.1/Cargo.lock
--rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 cbor_diag-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 cbor_diag-1.0.2/Cargo.toml
+-rw-r--r--   0     1001      127     6498 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127      755 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/.gitignore
+-rw-r--r--   0     1001      127      345 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/.readthedocs.yaml
+-rw-r--r--   0     1001      127     2404 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/README.rst
+-rw-r--r--   0     1001      127      130 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/doc/conf.py
+-rw-r--r--   0     1001      127      318 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/doc/index.rst
+-rw-r--r--   0     1001      127      501 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/doctest.txt
+-rw-r--r--   0     1001      127       40 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/pytest.ini
+-rw-r--r--   0     1001      127       85 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/python/cbor_diag/__init__.py
+-rw-r--r--   0     1001      127     2132 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/src/lib.rs
+-rw-r--r--   0     1001      127    12890 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/Cargo.lock
+-rw-r--r--   0     1001      127      616 2024-05-05 21:48:01.000000 cbor_diag-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 cbor_diag-1.0.2/PKG-INFO
```

### Comparing `cbor_diag-1.0.1/.gitignore` & `cbor_diag-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cbor_diag-1.0.1/README.rst` & `cbor_diag-1.0.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 and will likely manifest as extra arguments to ``cbor2diag``.
 
 This package is built using maturin_ and pyo3_
 and largely follows their template.
 The built module is renamed from ``cbor_diag`` to ``_cbor_diag``
 (and consequently wrapped manually)
 to avoid it being part of the package's public API.
+(The need for the workaround is tracked `at maturin`_ and through there `in the typing module`_).
 
 The package is currently hosted on GitHub at https://github.com/chrysn/cbor-diag-py
 because maturin can `not yet`_ build pipelines for GitLab or codeberg.
 
 License
 =======
 
@@ -52,10 +53,12 @@
 
 .. _`cbor-diag crate`: https://crates.io/crates/cbor-diag
 .. _cbor2: https://pypi.org/project/cbor2/
 .. _`on readthedocs`: https://cbor-diag.readthedocs.io/
 .. _`from PyPI`: https://pypi.org/project/cbor-diag/
 .. _maturin: https://www.maturin.rs/
 .. _pyo3: https://pyo3.rs/
+.. _`at maturin`: https://github.com/PyO3/maturin/issues/1399
+.. _`in the typing module`: https://github.com/python/typing/issues/1333
 .. _`not yet`: https://github.com/PyO3/maturin/issues/1507
 .. _MIT: https://spdx.org/licenses/MIT.html
 .. _Apache-2.0: https://spdx.org/licenses/Apache-2.0.html
```

### Comparing `cbor_diag-1.0.1/pyproject.toml` & `cbor_diag-1.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.5.1,<1.6"]
 build-backend = "maturin"
 
 [project]
 name = "cbor-diag"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 6 - Mature",
@@ -15,7 +15,8 @@
     "Programming Language :: Rust",
 ]
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
+module-name = "cbor_diag._cbor_diag"
```

### Comparing `cbor_diag-1.0.1/src/lib.rs` & `cbor_diag-1.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cbor_diag-1.0.1/Cargo.lock` & `cbor_diag-1.0.2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bs58"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f5353f36341f7451062466f0b755b96ac3a9547e4d7f6b70d603fc721a7d7896"
+checksum = "bf88ba1141d185c399bee5288d850d63b8369520c1eafc32a0430b5b6c287bf4"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "cbor-diag"
 version = "0.1.12"
@@ -40,103 +40,103 @@
  "separator",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "cbor-diag-python-package"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
  "cbor-diag",
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
- "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "data-encoding"
-version = "2.4.0"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+checksum = "e8566979429cf69b49a5c740c60791108e86440e8be149bbea4fe54d2c32d6e2"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "half"
-version = "2.2.1"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
+ "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
@@ -157,30 +157,29 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -190,61 +189,61 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -303,64 +302,64 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "separator"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f97841a747eef040fcd2e7b3b9a220a7205926e60488e673d9e4926d27772ce5"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
@@ -371,114 +370,112 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
-
-[[package]]
-name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "windows-targets"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `cbor_diag-1.0.1/PKG-INFO` & `cbor_diag-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cbor-diag
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Rust
@@ -48,14 +48,15 @@
 and will likely manifest as extra arguments to ``cbor2diag``.
 
 This package is built using maturin_ and pyo3_
 and largely follows their template.
 The built module is renamed from ``cbor_diag`` to ``_cbor_diag``
 (and consequently wrapped manually)
 to avoid it being part of the package's public API.
+(The need for the workaround is tracked `at maturin`_ and through there `in the typing module`_).
 
 The package is currently hosted on GitHub at https://github.com/chrysn/cbor-diag-py
 because maturin can `not yet`_ build pipelines for GitLab or codeberg.
 
 License
 =======
 
@@ -68,11 +69,13 @@
 
 .. _`cbor-diag crate`: https://crates.io/crates/cbor-diag
 .. _cbor2: https://pypi.org/project/cbor2/
 .. _`on readthedocs`: https://cbor-diag.readthedocs.io/
 .. _`from PyPI`: https://pypi.org/project/cbor-diag/
 .. _maturin: https://www.maturin.rs/
 .. _pyo3: https://pyo3.rs/
+.. _`at maturin`: https://github.com/PyO3/maturin/issues/1399
+.. _`in the typing module`: https://github.com/python/typing/issues/1333
 .. _`not yet`: https://github.com/PyO3/maturin/issues/1507
 .. _MIT: https://spdx.org/licenses/MIT.html
 .. _Apache-2.0: https://spdx.org/licenses/Apache-2.0.html
```

