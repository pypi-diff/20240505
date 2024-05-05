# Comparing `tmp/flackup-0.7.3.tar.gz` & `tmp/flackup-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flackup-0.7.3.tar", last modified: Sun Feb  4 20:46:06 2024, max compression
+gzip compressed data, was "flackup-0.7.4.tar", last modified: Sun May  5 19:16:54 2024, max compression
```

## Comparing `flackup-0.7.3.tar` & `flackup-0.7.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.251834 flackup-0.7.3/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       57 2022-03-14 21:45:24.000000 flackup-0.7.3/.gitignore
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        4 2023-02-14 01:13:33.000000 flackup-0.7.3/.python-version
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      809 2024-02-04 20:42:25.000000 flackup-0.7.3/CHANGELOG.md
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2022-03-14 21:21:38.000000 flackup-0.7.3/LICENSE
--rw-r--r--   0 alexander  (1000) alexander  (1000)     1840 2024-02-04 20:46:06.251834 flackup-0.7.3/PKG-INFO
--rw-r--r--   0 alexander  (1000) alexander  (1000)      294 2023-02-14 01:21:29.000000 flackup-0.7.3/Pipfile
--rw-r--r--   0 alexander  (1000) alexander  (1000)    37968 2024-02-04 20:41:25.000000 flackup-0.7.3/Pipfile.lock
--rw-r--r--   0 alexander  (1000) alexander  (1000)     1133 2023-07-09 13:57:17.000000 flackup-0.7.3/README.md
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      957 2024-02-04 20:40:48.000000 flackup-0.7.3/pyproject.toml
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      109 2024-02-04 20:46:06.251834 flackup-0.7.3/setup.cfg
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.247834 flackup-0.7.3/src/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.247834 flackup-0.7.3/src/flackup/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       35 2024-02-04 20:42:41.000000 flackup-0.7.3/src/flackup/__init__.py
--rw-r--r--   0 alexander  (1000) alexander  (1000)    12053 2023-02-08 23:51:40.000000 flackup-0.7.3/src/flackup/cli.py
--rw-r--r--   0 alexander  (1000) alexander  (1000)     7698 2021-07-15 12:49:53.000000 flackup-0.7.3/src/flackup/convert.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     9929 2021-07-19 11:34:42.000000 flackup-0.7.3/src/flackup/fileinfo.py
--rw-r--r--   0 alexander  (1000) alexander  (1000)    10500 2019-01-12 14:51:05.000000 flackup-0.7.3/src/flackup/musicbrainz.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.247834 flackup-0.7.3/src/flackup.egg-info/
--rw-r--r--   0 alexander  (1000) alexander  (1000)     1840 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      773 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/entry_points.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       58 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/requires.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        8 2024-02-04 20:46:06.000000 flackup-0.7.3/src/flackup.egg-info/top_level.txt
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.251834 flackup-0.7.3/tests/
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.251834 flackup-0.7.3/tests/test_cli/
--rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2021-07-16 18:51:42.000000 flackup-0.7.3/tests/test_cli/tagged.flac
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     2083 2023-02-08 22:23:58.000000 flackup-0.7.3/tests/test_cli.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.251834 flackup-0.7.3/tests/test_convert/
--rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-10 21:44:24.000000 flackup-0.7.3/tests/test_convert/date_original.flac
--rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-09 15:53:59.000000 flackup-0.7.3/tests/test_convert/tagged.flac
--rw-r--r--   0 alexander  (1000) alexander  (1000)     2072 2018-12-20 19:30:32.000000 flackup-0.7.3/tests/test_convert.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-02-04 20:46:06.251834 flackup-0.7.3/tests/test_fileinfo/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      274 2018-02-19 15:34:10.000000 flackup-0.7.3/tests/test_fileinfo/cover.png
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    26980 2018-02-18 14:39:31.000000 flackup-0.7.3/tests/test_fileinfo/empty.flac
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       25 2018-02-10 20:03:13.000000 flackup-0.7.3/tests/test_fileinfo/invalid.flac
--rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-09 15:53:59.000000 flackup-0.7.3/tests/test_fileinfo/tagged.flac
--rw-rw-r--   0 alexander  (1000) alexander  (1000)    89203 2018-02-11 21:57:39.000000 flackup-0.7.3/tests/test_fileinfo/test.flac
--rw-r--r--   0 alexander  (1000) alexander  (1000)     8554 2018-12-09 15:53:59.000000 flackup-0.7.3/tests/test_fileinfo.py
--rw-r--r--   0 alexander  (1000) alexander  (1000)     5511 2018-12-10 21:37:48.000000 flackup-0.7.3/tests/test_musicbrainz.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.177047 flackup-0.7.4/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       57 2022-03-14 21:45:24.000000 flackup-0.7.4/.gitignore
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        4 2023-02-14 01:13:33.000000 flackup-0.7.4/.python-version
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      843 2024-05-05 19:15:04.000000 flackup-0.7.4/CHANGELOG.md
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    35149 2022-03-14 21:21:38.000000 flackup-0.7.4/LICENSE
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1840 2024-05-05 19:16:54.177047 flackup-0.7.4/PKG-INFO
+-rw-r--r--   0 alexander  (1000) alexander  (1000)      294 2023-02-14 01:21:29.000000 flackup-0.7.4/Pipfile
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    39052 2024-05-05 17:20:44.000000 flackup-0.7.4/Pipfile.lock
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1133 2023-07-09 13:57:17.000000 flackup-0.7.4/README.md
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      957 2024-05-05 17:31:27.000000 flackup-0.7.4/pyproject.toml
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      109 2024-05-05 19:16:54.177047 flackup-0.7.4/setup.cfg
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.169047 flackup-0.7.4/src/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.173047 flackup-0.7.4/src/flackup/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       35 2024-05-05 19:15:12.000000 flackup-0.7.4/src/flackup/__init__.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    12053 2023-02-08 23:51:40.000000 flackup-0.7.4/src/flackup/cli.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     7698 2021-07-15 12:49:53.000000 flackup-0.7.4/src/flackup/convert.py
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     9929 2021-07-19 11:34:42.000000 flackup-0.7.4/src/flackup/fileinfo.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    10500 2019-01-12 14:51:05.000000 flackup-0.7.4/src/flackup/musicbrainz.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.173047 flackup-0.7.4/src/flackup.egg-info/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     1840 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      773 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       48 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/entry_points.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       58 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/requires.txt
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)        8 2024-05-05 19:16:54.000000 flackup-0.7.4/src/flackup.egg-info/top_level.txt
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.173047 flackup-0.7.4/tests/
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.173047 flackup-0.7.4/tests/test_cli/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2021-07-16 18:51:42.000000 flackup-0.7.4/tests/test_cli/tagged.flac
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)     2083 2023-02-08 22:23:58.000000 flackup-0.7.4/tests/test_cli.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.173047 flackup-0.7.4/tests/test_convert/
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-10 21:44:24.000000 flackup-0.7.4/tests/test_convert/date_original.flac
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-09 15:53:59.000000 flackup-0.7.4/tests/test_convert/tagged.flac
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     2072 2018-12-20 19:30:32.000000 flackup-0.7.4/tests/test_convert.py
+drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-05-05 19:16:54.177047 flackup-0.7.4/tests/test_fileinfo/
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)      274 2018-02-19 15:34:10.000000 flackup-0.7.4/tests/test_fileinfo/cover.png
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    26980 2018-02-18 14:39:31.000000 flackup-0.7.4/tests/test_fileinfo/empty.flac
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)       25 2018-02-10 20:03:13.000000 flackup-0.7.4/tests/test_fileinfo/invalid.flac
+-rw-r--r--   0 alexander  (1000) alexander  (1000)    89203 2018-12-09 15:53:59.000000 flackup-0.7.4/tests/test_fileinfo/tagged.flac
+-rw-rw-r--   0 alexander  (1000) alexander  (1000)    89203 2018-02-11 21:57:39.000000 flackup-0.7.4/tests/test_fileinfo/test.flac
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     8554 2018-12-09 15:53:59.000000 flackup-0.7.4/tests/test_fileinfo.py
+-rw-r--r--   0 alexander  (1000) alexander  (1000)     5511 2018-12-10 21:37:48.000000 flackup-0.7.4/tests/test_musicbrainz.py
```

### Comparing `flackup-0.7.3/CHANGELOG.md` & `flackup-0.7.4/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## v0.7.4
+
+- Update dependencies
+
 ## v0.7.3
 
 - Update dependencies
 
 ## v0.7.2
 
 - Update dependencies
```

### Comparing `flackup-0.7.3/LICENSE` & `flackup-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/PKG-INFO` & `flackup-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flackup
-Version: 0.7.3
+Version: 0.7.4
 Summary: FLAC CD Backup Manager
 Author-email: Alexander Dietrich <alexander@dietrich.cx>
 Project-URL: Homepage, https://codeberg.org/alxndr42/flackup
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click~=8.1
 Requires-Dist: musicbrainzngs~=0.7
 Requires-Dist: mutagen~=1.47
-Requires-Dist: pillow~=10.2
+Requires-Dist: pillow~=10.3
 
 # Flackup
 
 Flackup manages audio CD backups as single FLAC files with [embedded cue
 sheets][cuesheet], adds metadata from [MusicBrainz][] and converts albums to
 individual [Ogg Vorbis][] tracks.
```

### Comparing `flackup-0.7.3/Pipfile.lock` & `flackup-0.7.4/Pipfile.lock`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967013888888889%*

 * *Differences: {"'default'": "{'pillow': {'hashes': "*

 * *              "['sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c', "*

 * *              "'sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2', "*

 * *              "'sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb', "*

 * *              "'sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d', "*

 * *              "'sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa', "*

 * *             […]*

```diff
@@ -41,97 +41,106 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==1.47.0"
         },
         "pillow": {
             "hashes": [
-                "sha256:0304004f8067386b477d20a518b50f3fa658a28d44e4116970abfcd94fac34a8",
-                "sha256:0689b5a8c5288bc0504d9fcee48f61a6a586b9b98514d7d29b840143d6734f39",
-                "sha256:0eae2073305f451d8ecacb5474997c08569fb4eb4ac231ffa4ad7d342fdc25ac",
-                "sha256:0fb3e7fc88a14eacd303e90481ad983fd5b69c761e9e6ef94c983f91025da869",
-                "sha256:11fa2e5984b949b0dd6d7a94d967743d87c577ff0b83392f17cb3990d0d2fd6e",
-                "sha256:127cee571038f252a552760076407f9cff79761c3d436a12af6000cd182a9d04",
-                "sha256:154e939c5f0053a383de4fd3d3da48d9427a7e985f58af8e94d0b3c9fcfcf4f9",
-                "sha256:15587643b9e5eb26c48e49a7b33659790d28f190fc514a322d55da2fb5c2950e",
-                "sha256:170aeb00224ab3dc54230c797f8404507240dd868cf52066f66a41b33169bdbe",
-                "sha256:1b5e1b74d1bd1b78bc3477528919414874748dd363e6272efd5abf7654e68bef",
-                "sha256:1da3b2703afd040cf65ec97efea81cfba59cdbed9c11d8efc5ab09df9509fc56",
-                "sha256:1e23412b5c41e58cec602f1135c57dfcf15482013ce6e5f093a86db69646a5aa",
-                "sha256:2247178effb34a77c11c0e8ac355c7a741ceca0a732b27bf11e747bbc950722f",
-                "sha256:257d8788df5ca62c980314053197f4d46eefedf4e6175bc9412f14412ec4ea2f",
-                "sha256:3031709084b6e7852d00479fd1d310b07d0ba82765f973b543c8af5061cf990e",
-                "sha256:322209c642aabdd6207517e9739c704dc9f9db943015535783239022002f054a",
-                "sha256:322bdf3c9b556e9ffb18f93462e5f749d3444ce081290352c6070d014c93feb2",
-                "sha256:33870dc4653c5017bf4c8873e5488d8f8d5f8935e2f1fb9a2208c47cdd66efd2",
-                "sha256:35bb52c37f256f662abdfa49d2dfa6ce5d93281d323a9af377a120e89a9eafb5",
-                "sha256:3c31822339516fb3c82d03f30e22b1d038da87ef27b6a78c9549888f8ceda39a",
-                "sha256:3eedd52442c0a5ff4f887fab0c1c0bb164d8635b32c894bc1faf4c618dd89df2",
-                "sha256:3ff074fc97dd4e80543a3e91f69d58889baf2002b6be64347ea8cf5533188213",
-                "sha256:47c0995fc4e7f79b5cfcab1fc437ff2890b770440f7696a3ba065ee0fd496563",
-                "sha256:49d9ba1ed0ef3e061088cd1e7538a0759aab559e2e0a80a36f9fd9d8c0c21591",
-                "sha256:51f1a1bffc50e2e9492e87d8e09a17c5eea8409cda8d3f277eb6edc82813c17c",
-                "sha256:52a50aa3fb3acb9cf7213573ef55d31d6eca37f5709c69e6858fe3bc04a5c2a2",
-                "sha256:54f1852cd531aa981bc0965b7d609f5f6cc8ce8c41b1139f6ed6b3c54ab82bfb",
-                "sha256:609448742444d9290fd687940ac0b57fb35e6fd92bdb65386e08e99af60bf757",
-                "sha256:69ffdd6120a4737710a9eee73e1d2e37db89b620f702754b8f6e62594471dee0",
-                "sha256:6fad5ff2f13d69b7e74ce5b4ecd12cc0ec530fcee76356cac6742785ff71c452",
-                "sha256:7049e301399273a0136ff39b84c3678e314f2158f50f517bc50285fb5ec847ad",
-                "sha256:70c61d4c475835a19b3a5aa42492409878bbca7438554a1f89d20d58a7c75c01",
-                "sha256:716d30ed977be8b37d3ef185fecb9e5a1d62d110dfbdcd1e2a122ab46fddb03f",
-                "sha256:753cd8f2086b2b80180d9b3010dd4ed147efc167c90d3bf593fe2af21265e5a5",
-                "sha256:773efe0603db30c281521a7c0214cad7836c03b8ccff897beae9b47c0b657d61",
-                "sha256:7823bdd049099efa16e4246bdf15e5a13dbb18a51b68fa06d6c1d4d8b99a796e",
-                "sha256:7c8f97e8e7a9009bcacbe3766a36175056c12f9a44e6e6f2d5caad06dcfbf03b",
-                "sha256:823ef7a27cf86df6597fa0671066c1b596f69eba53efa3d1e1cb8b30f3533068",
-                "sha256:8373c6c251f7ef8bda6675dd6d2b3a0fcc31edf1201266b5cf608b62a37407f9",
-                "sha256:83b2021f2ade7d1ed556bc50a399127d7fb245e725aa0113ebd05cfe88aaf588",
-                "sha256:870ea1ada0899fd0b79643990809323b389d4d1d46c192f97342eeb6ee0b8483",
-                "sha256:8d12251f02d69d8310b046e82572ed486685c38f02176bd08baf216746eb947f",
-                "sha256:9c23f307202661071d94b5e384e1e1dc7dfb972a28a2310e4ee16103e66ddb67",
-                "sha256:9d189550615b4948f45252d7f005e53c2040cea1af5b60d6f79491a6e147eef7",
-                "sha256:a086c2af425c5f62a65e12fbf385f7c9fcb8f107d0849dba5839461a129cf311",
-                "sha256:a2b56ba36e05f973d450582fb015594aaa78834fefe8dfb8fcd79b93e64ba4c6",
-                "sha256:aebb6044806f2e16ecc07b2a2637ee1ef67a11840a66752751714a0d924adf72",
-                "sha256:b1b3020d90c2d8e1dae29cf3ce54f8094f7938460fb5ce8bc5c01450b01fbaf6",
-                "sha256:b4b6b1e20608493548b1f32bce8cca185bf0480983890403d3b8753e44077129",
-                "sha256:b6f491cdf80ae540738859d9766783e3b3c8e5bd37f5dfa0b76abdecc5081f13",
-                "sha256:b792a349405fbc0163190fde0dc7b3fef3c9268292586cf5645598b48e63dc67",
-                "sha256:b7c2286c23cd350b80d2fc9d424fc797575fb16f854b831d16fd47ceec078f2c",
-                "sha256:babf5acfede515f176833ed6028754cbcd0d206f7f614ea3447d67c33be12516",
-                "sha256:c365fd1703040de1ec284b176d6af5abe21b427cb3a5ff68e0759e1e313a5e7e",
-                "sha256:c4225f5220f46b2fde568c74fca27ae9771536c2e29d7c04f4fb62c83275ac4e",
-                "sha256:c570f24be1e468e3f0ce7ef56a89a60f0e05b30a3669a459e419c6eac2c35364",
-                "sha256:c6dafac9e0f2b3c78df97e79af707cdc5ef8e88208d686a4847bab8266870023",
-                "sha256:c8de2789052ed501dd829e9cae8d3dcce7acb4777ea4a479c14521c942d395b1",
-                "sha256:cb28c753fd5eb3dd859b4ee95de66cc62af91bcff5db5f2571d32a520baf1f04",
-                "sha256:cb4c38abeef13c61d6916f264d4845fab99d7b711be96c326b84df9e3e0ff62d",
-                "sha256:d1b35bcd6c5543b9cb547dee3150c93008f8dd0f1fef78fc0cd2b141c5baf58a",
-                "sha256:d8e6aeb9201e655354b3ad049cb77d19813ad4ece0df1249d3c793de3774f8c7",
-                "sha256:d8ecd059fdaf60c1963c58ceb8997b32e9dc1b911f5da5307aab614f1ce5c2fb",
-                "sha256:da2b52b37dad6d9ec64e653637a096905b258d2fc2b984c41ae7d08b938a67e4",
-                "sha256:e87f0b2c78157e12d7686b27d63c070fd65d994e8ddae6f328e0dcf4a0cd007e",
-                "sha256:edca80cbfb2b68d7b56930b84a0e45ae1694aeba0541f798e908a49d66b837f1",
-                "sha256:f379abd2f1e3dddb2b61bc67977a6b5a0a3f7485538bcc6f39ec76163891ee48",
-                "sha256:fe4c15f6c9285dc54ce6553a3ce908ed37c8f3825b5a51a15c91442bb955b868"
+                "sha256:048ad577748b9fa4a99a0548c64f2cb8d672d5bf2e643a739ac8faff1164238c",
+                "sha256:048eeade4c33fdf7e08da40ef402e748df113fd0b4584e32c4af74fe78baaeb2",
+                "sha256:0ba26351b137ca4e0db0342d5d00d2e355eb29372c05afd544ebf47c0956ffeb",
+                "sha256:0ea2a783a2bdf2a561808fe4a7a12e9aa3799b701ba305de596bc48b8bdfce9d",
+                "sha256:1530e8f3a4b965eb6a7785cf17a426c779333eb62c9a7d1bbcf3ffd5bf77a4aa",
+                "sha256:16563993329b79513f59142a6b02055e10514c1a8e86dca8b48a893e33cf91e3",
+                "sha256:19aeb96d43902f0a783946a0a87dbdad5c84c936025b8419da0a0cd7724356b1",
+                "sha256:1a1d1915db1a4fdb2754b9de292642a39a7fb28f1736699527bb649484fb966a",
+                "sha256:1b87bd9d81d179bd8ab871603bd80d8645729939f90b71e62914e816a76fc6bd",
+                "sha256:1dfc94946bc60ea375cc39cff0b8da6c7e5f8fcdc1d946beb8da5c216156ddd8",
+                "sha256:2034f6759a722da3a3dbd91a81148cf884e91d1b747992ca288ab88c1de15999",
+                "sha256:261ddb7ca91fcf71757979534fb4c128448b5b4c55cb6152d280312062f69599",
+                "sha256:2ed854e716a89b1afcedea551cd85f2eb2a807613752ab997b9974aaa0d56936",
+                "sha256:3102045a10945173d38336f6e71a8dc71bcaeed55c3123ad4af82c52807b9375",
+                "sha256:339894035d0ede518b16073bdc2feef4c991ee991a29774b33e515f1d308e08d",
+                "sha256:412444afb8c4c7a6cc11a47dade32982439925537e483be7c0ae0cf96c4f6a0b",
+                "sha256:4203efca580f0dd6f882ca211f923168548f7ba334c189e9eab1178ab840bf60",
+                "sha256:45ebc7b45406febf07fef35d856f0293a92e7417ae7933207e90bf9090b70572",
+                "sha256:4b5ec25d8b17217d635f8935dbc1b9aa5907962fae29dff220f2659487891cd3",
+                "sha256:4c8e73e99da7db1b4cad7f8d682cf6abad7844da39834c288fbfa394a47bbced",
+                "sha256:4e6f7d1c414191c1199f8996d3f2282b9ebea0945693fb67392c75a3a320941f",
+                "sha256:4eaa22f0d22b1a7e93ff0a596d57fdede2e550aecffb5a1ef1106aaece48e96b",
+                "sha256:50b8eae8f7334ec826d6eeffaeeb00e36b5e24aa0b9df322c247539714c6df19",
+                "sha256:50fd3f6b26e3441ae07b7c979309638b72abc1a25da31a81a7fbd9495713ef4f",
+                "sha256:51243f1ed5161b9945011a7360e997729776f6e5d7005ba0c6879267d4c5139d",
+                "sha256:5d512aafa1d32efa014fa041d38868fda85028e3f930a96f85d49c7d8ddc0383",
+                "sha256:5f77cf66e96ae734717d341c145c5949c63180842a545c47a0ce7ae52ca83795",
+                "sha256:6b02471b72526ab8a18c39cb7967b72d194ec53c1fd0a70b050565a0f366d355",
+                "sha256:6fb1b30043271ec92dc65f6d9f0b7a830c210b8a96423074b15c7bc999975f57",
+                "sha256:7161ec49ef0800947dc5570f86568a7bb36fa97dd09e9827dc02b718c5643f09",
+                "sha256:72d622d262e463dfb7595202d229f5f3ab4b852289a1cd09650362db23b9eb0b",
+                "sha256:74d28c17412d9caa1066f7a31df8403ec23d5268ba46cd0ad2c50fb82ae40462",
+                "sha256:78618cdbccaa74d3f88d0ad6cb8ac3007f1a6fa5c6f19af64b55ca170bfa1edf",
+                "sha256:793b4e24db2e8742ca6423d3fde8396db336698c55cd34b660663ee9e45ed37f",
+                "sha256:798232c92e7665fe82ac085f9d8e8ca98826f8e27859d9a96b41d519ecd2e49a",
+                "sha256:81d09caa7b27ef4e61cb7d8fbf1714f5aec1c6b6c5270ee53504981e6e9121ad",
+                "sha256:8ab74c06ffdab957d7670c2a5a6e1a70181cd10b727cd788c4dd9005b6a8acd9",
+                "sha256:8eb0908e954d093b02a543dc963984d6e99ad2b5e36503d8a0aaf040505f747d",
+                "sha256:90b9e29824800e90c84e4022dd5cc16eb2d9605ee13f05d47641eb183cd73d45",
+                "sha256:9797a6c8fe16f25749b371c02e2ade0efb51155e767a971c61734b1bf6293994",
+                "sha256:9d2455fbf44c914840c793e89aa82d0e1763a14253a000743719ae5946814b2d",
+                "sha256:9d3bea1c75f8c53ee4d505c3e67d8c158ad4df0d83170605b50b64025917f338",
+                "sha256:9e2ec1e921fd07c7cda7962bad283acc2f2a9ccc1b971ee4b216b75fad6f0463",
+                "sha256:9e91179a242bbc99be65e139e30690e081fe6cb91a8e77faf4c409653de39451",
+                "sha256:a0eaa93d054751ee9964afa21c06247779b90440ca41d184aeb5d410f20ff591",
+                "sha256:a2c405445c79c3f5a124573a051062300936b0281fee57637e706453e452746c",
+                "sha256:aa7e402ce11f0885305bfb6afb3434b3cd8f53b563ac065452d9d5654c7b86fd",
+                "sha256:aff76a55a8aa8364d25400a210a65ff59d0168e0b4285ba6bf2bd83cf675ba32",
+                "sha256:b09b86b27a064c9624d0a6c54da01c1beaf5b6cadfa609cf63789b1d08a797b9",
+                "sha256:b14f16f94cbc61215115b9b1236f9c18403c15dd3c52cf629072afa9d54c1cbf",
+                "sha256:b50811d664d392f02f7761621303eba9d1b056fb1868c8cdf4231279645c25f5",
+                "sha256:b7bc2176354defba3edc2b9a777744462da2f8e921fbaf61e52acb95bafa9828",
+                "sha256:c78e1b00a87ce43bb37642c0812315b411e856a905d58d597750eb79802aaaa3",
+                "sha256:c83341b89884e2b2e55886e8fbbf37c3fa5efd6c8907124aeb72f285ae5696e5",
+                "sha256:ca2870d5d10d8726a27396d3ca4cf7976cec0f3cb706debe88e3a5bd4610f7d2",
+                "sha256:ccce24b7ad89adb5a1e34a6ba96ac2530046763912806ad4c247356a8f33a67b",
+                "sha256:cd5e14fbf22a87321b24c88669aad3a51ec052eb145315b3da3b7e3cc105b9a2",
+                "sha256:ce49c67f4ea0609933d01c0731b34b8695a7a748d6c8d186f95e7d085d2fe475",
+                "sha256:d33891be6df59d93df4d846640f0e46f1a807339f09e79a8040bc887bdcd7ed3",
+                "sha256:d3b2348a78bc939b4fed6552abfd2e7988e0f81443ef3911a4b8498ca084f6eb",
+                "sha256:d886f5d353333b4771d21267c7ecc75b710f1a73d72d03ca06df49b09015a9ef",
+                "sha256:d93480005693d247f8346bc8ee28c72a2191bdf1f6b5db469c096c0c867ac015",
+                "sha256:dc1a390a82755a8c26c9964d457d4c9cbec5405896cba94cf51f36ea0d855002",
+                "sha256:dd78700f5788ae180b5ee8902c6aea5a5726bac7c364b202b4b3e3ba2d293170",
+                "sha256:e46f38133e5a060d46bd630faa4d9fa0202377495df1f068a8299fd78c84de84",
+                "sha256:e4b878386c4bf293578b48fc570b84ecfe477d3b77ba39a6e87150af77f40c57",
+                "sha256:f0d0591a0aeaefdaf9a5e545e7485f89910c977087e7de2b6c388aec32011e9f",
+                "sha256:fdcbb4068117dfd9ce0138d068ac512843c52295ed996ae6dd1faf537b6dbc27",
+                "sha256:ff61bfd9253c3915e6d41c651d5f962da23eda633cf02262990094a18a55371a"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==10.2.0"
+            "version": "==10.3.0"
         }
     },
     "develop": {
+        "backports.tarfile": {
+            "hashes": [
+                "sha256:73e0179647803d3726d82e76089d01d8549ceca9bace469953fcb4d97cf2d417",
+                "sha256:9c2ef9696cb73374f7164e17fc761389393ca76777036f5aad42e8b93fcd8009"
+            ],
+            "markers": "python_version < '3.12'",
+            "version": "==1.1.1"
+        },
         "build": {
             "hashes": [
-                "sha256:538aab1b64f9828977f84bc63ae570b060a8ed1be419e7870b8b4fc5e6ea553b",
-                "sha256:589bf99a67df7c9cf07ec0ac0e5e2ea5d4b37ac63301c4986d1acb126aa83f8f"
+                "sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d",
+                "sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==1.0.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.2.1"
         },
         "certifi": {
             "hashes": [
                 "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
                 "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
             "markers": "python_version >= '3.6'",
@@ -289,121 +298,137 @@
                 "sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==3.3.2"
         },
         "cryptography": {
             "hashes": [
-                "sha256:087887e55e0b9c8724cf05361357875adb5c20dec27e5816b653492980d20380",
-                "sha256:09a77e5b2e8ca732a19a90c5bca2d124621a1edb5438c5daa2d2738bfeb02589",
-                "sha256:130c0f77022b2b9c99d8cebcdd834d81705f61c68e91ddd614ce74c657f8b3ea",
-                "sha256:141e2aa5ba100d3788c0ad7919b288f89d1fe015878b9659b307c9ef867d3a65",
-                "sha256:28cb2c41f131a5758d6ba6a0504150d644054fd9f3203a1e8e8d7ac3aea7f73a",
-                "sha256:2f9f14185962e6a04ab32d1abe34eae8a9001569ee4edb64d2304bf0d65c53f3",
-                "sha256:320948ab49883557a256eab46149df79435a22d2fefd6a66fe6946f1b9d9d008",
-                "sha256:36d4b7c4be6411f58f60d9ce555a73df8406d484ba12a63549c88bd64f7967f1",
-                "sha256:3b15c678f27d66d247132cbf13df2f75255627bcc9b6a570f7d2fd08e8c081d2",
-                "sha256:3dbd37e14ce795b4af61b89b037d4bc157f2cb23e676fa16932185a04dfbf635",
-                "sha256:4383b47f45b14459cab66048d384614019965ba6c1a1a141f11b5a551cace1b2",
-                "sha256:44c95c0e96b3cb628e8452ec060413a49002a247b2b9938989e23a2c8291fc90",
-                "sha256:4b063d3413f853e056161eb0c7724822a9740ad3caa24b8424d776cebf98e7ee",
-                "sha256:52ed9ebf8ac602385126c9a2fe951db36f2cb0c2538d22971487f89d0de4065a",
-                "sha256:55d1580e2d7e17f45d19d3b12098e352f3a37fe86d380bf45846ef257054b242",
-                "sha256:5ef9bc3d046ce83c4bbf4c25e1e0547b9c441c01d30922d812e887dc5f125c12",
-                "sha256:5fa82a26f92871eca593b53359c12ad7949772462f887c35edaf36f87953c0e2",
-                "sha256:61321672b3ac7aade25c40449ccedbc6db72c7f5f0fdf34def5e2f8b51ca530d",
-                "sha256:701171f825dcab90969596ce2af253143b93b08f1a716d4b2a9d2db5084ef7be",
-                "sha256:841ec8af7a8491ac76ec5a9522226e287187a3107e12b7d686ad354bb78facee",
-                "sha256:8a06641fb07d4e8f6c7dda4fc3f8871d327803ab6542e33831c7ccfdcb4d0ad6",
-                "sha256:8e88bb9eafbf6a4014d55fb222e7360eef53e613215085e65a13290577394529",
-                "sha256:a00aee5d1b6c20620161984f8ab2ab69134466c51f58c052c11b076715e72929",
-                "sha256:a047682d324ba56e61b7ea7c7299d51e61fd3bca7dad2ccc39b72bd0118d60a1",
-                "sha256:a7ef8dd0bf2e1d0a27042b231a3baac6883cdd5557036f5e8df7139255feaac6",
-                "sha256:ad28cff53f60d99a928dfcf1e861e0b2ceb2bc1f08a074fdd601b314e1cc9e0a",
-                "sha256:b9097a208875fc7bbeb1286d0125d90bdfed961f61f214d3f5be62cd4ed8a446",
-                "sha256:b97fe7d7991c25e6a31e5d5e795986b18fbbb3107b873d5f3ae6dc9a103278e9",
-                "sha256:e0ec52ba3c7f1b7d813cd52649a5b3ef1fc0d433219dc8c93827c57eab6cf888",
-                "sha256:ea2c3ffb662fec8bbbfce5602e2c159ff097a4631d96235fcf0fb00e59e3ece4",
-                "sha256:fa3dec4ba8fb6e662770b74f62f1a0c7d4e37e25b58b2bf2c1be4c95372b4a33",
-                "sha256:fbeb725c9dc799a574518109336acccaf1303c30d45c075c665c0793c2f79a7f"
+                "sha256:00c0faa5b021457848d031ecff041262211cc1e2bce5f6e6e6c8108018f6b44a",
+                "sha256:073104df012fc815eed976cd7d0a386c8725d0d0947cf9c37f6c36a6c20feb1b",
+                "sha256:076c92b08dd1ab88108bc84545187e10d3693a9299c593f98c4ea195a0b0ead7",
+                "sha256:089aeb297ff89615934b22c7631448598495ffd775b7d540a55cfee35a677bf4",
+                "sha256:3b750279f3e7715df6f68050707a0cee7cbe81ba2eeb2f21d081bd205885ffed",
+                "sha256:43e521f21c2458038d72e8cdfd4d4d9f1d00906a7b6636c4272e35f650d1699b",
+                "sha256:4bdb39ecbf05626e4bfa1efd773bb10346af297af14fb3f4c7cb91a1d2f34a46",
+                "sha256:5967e3632f42b0c0f9dc2c9da88c79eabdda317860b246d1fbbde4a8bbbc3b44",
+                "sha256:65d529c31bd65d54ce6b926a01e1b66eacf770b7e87c0622516a840e400ec732",
+                "sha256:6981acac509cc9415344cb5bfea8130096ea6ebcc917e75503143a1e9e829160",
+                "sha256:81dbe47e28b703bc4711ac74a64ef8b758a0cf056ce81d08e39116ab4bc126fa",
+                "sha256:8b90c57b3cd6128e0863b894ce77bd36fcb5f430bf2377bc3678c2f56e232316",
+                "sha256:9184aff0856261ecb566a3eb26a05dfe13a292c85ce5c59b04e4aa09e5814187",
+                "sha256:945a43ebf036dd4b43ebfbbd6b0f2db29ad3d39df824fb77476ca5777a9dde33",
+                "sha256:97eeacae9aa526ddafe68b9202a535f581e21d78f16688a84c8dcc063618e121",
+                "sha256:9f1a3bc2747166b0643b00e0b56cd9b661afc9d5ff963acaac7a9c7b2b1ef638",
+                "sha256:9ff75b88a4d273c06d968ad535e6cb6a039dd32db54fe36f05ed62ac3ef64a44",
+                "sha256:aeb6f56b004e898df5530fa873e598ec78eb338ba35f6fa1449970800b1d97c2",
+                "sha256:b16b90605c62bcb3aa7755d62cf5e746828cfc3f965a65211849e00c46f8348d",
+                "sha256:b99831397fdc6e6e0aa088b060c278c6e635d25c0d4d14bdf045bf81792fda0a",
+                "sha256:bc954251edcd8a952eeaec8ae989fec7fe48109ab343138d537b7ea5bb41071a",
+                "sha256:c05230d8aaaa6b8ab3ab41394dc06eb3d916131df1c9dcb4c94e8f041f704b74",
+                "sha256:d16a310c770cc49908c500c2ceb011f2840674101a587d39fa3ea828915b7e83",
+                "sha256:d93080d2b01b292e7ee4d247bf93ed802b0100f5baa3fa5fd6d374716fa480d4",
+                "sha256:e1f5f15c5ddadf6ee4d1d624a2ae940f14bd74536230b0056ccb28bb6248e42a",
+                "sha256:e3442601d276bd9e961d618b799761b4e5d892f938e8a4fe1efbe2752be90455",
+                "sha256:e85f433230add2aa26b66d018e21134000067d210c9c68ef7544ba65fc52e3eb",
+                "sha256:eecca86813c6a923cabff284b82ff4d73d9e91241dc176250192c3a9b9902a54",
+                "sha256:f1e933b238978ccfa77b1fee0a297b3c04983f4cb84ae1c33b0ea4ae08266cc9",
+                "sha256:f4cece02478d73dacd52be57a521d168af64ae03d2a567c0c4eb6f189c3b9d79",
+                "sha256:f567a82b7c2b99257cca2a1c902c1b129787278ff67148f188784245c7ed5495",
+                "sha256:f987a244dfb0333fbd74a691c36000a2569eaf7c7cc2ac838f85f59f0588ddc9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==42.0.2"
+            "version": "==42.0.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
                 "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.20.1"
         },
         "exceptiongroup": {
             "hashes": [
-                "sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14",
-                "sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68"
+                "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad",
+                "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"
             ],
             "markers": "python_version < '3.11'",
-            "version": "==1.2.0"
+            "version": "==1.2.1"
         },
         "idna": {
             "hashes": [
-                "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca",
-                "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.6"
+            "version": "==3.7"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:4805911c3a4ec7c3966410053e9ec6a1fecd629117df5adee56dfc9432a1081e",
-                "sha256:f238736bb06590ae52ac1fab06a3a9ef1d8dce2b7a35b5ab329371d6c8f5d2cc"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==7.0.1"
+            "markers": "python_full_version < '3.10.2'",
+            "version": "==7.1.0"
         },
         "importlib-resources": {
             "hashes": [
-                "sha256:3893a00122eafde6894c59914446a512f728a0c1a45f9bb9b63721b6bacf0b4a",
-                "sha256:e8bf90d8213b486f428c9c39714b920041cb02c184686a3dee24905aaa8105d6"
+                "sha256:50d10f043df931902d4194ea07ec57960f66a80449ff867bfe782b4c486ba78c",
+                "sha256:cdb2b453b8046ca4e3798eb1d84f3cce1446a0e8e7b5ef4efb600f19fc398145"
             ],
             "markers": "python_version < '3.9'",
-            "version": "==6.1.1"
+            "version": "==6.4.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb",
-                "sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621"
+                "sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd",
+                "sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.4.0"
+        },
+        "jaraco.context": {
+            "hashes": [
+                "sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266",
+                "sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.3.0"
+            "version": "==5.3.0"
+        },
+        "jaraco.functools": {
+            "hashes": [
+                "sha256:3b24ccb921d6b593bdceb56ce14799204f473976e2a9d4b15b04d0f2c2326664",
+                "sha256:d33fa765374c0611b52f8b3a795f8900869aa88c84769d4d1746cd68fb28c3e8"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.1"
         },
         "jeepney": {
             "hashes": [
                 "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
                 "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
             ],
             "markers": "sys_platform == 'linux'",
             "version": "==0.8.0"
         },
         "keyring": {
             "hashes": [
-                "sha256:4446d35d636e6a10b8bce7caa66913dd9eca5fd222ca03a3d42c38608ac30836",
-                "sha256:e730ecffd309658a08ee82535a3b5ec4b4c8669a9be11efb66249d8e0aeb9a25"
+                "sha256:19f17d40335444aab84b19a0d16a77ec0758a9c384e3446ae2ed8bd6d53b67a5",
+                "sha256:7045f367268ce42dba44745050164b431e46f6e92f99ef2937dfadaef368d8cf"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==24.3.0"
+            "version": "==25.2.0"
         },
         "markdown-it-py": {
             "hashes": [
                 "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
                 "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
             "markers": "python_version >= '3.8'",
@@ -423,98 +448,98 @@
                 "sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==10.2.0"
         },
         "nh3": {
             "hashes": [
-                "sha256:0d02d0ff79dfd8208ed25a39c12cbda092388fff7f1662466e27d97ad011b770",
-                "sha256:3277481293b868b2715907310c7be0f1b9d10491d5adf9fce11756a97e97eddf",
-                "sha256:3b803a5875e7234907f7d64777dfde2b93db992376f3d6d7af7f3bc347deb305",
-                "sha256:427fecbb1031db085eaac9931362adf4a796428ef0163070c484b5a768e71601",
-                "sha256:5f0d77272ce6d34db6c87b4f894f037d55183d9518f948bba236fe81e2bb4e28",
-                "sha256:60684857cfa8fdbb74daa867e5cad3f0c9789415aba660614fe16cd66cbb9ec7",
-                "sha256:6f42f99f0cf6312e470b6c09e04da31f9abaadcd3eb591d7d1a88ea931dca7f3",
-                "sha256:86e447a63ca0b16318deb62498db4f76fc60699ce0a1231262880b38b6cff911",
-                "sha256:8d595df02413aa38586c24811237e95937ef18304e108b7e92c890a06793e3bf",
-                "sha256:9c0d415f6b7f2338f93035bba5c0d8c1b464e538bfbb1d598acd47d7969284f0",
-                "sha256:a5167a6403d19c515217b6bcaaa9be420974a6ac30e0da9e84d4fc67a5d474c5",
-                "sha256:ac19c0d68cd42ecd7ead91a3a032fdfff23d29302dbb1311e641a130dfefba97",
-                "sha256:b1e97221cedaf15a54f5243f2c5894bb12ca951ae4ddfd02a9d4ea9df9e1a29d",
-                "sha256:bc2d086fb540d0fa52ce35afaded4ea526b8fc4d3339f783db55c95de40ef02e",
-                "sha256:d1e30ff2d8d58fb2a14961f7aac1bbb1c51f9bdd7da727be35c63826060b0bf3",
-                "sha256:f3b53ba93bb7725acab1e030bc2ecd012a817040fd7851b332f86e2f9bb98dc6"
+                "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
+                "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
+                "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
+                "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
+                "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
+                "sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028",
+                "sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9",
+                "sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3",
+                "sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351",
+                "sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10",
+                "sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71",
+                "sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f",
+                "sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b",
+                "sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a",
+                "sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062",
+                "sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a"
             ],
-            "version": "==0.2.15"
+            "version": "==0.2.17"
         },
         "packaging": {
             "hashes": [
-                "sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5",
-                "sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.2"
+            "version": "==24.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
-                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
+                "sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297",
+                "sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.9.6"
+            "version": "==1.10.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981",
-                "sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be"
+                "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1",
+                "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==1.4.0"
+            "version": "==1.5.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f",
                 "sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
             "version": "==2.11.1"
         },
         "pycparser": {
             "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+                "sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6",
+                "sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.21"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.22"
         },
         "pygments": {
             "hashes": [
-                "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c",
-                "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
+                "sha256:786ff802f32e91311bff3889f6e9a86e81505fe99f2735bb6d60ae0c5004f199",
+                "sha256:b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.17.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.18.0"
         },
         "pyproject-hooks": {
             "hashes": [
-                "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
-                "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
+                "sha256:4b37730834edbd6bd37f26ece6b44802fb1c1ee2ece0e54ddff8bfc06db86965",
+                "sha256:7ceeefe9aec63a1064c18d939bdc3adf2d8aa1988a510afec15151578b232aa2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.0.0"
+            "version": "==1.1.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:249b1b0864530ba251b7438274c4d251c58d868edaaec8762893ad4a0d71c36c",
-                "sha256:50fb9cbe836c3f20f0dfa99c565201fb75dc54c8d76373cd1bde06b06657bdb6"
+                "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233",
+                "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.8'",
-            "version": "==8.0.0"
+            "version": "==8.2.0"
         },
         "pytest-datadir": {
             "hashes": [
                 "sha256:1617ed92f9afda0c877e4eac91904b5f779d24ba8f5e438752e3ae39d8d2ee3f",
                 "sha256:34adf361bcc7b37961bbc1dfa8d25a4829e778bab461703c38a5c50ca9c36dc8"
             ],
             "index": "pypi",
@@ -528,19 +553,19 @@
             ],
             "index": "pypi",
             "markers": "python_version >= '3.7'",
             "version": "==6.0.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:13d039515c1f24de668e2c93f2e877b9dbe6c6c32328b90a40a49d8b2b85f36d",
-                "sha256:2d55489f83be4992fe4454939d1a051c33edbab778e82761d060c9fc6b308cd1"
+                "sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311",
+                "sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==42.0"
+            "version": "==43.0"
         },
         "requests": {
             "hashes": [
                 "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
                 "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "markers": "python_version >= '3.7'",
@@ -560,19 +585,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa",
-                "sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235"
+                "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
+                "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.7.0"
+            "version": "==13.7.1"
         },
         "secretstorage": {
             "hashes": [
                 "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
                 "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
             ],
             "markers": "sys_platform == 'linux'",
@@ -584,40 +609,40 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "twine": {
             "hashes": [
-                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
-                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
+                "sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4",
+                "sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0"
             ],
             "index": "pypi",
-            "markers": "python_version >= '3.7'",
-            "version": "==4.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783",
-                "sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
             "markers": "python_version < '3.9'",
-            "version": "==4.9.0"
+            "version": "==4.11.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:051d961ad0c62a94e50ecf1af379c3aba230c66c710493493560c0c223c49f20",
-                "sha256:ce3711610ddce217e6d113a2732fafad960a03fd0318c91faa79481e35c11224"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==2.2.0"
+            "version": "==2.2.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31",
-                "sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==3.17.0"
+            "version": "==3.18.1"
         }
     }
 }
```

### Comparing `flackup-0.7.3/README.md` & `flackup-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/pyproject.toml` & `flackup-0.7.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Topic :: Multimedia :: Sound/Audio :: CD Audio",
     "Topic :: Multimedia :: Sound/Audio :: Conversion",
 ]
 dependencies = [
     "click ~= 8.1",
     "musicbrainzngs ~= 0.7",
     "mutagen ~= 1.47",
-    "pillow ~= 10.2",
+    "pillow ~= 10.3",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 flackup = "flackup.cli:flackup"
 
 [project.urls]
```

### Comparing `flackup-0.7.3/src/flackup/cli.py` & `flackup-0.7.4/src/flackup/cli.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/src/flackup/convert.py` & `flackup-0.7.4/src/flackup/convert.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/src/flackup/fileinfo.py` & `flackup-0.7.4/src/flackup/fileinfo.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/src/flackup/musicbrainz.py` & `flackup-0.7.4/src/flackup/musicbrainz.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/src/flackup.egg-info/PKG-INFO` & `flackup-0.7.4/src/flackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flackup
-Version: 0.7.3
+Version: 0.7.4
 Summary: FLAC CD Backup Manager
 Author-email: Alexander Dietrich <alexander@dietrich.cx>
 Project-URL: Homepage, https://codeberg.org/alxndr42/flackup
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click~=8.1
 Requires-Dist: musicbrainzngs~=0.7
 Requires-Dist: mutagen~=1.47
-Requires-Dist: pillow~=10.2
+Requires-Dist: pillow~=10.3
 
 # Flackup
 
 Flackup manages audio CD backups as single FLAC files with [embedded cue
 sheets][cuesheet], adds metadata from [MusicBrainz][] and converts albums to
 individual [Ogg Vorbis][] tracks.
```

### Comparing `flackup-0.7.3/src/flackup.egg-info/SOURCES.txt` & `flackup-0.7.4/src/flackup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_cli/tagged.flac` & `flackup-0.7.4/tests/test_cli/tagged.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_cli.py` & `flackup-0.7.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_convert/date_original.flac` & `flackup-0.7.4/tests/test_convert/date_original.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_convert/tagged.flac` & `flackup-0.7.4/tests/test_convert/tagged.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_convert.py` & `flackup-0.7.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_fileinfo/empty.flac` & `flackup-0.7.4/tests/test_fileinfo/empty.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_fileinfo/tagged.flac` & `flackup-0.7.4/tests/test_fileinfo/tagged.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_fileinfo/test.flac` & `flackup-0.7.4/tests/test_fileinfo/test.flac`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_fileinfo.py` & `flackup-0.7.4/tests/test_fileinfo.py`

 * *Files identical despite different names*

### Comparing `flackup-0.7.3/tests/test_musicbrainz.py` & `flackup-0.7.4/tests/test_musicbrainz.py`

 * *Files identical despite different names*

