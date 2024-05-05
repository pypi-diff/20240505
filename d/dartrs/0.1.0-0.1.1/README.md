# Comparing `tmp/dartrs-0.1.0.tar.gz` & `tmp/dartrs-0.1.1.tar.gz`

## Comparing `dartrs-0.1.0.tar` & `dartrs-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.0/Cargo.toml
--rw-r--r--   0        0        0     4359 2024-05-05 06:18:46.000000 dartrs-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      470 2024-05-02 08:58:01.000000 dartrs-0.1.0/.gitignore
--rw-r--r--   0        0        0      153 2024-05-02 09:34:08.000000 dartrs-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0    11357 2024-04-29 15:26:29.000000 dartrs-0.1.0/LICENSE
--rw-r--r--   0        0        0       31 2024-05-04 13:40:31.000000 dartrs-0.1.0/README.md
--rw-r--r--   0        0        0     1704 2024-05-05 06:08:45.000000 dartrs-0.1.0/examples/main.py
--rw-r--r--   0        0        0     4874 2024-05-02 08:40:41.000000 dartrs-0.1.0/pdm.lock
--rw-r--r--   0        0        0      113 2024-05-03 10:16:31.000000 dartrs-0.1.0/python/dartrs/__init__.py
--rw-r--r--   0        0        0     2404 2024-05-05 06:08:52.000000 dartrs-0.1.0/python/dartrs/dartrs.pyi
--rw-r--r--   0        0        0        0 2024-05-02 09:24:39.000000 dartrs-0.1.0/python/dartrs/py.typed
--rw-r--r--   0        0        0      693 2024-05-04 14:20:55.000000 dartrs-0.1.0/python/dartrs/utils.py
--rw-r--r--   0        0        0     2565 2024-05-05 06:08:05.000000 dartrs-0.1.0/python/dartrs/v2.py
--rw-r--r--   0        0        0     1537 2024-05-04 14:10:46.000000 dartrs-0.1.0/src/bindings/generation.rs
--rw-r--r--   0        0        0     5946 2024-05-03 12:53:24.000000 dartrs-0.1.0/src/bindings/models.rs
--rw-r--r--   0        0        0      907 2024-05-03 13:21:02.000000 dartrs-0.1.0/src/bindings/prompt.rs
--rw-r--r--   0        0        0     6881 2024-05-04 07:36:20.000000 dartrs-0.1.0/src/bindings/tags.rs
--rw-r--r--   0        0        0       94 2024-05-03 13:11:21.000000 dartrs-0.1.0/src/bindings.rs
--rw-r--r--   0        0        0     1587 2024-05-03 12:50:43.000000 dartrs-0.1.0/src/configs.rs
--rw-r--r--   0        0        0     8784 2024-05-04 13:26:21.000000 dartrs-0.1.0/src/generation.rs
--rw-r--r--   0        0        0      790 2024-05-03 13:20:55.000000 dartrs-0.1.0/src/lib.rs
--rw-r--r--   0        0        0    12661 2024-05-03 12:37:06.000000 dartrs-0.1.0/src/models/mistral.rs
--rw-r--r--   0        0        0    17489 2024-05-03 12:36:45.000000 dartrs-0.1.0/src/models/mixtral.rs
--rw-r--r--   0        0        0     3446 2024-05-03 12:51:12.000000 dartrs-0.1.0/src/models.rs
--rw-r--r--   0        0        0     1404 2024-05-03 13:09:55.000000 dartrs-0.1.0/src/prompt.rs
--rw-r--r--   0        0        0     5702 2024-05-04 15:23:42.000000 dartrs-0.1.0/src/tags.rs
--rw-r--r--   0        0        0        0 2024-05-02 08:36:22.000000 dartrs-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-03 13:31:47.000000 dartrs-0.1.0/tests/test_configs.py
--rw-r--r--   0        0        0     4555 2024-05-03 14:21:39.000000 dartrs-0.1.0/tests/test_model.py
--rw-r--r--   0        0        0     1342 2024-05-03 14:23:30.000000 dartrs-0.1.0/tests/test_prompt.py
--rw-r--r--   0        0        0    50585 2024-05-05 04:13:01.000000 dartrs-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      688 2024-05-03 10:53:31.000000 dartrs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 dartrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 dartrs-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     4367 2024-05-05 06:39:52.000000 dartrs-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      470 2024-05-05 06:39:52.000000 dartrs-0.1.1/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-05-05 06:39:52.000000 dartrs-0.1.1/LICENSE
+-rw-r--r--   0     1001      127       28 2024-05-05 06:39:52.000000 dartrs-0.1.1/README.md
+-rw-r--r--   0     1001      127     1632 2024-05-05 06:39:52.000000 dartrs-0.1.1/examples/main.py
+-rw-r--r--   0     1001      127     4742 2024-05-05 06:39:52.000000 dartrs-0.1.1/pdm.lock
+-rw-r--r--   0     1001      127      108 2024-05-05 06:39:52.000000 dartrs-0.1.1/python/dartrs/__init__.py
+-rw-r--r--   0     1001      127     2304 2024-05-05 06:39:52.000000 dartrs-0.1.1/python/dartrs/dartrs.pyi
+-rw-r--r--   0     1001      127        0 2024-05-05 06:39:52.000000 dartrs-0.1.1/python/dartrs/py.typed
+-rw-r--r--   0     1001      127      668 2024-05-05 06:39:52.000000 dartrs-0.1.1/python/dartrs/utils.py
+-rw-r--r--   0     1001      127     2473 2024-05-05 06:39:52.000000 dartrs-0.1.1/python/dartrs/v2.py
+-rw-r--r--   0     1001      127     1537 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/bindings/generation.rs
+-rw-r--r--   0     1001      127     5946 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/bindings/models.rs
+-rw-r--r--   0     1001      127      875 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/bindings/prompt.rs
+-rw-r--r--   0     1001      127     6661 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/bindings/tags.rs
+-rw-r--r--   0     1001      127       94 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/bindings.rs
+-rw-r--r--   0     1001      127     1587 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/configs.rs
+-rw-r--r--   0     1001      127     8784 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/generation.rs
+-rw-r--r--   0     1001      127      790 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127    12295 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/models/mistral.rs
+-rw-r--r--   0     1001      127    17025 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     3446 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/models.rs
+-rw-r--r--   0     1001      127     1404 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/prompt.rs
+-rw-r--r--   0     1001      127     5702 2024-05-05 06:39:52.000000 dartrs-0.1.1/src/tags.rs
+-rw-r--r--   0     1001      127        0 2024-05-05 06:39:52.000000 dartrs-0.1.1/tests/__init__.py
+-rw-r--r--   0     1001      127     1117 2024-05-05 06:39:52.000000 dartrs-0.1.1/tests/test_configs.py
+-rw-r--r--   0     1001      127     4353 2024-05-05 06:39:52.000000 dartrs-0.1.1/tests/test_model.py
+-rw-r--r--   0     1001      127     1299 2024-05-05 06:39:52.000000 dartrs-0.1.1/tests/test_prompt.py
+-rw-r--r--   0     1001      127    52911 2024-05-05 06:40:05.000000 dartrs-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      127      662 2024-05-05 06:39:52.000000 dartrs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 dartrs-0.1.1/PKG-INFO
```

### Comparing `dartrs-0.1.0/Cargo.toml` & `dartrs-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dartrs"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "dartrs"
 crate-type = ["cdylib", "lib"]
```

### Comparing `dartrs-0.1.0/.github/workflows/CI.yml` & `dartrs-0.1.1/.github/workflows/CI.yml`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     environment: publishing
     if: startsWith(github.ref, 'refs/tags/')
-    needs: [linux, windows, macos, sdist]
+    needs: [linux, linux2, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
```

### Comparing `dartrs-0.1.0/LICENSE` & `dartrs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/examples/main.py` & `dartrs-0.1.1/examples/main.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from dartrs.dartrs import DartDevice, DartTokenizer, GenerationConfig
-from dartrs.utils import get_generation_config
-from dartrs.v2 import (
-    compose_prompt,
-    MixtralModel,
-    V2Model,
-)
-import time
-
-MODEL_NAME = "p1atdev/dart-v2-mixtral-160m-sft-8"
-
-
-def prepare_models():
-    model = MixtralModel.from_pretrained(MODEL_NAME)
-    tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
-
-    return model, tokenizer
-
-
-def generate(model: V2Model, config: GenerationConfig):
-    start = time.time()
-    output = model.generate(config)
-    end = time.time()
-
-    print(output)
-    print(f"Time taken: {end - start:.2f}s")
-
-
-def main():
-    model, tokenizer = prepare_models()
-
-    # generate 5 times
-    generate(
-        model,
-        get_generation_config(
-            prompt=compose_prompt(
-                copyright="",
-                character="",
-                rating="<|rating:general|>",
-                aspect_ratio="<|aspect_ratio:tall|>",
-                length="<|length:medium|>",
-                identity="<|identity:none|>",
-                prompt="1girl, cat ears",
-            ),
-            tokenizer=tokenizer,
-            seed=42,
-        ),
-    )
-    generate(
-        model,
-        get_generation_config(
-            prompt=compose_prompt(
-                prompt="2girls",
-            ),
-            tokenizer=tokenizer,
-            seed=999999,
-        ),
-    )
-
-    generate(
-        model,
-        get_generation_config(
-            prompt=compose_prompt(
-                prompt="1girl, solo",
-            ),
-            tokenizer=tokenizer,
-        ),
-    )
-
-
-if __name__ == "__main__":
-    main()
+from dartrs.dartrs import DartDevice, DartTokenizer, GenerationConfig
+from dartrs.utils import get_generation_config
+from dartrs.v2 import (
+    compose_prompt,
+    MixtralModel,
+    V2Model,
+)
+import time
+
+MODEL_NAME = "p1atdev/dart-v2-mixtral-160m-sft-8"
+
+
+def prepare_models():
+    model = MixtralModel.from_pretrained(MODEL_NAME)
+    tokenizer = DartTokenizer.from_pretrained(MODEL_NAME)
+
+    return model, tokenizer
+
+
+def generate(model: V2Model, config: GenerationConfig):
+    start = time.time()
+    output = model.generate(config)
+    end = time.time()
+
+    print(output)
+    print(f"Time taken: {end - start:.2f}s")
+
+
+def main():
+    model, tokenizer = prepare_models()
+
+    # generate 5 times
+    generate(
+        model,
+        get_generation_config(
+            prompt=compose_prompt(
+                copyright="",
+                character="",
+                rating="<|rating:general|>",
+                aspect_ratio="<|aspect_ratio:tall|>",
+                length="<|length:medium|>",
+                identity="<|identity:none|>",
+                prompt="1girl, cat ears",
+            ),
+            tokenizer=tokenizer,
+            seed=42,
+        ),
+    )
+    generate(
+        model,
+        get_generation_config(
+            prompt=compose_prompt(
+                prompt="2girls",
+            ),
+            tokenizer=tokenizer,
+            seed=999999,
+        ),
+    )
+
+    generate(
+        model,
+        get_generation_config(
+            prompt=compose_prompt(
+                prompt="1girl, solo",
+            ),
+            tokenizer=tokenizer,
+        ),
+    )
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dartrs-0.1.0/pdm.lock` & `dartrs-0.1.1/pdm.lock`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-# This file is @generated by PDM.
-# It is not intended for manual editing.
-
-[metadata]
-groups = ["default", "dev"]
-strategy = ["cross_platform", "inherit_metadata"]
-lock_version = "4.4.1"
-content_hash = "sha256:8fdb3da9aa93523114be19d2c9eb41ff6576de331d4b0746aa084d3a0ee1f9b7"
-
-[[package]]
-name = "colorama"
-version = "0.4.6"
-requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
-summary = "Cross-platform colored terminal text."
-groups = ["dev"]
-marker = "sys_platform == \"win32\""
-files = [
-    {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
-    {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
-]
-
-[[package]]
-name = "exceptiongroup"
-version = "1.2.1"
-requires_python = ">=3.7"
-summary = "Backport of PEP 654 (exception groups)"
-groups = ["dev"]
-marker = "python_version < \"3.11\""
-files = [
-    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
-    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
-]
-
-[[package]]
-name = "icdiff"
-version = "2.0.7"
-summary = "improved colored diff"
-groups = ["dev"]
-files = [
-    {file = "icdiff-2.0.7-py3-none-any.whl", hash = "sha256:f05d1b3623223dd1c70f7848da7d699de3d9a2550b902a8234d9026292fb5762"},
-    {file = "icdiff-2.0.7.tar.gz", hash = "sha256:f79a318891adbf59a45e3a7694f5e1f18c5407065264637072ac8363b759866f"},
-]
-
-[[package]]
-name = "iniconfig"
-version = "2.0.0"
-requires_python = ">=3.7"
-summary = "brain-dead simple config-ini parsing"
-groups = ["dev"]
-files = [
-    {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
-    {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
-]
-
-[[package]]
-name = "packaging"
-version = "24.0"
-requires_python = ">=3.7"
-summary = "Core utilities for Python packages"
-groups = ["dev"]
-files = [
-    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
-    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
-]
-
-[[package]]
-name = "pluggy"
-version = "1.5.0"
-requires_python = ">=3.8"
-summary = "plugin and hook calling mechanisms for python"
-groups = ["dev"]
-files = [
-    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
-    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
-]
-
-[[package]]
-name = "pprintpp"
-version = "0.4.0"
-summary = "A drop-in replacement for pprint that's actually pretty"
-groups = ["dev"]
-files = [
-    {file = "pprintpp-0.4.0-py2.py3-none-any.whl", hash = "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d"},
-    {file = "pprintpp-0.4.0.tar.gz", hash = "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"},
-]
-
-[[package]]
-name = "pytest"
-version = "8.2.0"
-requires_python = ">=3.8"
-summary = "pytest: simple powerful testing with Python"
-groups = ["dev"]
-dependencies = [
-    "colorama; sys_platform == \"win32\"",
-    "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
-    "iniconfig",
-    "packaging",
-    "pluggy<2.0,>=1.5",
-    "tomli>=1; python_version < \"3.11\"",
-]
-files = [
-    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
-    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
-]
-
-[[package]]
-name = "pytest-icdiff"
-version = "0.9"
-requires_python = ">=3.7"
-summary = "use icdiff for better error messages in pytest assertions"
-groups = ["dev"]
-dependencies = [
-    "icdiff",
-    "pprintpp",
-    "pytest",
-]
-files = [
-    {file = "pytest-icdiff-0.9.tar.gz", hash = "sha256:13aede616202e57fcc882568b64589002ef85438046f012ac30a8d959dac8b75"},
-    {file = "pytest_icdiff-0.9-py3-none-any.whl", hash = "sha256:efee0da3bd1b24ef2d923751c5c547fbb8df0a46795553fba08ef57c3ca03d82"},
-]
-
-[[package]]
-name = "tomli"
-version = "2.0.1"
-requires_python = ">=3.7"
-summary = "A lil' TOML parser"
-groups = ["dev"]
-marker = "python_version < \"3.11\""
-files = [
-    {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
-    {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
-]
+# This file is @generated by PDM.
+# It is not intended for manual editing.
+
+[metadata]
+groups = ["default", "dev"]
+strategy = ["cross_platform", "inherit_metadata"]
+lock_version = "4.4.1"
+content_hash = "sha256:8fdb3da9aa93523114be19d2c9eb41ff6576de331d4b0746aa084d3a0ee1f9b7"
+
+[[package]]
+name = "colorama"
+version = "0.4.6"
+requires_python = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
+summary = "Cross-platform colored terminal text."
+groups = ["dev"]
+marker = "sys_platform == \"win32\""
+files = [
+    {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
+    {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
+]
+
+[[package]]
+name = "exceptiongroup"
+version = "1.2.1"
+requires_python = ">=3.7"
+summary = "Backport of PEP 654 (exception groups)"
+groups = ["dev"]
+marker = "python_version < \"3.11\""
+files = [
+    {file = "exceptiongroup-1.2.1-py3-none-any.whl", hash = "sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad"},
+    {file = "exceptiongroup-1.2.1.tar.gz", hash = "sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16"},
+]
+
+[[package]]
+name = "icdiff"
+version = "2.0.7"
+summary = "improved colored diff"
+groups = ["dev"]
+files = [
+    {file = "icdiff-2.0.7-py3-none-any.whl", hash = "sha256:f05d1b3623223dd1c70f7848da7d699de3d9a2550b902a8234d9026292fb5762"},
+    {file = "icdiff-2.0.7.tar.gz", hash = "sha256:f79a318891adbf59a45e3a7694f5e1f18c5407065264637072ac8363b759866f"},
+]
+
+[[package]]
+name = "iniconfig"
+version = "2.0.0"
+requires_python = ">=3.7"
+summary = "brain-dead simple config-ini parsing"
+groups = ["dev"]
+files = [
+    {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
+    {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
+]
+
+[[package]]
+name = "packaging"
+version = "24.0"
+requires_python = ">=3.7"
+summary = "Core utilities for Python packages"
+groups = ["dev"]
+files = [
+    {file = "packaging-24.0-py3-none-any.whl", hash = "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5"},
+    {file = "packaging-24.0.tar.gz", hash = "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"},
+]
+
+[[package]]
+name = "pluggy"
+version = "1.5.0"
+requires_python = ">=3.8"
+summary = "plugin and hook calling mechanisms for python"
+groups = ["dev"]
+files = [
+    {file = "pluggy-1.5.0-py3-none-any.whl", hash = "sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669"},
+    {file = "pluggy-1.5.0.tar.gz", hash = "sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1"},
+]
+
+[[package]]
+name = "pprintpp"
+version = "0.4.0"
+summary = "A drop-in replacement for pprint that's actually pretty"
+groups = ["dev"]
+files = [
+    {file = "pprintpp-0.4.0-py2.py3-none-any.whl", hash = "sha256:b6b4dcdd0c0c0d75e4d7b2f21a9e933e5b2ce62b26e1a54537f9651ae5a5c01d"},
+    {file = "pprintpp-0.4.0.tar.gz", hash = "sha256:ea826108e2c7f49dc6d66c752973c3fc9749142a798d6b254e1e301cfdbc6403"},
+]
+
+[[package]]
+name = "pytest"
+version = "8.2.0"
+requires_python = ">=3.8"
+summary = "pytest: simple powerful testing with Python"
+groups = ["dev"]
+dependencies = [
+    "colorama; sys_platform == \"win32\"",
+    "exceptiongroup>=1.0.0rc8; python_version < \"3.11\"",
+    "iniconfig",
+    "packaging",
+    "pluggy<2.0,>=1.5",
+    "tomli>=1; python_version < \"3.11\"",
+]
+files = [
+    {file = "pytest-8.2.0-py3-none-any.whl", hash = "sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233"},
+    {file = "pytest-8.2.0.tar.gz", hash = "sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f"},
+]
+
+[[package]]
+name = "pytest-icdiff"
+version = "0.9"
+requires_python = ">=3.7"
+summary = "use icdiff for better error messages in pytest assertions"
+groups = ["dev"]
+dependencies = [
+    "icdiff",
+    "pprintpp",
+    "pytest",
+]
+files = [
+    {file = "pytest-icdiff-0.9.tar.gz", hash = "sha256:13aede616202e57fcc882568b64589002ef85438046f012ac30a8d959dac8b75"},
+    {file = "pytest_icdiff-0.9-py3-none-any.whl", hash = "sha256:efee0da3bd1b24ef2d923751c5c547fbb8df0a46795553fba08ef57c3ca03d82"},
+]
+
+[[package]]
+name = "tomli"
+version = "2.0.1"
+requires_python = ">=3.7"
+summary = "A lil' TOML parser"
+groups = ["dev"]
+marker = "python_version < \"3.11\""
+files = [
+    {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
+    {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
+]
```

### Comparing `dartrs-0.1.0/python/dartrs/utils.py` & `dartrs-0.1.1/python/dartrs/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from . import dartrs
-
-
-def get_generation_config(
-    prompt: str,
-    tokenizer: dartrs.DartTokenizer,
-    device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
-    eos_token: str | None = None,
-    max_new_tokens: int | None = 256,
-    temperature: float | None = 1.0,
-    top_p: float | None = 1.0,
-    top_k: int | None = 100,
-    seed: int | None = None,
-) -> dartrs.GenerationConfig:
-    return dartrs.GenerationConfig(
-        device=device,
-        tokenizer=tokenizer,
-        prompt=prompt,
-        eos_token=eos_token,
-        max_new_tokens=max_new_tokens,
-        temperature=temperature,
-        top_p=top_p,
-        top_k=top_k,
-        seed=seed,
-    )
+from . import dartrs
+
+
+def get_generation_config(
+    prompt: str,
+    tokenizer: dartrs.DartTokenizer,
+    device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
+    eos_token: str | None = None,
+    max_new_tokens: int | None = 256,
+    temperature: float | None = 1.0,
+    top_p: float | None = 1.0,
+    top_k: int | None = 100,
+    seed: int | None = None,
+) -> dartrs.GenerationConfig:
+    return dartrs.GenerationConfig(
+        device=device,
+        tokenizer=tokenizer,
+        prompt=prompt,
+        eos_token=eos_token,
+        max_new_tokens=max_new_tokens,
+        temperature=temperature,
+        top_p=top_p,
+        top_k=top_k,
+        seed=seed,
+    )
```

### Comparing `dartrs-0.1.0/python/dartrs/v2.py` & `dartrs-0.1.1/python/dartrs/v2.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from typing import Literal
-
-from . import dartrs
-
-
-LengthTag = (
-    Literal["<|length:very_short|>"]
-    | Literal["<|length:short|>"]
-    | Literal["<|length:medium|>"]
-    | Literal["<|length:long|>"]
-    | Literal["<|length:very_long|>"]
-)
-
-AspectRatioTag = (
-    Literal["<|aspect_ratio:ultra_wide|>"]
-    | Literal["<|aspect_ratio:wide|>"]
-    | Literal["<|aspect_ratio:square|>"]
-    | Literal["<|aspect_ratio:tall|>"]
-    | Literal["<|aspect_ratio:ultra_tall|>"]
-)
-
-RatingTag = (
-    Literal["<|rating:sfw|>"]
-    | Literal["<|rating:general|>"]
-    | Literal["<|rating:sensitive|>"]
-    | Literal["<|rating:nsfw|>"]
-    | Literal["<|rating:questionable|>"]
-    | Literal["<|rating:explicit|>"]
-)
-
-IdentityTag = (
-    Literal["<|identity:none|>"]
-    | Literal["<|identity:lax|>"]
-    | Literal["<|identity:strict|>"]
-)
-
-
-def compose_prompt(
-    prompt: str = "",
-    copyright: str = "",
-    character: str = "",
-    rating: RatingTag = "<|rating:general|>",
-    aspect_ratio: AspectRatioTag = "<|aspect_ratio:tall|>",
-    length: LengthTag = "<|length:medium|>",
-    identity: IdentityTag = "<|identity:none|>",
-):
-    return dartrs.compose_prompt_v2(
-        copyright=copyright,
-        character=character,
-        rating=dartrs.RatingTag(rating),
-        aspect_ratio=dartrs.AspectRatioTag(aspect_ratio),
-        length=dartrs.LengthTag(length),
-        identity_level=dartrs.IdentityTag(identity),
-        prompt=prompt,
-    )
-
-
-class V2Model:
-    model: dartrs.DartV2Mistral | dartrs.DartV2Mixtral
-
-    def __init__(
-        self,
-        model: dartrs.DartV2Mistral | dartrs.DartV2Mixtral,
-    ) -> None:
-        self.model = model
-
-    def generate(self, config: dartrs.GenerationConfig) -> str:
-        return self.model.generate(config)
-
-
-class MixtralModel(V2Model):
-    @classmethod
-    def from_pretrained(
-        cls,
-        hub_name: str,
-        revision: str | None = None,
-        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
-        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
-    ) -> V2Model:
-        return cls(dartrs.DartV2Mixtral(hub_name, revision, dtype, device))
-
-
-class MistralModel(V2Model):
-    @classmethod
-    def from_pretrained(
-        cls,
-        hub_name: str,
-        revision: str | None = None,
-        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
-        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
-    ) -> V2Model:
-        return cls(dartrs.DartV2Mistral(hub_name, revision, dtype, device))
+from typing import Literal
+
+from . import dartrs
+
+
+LengthTag = (
+    Literal["<|length:very_short|>"]
+    | Literal["<|length:short|>"]
+    | Literal["<|length:medium|>"]
+    | Literal["<|length:long|>"]
+    | Literal["<|length:very_long|>"]
+)
+
+AspectRatioTag = (
+    Literal["<|aspect_ratio:ultra_wide|>"]
+    | Literal["<|aspect_ratio:wide|>"]
+    | Literal["<|aspect_ratio:square|>"]
+    | Literal["<|aspect_ratio:tall|>"]
+    | Literal["<|aspect_ratio:ultra_tall|>"]
+)
+
+RatingTag = (
+    Literal["<|rating:sfw|>"]
+    | Literal["<|rating:general|>"]
+    | Literal["<|rating:sensitive|>"]
+    | Literal["<|rating:nsfw|>"]
+    | Literal["<|rating:questionable|>"]
+    | Literal["<|rating:explicit|>"]
+)
+
+IdentityTag = (
+    Literal["<|identity:none|>"]
+    | Literal["<|identity:lax|>"]
+    | Literal["<|identity:strict|>"]
+)
+
+
+def compose_prompt(
+    prompt: str = "",
+    copyright: str = "",
+    character: str = "",
+    rating: RatingTag = "<|rating:general|>",
+    aspect_ratio: AspectRatioTag = "<|aspect_ratio:tall|>",
+    length: LengthTag = "<|length:medium|>",
+    identity: IdentityTag = "<|identity:none|>",
+):
+    return dartrs.compose_prompt_v2(
+        copyright=copyright,
+        character=character,
+        rating=dartrs.RatingTag(rating),
+        aspect_ratio=dartrs.AspectRatioTag(aspect_ratio),
+        length=dartrs.LengthTag(length),
+        identity_level=dartrs.IdentityTag(identity),
+        prompt=prompt,
+    )
+
+
+class V2Model:
+    model: dartrs.DartV2Mistral | dartrs.DartV2Mixtral
+
+    def __init__(
+        self,
+        model: dartrs.DartV2Mistral | dartrs.DartV2Mixtral,
+    ) -> None:
+        self.model = model
+
+    def generate(self, config: dartrs.GenerationConfig) -> str:
+        return self.model.generate(config)
+
+
+class MixtralModel(V2Model):
+    @classmethod
+    def from_pretrained(
+        cls,
+        hub_name: str,
+        revision: str | None = None,
+        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
+        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
+    ) -> V2Model:
+        return cls(dartrs.DartV2Mixtral(hub_name, revision, dtype, device))
+
+
+class MistralModel(V2Model):
+    @classmethod
+    def from_pretrained(
+        cls,
+        hub_name: str,
+        revision: str | None = None,
+        dtype: dartrs.DartDType = dartrs.DartDType.FP32,
+        device: dartrs.DartDevice = dartrs.DartDevice.Cpu(),
+    ) -> V2Model:
+        return cls(dartrs.DartV2Mistral(hub_name, revision, dtype, device))
```

### Comparing `dartrs-0.1.0/src/bindings/generation.rs` & `dartrs-0.1.1/src/bindings/generation.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/bindings/models.rs` & `dartrs-0.1.1/src/bindings/models.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/bindings/prompt.rs` & `dartrs-0.1.1/src/prompt.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,56 @@
-use crate::bindings::tags::{DartAspectRatioTag, DartIdentityTag, DartLengthTag, DartRatingTag};
-use crate::prompt::compose_prompt_v2;
-
-use crate::tags::{AspectRatioTag, IdentityTag, LengthTag, RatingTag};
-
-use pyo3::prelude::*;
-
-#[pyfunction(name = "compose_prompt_v2")]
-pub fn dart_compose_prompt_v2(
-    copyright: &str,
-    character: &str,
-    rating: DartRatingTag,
-    aspect_ratio: DartAspectRatioTag,
-    length: DartLengthTag,
-    identity_level: DartIdentityTag,
-    prompt: &str,
-) -> String {
-    let rating = RatingTag::from(rating);
-    let aspect_ratio = AspectRatioTag::from(aspect_ratio);
-    let length = LengthTag::from(length);
-    let identity_level = IdentityTag::from(identity_level);
-
-    compose_prompt_v2(
-        &copyright,
-        &character,
-        rating,
-        aspect_ratio,
-        length,
-        identity_level,
-        &prompt,
-    )
-}
+use crate::tags::ReservedTag::{
+    Bos, CharacterEnd, CharacterStart, CopyrightEnd, CopyrightStart, GeneralStart, InputEnd,
+};
+use crate::tags::{AspectRatioTag, IdentityTag, LengthTag, RatingTag, SpecialTag};
+
+pub fn compose_prompt_v2(
+    copyright: &str,
+    character: &str,
+    rating: RatingTag,
+    aspect_ratio: AspectRatioTag,
+    length: LengthTag,
+    identity_level: IdentityTag,
+    prompt: &str,
+) -> String {
+    let rating = rating.to_tag();
+    let aspect_ratio = aspect_ratio.to_tag();
+    let length = length.to_tag();
+    let identity_level = identity_level.to_tag();
+
+    format!(
+        "\
+{Bos}\
+{CopyrightStart}{copyright}{CopyrightEnd}\
+{CharacterStart}{character}{CharacterEnd}\
+{rating}{aspect_ratio}{length}\
+{GeneralStart}{prompt}{identity_level}{InputEnd}"
+    )
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_compose_prompt() {
+        let prompt = compose_prompt_v2(
+            "vocaloid",
+            "hatsune miku",
+            RatingTag::Sfw,
+            AspectRatioTag::Tall,
+            LengthTag::Long,
+            IdentityTag::None,
+            "1girl, blue hair",
+        );
+
+        assert_eq!(
+            prompt,
+            r"\
+<|bos|>\
+<copyright>vocaloid</copyright>\
+<character>hatsune miku</character>\
+<|rating:sfw|><|aspect_ratio:tall|><|length:long|>\
+<general>1girl, blue hair<|identity:none|><|input_end|>"
+        )
+    }
+}
```

### Comparing `dartrs-0.1.0/src/bindings/tags.rs` & `dartrs-0.1.1/src/bindings/tags.rs`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-use crate::tags::{AspectRatioTag, IdentityTag, LengthTag, RatingTag, ReservedTag, SpecialTag};
-
-use pyo3::exceptions;
-use pyo3::prelude::*;
-
-#[pyclass(name = "LengthTag")]
-#[derive(Debug, Clone)]
-pub enum DartLengthTag {
-    VeryShort,
-    Short,
-    Medium,
-    Long,
-    VeryLong,
-}
-
-impl From<DartLengthTag> for LengthTag {
-    fn from(tag: DartLengthTag) -> Self {
-        match tag {
-            DartLengthTag::VeryShort => LengthTag::VeryShort,
-            DartLengthTag::Short => LengthTag::Short,
-            DartLengthTag::Medium => LengthTag::Medium,
-            DartLengthTag::Long => LengthTag::Long,
-            DartLengthTag::VeryLong => LengthTag::VeryLong,
-        }
-    }
-}
-
-#[pymethods]
-impl DartLengthTag {
-    #[new]
-    fn new(tag: &str) -> PyResult<Self> {
-        match tag {
-            "<|length:very_short|>" => Ok(DartLengthTag::VeryShort),
-            "<|length:short|>" => Ok(DartLengthTag::Short),
-            "<|length:medium|>" => Ok(DartLengthTag::Medium),
-            "<|length:long|>" => Ok(DartLengthTag::Long),
-            "<|length:very_long|>" => Ok(DartLengthTag::VeryLong),
-            _ => Err(exceptions::PyValueError::new_err("invalid length tag")),
-        }
-    }
-
-    fn to_tag(&self) -> String {
-        LengthTag::from(self.clone()).to_tag()
-    }
-}
-
-#[pyclass(name = "AspectRatioTag")]
-#[derive(Debug, Clone)]
-pub enum DartAspectRatioTag {
-    UltraWide,
-    Wide,
-    Square,
-    Tall,
-    UltraTall,
-}
-
-impl From<DartAspectRatioTag> for AspectRatioTag {
-    fn from(tag: DartAspectRatioTag) -> Self {
-        match tag {
-            DartAspectRatioTag::UltraWide => AspectRatioTag::UltraWide,
-            DartAspectRatioTag::Wide => AspectRatioTag::Wide,
-            DartAspectRatioTag::Square => AspectRatioTag::Square,
-            DartAspectRatioTag::Tall => AspectRatioTag::Tall,
-            DartAspectRatioTag::UltraTall => AspectRatioTag::UltraTall,
-        }
-    }
-}
-
-#[pymethods]
-impl DartAspectRatioTag {
-    #[new]
-    fn new(tag: &str) -> PyResult<Self> {
-        match tag {
-            "<|aspect_ratio:ultra_wide|>" => Ok(DartAspectRatioTag::UltraWide),
-            "<|aspect_ratio:wide|>" => Ok(DartAspectRatioTag::Wide),
-            "<|aspect_ratio:square|>" => Ok(DartAspectRatioTag::Square),
-            "<|aspect_ratio:tall|>" => Ok(DartAspectRatioTag::Tall),
-            "<|aspect_ratio:ultra_tall|>" => Ok(DartAspectRatioTag::UltraTall),
-            _ => Err(exceptions::PyValueError::new_err(
-                "invalid aspect ratio tag",
-            )),
-        }
-    }
-
-    fn to_tag(&self) -> String {
-        AspectRatioTag::from(self.clone()).to_tag()
-    }
-}
-
-#[pyclass(name = "RatingTag")]
-#[derive(Debug, Clone)]
-pub enum DartRatingTag {
-    Sfw,
-    General,
-    Sensitive,
-    Nsfw,
-    Questionable,
-    Explicit,
-}
-
-impl From<DartRatingTag> for RatingTag {
-    fn from(tag: DartRatingTag) -> Self {
-        match tag {
-            DartRatingTag::Sfw => RatingTag::Sfw,
-            DartRatingTag::General => RatingTag::General,
-            DartRatingTag::Sensitive => RatingTag::Sensitive,
-            DartRatingTag::Nsfw => RatingTag::Nsfw,
-            DartRatingTag::Questionable => RatingTag::Questionable,
-            DartRatingTag::Explicit => RatingTag::Explicit,
-        }
-    }
-}
-
-#[pymethods]
-impl DartRatingTag {
-    #[new]
-    fn new(tag: &str) -> PyResult<Self> {
-        match tag {
-            "<|rating:sfw|>" => Ok(DartRatingTag::Sfw),
-            "<|rating:general|>" => Ok(DartRatingTag::General),
-            "<|rating:sensitive|>" => Ok(DartRatingTag::Sensitive),
-            "<|rating:nsfw|>" => Ok(DartRatingTag::Nsfw),
-            "<|rating:questionable|>" => Ok(DartRatingTag::Questionable),
-            "<|rating:explicit|>" => Ok(DartRatingTag::Explicit),
-            _ => Err(exceptions::PyValueError::new_err("invalid rating tag")),
-        }
-    }
-
-    fn to_tag(&self) -> String {
-        RatingTag::from(self.clone()).to_tag()
-    }
-}
-
-#[pyclass(name = "IdentityTag")]
-#[derive(Debug, Clone)]
-pub enum DartIdentityTag {
-    Free,
-    Lax,
-    Strict,
-}
-
-impl From<DartIdentityTag> for IdentityTag {
-    fn from(tag: DartIdentityTag) -> Self {
-        match tag {
-            DartIdentityTag::Free => IdentityTag::None,
-            DartIdentityTag::Lax => IdentityTag::Lax,
-            DartIdentityTag::Strict => IdentityTag::Strict,
-        }
-    }
-}
-
-#[pymethods]
-impl DartIdentityTag {
-    #[new]
-    fn new(tag: &str) -> PyResult<Self> {
-        match tag {
-            "<|identity:none|>" => Ok(DartIdentityTag::Free),
-            "<|identity:lax|>" => Ok(DartIdentityTag::Lax),
-            "<|identity:strict|>" => Ok(DartIdentityTag::Strict),
-            _ => Err(exceptions::PyValueError::new_err("invalid identity tag")),
-        }
-    }
-
-    fn to_tag(&self) -> String {
-        IdentityTag::from(self.clone()).to_tag()
-    }
-}
-
-#[pyclass(name = "ReservedTag")]
-#[derive(Debug, Clone)]
-pub enum DartReservedTag {
-    Bos,
-    Eos,
-    CopyrightStart,
-    CopyrightEnd,
-    CharacterStart,
-    CharacterEnd,
-    GeneralStart,
-    GeneralEnd,
-    InputEnd,
-}
-
-impl From<DartReservedTag> for ReservedTag {
-    fn from(tag: DartReservedTag) -> Self {
-        match tag {
-            DartReservedTag::Bos => ReservedTag::Bos,
-            DartReservedTag::Eos => ReservedTag::Eos,
-            DartReservedTag::CopyrightStart => ReservedTag::CopyrightStart,
-            DartReservedTag::CopyrightEnd => ReservedTag::CopyrightEnd,
-            DartReservedTag::CharacterStart => ReservedTag::CharacterStart,
-            DartReservedTag::CharacterEnd => ReservedTag::CharacterEnd,
-            DartReservedTag::GeneralStart => ReservedTag::GeneralStart,
-            DartReservedTag::GeneralEnd => ReservedTag::GeneralEnd,
-            DartReservedTag::InputEnd => ReservedTag::InputEnd,
-        }
-    }
-}
-
-#[pymethods]
-impl DartReservedTag {
-    #[new]
-    fn new(tag: &str) -> PyResult<Self> {
-        match tag {
-            "<|bos|>" => Ok(DartReservedTag::Bos),
-            "<|eos|>" => Ok(DartReservedTag::Eos),
-            "<copyright>" => Ok(DartReservedTag::CopyrightStart),
-            "</copyright>" => Ok(DartReservedTag::CopyrightEnd),
-            "<character>" => Ok(DartReservedTag::CharacterStart),
-            "</character>" => Ok(DartReservedTag::CharacterEnd),
-            "<general>" => Ok(DartReservedTag::GeneralStart),
-            "</general>" => Ok(DartReservedTag::GeneralEnd),
-            "<|input_end|>" => Ok(DartReservedTag::InputEnd),
-            _ => Err(exceptions::PyValueError::new_err("invalid reserved tag")),
-        }
-    }
-
-    fn to_tag(&self) -> String {
-        ReservedTag::from(self.clone()).to_tag()
-    }
-}
+use crate::tags::{AspectRatioTag, IdentityTag, LengthTag, RatingTag, ReservedTag, SpecialTag};
+
+use pyo3::exceptions;
+use pyo3::prelude::*;
+
+#[pyclass(name = "LengthTag")]
+#[derive(Debug, Clone)]
+pub enum DartLengthTag {
+    VeryShort,
+    Short,
+    Medium,
+    Long,
+    VeryLong,
+}
+
+impl From<DartLengthTag> for LengthTag {
+    fn from(tag: DartLengthTag) -> Self {
+        match tag {
+            DartLengthTag::VeryShort => LengthTag::VeryShort,
+            DartLengthTag::Short => LengthTag::Short,
+            DartLengthTag::Medium => LengthTag::Medium,
+            DartLengthTag::Long => LengthTag::Long,
+            DartLengthTag::VeryLong => LengthTag::VeryLong,
+        }
+    }
+}
+
+#[pymethods]
+impl DartLengthTag {
+    #[new]
+    fn new(tag: &str) -> PyResult<Self> {
+        match tag {
+            "<|length:very_short|>" => Ok(DartLengthTag::VeryShort),
+            "<|length:short|>" => Ok(DartLengthTag::Short),
+            "<|length:medium|>" => Ok(DartLengthTag::Medium),
+            "<|length:long|>" => Ok(DartLengthTag::Long),
+            "<|length:very_long|>" => Ok(DartLengthTag::VeryLong),
+            _ => Err(exceptions::PyValueError::new_err("invalid length tag")),
+        }
+    }
+
+    fn to_tag(&self) -> String {
+        LengthTag::from(self.clone()).to_tag()
+    }
+}
+
+#[pyclass(name = "AspectRatioTag")]
+#[derive(Debug, Clone)]
+pub enum DartAspectRatioTag {
+    UltraWide,
+    Wide,
+    Square,
+    Tall,
+    UltraTall,
+}
+
+impl From<DartAspectRatioTag> for AspectRatioTag {
+    fn from(tag: DartAspectRatioTag) -> Self {
+        match tag {
+            DartAspectRatioTag::UltraWide => AspectRatioTag::UltraWide,
+            DartAspectRatioTag::Wide => AspectRatioTag::Wide,
+            DartAspectRatioTag::Square => AspectRatioTag::Square,
+            DartAspectRatioTag::Tall => AspectRatioTag::Tall,
+            DartAspectRatioTag::UltraTall => AspectRatioTag::UltraTall,
+        }
+    }
+}
+
+#[pymethods]
+impl DartAspectRatioTag {
+    #[new]
+    fn new(tag: &str) -> PyResult<Self> {
+        match tag {
+            "<|aspect_ratio:ultra_wide|>" => Ok(DartAspectRatioTag::UltraWide),
+            "<|aspect_ratio:wide|>" => Ok(DartAspectRatioTag::Wide),
+            "<|aspect_ratio:square|>" => Ok(DartAspectRatioTag::Square),
+            "<|aspect_ratio:tall|>" => Ok(DartAspectRatioTag::Tall),
+            "<|aspect_ratio:ultra_tall|>" => Ok(DartAspectRatioTag::UltraTall),
+            _ => Err(exceptions::PyValueError::new_err(
+                "invalid aspect ratio tag",
+            )),
+        }
+    }
+
+    fn to_tag(&self) -> String {
+        AspectRatioTag::from(self.clone()).to_tag()
+    }
+}
+
+#[pyclass(name = "RatingTag")]
+#[derive(Debug, Clone)]
+pub enum DartRatingTag {
+    Sfw,
+    General,
+    Sensitive,
+    Nsfw,
+    Questionable,
+    Explicit,
+}
+
+impl From<DartRatingTag> for RatingTag {
+    fn from(tag: DartRatingTag) -> Self {
+        match tag {
+            DartRatingTag::Sfw => RatingTag::Sfw,
+            DartRatingTag::General => RatingTag::General,
+            DartRatingTag::Sensitive => RatingTag::Sensitive,
+            DartRatingTag::Nsfw => RatingTag::Nsfw,
+            DartRatingTag::Questionable => RatingTag::Questionable,
+            DartRatingTag::Explicit => RatingTag::Explicit,
+        }
+    }
+}
+
+#[pymethods]
+impl DartRatingTag {
+    #[new]
+    fn new(tag: &str) -> PyResult<Self> {
+        match tag {
+            "<|rating:sfw|>" => Ok(DartRatingTag::Sfw),
+            "<|rating:general|>" => Ok(DartRatingTag::General),
+            "<|rating:sensitive|>" => Ok(DartRatingTag::Sensitive),
+            "<|rating:nsfw|>" => Ok(DartRatingTag::Nsfw),
+            "<|rating:questionable|>" => Ok(DartRatingTag::Questionable),
+            "<|rating:explicit|>" => Ok(DartRatingTag::Explicit),
+            _ => Err(exceptions::PyValueError::new_err("invalid rating tag")),
+        }
+    }
+
+    fn to_tag(&self) -> String {
+        RatingTag::from(self.clone()).to_tag()
+    }
+}
+
+#[pyclass(name = "IdentityTag")]
+#[derive(Debug, Clone)]
+pub enum DartIdentityTag {
+    Free,
+    Lax,
+    Strict,
+}
+
+impl From<DartIdentityTag> for IdentityTag {
+    fn from(tag: DartIdentityTag) -> Self {
+        match tag {
+            DartIdentityTag::Free => IdentityTag::None,
+            DartIdentityTag::Lax => IdentityTag::Lax,
+            DartIdentityTag::Strict => IdentityTag::Strict,
+        }
+    }
+}
+
+#[pymethods]
+impl DartIdentityTag {
+    #[new]
+    fn new(tag: &str) -> PyResult<Self> {
+        match tag {
+            "<|identity:none|>" => Ok(DartIdentityTag::Free),
+            "<|identity:lax|>" => Ok(DartIdentityTag::Lax),
+            "<|identity:strict|>" => Ok(DartIdentityTag::Strict),
+            _ => Err(exceptions::PyValueError::new_err("invalid identity tag")),
+        }
+    }
+
+    fn to_tag(&self) -> String {
+        IdentityTag::from(self.clone()).to_tag()
+    }
+}
+
+#[pyclass(name = "ReservedTag")]
+#[derive(Debug, Clone)]
+pub enum DartReservedTag {
+    Bos,
+    Eos,
+    CopyrightStart,
+    CopyrightEnd,
+    CharacterStart,
+    CharacterEnd,
+    GeneralStart,
+    GeneralEnd,
+    InputEnd,
+}
+
+impl From<DartReservedTag> for ReservedTag {
+    fn from(tag: DartReservedTag) -> Self {
+        match tag {
+            DartReservedTag::Bos => ReservedTag::Bos,
+            DartReservedTag::Eos => ReservedTag::Eos,
+            DartReservedTag::CopyrightStart => ReservedTag::CopyrightStart,
+            DartReservedTag::CopyrightEnd => ReservedTag::CopyrightEnd,
+            DartReservedTag::CharacterStart => ReservedTag::CharacterStart,
+            DartReservedTag::CharacterEnd => ReservedTag::CharacterEnd,
+            DartReservedTag::GeneralStart => ReservedTag::GeneralStart,
+            DartReservedTag::GeneralEnd => ReservedTag::GeneralEnd,
+            DartReservedTag::InputEnd => ReservedTag::InputEnd,
+        }
+    }
+}
+
+#[pymethods]
+impl DartReservedTag {
+    #[new]
+    fn new(tag: &str) -> PyResult<Self> {
+        match tag {
+            "<|bos|>" => Ok(DartReservedTag::Bos),
+            "<|eos|>" => Ok(DartReservedTag::Eos),
+            "<copyright>" => Ok(DartReservedTag::CopyrightStart),
+            "</copyright>" => Ok(DartReservedTag::CopyrightEnd),
+            "<character>" => Ok(DartReservedTag::CharacterStart),
+            "</character>" => Ok(DartReservedTag::CharacterEnd),
+            "<general>" => Ok(DartReservedTag::GeneralStart),
+            "</general>" => Ok(DartReservedTag::GeneralEnd),
+            "<|input_end|>" => Ok(DartReservedTag::InputEnd),
+            _ => Err(exceptions::PyValueError::new_err("invalid reserved tag")),
+        }
+    }
+
+    fn to_tag(&self) -> String {
+        ReservedTag::from(self.clone()).to_tag()
+    }
+}
```

### Comparing `dartrs-0.1.0/src/configs.rs` & `dartrs-0.1.1/src/configs.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/generation.rs` & `dartrs-0.1.1/src/generation.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/lib.rs` & `dartrs-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/models/mistral.rs` & `dartrs-0.1.1/src/models/mistral.rs`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,366 +1,366 @@
-// copied and modified from https://github.com/huggingface/candle/blob/3ad4770eb61be34e6d2a7914a935b007d8dee49f/candle-transformers/src/models/mistral.rs
-
-/// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{DType, Device, Module, Result, Tensor, D};
-use candle_nn::{Activation, VarBuilder};
-use candle_transformers::models::with_tracing::{linear_no_bias, Linear, RmsNorm};
-use std::sync::Arc;
-
-#[derive(Debug, Clone, PartialEq, serde::Deserialize)]
-pub struct Config {
-    pub vocab_size: usize,
-    pub hidden_size: usize,
-    pub intermediate_size: usize,
-    pub num_hidden_layers: usize,
-    pub num_attention_heads: usize,
-    pub num_key_value_heads: usize,
-    pub hidden_act: Activation,
-    pub max_position_embeddings: usize,
-    pub rms_norm_eps: f64,
-    pub rope_theta: f64,
-    pub sliding_window: Option<usize>,
-    pub use_flash_attn: bool,
-}
-
-impl Config {
-    // TODO: dart
-}
-
-#[derive(Debug, Clone)]
-struct RotaryEmbedding {
-    sin: Tensor,
-    cos: Tensor,
-}
-
-impl RotaryEmbedding {
-    fn new(dtype: DType, cfg: &Config, dev: &Device) -> Result<Self> {
-        let rope_theta = cfg.rope_theta as f32;
-        let dim = cfg.hidden_size / cfg.num_attention_heads;
-        let max_seq_len = cfg.max_position_embeddings;
-        let inv_freq: Vec<_> = (0..dim)
-            .step_by(2)
-            .map(|i| 1f32 / rope_theta.powf(i as f32 / dim as f32))
-            .collect();
-        let inv_freq_len = inv_freq.len();
-        let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
-        let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-            .to_dtype(dtype)?
-            .reshape((max_seq_len, 1))?;
-        let freqs = t.matmul(&inv_freq)?;
-        Ok(Self {
-            sin: freqs.sin()?,
-            cos: freqs.cos()?,
-        })
-    }
-
-    fn apply_rotary_emb_qkv(
-        &self,
-        q: &Tensor,
-        k: &Tensor,
-        seqlen_offset: usize,
-    ) -> Result<(Tensor, Tensor)> {
-        let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
-        let cos = self.cos.narrow(0, seqlen_offset, seq_len)?;
-        let sin = self.sin.narrow(0, seqlen_offset, seq_len)?;
-        let q_embed = candle_nn::rotary_emb::rope(q, &cos, &sin)?;
-        let k_embed = candle_nn::rotary_emb::rope(k, &cos, &sin)?;
-        Ok((q_embed, k_embed))
-    }
-}
-
-#[derive(Debug, Clone)]
-#[allow(clippy::upper_case_acronyms)]
-struct MLP {
-    gate_proj: Linear,
-    up_proj: Linear,
-    down_proj: Linear,
-    act_fn: Activation,
-}
-
-impl MLP {
-    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let intermediate_sz = cfg.intermediate_size;
-        let gate_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("gate_proj"))?;
-        let up_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("up_proj"))?;
-        let down_proj = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("down_proj"))?;
-        Ok(Self {
-            gate_proj,
-            up_proj,
-            down_proj,
-            act_fn: cfg.hidden_act,
-        })
-    }
-}
-
-impl Module for MLP {
-    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let lhs = xs.apply(&self.gate_proj)?.apply(&self.act_fn)?;
-        let rhs = xs.apply(&self.up_proj)?;
-        (lhs * rhs)?.apply(&self.down_proj)
-    }
-}
-
-#[cfg(feature = "flash-attn")]
-fn flash_attn(
-    q: &Tensor,
-    k: &Tensor,
-    v: &Tensor,
-    softmax_scale: f32,
-    causal: bool,
-) -> Result<Tensor> {
-    candle_flash_attn::flash_attn(q, k, v, softmax_scale, causal)
-}
-
-#[cfg(not(feature = "flash-attn"))]
-fn flash_attn(_: &Tensor, _: &Tensor, _: &Tensor, _: f32, _: bool) -> Result<Tensor> {
-    unimplemented!("compile with '--features flash-attn'")
-}
-
-#[derive(Debug, Clone)]
-struct Attention {
-    q_proj: Linear,
-    k_proj: Linear,
-    v_proj: Linear,
-    o_proj: Linear,
-    num_heads: usize,
-    num_kv_heads: usize,
-    num_kv_groups: usize,
-    head_dim: usize,
-    hidden_size: usize,
-    rotary_emb: Arc<RotaryEmbedding>,
-    kv_cache: Option<(Tensor, Tensor)>,
-    use_flash_attn: bool,
-}
-
-impl Attention {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let num_heads = cfg.num_attention_heads;
-        let num_kv_heads = cfg.num_key_value_heads;
-        let num_kv_groups = num_heads / num_kv_heads;
-        let head_dim = hidden_sz / num_heads;
-        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
-        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
-        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
-        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
-        Ok(Self {
-            q_proj,
-            k_proj,
-            v_proj,
-            o_proj,
-            num_heads,
-            num_kv_heads,
-            num_kv_groups,
-            head_dim,
-            hidden_size: hidden_sz,
-            rotary_emb,
-            kv_cache: None,
-            use_flash_attn: cfg.use_flash_attn,
-        })
-    }
-
-    fn forward(
-        &mut self,
-        xs: &Tensor,
-        attention_mask: Option<&Tensor>,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let (b_sz, q_len, _) = xs.dims3()?;
-
-        let query_states = self.q_proj.forward(xs)?;
-        let key_states = self.k_proj.forward(xs)?;
-        let value_states = self.v_proj.forward(xs)?;
-
-        let query_states = query_states
-            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
-            .transpose(1, 2)?
-            .contiguous()?;
-        let key_states = key_states
-            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-            .transpose(1, 2)?
-            .contiguous()?;
-        let value_states = value_states
-            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-            .transpose(1, 2)?;
-
-        let (query_states, key_states) =
-            self.rotary_emb
-                .apply_rotary_emb_qkv(&query_states, &key_states, seqlen_offset)?;
-
-        let (key_states, value_states) = match &self.kv_cache {
-            None => (key_states, value_states),
-            Some((prev_k, prev_v)) => {
-                let key_states = Tensor::cat(&[prev_k, &key_states], 2)?;
-                let value_states = Tensor::cat(&[prev_v, &value_states], 2)?;
-                (key_states, value_states)
-            }
-        };
-        self.kv_cache = Some((key_states.clone(), value_states.clone()));
-
-        let key_states = candle_transformers::utils::repeat_kv(key_states, self.num_kv_groups)?;
-        let value_states = candle_transformers::utils::repeat_kv(value_states, self.num_kv_groups)?;
-
-        let attn_output = if self.use_flash_attn {
-            // flash-attn expects (b_sz, seq_len, nheads, head_dim)
-            let q = query_states.transpose(1, 2)?;
-            let k = key_states.transpose(1, 2)?;
-            let v = value_states.transpose(1, 2)?;
-            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
-            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
-        } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (query_states.matmul(&key_states.transpose(2, 3)?)? * scale)?;
-
-            let attn_weights = match attention_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
-            };
-            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&value_states)?
-        };
-        attn_output
-            .transpose(1, 2)?
-            .reshape((b_sz, q_len, self.hidden_size))?
-            .apply(&self.o_proj)
-    }
-
-    fn clear_kv_cache(&mut self) {
-        self.kv_cache = None
-    }
-}
-
-#[derive(Debug, Clone)]
-struct DecoderLayer {
-    self_attn: Attention,
-    mlp: MLP,
-    input_layernorm: RmsNorm,
-    post_attention_layernorm: RmsNorm,
-}
-
-impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
-        let post_attention_layernorm = RmsNorm::new(
-            cfg.hidden_size,
-            cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
-        )?;
-        Ok(Self {
-            self_attn,
-            mlp,
-            input_layernorm,
-            post_attention_layernorm,
-        })
-    }
-
-    fn forward(
-        &mut self,
-        xs: &Tensor,
-        attention_mask: Option<&Tensor>,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let residual = xs;
-        let xs = self.input_layernorm.forward(xs)?;
-        let xs = self.self_attn.forward(&xs, attention_mask, seqlen_offset)?;
-        let xs = (xs + residual)?;
-        let residual = &xs;
-        let xs = xs.apply(&self.post_attention_layernorm)?.apply(&self.mlp)?;
-        residual + xs
-    }
-
-    fn clear_kv_cache(&mut self) {
-        self.self_attn.clear_kv_cache()
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct Model {
-    embed_tokens: candle_nn::Embedding,
-    layers: Vec<DecoderLayer>,
-    norm: RmsNorm,
-    lm_head: Linear,
-    sliding_window: Option<usize>,
-    device: Device,
-    dtype: DType,
-}
-
-impl Model {
-    pub fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
-        let rotary_emb = Arc::new(RotaryEmbedding::new(vb.dtype(), cfg, vb_m.device())?);
-        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
-        let vb_l = vb_m.pp("layers");
-        for layer_idx in 0..cfg.num_hidden_layers {
-            let layer = DecoderLayer::new(rotary_emb.clone(), cfg, vb_l.pp(layer_idx))?;
-            layers.push(layer)
-        }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
-        Ok(Self {
-            embed_tokens,
-            layers,
-            norm,
-            lm_head,
-            sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
-            dtype: vb.dtype(),
-        })
-    }
-
-    fn prepare_decoder_attention_mask(
-        &self,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((1, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    pub fn forward(&mut self, input_ids: &Tensor, seqlen_offset: usize) -> Result<Tensor> {
-        let (_b_size, seq_len) = input_ids.dims2()?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask = self.prepare_decoder_attention_mask(seq_len, seqlen_offset)?;
-            Some(mask)
-        };
-        let mut xs = self.embed_tokens.forward(input_ids)?;
-        for layer in self.layers.iter_mut() {
-            xs = layer.forward(&xs, attention_mask.as_ref(), seqlen_offset)?
-        }
-        xs.narrow(1, seq_len - 1, 1)?
-            .apply(&self.norm)?
-            .apply(&self.lm_head)
-    }
-
-    pub fn clear_kv_cache(&mut self) {
-        for layer in self.layers.iter_mut() {
-            layer.clear_kv_cache()
-        }
-    }
-}
+// copied and modified from https://github.com/huggingface/candle/blob/3ad4770eb61be34e6d2a7914a935b007d8dee49f/candle-transformers/src/models/mistral.rs
+
+/// Mistral LLM, https://github.com/mistralai/mistral-src
+use candle_core::{DType, Device, Module, Result, Tensor, D};
+use candle_nn::{Activation, VarBuilder};
+use candle_transformers::models::with_tracing::{linear_no_bias, Linear, RmsNorm};
+use std::sync::Arc;
+
+#[derive(Debug, Clone, PartialEq, serde::Deserialize)]
+pub struct Config {
+    pub vocab_size: usize,
+    pub hidden_size: usize,
+    pub intermediate_size: usize,
+    pub num_hidden_layers: usize,
+    pub num_attention_heads: usize,
+    pub num_key_value_heads: usize,
+    pub hidden_act: Activation,
+    pub max_position_embeddings: usize,
+    pub rms_norm_eps: f64,
+    pub rope_theta: f64,
+    pub sliding_window: Option<usize>,
+    pub use_flash_attn: bool,
+}
+
+impl Config {
+    // TODO: dart
+}
+
+#[derive(Debug, Clone)]
+struct RotaryEmbedding {
+    sin: Tensor,
+    cos: Tensor,
+}
+
+impl RotaryEmbedding {
+    fn new(dtype: DType, cfg: &Config, dev: &Device) -> Result<Self> {
+        let rope_theta = cfg.rope_theta as f32;
+        let dim = cfg.hidden_size / cfg.num_attention_heads;
+        let max_seq_len = cfg.max_position_embeddings;
+        let inv_freq: Vec<_> = (0..dim)
+            .step_by(2)
+            .map(|i| 1f32 / rope_theta.powf(i as f32 / dim as f32))
+            .collect();
+        let inv_freq_len = inv_freq.len();
+        let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
+        let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
+            .to_dtype(dtype)?
+            .reshape((max_seq_len, 1))?;
+        let freqs = t.matmul(&inv_freq)?;
+        Ok(Self {
+            sin: freqs.sin()?,
+            cos: freqs.cos()?,
+        })
+    }
+
+    fn apply_rotary_emb_qkv(
+        &self,
+        q: &Tensor,
+        k: &Tensor,
+        seqlen_offset: usize,
+    ) -> Result<(Tensor, Tensor)> {
+        let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
+        let cos = self.cos.narrow(0, seqlen_offset, seq_len)?;
+        let sin = self.sin.narrow(0, seqlen_offset, seq_len)?;
+        let q_embed = candle_nn::rotary_emb::rope(q, &cos, &sin)?;
+        let k_embed = candle_nn::rotary_emb::rope(k, &cos, &sin)?;
+        Ok((q_embed, k_embed))
+    }
+}
+
+#[derive(Debug, Clone)]
+#[allow(clippy::upper_case_acronyms)]
+struct MLP {
+    gate_proj: Linear,
+    up_proj: Linear,
+    down_proj: Linear,
+    act_fn: Activation,
+}
+
+impl MLP {
+    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let gate_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("gate_proj"))?;
+        let up_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("up_proj"))?;
+        let down_proj = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("down_proj"))?;
+        Ok(Self {
+            gate_proj,
+            up_proj,
+            down_proj,
+            act_fn: cfg.hidden_act,
+        })
+    }
+}
+
+impl Module for MLP {
+    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let lhs = xs.apply(&self.gate_proj)?.apply(&self.act_fn)?;
+        let rhs = xs.apply(&self.up_proj)?;
+        (lhs * rhs)?.apply(&self.down_proj)
+    }
+}
+
+#[cfg(feature = "flash-attn")]
+fn flash_attn(
+    q: &Tensor,
+    k: &Tensor,
+    v: &Tensor,
+    softmax_scale: f32,
+    causal: bool,
+) -> Result<Tensor> {
+    candle_flash_attn::flash_attn(q, k, v, softmax_scale, causal)
+}
+
+#[cfg(not(feature = "flash-attn"))]
+fn flash_attn(_: &Tensor, _: &Tensor, _: &Tensor, _: f32, _: bool) -> Result<Tensor> {
+    unimplemented!("compile with '--features flash-attn'")
+}
+
+#[derive(Debug, Clone)]
+struct Attention {
+    q_proj: Linear,
+    k_proj: Linear,
+    v_proj: Linear,
+    o_proj: Linear,
+    num_heads: usize,
+    num_kv_heads: usize,
+    num_kv_groups: usize,
+    head_dim: usize,
+    hidden_size: usize,
+    rotary_emb: Arc<RotaryEmbedding>,
+    kv_cache: Option<(Tensor, Tensor)>,
+    use_flash_attn: bool,
+}
+
+impl Attention {
+    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let num_heads = cfg.num_attention_heads;
+        let num_kv_heads = cfg.num_key_value_heads;
+        let num_kv_groups = num_heads / num_kv_heads;
+        let head_dim = hidden_sz / num_heads;
+        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
+        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
+        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
+        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
+        Ok(Self {
+            q_proj,
+            k_proj,
+            v_proj,
+            o_proj,
+            num_heads,
+            num_kv_heads,
+            num_kv_groups,
+            head_dim,
+            hidden_size: hidden_sz,
+            rotary_emb,
+            kv_cache: None,
+            use_flash_attn: cfg.use_flash_attn,
+        })
+    }
+
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let (b_sz, q_len, _) = xs.dims3()?;
+
+        let query_states = self.q_proj.forward(xs)?;
+        let key_states = self.k_proj.forward(xs)?;
+        let value_states = self.v_proj.forward(xs)?;
+
+        let query_states = query_states
+            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
+            .transpose(1, 2)?
+            .contiguous()?;
+        let key_states = key_states
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?
+            .contiguous()?;
+        let value_states = value_states
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
+
+        let (query_states, key_states) =
+            self.rotary_emb
+                .apply_rotary_emb_qkv(&query_states, &key_states, seqlen_offset)?;
+
+        let (key_states, value_states) = match &self.kv_cache {
+            None => (key_states, value_states),
+            Some((prev_k, prev_v)) => {
+                let key_states = Tensor::cat(&[prev_k, &key_states], 2)?;
+                let value_states = Tensor::cat(&[prev_v, &value_states], 2)?;
+                (key_states, value_states)
+            }
+        };
+        self.kv_cache = Some((key_states.clone(), value_states.clone()));
+
+        let key_states = candle_transformers::utils::repeat_kv(key_states, self.num_kv_groups)?;
+        let value_states = candle_transformers::utils::repeat_kv(value_states, self.num_kv_groups)?;
+
+        let attn_output = if self.use_flash_attn {
+            // flash-attn expects (b_sz, seq_len, nheads, head_dim)
+            let q = query_states.transpose(1, 2)?;
+            let k = key_states.transpose(1, 2)?;
+            let v = value_states.transpose(1, 2)?;
+            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
+            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
+        } else {
+            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
+            let attn_weights = (query_states.matmul(&key_states.transpose(2, 3)?)? * scale)?;
+
+            let attn_weights = match attention_mask {
+                None => attn_weights,
+                Some(mask) => attn_weights.broadcast_add(mask)?,
+            };
+            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
+            attn_weights.matmul(&value_states)?
+        };
+        attn_output
+            .transpose(1, 2)?
+            .reshape((b_sz, q_len, self.hidden_size))?
+            .apply(&self.o_proj)
+    }
+
+    fn clear_kv_cache(&mut self) {
+        self.kv_cache = None
+    }
+}
+
+#[derive(Debug, Clone)]
+struct DecoderLayer {
+    self_attn: Attention,
+    mlp: MLP,
+    input_layernorm: RmsNorm,
+    post_attention_layernorm: RmsNorm,
+}
+
+impl DecoderLayer {
+    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
+        let mlp = MLP::new(cfg, vb.pp("mlp"))?;
+        let input_layernorm =
+            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let post_attention_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            vb.pp("post_attention_layernorm"),
+        )?;
+        Ok(Self {
+            self_attn,
+            mlp,
+            input_layernorm,
+            post_attention_layernorm,
+        })
+    }
+
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let residual = xs;
+        let xs = self.input_layernorm.forward(xs)?;
+        let xs = self.self_attn.forward(&xs, attention_mask, seqlen_offset)?;
+        let xs = (xs + residual)?;
+        let residual = &xs;
+        let xs = xs.apply(&self.post_attention_layernorm)?.apply(&self.mlp)?;
+        residual + xs
+    }
+
+    fn clear_kv_cache(&mut self) {
+        self.self_attn.clear_kv_cache()
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct Model {
+    embed_tokens: candle_nn::Embedding,
+    layers: Vec<DecoderLayer>,
+    norm: RmsNorm,
+    lm_head: Linear,
+    sliding_window: Option<usize>,
+    device: Device,
+    dtype: DType,
+}
+
+impl Model {
+    pub fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let vb_m = vb.pp("model");
+        let embed_tokens =
+            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let rotary_emb = Arc::new(RotaryEmbedding::new(vb.dtype(), cfg, vb_m.device())?);
+        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let vb_l = vb_m.pp("layers");
+        for layer_idx in 0..cfg.num_hidden_layers {
+            let layer = DecoderLayer::new(rotary_emb.clone(), cfg, vb_l.pp(layer_idx))?;
+            layers.push(layer)
+        }
+        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
+        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        Ok(Self {
+            embed_tokens,
+            layers,
+            norm,
+            lm_head,
+            sliding_window: cfg.sliding_window,
+            device: vb.device().clone(),
+            dtype: vb.dtype(),
+        })
+    }
+
+    fn prepare_decoder_attention_mask(
+        &self,
+        tgt_len: usize,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
+        let mask: Vec<_> = (0..tgt_len)
+            .flat_map(|i| {
+                (0..tgt_len).map(move |j| {
+                    if i < j || j + sliding_window < i {
+                        f32::NEG_INFINITY
+                    } else {
+                        0.
+                    }
+                })
+            })
+            .collect();
+        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
+        let mask = if seqlen_offset > 0 {
+            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
+            Tensor::cat(&[&mask0, &mask], D::Minus1)?
+        } else {
+            mask
+        };
+        mask.expand((1, 1, tgt_len, tgt_len + seqlen_offset))?
+            .to_dtype(self.dtype)
+    }
+
+    pub fn forward(&mut self, input_ids: &Tensor, seqlen_offset: usize) -> Result<Tensor> {
+        let (_b_size, seq_len) = input_ids.dims2()?;
+        let attention_mask = if seq_len <= 1 {
+            None
+        } else {
+            let mask = self.prepare_decoder_attention_mask(seq_len, seqlen_offset)?;
+            Some(mask)
+        };
+        let mut xs = self.embed_tokens.forward(input_ids)?;
+        for layer in self.layers.iter_mut() {
+            xs = layer.forward(&xs, attention_mask.as_ref(), seqlen_offset)?
+        }
+        xs.narrow(1, seq_len - 1, 1)?
+            .apply(&self.norm)?
+            .apply(&self.lm_head)
+    }
+
+    pub fn clear_kv_cache(&mut self) {
+        for layer in self.layers.iter_mut() {
+            layer.clear_kv_cache()
+        }
+    }
+}
```

### Comparing `dartrs-0.1.0/src/models/mixtral.rs` & `dartrs-0.1.1/src/models/mixtral.rs`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,464 +1,464 @@
-// copied and modified from https://github.com/huggingface/candle/blob/3ad4770eb61be34e6d2a7914a935b007d8dee49f/candle-transformers/src/models/mixtral.rs
-
-/// Mixtral Model
-/// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
-/// https://mistral.ai/news/mixtral-of-experts/
-use candle_core::{DType, Device, Module, Result, Tensor, D};
-use candle_nn::{Activation, VarBuilder};
-use candle_transformers::models::with_tracing::{linear_no_bias, Linear, RmsNorm};
-use serde::Deserialize;
-use std::sync::Arc;
-
-/// https://github.com/huggingface/transformers/blob/1a585c1222a56bcaecc070966d558d4a9d862e83/src/transformers/models/mixtral/configuration_mixtral.py#L113
-#[derive(Debug, Clone, PartialEq, Deserialize)]
-pub struct Config {
-    pub vocab_size: usize,
-    pub hidden_size: usize,
-    pub intermediate_size: usize,
-    pub num_hidden_layers: usize,
-    pub num_attention_heads: usize,
-    pub num_key_value_heads: usize,
-    pub hidden_act: Activation,
-    pub max_position_embeddings: usize,
-    pub rms_norm_eps: f64,
-    pub rope_theta: f64,
-    pub sliding_window: Option<usize>,
-    pub num_experts_per_tok: usize,
-    pub num_local_experts: usize,
-    pub use_flash_attn: bool,
-}
-
-impl Config {
-    // TODO: dart
-}
-
-#[derive(Debug, Clone)]
-struct RotaryEmbedding {
-    sin: Tensor,
-    cos: Tensor,
-}
-
-fn rotate_half(xs: &Tensor) -> Result<Tensor> {
-    let last_dim = xs.dim(D::Minus1)?;
-    let xs1 = xs.narrow(D::Minus1, 0, last_dim / 2)?;
-    let xs2 = xs.narrow(D::Minus1, last_dim / 2, last_dim - last_dim / 2)?;
-    Tensor::cat(&[&xs2.neg()?, &xs1], D::Minus1)
-}
-
-impl RotaryEmbedding {
-    fn new(dtype: DType, cfg: &Config, dev: &Device) -> Result<Self> {
-        let dim = cfg.hidden_size / cfg.num_attention_heads;
-        let max_seq_len = cfg.max_position_embeddings;
-        let inv_freq: Vec<_> = (0..dim)
-            .step_by(2)
-            .map(|i| 1f32 / (cfg.rope_theta as f32).powf(i as f32 / dim as f32))
-            .collect();
-        let inv_freq_len = inv_freq.len();
-        let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
-        let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-            .to_dtype(dtype)?
-            .reshape((max_seq_len, 1))?;
-        let freqs = t.matmul(&inv_freq)?;
-        let freqs = Tensor::cat(&[&freqs, &freqs], D::Minus1)?;
-        Ok(Self {
-            sin: freqs.sin()?,
-            cos: freqs.cos()?,
-        })
-    }
-
-    fn apply_rotary_emb_qkv(
-        &self,
-        q: &Tensor,
-        k: &Tensor,
-        seqlen_offset: usize,
-    ) -> Result<(Tensor, Tensor)> {
-        let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
-        let cos = self.cos.narrow(0, seqlen_offset, seq_len)?;
-        let sin = self.sin.narrow(0, seqlen_offset, seq_len)?;
-        let cos = cos.unsqueeze(0)?.unsqueeze(0)?; // (1, 1, seq_len, dim)
-        let sin = sin.unsqueeze(0)?.unsqueeze(0)?; // (1, 1, seq_len, dim)
-        let q_embed = (q.broadcast_mul(&cos)? + rotate_half(q)?.broadcast_mul(&sin))?;
-        let k_embed = (k.broadcast_mul(&cos)? + rotate_half(k)?.broadcast_mul(&sin))?;
-        Ok((q_embed, k_embed))
-    }
-}
-
-#[cfg(feature = "flash-attn")]
-fn flash_attn(
-    q: &Tensor,
-    k: &Tensor,
-    v: &Tensor,
-    softmax_scale: f32,
-    causal: bool,
-) -> Result<Tensor> {
-    candle_flash_attn::flash_attn(q, k, v, softmax_scale, causal)
-}
-
-#[cfg(not(feature = "flash-attn"))]
-fn flash_attn(_: &Tensor, _: &Tensor, _: &Tensor, _: f32, _: bool) -> Result<Tensor> {
-    unimplemented!("compile with '--features flash-attn'")
-}
-
-#[derive(Debug, Clone)]
-struct Attention {
-    q_proj: Linear,
-    k_proj: Linear,
-    v_proj: Linear,
-    o_proj: Linear,
-    num_heads: usize,
-    num_kv_heads: usize,
-    num_kv_groups: usize,
-    head_dim: usize,
-    hidden_size: usize,
-    rotary_emb: Arc<RotaryEmbedding>,
-    kv_cache: Option<(Tensor, Tensor)>,
-    use_flash_attn: bool,
-}
-
-impl Attention {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let num_heads = cfg.num_attention_heads;
-        let num_kv_heads = cfg.num_key_value_heads;
-        let num_kv_groups = num_heads / num_kv_heads;
-        let head_dim = hidden_sz / num_heads;
-        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
-        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
-        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
-        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
-        Ok(Self {
-            q_proj,
-            k_proj,
-            v_proj,
-            o_proj,
-            num_heads,
-            num_kv_heads,
-            num_kv_groups,
-            head_dim,
-            hidden_size: hidden_sz,
-            rotary_emb,
-            kv_cache: None,
-            use_flash_attn: cfg.use_flash_attn,
-        })
-    }
-
-    fn forward(
-        &mut self,
-        xs: &Tensor,
-        attention_mask: Option<&Tensor>,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let (b_sz, q_len, _) = xs.dims3()?;
-
-        let query_states = self.q_proj.forward(xs)?;
-        let key_states = self.k_proj.forward(xs)?;
-        let value_states = self.v_proj.forward(xs)?;
-
-        let query_states = query_states
-            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
-            .transpose(1, 2)?;
-        let key_states = key_states
-            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-            .transpose(1, 2)?;
-        let value_states = value_states
-            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-            .transpose(1, 2)?;
-
-        let (query_states, key_states) =
-            self.rotary_emb
-                .apply_rotary_emb_qkv(&query_states, &key_states, seqlen_offset)?;
-
-        let (key_states, value_states) = match &self.kv_cache {
-            None => (key_states, value_states),
-            Some((prev_k, prev_v)) => {
-                let key_states = Tensor::cat(&[prev_k, &key_states], 2)?;
-                let value_states = Tensor::cat(&[prev_v, &value_states], 2)?;
-                (key_states, value_states)
-            }
-        };
-        self.kv_cache = Some((key_states.clone(), value_states.clone()));
-
-        let key_states = candle_transformers::utils::repeat_kv(key_states, self.num_kv_groups)?;
-        let value_states = candle_transformers::utils::repeat_kv(value_states, self.num_kv_groups)?;
-
-        let attn_output = if self.use_flash_attn {
-            // flash-attn expects (b_sz, seq_len, nheads, head_dim)
-            let q = query_states.transpose(1, 2)?;
-            let k = key_states.transpose(1, 2)?;
-            let v = value_states.transpose(1, 2)?;
-            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
-            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
-        } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (query_states.matmul(&key_states.transpose(2, 3)?)? * scale)?;
-
-            let attn_weights = match attention_mask {
-                None => attn_weights,
-                Some(mask) => attn_weights.broadcast_add(mask)?,
-            };
-            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&value_states)?
-        };
-        attn_output
-            .transpose(1, 2)?
-            .reshape((b_sz, q_len, self.hidden_size))?
-            .apply(&self.o_proj)
-    }
-
-    fn clear_kv_cache(&mut self) {
-        self.kv_cache = None
-    }
-}
-
-#[derive(Debug, Clone)]
-struct BlockSparseTop2MLP {
-    w1: Linear,
-    w2: Linear,
-    w3: Linear,
-    act_fn: Activation,
-}
-
-impl BlockSparseTop2MLP {
-    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let hidden_sz = cfg.hidden_size;
-        let intermediate_sz = cfg.intermediate_size;
-        let w1 = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("w1"))?;
-        let w2 = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("w2"))?;
-        let w3 = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("w3"))?;
-        Ok(Self {
-            w1,
-            w2,
-            w3,
-            act_fn: cfg.hidden_act,
-        })
-    }
-}
-
-impl Module for BlockSparseTop2MLP {
-    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let lhs = xs.apply(&self.w1)?.apply(&self.act_fn)?;
-        let rhs = xs.apply(&self.w3)?;
-        (lhs * rhs)?.apply(&self.w2)
-    }
-}
-
-#[derive(Debug, Clone)]
-struct SparseMoeBlock {
-    gate: Linear,
-    experts: Vec<BlockSparseTop2MLP>,
-    num_experts_per_tok: usize,
-}
-
-impl SparseMoeBlock {
-    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let gate = linear_no_bias(cfg.hidden_size, cfg.num_local_experts, vb.pp("gate"))?;
-        let mut experts = Vec::with_capacity(cfg.num_local_experts);
-        let vb = vb.pp("experts");
-        for idx in 0..cfg.num_local_experts {
-            let expert = BlockSparseTop2MLP::new(cfg, vb.pp(idx))?;
-            experts.push(expert)
-        }
-        Ok(SparseMoeBlock {
-            gate,
-            experts,
-            num_experts_per_tok: cfg.num_experts_per_tok,
-        })
-    }
-}
-
-impl Module for SparseMoeBlock {
-    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let (b_size, seq_len, hidden_dim) = xs.dims3()?;
-        let xs = xs.reshape(((), hidden_dim))?;
-        let router_logits = xs.apply(&self.gate)?;
-        let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
-
-        // In order to extract topk, we extract the data from the tensor and manipulate it
-        // directly. Maybe we will want to use some custom ops instead at some point.
-        let routing_weights = routing_weights.to_dtype(DType::F32)?.to_vec2::<f32>()?;
-
-        // routing_weights, selected_experts = torch.topk(routing_weights, self.top_k, dim=-1)
-        // top_x contains the row indexes to evaluate for each expert.
-        let mut top_x = vec![vec![]; self.experts.len()];
-        let mut selected_rws = vec![vec![]; self.experts.len()];
-        for (row_idx, rw) in routing_weights.iter().enumerate() {
-            let mut dst = (0..rw.len() as u32).collect::<Vec<u32>>();
-            dst.sort_by(|&i, &j| rw[j as usize].total_cmp(&rw[i as usize]));
-            let mut sum_routing_weights = 0f32;
-            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
-                let expert_idx = expert_idx as usize;
-                let routing_weight = rw[expert_idx];
-                sum_routing_weights += routing_weight;
-                top_x[expert_idx].push(row_idx as u32);
-            }
-            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
-                let expert_idx = expert_idx as usize;
-                let routing_weight = rw[expert_idx];
-                selected_rws[expert_idx].push(routing_weight / sum_routing_weights)
-            }
-        }
-
-        // routing_weights /= routing_weights.sum(dim=-1, keepdim=True)
-        // expert_mask = torch.nn.functional.one_hot(selected_experts, num_classes=self.num_experts).permute(2, 1, 0)
-
-        let mut ys = xs.zeros_like()?;
-        for (expert_idx, expert_layer) in self.experts.iter().enumerate() {
-            let top_x = &top_x[expert_idx];
-            if top_x.is_empty() {
-                continue;
-            }
-            let top_x = Tensor::new(top_x.as_slice(), xs.device())?;
-            let selected_rws =
-                Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?.reshape(((), 1))?;
-            // Index the correct hidden states and compute the expert hidden state for
-            // the current expert. We need to make sure to multiply the output hidden
-            // states by `routing_weights` on the corresponding tokens (top-1 and top-2)
-            let current_state = xs.index_select(&top_x, 0)?.reshape(((), hidden_dim))?;
-            // current_hidden_states = expert_layer(current_state, routing_weights[top_x_list, idx_list, None])
-            let current_hidden_states = expert_layer.forward(&current_state)?;
-            let current_hidden_states = current_hidden_states.broadcast_mul(&selected_rws)?;
-            ys = ys.index_add(&top_x, &current_hidden_states, 0)?;
-        }
-
-        let ys = ys.reshape((b_size, seq_len, hidden_dim))?;
-        Ok(ys)
-    }
-}
-
-#[derive(Debug, Clone)]
-struct DecoderLayer {
-    self_attn: Attention,
-    block_sparse_moe: SparseMoeBlock,
-    input_layernorm: RmsNorm,
-    post_attention_layernorm: RmsNorm,
-}
-
-impl DecoderLayer {
-    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
-        let block_sparse_moe = SparseMoeBlock::new(cfg, vb.pp("block_sparse_moe"))?;
-        let input_layernorm =
-            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
-        let post_attention_layernorm = RmsNorm::new(
-            cfg.hidden_size,
-            cfg.rms_norm_eps,
-            vb.pp("post_attention_layernorm"),
-        )?;
-        Ok(Self {
-            self_attn,
-            block_sparse_moe,
-            input_layernorm,
-            post_attention_layernorm,
-        })
-    }
-
-    fn forward(
-        &mut self,
-        xs: &Tensor,
-        attention_mask: Option<&Tensor>,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let residual = xs;
-        let xs = self.input_layernorm.forward(xs)?;
-        let xs = self.self_attn.forward(&xs, attention_mask, seqlen_offset)?;
-        let xs = (xs + residual)?;
-        let residual = &xs;
-        let xs = xs
-            .apply(&self.post_attention_layernorm)?
-            .apply(&self.block_sparse_moe)?;
-        residual + xs
-    }
-
-    fn clear_kv_cache(&mut self) {
-        self.self_attn.clear_kv_cache()
-    }
-}
-
-#[derive(Debug, Clone)]
-pub struct Model {
-    embed_tokens: candle_nn::Embedding,
-    layers: Vec<DecoderLayer>,
-    norm: RmsNorm,
-    lm_head: Linear,
-    sliding_window: Option<usize>,
-    device: Device,
-    dtype: DType,
-}
-
-impl Model {
-    pub fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let vb_m = vb.pp("model");
-        let embed_tokens =
-            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
-        let rotary_emb = Arc::new(RotaryEmbedding::new(vb.dtype(), cfg, vb_m.device())?);
-        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
-        let vb_l = vb_m.pp("layers");
-        for layer_idx in 0..cfg.num_hidden_layers {
-            let layer = DecoderLayer::new(rotary_emb.clone(), cfg, vb_l.pp(layer_idx))?;
-            layers.push(layer)
-        }
-        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
-        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
-        Ok(Self {
-            embed_tokens,
-            layers,
-            norm,
-            lm_head,
-            sliding_window: cfg.sliding_window,
-            device: vb.device().clone(),
-            dtype: vb.dtype(),
-        })
-    }
-
-    fn prepare_decoder_attention_mask(
-        &self,
-        b_size: usize,
-        tgt_len: usize,
-        seqlen_offset: usize,
-    ) -> Result<Tensor> {
-        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| {
-                (0..tgt_len).map(move |j| {
-                    if i < j || j + sliding_window < i {
-                        f32::NEG_INFINITY
-                    } else {
-                        0.
-                    }
-                })
-            })
-            .collect();
-        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
-        let mask = if seqlen_offset > 0 {
-            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
-            Tensor::cat(&[&mask0, &mask], D::Minus1)?
-        } else {
-            mask
-        };
-        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
-            .to_dtype(self.dtype)
-    }
-
-    pub fn forward(&mut self, input_ids: &Tensor, seqlen_offset: usize) -> Result<Tensor> {
-        let (b_size, seq_len) = input_ids.dims2()?;
-        let attention_mask = if seq_len <= 1 {
-            None
-        } else {
-            let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offset)?;
-            Some(mask)
-        };
-        let mut xs = self.embed_tokens.forward(input_ids)?;
-        for layer in self.layers.iter_mut() {
-            xs = layer.forward(&xs, attention_mask.as_ref(), seqlen_offset)?
-        }
-        xs.narrow(1, seq_len - 1, 1)?
-            .apply(&self.norm)?
-            .apply(&self.lm_head)
-    }
-
-    pub fn clear_kv_cache(&mut self) {
-        for layer in self.layers.iter_mut() {
-            layer.clear_kv_cache()
-        }
-    }
-}
+// copied and modified from https://github.com/huggingface/candle/blob/3ad4770eb61be34e6d2a7914a935b007d8dee49f/candle-transformers/src/models/mixtral.rs
+
+/// Mixtral Model
+/// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
+/// https://mistral.ai/news/mixtral-of-experts/
+use candle_core::{DType, Device, Module, Result, Tensor, D};
+use candle_nn::{Activation, VarBuilder};
+use candle_transformers::models::with_tracing::{linear_no_bias, Linear, RmsNorm};
+use serde::Deserialize;
+use std::sync::Arc;
+
+/// https://github.com/huggingface/transformers/blob/1a585c1222a56bcaecc070966d558d4a9d862e83/src/transformers/models/mixtral/configuration_mixtral.py#L113
+#[derive(Debug, Clone, PartialEq, Deserialize)]
+pub struct Config {
+    pub vocab_size: usize,
+    pub hidden_size: usize,
+    pub intermediate_size: usize,
+    pub num_hidden_layers: usize,
+    pub num_attention_heads: usize,
+    pub num_key_value_heads: usize,
+    pub hidden_act: Activation,
+    pub max_position_embeddings: usize,
+    pub rms_norm_eps: f64,
+    pub rope_theta: f64,
+    pub sliding_window: Option<usize>,
+    pub num_experts_per_tok: usize,
+    pub num_local_experts: usize,
+    pub use_flash_attn: bool,
+}
+
+impl Config {
+    // TODO: dart
+}
+
+#[derive(Debug, Clone)]
+struct RotaryEmbedding {
+    sin: Tensor,
+    cos: Tensor,
+}
+
+fn rotate_half(xs: &Tensor) -> Result<Tensor> {
+    let last_dim = xs.dim(D::Minus1)?;
+    let xs1 = xs.narrow(D::Minus1, 0, last_dim / 2)?;
+    let xs2 = xs.narrow(D::Minus1, last_dim / 2, last_dim - last_dim / 2)?;
+    Tensor::cat(&[&xs2.neg()?, &xs1], D::Minus1)
+}
+
+impl RotaryEmbedding {
+    fn new(dtype: DType, cfg: &Config, dev: &Device) -> Result<Self> {
+        let dim = cfg.hidden_size / cfg.num_attention_heads;
+        let max_seq_len = cfg.max_position_embeddings;
+        let inv_freq: Vec<_> = (0..dim)
+            .step_by(2)
+            .map(|i| 1f32 / (cfg.rope_theta as f32).powf(i as f32 / dim as f32))
+            .collect();
+        let inv_freq_len = inv_freq.len();
+        let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?.to_dtype(dtype)?;
+        let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
+            .to_dtype(dtype)?
+            .reshape((max_seq_len, 1))?;
+        let freqs = t.matmul(&inv_freq)?;
+        let freqs = Tensor::cat(&[&freqs, &freqs], D::Minus1)?;
+        Ok(Self {
+            sin: freqs.sin()?,
+            cos: freqs.cos()?,
+        })
+    }
+
+    fn apply_rotary_emb_qkv(
+        &self,
+        q: &Tensor,
+        k: &Tensor,
+        seqlen_offset: usize,
+    ) -> Result<(Tensor, Tensor)> {
+        let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
+        let cos = self.cos.narrow(0, seqlen_offset, seq_len)?;
+        let sin = self.sin.narrow(0, seqlen_offset, seq_len)?;
+        let cos = cos.unsqueeze(0)?.unsqueeze(0)?; // (1, 1, seq_len, dim)
+        let sin = sin.unsqueeze(0)?.unsqueeze(0)?; // (1, 1, seq_len, dim)
+        let q_embed = (q.broadcast_mul(&cos)? + rotate_half(q)?.broadcast_mul(&sin))?;
+        let k_embed = (k.broadcast_mul(&cos)? + rotate_half(k)?.broadcast_mul(&sin))?;
+        Ok((q_embed, k_embed))
+    }
+}
+
+#[cfg(feature = "flash-attn")]
+fn flash_attn(
+    q: &Tensor,
+    k: &Tensor,
+    v: &Tensor,
+    softmax_scale: f32,
+    causal: bool,
+) -> Result<Tensor> {
+    candle_flash_attn::flash_attn(q, k, v, softmax_scale, causal)
+}
+
+#[cfg(not(feature = "flash-attn"))]
+fn flash_attn(_: &Tensor, _: &Tensor, _: &Tensor, _: f32, _: bool) -> Result<Tensor> {
+    unimplemented!("compile with '--features flash-attn'")
+}
+
+#[derive(Debug, Clone)]
+struct Attention {
+    q_proj: Linear,
+    k_proj: Linear,
+    v_proj: Linear,
+    o_proj: Linear,
+    num_heads: usize,
+    num_kv_heads: usize,
+    num_kv_groups: usize,
+    head_dim: usize,
+    hidden_size: usize,
+    rotary_emb: Arc<RotaryEmbedding>,
+    kv_cache: Option<(Tensor, Tensor)>,
+    use_flash_attn: bool,
+}
+
+impl Attention {
+    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let num_heads = cfg.num_attention_heads;
+        let num_kv_heads = cfg.num_key_value_heads;
+        let num_kv_groups = num_heads / num_kv_heads;
+        let head_dim = hidden_sz / num_heads;
+        let q_proj = linear_no_bias(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
+        let k_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
+        let v_proj = linear_no_bias(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
+        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
+        Ok(Self {
+            q_proj,
+            k_proj,
+            v_proj,
+            o_proj,
+            num_heads,
+            num_kv_heads,
+            num_kv_groups,
+            head_dim,
+            hidden_size: hidden_sz,
+            rotary_emb,
+            kv_cache: None,
+            use_flash_attn: cfg.use_flash_attn,
+        })
+    }
+
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let (b_sz, q_len, _) = xs.dims3()?;
+
+        let query_states = self.q_proj.forward(xs)?;
+        let key_states = self.k_proj.forward(xs)?;
+        let value_states = self.v_proj.forward(xs)?;
+
+        let query_states = query_states
+            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
+            .transpose(1, 2)?;
+        let key_states = key_states
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
+        let value_states = value_states
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
+
+        let (query_states, key_states) =
+            self.rotary_emb
+                .apply_rotary_emb_qkv(&query_states, &key_states, seqlen_offset)?;
+
+        let (key_states, value_states) = match &self.kv_cache {
+            None => (key_states, value_states),
+            Some((prev_k, prev_v)) => {
+                let key_states = Tensor::cat(&[prev_k, &key_states], 2)?;
+                let value_states = Tensor::cat(&[prev_v, &value_states], 2)?;
+                (key_states, value_states)
+            }
+        };
+        self.kv_cache = Some((key_states.clone(), value_states.clone()));
+
+        let key_states = candle_transformers::utils::repeat_kv(key_states, self.num_kv_groups)?;
+        let value_states = candle_transformers::utils::repeat_kv(value_states, self.num_kv_groups)?;
+
+        let attn_output = if self.use_flash_attn {
+            // flash-attn expects (b_sz, seq_len, nheads, head_dim)
+            let q = query_states.transpose(1, 2)?;
+            let k = key_states.transpose(1, 2)?;
+            let v = value_states.transpose(1, 2)?;
+            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
+            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
+        } else {
+            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
+            let attn_weights = (query_states.matmul(&key_states.transpose(2, 3)?)? * scale)?;
+
+            let attn_weights = match attention_mask {
+                None => attn_weights,
+                Some(mask) => attn_weights.broadcast_add(mask)?,
+            };
+            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
+            attn_weights.matmul(&value_states)?
+        };
+        attn_output
+            .transpose(1, 2)?
+            .reshape((b_sz, q_len, self.hidden_size))?
+            .apply(&self.o_proj)
+    }
+
+    fn clear_kv_cache(&mut self) {
+        self.kv_cache = None
+    }
+}
+
+#[derive(Debug, Clone)]
+struct BlockSparseTop2MLP {
+    w1: Linear,
+    w2: Linear,
+    w3: Linear,
+    act_fn: Activation,
+}
+
+impl BlockSparseTop2MLP {
+    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let w1 = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("w1"))?;
+        let w2 = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("w2"))?;
+        let w3 = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("w3"))?;
+        Ok(Self {
+            w1,
+            w2,
+            w3,
+            act_fn: cfg.hidden_act,
+        })
+    }
+}
+
+impl Module for BlockSparseTop2MLP {
+    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let lhs = xs.apply(&self.w1)?.apply(&self.act_fn)?;
+        let rhs = xs.apply(&self.w3)?;
+        (lhs * rhs)?.apply(&self.w2)
+    }
+}
+
+#[derive(Debug, Clone)]
+struct SparseMoeBlock {
+    gate: Linear,
+    experts: Vec<BlockSparseTop2MLP>,
+    num_experts_per_tok: usize,
+}
+
+impl SparseMoeBlock {
+    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let gate = linear_no_bias(cfg.hidden_size, cfg.num_local_experts, vb.pp("gate"))?;
+        let mut experts = Vec::with_capacity(cfg.num_local_experts);
+        let vb = vb.pp("experts");
+        for idx in 0..cfg.num_local_experts {
+            let expert = BlockSparseTop2MLP::new(cfg, vb.pp(idx))?;
+            experts.push(expert)
+        }
+        Ok(SparseMoeBlock {
+            gate,
+            experts,
+            num_experts_per_tok: cfg.num_experts_per_tok,
+        })
+    }
+}
+
+impl Module for SparseMoeBlock {
+    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let (b_size, seq_len, hidden_dim) = xs.dims3()?;
+        let xs = xs.reshape(((), hidden_dim))?;
+        let router_logits = xs.apply(&self.gate)?;
+        let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
+
+        // In order to extract topk, we extract the data from the tensor and manipulate it
+        // directly. Maybe we will want to use some custom ops instead at some point.
+        let routing_weights = routing_weights.to_dtype(DType::F32)?.to_vec2::<f32>()?;
+
+        // routing_weights, selected_experts = torch.topk(routing_weights, self.top_k, dim=-1)
+        // top_x contains the row indexes to evaluate for each expert.
+        let mut top_x = vec![vec![]; self.experts.len()];
+        let mut selected_rws = vec![vec![]; self.experts.len()];
+        for (row_idx, rw) in routing_weights.iter().enumerate() {
+            let mut dst = (0..rw.len() as u32).collect::<Vec<u32>>();
+            dst.sort_by(|&i, &j| rw[j as usize].total_cmp(&rw[i as usize]));
+            let mut sum_routing_weights = 0f32;
+            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
+                let expert_idx = expert_idx as usize;
+                let routing_weight = rw[expert_idx];
+                sum_routing_weights += routing_weight;
+                top_x[expert_idx].push(row_idx as u32);
+            }
+            for &expert_idx in dst.iter().take(self.num_experts_per_tok) {
+                let expert_idx = expert_idx as usize;
+                let routing_weight = rw[expert_idx];
+                selected_rws[expert_idx].push(routing_weight / sum_routing_weights)
+            }
+        }
+
+        // routing_weights /= routing_weights.sum(dim=-1, keepdim=True)
+        // expert_mask = torch.nn.functional.one_hot(selected_experts, num_classes=self.num_experts).permute(2, 1, 0)
+
+        let mut ys = xs.zeros_like()?;
+        for (expert_idx, expert_layer) in self.experts.iter().enumerate() {
+            let top_x = &top_x[expert_idx];
+            if top_x.is_empty() {
+                continue;
+            }
+            let top_x = Tensor::new(top_x.as_slice(), xs.device())?;
+            let selected_rws =
+                Tensor::new(selected_rws[expert_idx].as_slice(), xs.device())?.reshape(((), 1))?;
+            // Index the correct hidden states and compute the expert hidden state for
+            // the current expert. We need to make sure to multiply the output hidden
+            // states by `routing_weights` on the corresponding tokens (top-1 and top-2)
+            let current_state = xs.index_select(&top_x, 0)?.reshape(((), hidden_dim))?;
+            // current_hidden_states = expert_layer(current_state, routing_weights[top_x_list, idx_list, None])
+            let current_hidden_states = expert_layer.forward(&current_state)?;
+            let current_hidden_states = current_hidden_states.broadcast_mul(&selected_rws)?;
+            ys = ys.index_add(&top_x, &current_hidden_states, 0)?;
+        }
+
+        let ys = ys.reshape((b_size, seq_len, hidden_dim))?;
+        Ok(ys)
+    }
+}
+
+#[derive(Debug, Clone)]
+struct DecoderLayer {
+    self_attn: Attention,
+    block_sparse_moe: SparseMoeBlock,
+    input_layernorm: RmsNorm,
+    post_attention_layernorm: RmsNorm,
+}
+
+impl DecoderLayer {
+    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let self_attn = Attention::new(rotary_emb, cfg, vb.pp("self_attn"))?;
+        let block_sparse_moe = SparseMoeBlock::new(cfg, vb.pp("block_sparse_moe"))?;
+        let input_layernorm =
+            RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb.pp("input_layernorm"))?;
+        let post_attention_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            vb.pp("post_attention_layernorm"),
+        )?;
+        Ok(Self {
+            self_attn,
+            block_sparse_moe,
+            input_layernorm,
+            post_attention_layernorm,
+        })
+    }
+
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let residual = xs;
+        let xs = self.input_layernorm.forward(xs)?;
+        let xs = self.self_attn.forward(&xs, attention_mask, seqlen_offset)?;
+        let xs = (xs + residual)?;
+        let residual = &xs;
+        let xs = xs
+            .apply(&self.post_attention_layernorm)?
+            .apply(&self.block_sparse_moe)?;
+        residual + xs
+    }
+
+    fn clear_kv_cache(&mut self) {
+        self.self_attn.clear_kv_cache()
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct Model {
+    embed_tokens: candle_nn::Embedding,
+    layers: Vec<DecoderLayer>,
+    norm: RmsNorm,
+    lm_head: Linear,
+    sliding_window: Option<usize>,
+    device: Device,
+    dtype: DType,
+}
+
+impl Model {
+    pub fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let vb_m = vb.pp("model");
+        let embed_tokens =
+            candle_nn::embedding(cfg.vocab_size, cfg.hidden_size, vb_m.pp("embed_tokens"))?;
+        let rotary_emb = Arc::new(RotaryEmbedding::new(vb.dtype(), cfg, vb_m.device())?);
+        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let vb_l = vb_m.pp("layers");
+        for layer_idx in 0..cfg.num_hidden_layers {
+            let layer = DecoderLayer::new(rotary_emb.clone(), cfg, vb_l.pp(layer_idx))?;
+            layers.push(layer)
+        }
+        let norm = RmsNorm::new(cfg.hidden_size, cfg.rms_norm_eps, vb_m.pp("norm"))?;
+        let lm_head = linear_no_bias(cfg.hidden_size, cfg.vocab_size, vb.pp("lm_head"))?;
+        Ok(Self {
+            embed_tokens,
+            layers,
+            norm,
+            lm_head,
+            sliding_window: cfg.sliding_window,
+            device: vb.device().clone(),
+            dtype: vb.dtype(),
+        })
+    }
+
+    fn prepare_decoder_attention_mask(
+        &self,
+        b_size: usize,
+        tgt_len: usize,
+        seqlen_offset: usize,
+    ) -> Result<Tensor> {
+        let sliding_window = self.sliding_window.unwrap_or(tgt_len + 1);
+        let mask: Vec<_> = (0..tgt_len)
+            .flat_map(|i| {
+                (0..tgt_len).map(move |j| {
+                    if i < j || j + sliding_window < i {
+                        f32::NEG_INFINITY
+                    } else {
+                        0.
+                    }
+                })
+            })
+            .collect();
+        let mask = Tensor::from_slice(&mask, (tgt_len, tgt_len), &self.device)?;
+        let mask = if seqlen_offset > 0 {
+            let mask0 = Tensor::zeros((tgt_len, seqlen_offset), DType::F32, &self.device)?;
+            Tensor::cat(&[&mask0, &mask], D::Minus1)?
+        } else {
+            mask
+        };
+        mask.expand((b_size, 1, tgt_len, tgt_len + seqlen_offset))?
+            .to_dtype(self.dtype)
+    }
+
+    pub fn forward(&mut self, input_ids: &Tensor, seqlen_offset: usize) -> Result<Tensor> {
+        let (b_size, seq_len) = input_ids.dims2()?;
+        let attention_mask = if seq_len <= 1 {
+            None
+        } else {
+            let mask = self.prepare_decoder_attention_mask(b_size, seq_len, seqlen_offset)?;
+            Some(mask)
+        };
+        let mut xs = self.embed_tokens.forward(input_ids)?;
+        for layer in self.layers.iter_mut() {
+            xs = layer.forward(&xs, attention_mask.as_ref(), seqlen_offset)?
+        }
+        xs.narrow(1, seq_len - 1, 1)?
+            .apply(&self.norm)?
+            .apply(&self.lm_head)
+    }
+
+    pub fn clear_kv_cache(&mut self) {
+        for layer in self.layers.iter_mut() {
+            layer.clear_kv_cache()
+        }
+    }
+}
```

### Comparing `dartrs-0.1.0/src/models.rs` & `dartrs-0.1.1/src/models.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/src/tags.rs` & `dartrs-0.1.1/src/tags.rs`

 * *Files identical despite different names*

### Comparing `dartrs-0.1.0/tests/test_prompt.py` & `dartrs-0.1.1/tests/test_prompt.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from dartrs import dartrs, v2
-
-
-def test_compose_prompt_v2():
-    prompt = dartrs.compose_prompt_v2(
-        copyright="vocaloid",
-        character="hatsune miku",
-        rating=dartrs.RatingTag.Sfw,
-        aspect_ratio=dartrs.AspectRatioTag.Tall,
-        length=dartrs.LengthTag.Long,
-        identity_level=dartrs.IdentityTag.Lax,
-        prompt="1girl, cat ears",
-    )
-
-    assert prompt is not None
-    assert prompt == (
-        f"<|bos|>"
-        f"<copyright>vocaloid</copyright>"
-        f"<character>hatsune miku</character>"
-        f"<|rating:sfw|><|aspect_ratio:tall|><|length:long|>"
-        f"<general>1girl, cat ears<|identity:lax|><|input_end|>"
-    )
-
-
-def test_compose_prompt_v2_wrapper():
-    prompt = v2.compose_prompt(
-        prompt="1girl, cat ears",
-        copyright="vocaloid",
-        character="hatsune miku",
-        rating=v2.RatingTag.Sfw,
-        aspect_ratio=v2.AspectRatioTag.Tall,
-        length=v2.LengthTag.Long,
-        identity_level=v2.IdentityTag.Lax,
-    )
-
-    assert prompt is not None
-    assert prompt == (
-        f"<|bos|>"
-        f"<copyright>vocaloid</copyright>"
-        f"<character>hatsune miku</character>"
-        f"<|rating:sfw|><|aspect_ratio:tall|><|length:long|>"
-        f"<general>1girl, cat ears<|identity:lax|><|input_end|>"
-    )
+from dartrs import dartrs, v2
+
+
+def test_compose_prompt_v2():
+    prompt = dartrs.compose_prompt_v2(
+        copyright="vocaloid",
+        character="hatsune miku",
+        rating=dartrs.RatingTag.Sfw,
+        aspect_ratio=dartrs.AspectRatioTag.Tall,
+        length=dartrs.LengthTag.Long,
+        identity_level=dartrs.IdentityTag.Lax,
+        prompt="1girl, cat ears",
+    )
+
+    assert prompt is not None
+    assert prompt == (
+        f"<|bos|>"
+        f"<copyright>vocaloid</copyright>"
+        f"<character>hatsune miku</character>"
+        f"<|rating:sfw|><|aspect_ratio:tall|><|length:long|>"
+        f"<general>1girl, cat ears<|identity:lax|><|input_end|>"
+    )
+
+
+def test_compose_prompt_v2_wrapper():
+    prompt = v2.compose_prompt(
+        prompt="1girl, cat ears",
+        copyright="vocaloid",
+        character="hatsune miku",
+        rating=v2.RatingTag.Sfw,
+        aspect_ratio=v2.AspectRatioTag.Tall,
+        length=v2.LengthTag.Long,
+        identity_level=v2.IdentityTag.Lax,
+    )
+
+    assert prompt is not None
+    assert prompt == (
+        f"<|bos|>"
+        f"<copyright>vocaloid</copyright>"
+        f"<character>hatsune miku</character>"
+        f"<|rating:sfw|><|aspect_ratio:tall|><|length:long|>"
+        f"<general>1girl, cat ears<|identity:lax|><|input_end|>"
+    )
```

### Comparing `dartrs-0.1.0/Cargo.lock` & `dartrs-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 dependencies = [
  "derive_arbitrary",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bindgen_cuda"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f8489af5b7d17a81bffe37e0f4d6e1e4de87c87329d05447f22c35d95a1227d"
 dependencies = [
@@ -113,15 +113,15 @@
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "candle-core"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#89f53b9d7b36bbc0f555cd3c9882d21f84b2e13f"
+source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
 dependencies = [
  "byteorder",
  "candle-kernels",
  "cudarc",
  "gemm",
  "half",
  "memmap2",
@@ -135,37 +135,37 @@
  "yoke",
  "zip",
 ]
 
 [[package]]
 name = "candle-kernels"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#89f53b9d7b36bbc0f555cd3c9882d21f84b2e13f"
+source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-nn"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#89f53b9d7b36bbc0f555cd3c9882d21f84b2e13f"
+source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
 dependencies = [
  "candle-core",
  "half",
  "num-traits",
  "rayon",
  "safetensors",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
 version = "0.5.1"
-source = "git+https://github.com/huggingface/candle.git#89f53b9d7b36bbc0f555cd3c9882d21f84b2e13f"
+source = "git+https://github.com/huggingface/candle.git#01794dc16ef8d896933d61e9bd9b8a981cd51930"
 dependencies = [
  "byteorder",
  "candle-core",
  "candle-nn",
  "fancy-regex",
  "num-traits",
  "rand",
@@ -174,17 +174,17 @@
  "serde_json",
  "serde_plain",
  "tracing",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -299,15 +299,15 @@
  "darling_core",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "dartrs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "candle-core",
  "candle-nn",
  "candle-transformers",
  "hf-hub",
  "openssl",
@@ -378,14 +378,25 @@
  "libc",
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "displaydoc"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "dyn-stack"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56e53799688f5632f364f8fb387488dd05db9fe45db7011be066fc20e7027f8b"
 dependencies = [
  "bytemuck",
  "reborrow",
@@ -412,14 +423,20 @@
  "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "equivalent"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
+
+[[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
@@ -449,17 +466,17 @@
 name = "fastrand"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "flate2"
-version = "1.0.29"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4556222738635b7a3417ae6130d8f52201e45a0c4d1a907f0826383adb5f85e7"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -637,14 +654,20 @@
  "crunchy",
  "num-traits",
  "rand",
  "rand_distr",
 ]
 
 [[package]]
+name = "hashbrown"
+version = "0.14.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
@@ -682,14 +705,24 @@
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "indexmap"
+version = "2.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+dependencies = [
+ "equivalent",
+ "hashbrown",
+]
+
+[[package]]
 name = "indicatif"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "763a5a8f45087d6bcea4222e7b72c291a054edf80e4ef6efd2a4979878c7bea3"
 dependencies = [
  "console",
  "instant",
@@ -741,17 +774,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
@@ -900,17 +933,17 @@
 dependencies = [
  "bytemuck",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -919,14 +952,35 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "num_enum"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
+dependencies = [
+ "num_enum_derive",
+]
+
+[[package]]
+name = "num_enum_derive"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
+dependencies = [
+ "proc-macro-crate",
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
 
 [[package]]
 name = "once_cell"
@@ -986,17 +1040,17 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "300.1.6+3.1.4"
+version = "300.2.3+3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "439fac53e092cd7442a3660c85dde4643ab3b5bd39040912388dcdabf6b88085"
+checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
 version = "0.9.102"
@@ -1072,14 +1126,23 @@
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "proc-macro-crate"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
+dependencies = [
+ "toml_edit",
+]
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
@@ -1429,26 +1492,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1631,14 +1694,31 @@
  "thiserror",
  "unicode-normalization-alignments",
  "unicode-segmentation",
  "unicode_categories",
 ]
 
 [[package]]
+name = "toml_datetime"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+
+[[package]]
+name = "toml_edit"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
+dependencies = [
+ "indexmap",
+ "toml_datetime",
+ "winnow",
+]
+
+[[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
  "pin-project-lite",
  "tracing-attributes",
@@ -1727,15 +1807,15 @@
 
 [[package]]
 name = "ureq"
 version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
@@ -1932,14 +2012,23 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
+name = "winnow"
+version = "0.5.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "yoke"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "65e71b2e4f287f467794c671e2b8f8a5f3716b3c829079a1c44740148eff07e4"
 dependencies = [
  "serde",
  "stable_deref_trait",
@@ -1984,16 +2073,19 @@
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 
 [[package]]
 name = "zip"
-version = "1.1.2"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a23468b4a7a4e9e1e62812f8d1dd614f67f148e2b3faa72f4843bf00b573fd7"
+checksum = "9cc23c04387f4da0374be4533ad1208cbb091d5c11d070dfef13676ad6497164"
 dependencies = [
  "arbitrary",
- "byteorder",
  "crc32fast",
  "crossbeam-utils",
+ "displaydoc",
+ "indexmap",
+ "num_enum",
+ "thiserror",
 ]
```

