# Comparing `tmp/tantivy-0.21.0.tar.gz` & `tmp/tantivy-0.22.0.tar.gz`

## Comparing `tantivy-0.21.0.tar` & `tantivy-0.22.0.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 tantivy-0.21.0/Cargo.toml
--rw-r--r--   0     1001      127      110 2023-11-21 00:16:39.000000 tantivy-0.21.0/.cargo/config.toml
--rw-r--r--   0     1001      127      110 2023-11-21 00:16:39.000000 tantivy-0.21.0/.github/dependabot.yaml
--rw-r--r--   0     1001      127     2280 2023-11-21 00:16:39.000000 tantivy-0.21.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     2982 2023-11-21 00:16:39.000000 tantivy-0.21.0/.github/workflows/codeql.yml
--rw-r--r--   0     1001      127     6246 2023-11-21 00:16:39.000000 tantivy-0.21.0/.github/workflows/publish.yaml
--rw-r--r--   0     1001      127     2856 2023-11-21 00:16:39.000000 tantivy-0.21.0/.github/workflows/scorecards.yml
--rw-r--r--   0     1001      127      148 2023-11-21 00:16:39.000000 tantivy-0.21.0/.gitignore
--rw-r--r--   0     1001      127      839 2023-11-21 00:16:39.000000 tantivy-0.21.0/.readthedocs.yaml
--rw-r--r--   0     1001      127     1086 2023-11-21 00:16:39.000000 tantivy-0.21.0/LICENSE
--rw-r--r--   0     1001      127       83 2023-11-21 00:16:39.000000 tantivy-0.21.0/MANIFEST.in
--rw-r--r--   0     1001      127      505 2023-11-21 00:16:39.000000 tantivy-0.21.0/Makefile
--rw-r--r--   0     1001      127     5363 2023-11-21 00:16:39.000000 tantivy-0.21.0/README.md
--rw-r--r--   0     1001      127       71 2023-11-21 00:16:39.000000 tantivy-0.21.0/build.rs
--rwxr-xr-x   0     1001      127      236 2023-11-21 00:16:39.000000 tantivy-0.21.0/ci/deploy.sh
--rwxr-xr-x   0     1001      127      148 2023-11-21 00:16:39.000000 tantivy-0.21.0/ci/deploy_mac.sh
--rw-r--r--   0     1001      127        8 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/about.md
--rw-r--r--   0     1001      127       14 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/explanation.md
--rw-r--r--   0     1001      127     4452 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/howto.md
--rw-r--r--   0     1001      127     1158 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/index.md
--rw-r--r--   0     1001      127     1390 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/reference.md
--rw-r--r--   0     1001      127       14 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/requirements.txt
--rw-r--r--   0     1001      127     2357 2023-11-21 00:16:39.000000 tantivy-0.21.0/docs/tutorials.md
--rw-r--r--   0     1001      127      398 2023-11-21 00:16:39.000000 tantivy-0.21.0/mkdocs.yml
--rw-r--r--   0     1001      127      237 2023-11-21 00:16:39.000000 tantivy-0.21.0/noxfile.py
--rw-r--r--   0     1001      127       20 2023-11-21 00:16:39.000000 tantivy-0.21.0/requirements-dev.txt
--rw-r--r--   0     1001      127       31 2023-11-21 00:16:39.000000 tantivy-0.21.0/rust-toolchain.toml
--rw-r--r--   0     1001      127       14 2023-11-21 00:16:39.000000 tantivy-0.21.0/rustfmt.toml
--rw-r--r--   0     1001      127    28239 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/document.rs
--rw-r--r--   0     1001      127     3207 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/facet.rs
--rw-r--r--   0     1001      127    18905 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/index.rs
--rw-r--r--   0     1001      127     5385 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/lib.rs
--rw-r--r--   0     1001      127    26904 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/parser_error.rs
--rw-r--r--   0     1001      127      383 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/query.rs
--rw-r--r--   0     1001      127     1326 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/schema.rs
--rw-r--r--   0     1001      127    17880 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/schemabuilder.rs
--rw-r--r--   0     1001      127    10536 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/searcher.rs
--rw-r--r--   0     1001      127     1956 2023-11-21 00:16:39.000000 tantivy-0.21.0/src/snippet.rs
--rw-r--r--   0     1001      127       22 2023-11-21 00:16:39.000000 tantivy-0.21.0/tantivy/__init__.py
--rw-r--r--   0     1001      127    30829 2023-11-21 00:16:39.000000 tantivy-0.21.0/tests/tantivy_test.py
--rw-r--r--   0     1001      127    40939 2023-11-21 00:16:39.000000 tantivy-0.21.0/Cargo.lock
--rw-r--r--   0     1001      127      610 2023-11-21 00:16:39.000000 tantivy-0.21.0/pyproject.toml
--rw-r--r--   0        0        0     5695 1970-01-01 00:00:00.000000 tantivy-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 tantivy-0.22.0/Cargo.toml
+-rw-r--r--   0     1001      127      110 2024-05-05 14:04:07.000000 tantivy-0.22.0/.cargo/config.toml
+-rw-r--r--   0     1001      127      190 2024-05-05 14:04:07.000000 tantivy-0.22.0/.github/dependabot.yaml
+-rw-r--r--   0     1001      127     2753 2024-05-05 14:04:07.000000 tantivy-0.22.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     2982 2024-05-05 14:04:07.000000 tantivy-0.22.0/.github/workflows/codeql.yml
+-rw-r--r--   0     1001      127     7008 2024-05-05 14:04:07.000000 tantivy-0.22.0/.github/workflows/publish.yaml
+-rw-r--r--   0     1001      127     2856 2024-05-05 14:04:07.000000 tantivy-0.22.0/.github/workflows/scorecards.yml
+-rw-r--r--   0     1001      127      148 2024-05-05 14:04:07.000000 tantivy-0.22.0/.gitignore
+-rw-r--r--   0     1001      127      839 2024-05-05 14:04:07.000000 tantivy-0.22.0/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1086 2024-05-05 14:04:07.000000 tantivy-0.22.0/LICENSE
+-rw-r--r--   0     1001      127       83 2024-05-05 14:04:07.000000 tantivy-0.22.0/MANIFEST.in
+-rw-r--r--   0     1001      127      913 2024-05-05 14:04:07.000000 tantivy-0.22.0/README.md
+-rw-r--r--   0     1001      127       71 2024-05-05 14:04:07.000000 tantivy-0.22.0/build.rs
+-rwxr-xr-x   0     1001      127      236 2024-05-05 14:04:07.000000 tantivy-0.22.0/ci/deploy.sh
+-rwxr-xr-x   0     1001      127      148 2024-05-05 14:04:07.000000 tantivy-0.22.0/ci/deploy_mac.sh
+-rw-r--r--   0     1001      127        8 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/about.md
+-rw-r--r--   0     1001      127     1332 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/explanation.md
+-rw-r--r--   0     1001      127     4452 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/howto.md
+-rw-r--r--   0     1001      127     1158 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/index.md
+-rw-r--r--   0     1001      127     3202 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/reference.md
+-rw-r--r--   0     1001      127       32 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/requirements.txt
+-rw-r--r--   0     1001      127     6766 2024-05-05 14:04:07.000000 tantivy-0.22.0/docs/tutorials.md
+-rw-r--r--   0     1001      127      398 2024-05-05 14:04:07.000000 tantivy-0.22.0/mkdocs.yml
+-rw-r--r--   0     1001      127      245 2024-05-05 14:04:07.000000 tantivy-0.22.0/noxfile.py
+-rw-r--r--   0     1001      127       38 2024-05-05 14:04:07.000000 tantivy-0.22.0/requirements-dev.txt
+-rw-r--r--   0     1001      127       31 2024-05-05 14:04:07.000000 tantivy-0.22.0/rust-toolchain.toml
+-rw-r--r--   0     1001      127       14 2024-05-05 14:04:07.000000 tantivy-0.22.0/rustfmt.toml
+-rw-r--r--   0     1001      127    28435 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/document.rs
+-rw-r--r--   0     1001      127     3215 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/facet.rs
+-rw-r--r--   0     1001      127    21248 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/index.rs
+-rw-r--r--   0     1001      127     6481 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/lib.rs
+-rw-r--r--   0     1001      127    27209 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/parser_error.rs
+-rw-r--r--   0     1001      127    10897 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/query.rs
+-rw-r--r--   0     1001      127     1334 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/schema.rs
+-rw-r--r--   0     1001      127    19514 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/schemabuilder.rs
+-rw-r--r--   0     1001      127    10942 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/searcher.rs
+-rw-r--r--   0     1001      127     2123 2024-05-05 14:04:07.000000 tantivy-0.22.0/src/snippet.rs
+-rw-r--r--   0     1001      127       22 2024-05-05 14:04:07.000000 tantivy-0.22.0/tantivy/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-05 14:04:07.000000 tantivy-0.22.0/tantivy/py.typed
+-rw-r--r--   0     1001      127     8491 2024-05-05 14:04:07.000000 tantivy-0.22.0/tantivy/tantivy.pyi
+-rw-r--r--   0     1001      127     7055 2024-05-05 14:04:07.000000 tantivy-0.22.0/tests/conftest.py
+-rw-r--r--   0     1001      127    42774 2024-05-05 14:04:07.000000 tantivy-0.22.0/tests/tantivy_test.py
+-rw-r--r--   0     1001      127      221 2024-05-05 14:04:07.000000 tantivy-0.22.0/tests/test_docs.py
+-rw-r--r--   0     1001      127     1150 2024-05-05 14:04:07.000000 tantivy-0.22.0/tests/test_escapes.py
+-rw-r--r--   0     1001      127    44557 2024-05-05 14:04:07.000000 tantivy-0.22.0/Cargo.lock
+-rw-r--r--   0     1001      127      610 2024-05-05 14:04:07.000000 tantivy-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0     1245 1970-01-01 00:00:00.000000 tantivy-0.22.0/PKG-INFO
```

### Comparing `tantivy-0.21.0/.github/workflows/codeql.yml` & `tantivy-0.22.0/.github/workflows/codeql.yml`

 * *Files 20% similar despite different names*

```diff
@@ -26,53 +26,53 @@
       matrix:
         language: ["python"]
         # CodeQL supports [ $supported-codeql-languages ]
         # Learn more about CodeQL language support at https://aka.ms/codeql-docs/language-support
 
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895 # v2.2.1
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.2.1
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             files.pythonhosted.org:443
             objects.githubusercontent.com:443
             github.com:443
             pypi.org:443
             uploads.github.com:443
 
       - name: Checkout repository
-        uses: actions/checkout@ac593985615ec2ede58e132d2e21d2b1cbd6127c # v3.3.0
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
 
       # Initializes the CodeQL tools for scanning.
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@66b90a5db151a8042fa97405c6cf843bbe433f7b # v2.2.5
+        uses: github/codeql-action/init@d39d31e687223d841ef683f52467bd88e9b21c14 # v2.2.5
         with:
           languages: ${{ matrix.language }}
           # If you wish to specify custom queries, you can do so here or in a config file.
           # By default, queries listed here will override any specified in a config file.
           # Prefix the list here with "+" to use these queries and those in the config file.
 
           # Details on CodeQL's query packs refer to : https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs
           # queries: security-extended,security-and-quality
 
       # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
       # If this step fails, then you should remove it and run the build manually (see below)
       - name: Autobuild
-        uses: github/codeql-action/autobuild@66b90a5db151a8042fa97405c6cf843bbe433f7b # v2.2.5
+        uses: github/codeql-action/autobuild@d39d31e687223d841ef683f52467bd88e9b21c14 # v2.2.5
 
       # ℹ️ Command-line programs to run using the OS shell.
       # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
       #   If the Autobuild fails above, remove it and uncomment the following three lines.
       #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
       # - run: |
       #   echo "Run, Build Application using script"
       #   ./location_of_script_within_repo/buildscript.sh
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@66b90a5db151a8042fa97405c6cf843bbe433f7b # v2.2.5
+        uses: github/codeql-action/analyze@d39d31e687223d841ef683f52467bd88e9b21c14 # v2.2.5
         with:
           category: "/language:${{matrix.language}}"
```

### Comparing `tantivy-0.21.0/.github/workflows/publish.yaml` & `tantivy-0.22.0/.github/workflows/publish.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,195 +1,213 @@
 name: Test & Release
 
 on:
   release:
     types: [published]
 
-# on:
-#   pull_request:
-#     branches:
-#       - master
+  # pull_request:
+  #   branches:
+  #     - master
+
+permissions:
+  contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write  # ability to mint the OIDC token permission is necessary to persist the attestation
+      contents: read
+      attestations: write  # persist the attestation
     strategy:
       matrix:
         platform: [ 'x86_64-unknown-linux-gnu', 'aarch64-unknown-linux-gnu' ]
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4
         with:
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             cdn.quay.io:443
             cdn01.quay.io:443
             cdn02.quay.io:443
             cdn03.quay.io:443
             crates.io:443
             files.pythonhosted.org:443
             ghcr.io:443
             github.com:443
             index.crates.io:443
             objects.githubusercontent.com:443
-            uploads.github.com:443
             pkg-containers.githubusercontent.com:443
             pypi.org:443
             quay.io:443
             sh.rustup.rs:443
             static.crates.io:443
             static.rust-lang.org:443
+            uploads.github.com:443
 
-      - uses: actions/checkout@61b9e3751b92087fd0b06925ba6dd6314e06f089
-      - uses: actions/setup-python@65d7f2d534ac1bc67fcd62888c5f4f3d2cb2b236
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: 3.8
           architecture: x64
 
-      - uses: PyO3/maturin-action@683eb33e2cda131da55757dbac7628b2ef22df2f
+      - uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31
         with:
           manylinux: auto
           target: ${{ matrix.platform }}
           command: build
           args: --release --sdist -o dist -i 3.8 3.9 3.10 3.11 3.12
 
       - name: Upload wheels
-        uses: actions/upload-artifact@a8a3f3ad30e3422c9c7b888a15615d19a852ae32  # 3.1.3
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808  # 4.3.3
         with:
-          name: wheels
+          name: wheels-linux-${{ matrix.platform }}
           path: dist
 
   windows:
     runs-on: windows-latest
+    permissions:
+      id-token: write  # ability to mint the OIDC token permission is necessary to persist the attestation
+      contents: read
+      attestations: write  # persist the attestation
     strategy:
       matrix:
         target: [x64]
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4
         with:
-          egress-policy: audit # TODO: change to 'egress-policy: block' after couple of runs
+          egress-policy: audit
 
-      - uses: actions/checkout@61b9e3751b92087fd0b06925ba6dd6314e06f089
-      - uses: actions/setup-python@65d7f2d534ac1bc67fcd62888c5f4f3d2cb2b236
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: ${{ matrix.python-version }}
 
-      - uses: PyO3/maturin-action@683eb33e2cda131da55757dbac7628b2ef22df2f
+      - uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31
         env:
           PYO3_PYTHON: python${{ matrix.python-version }}
         with:
           command: build
           args: --release -o dist
 
       - name: Upload wheels
-        uses: actions/upload-artifact@a8a3f3ad30e3422c9c7b888a15615d19a852ae32  # 3.1.3
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808  # 4.3.3
         with:
-          name: wheels
+          name: wheels-windows-${{ matrix.python-version }}-${{ matrix.target }}
           path: dist
 
   macos:
     runs-on: macos-latest
+    permissions:
+      id-token: write  # ability to mint the OIDC token permission is necessary to persist the attestation
+      contents: read
+      attestations: write  # persist the attestation
     strategy:
       matrix:
         python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
         target: ['universal2', 'x86_64-apple-darwin']
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4
         with:
           egress-policy: audit # TODO: change to 'egress-policy: block' after couple of runs
 
-      - uses: actions/checkout@61b9e3751b92087fd0b06925ba6dd6314e06f089
-      - uses: actions/setup-python@65d7f2d534ac1bc67fcd62888c5f4f3d2cb2b236
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b
+      - uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Build wheels - ${{ matrix.target }}
-        uses: PyO3/maturin-action@683eb33e2cda131da55757dbac7628b2ef22df2f
+        uses: PyO3/maturin-action@52b28abb0c6729beb388babfc348bf6ff5aaff31
         env:
           PYO3_PYTHON: python${{ matrix.python-version }}
         with:
           target: ${{ matrix.target }}
           command: build
           args: --release -o dist
 
       - name: Upload wheels
-        uses: actions/upload-artifact@a8a3f3ad30e3422c9c7b888a15615d19a852ae32  # 3.1.3
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808  # 4.3.3
         with:
-          name: wheels
+          name: wheels-macos-${{ matrix.python-version }}-${{ matrix.target }}
           path: dist
 
   python-release-github:
     runs-on: ubuntu-latest
     needs: [ macos, windows, linux ]
     permissions:
       contents: write # To add assets to a release.
+      checks: write
+      packages: write
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895 # v2.1.0
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.1.0
         with:
           disable-sudo: true
           egress-policy: block
           allowed-endpoints: >
             api.github.com:443
             github.com:443
             uploads.github.com:443
             static.rust-lang.org:443 
 
-      - uses: actions/checkout@ac593985615ec2ede58e132d2e21d2b1cbd6127c # v3.3.0
+      - uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
         with:
           ref: ${{ github.head_ref }}
 
-      - uses: dtolnay/rust-toolchain@439cf607258077187679211f12aa6f19af4a0af7
+      - uses: dtolnay/rust-toolchain@d8352f6b1d2e870bc5716e7a6d9b65c4cc244a1a
         with:
-          toolchain: 1.73.0
+          toolchain: "1.73.0"
 
       - name: Set up Python 3.8
-        uses: actions/setup-python@65d7f2d534ac1bc67fcd62888c5f4f3d2cb2b236 # v4.7.1
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d # v5.1.0
         with:
           python-version: 3.8
 
-      - uses: actions/download-artifact@9bc31d5ccc31df68ecc42ccf4149144866c47d8a # v3.0.2
+      - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e # v4.1.7
         with:
-          name: wheels
           path: wheels
+          pattern: wheels-*
+          merge-multiple: true
 
       - name: Upload release binaries
-        uses: alexellis/upload-assets@259de5111cb56966d046ced998941e93f91d2c93
+        uses: alexellis/upload-assets@13926a61cdb2cb35f5fdef1c06b8b591523236d3 # 0.4.1
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         with:
           asset_paths: '["./wheels/tantivy-*"]'
 
   release-pypy:
     name: Release
     runs-on: ubuntu-latest
     needs: [ macos, windows, linux ]
     permissions:
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - name: Harden Runner
-        uses: step-security/harden-runner@eb238b55efaa70779f274895e782ed17c84f2895
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4
         with:
-          egress-policy: audit # TODO: change to 'egress-policy: block' after couple of runs
+          egress-policy: audit
 
-      - uses: actions/download-artifact@9bc31d5ccc31df68ecc42ccf4149144866c47d8a # v3.0.2
+      - uses: actions/download-artifact@65a9edc5881444af0b9093a5e628f2fe47ea3b2e # v4.1.7
         with:
-          name: wheels
           path: wheels
+          pattern: wheels-*
+          merge-multiple: true
 
       - name: Publish package distributions to Test PyPI
-        uses: pypa/gh-action-pypi-publish@b7f401de30cb6434a1e19f805ff006643653240e # v1.8.10
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450 # v1.8.14
         with:
           repository-url: https://test.pypi.org/legacy/
           packages-dir: wheels/
           skip-existing: true
 
       - name: Publish package distributions to PyPI
         if: always()
-        uses: pypa/gh-action-pypi-publish@b7f401de30cb6434a1e19f805ff006643653240e # v1.8.10
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450 # v1.8.14
         with:
           packages-dir: wheels/
           skip-existing: true
```

### Comparing `tantivy-0.21.0/.github/workflows/scorecards.yml` & `tantivy-0.22.0/.github/workflows/scorecards.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       # Needed to upload the results to code-scanning dashboard.
       security-events: write
       # Needed to publish results and get a badge (see publish_results below).
       id-token: write
 
     steps:
       - name: "Checkout code"
-        uses: actions/checkout@93ea575cb5d8a053eaa0ac8fa3b40d7e05a33cc8 # v3.1.0
+        uses: actions/checkout@0ad4b8fadaa221de15dcec353f45205ec38ea70b # v4.1.4
         with:
           persist-credentials: false
 
       - name: "Run analysis"
         uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
         with:
           results_file: results.sarif
@@ -52,18 +52,18 @@
           #   - `publish_results` will always be set to `false`, regardless
           #     of the value entered here.
           publish_results: true
 
       # Upload the results as artifacts (optional). Commenting out will disable uploads of run results in SARIF
       # format to the repository Actions tab.
       - name: "Upload artifact"
-        uses: actions/upload-artifact@a8a3f3ad30e3422c9c7b888a15615d19a852ae32 # v3.1.3
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808 # v4.3.3
         with:
           name: SARIF file
           path: results.sarif
           retention-days: 5
 
       # Upload the results to GitHub's code scanning dashboard.
       - name: "Upload to code-scanning"
-        uses: github/codeql-action/upload-sarif@66b90a5db151a8042fa97405c6cf843bbe433f7b # v2.22.7
+        uses: github/codeql-action/upload-sarif@d39d31e687223d841ef683f52467bd88e9b21c14 # v3.25.3
         with:
           sarif_file: results.sarif
```

### Comparing `tantivy-0.21.0/.readthedocs.yaml` & `tantivy-0.22.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `tantivy-0.21.0/LICENSE` & `tantivy-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tantivy-0.21.0/docs/howto.md` & `tantivy-0.22.0/docs/howto.md`

 * *Files identical despite different names*

### Comparing `tantivy-0.21.0/docs/index.md` & `tantivy-0.22.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `tantivy-0.21.0/src/document.rs` & `tantivy-0.22.0/src/document.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,22 @@
         PyTimeAccess, PyTuple,
     },
     Python,
 };
 
 use chrono::{offset::TimeZone, NaiveDateTime, Utc};
 
-use tantivy::{self as tv, schema::Value};
+use tantivy::{self as tv, schema::document::OwnedValue as Value};
 
 use crate::{facet::Facet, schema::Schema, to_pyerr};
 use serde::{
     ser::SerializeMap, Deserialize, Deserializer, Serialize, Serializer,
 };
-use serde_json::Value as JsonValue;
 use std::{
-    collections::{BTreeMap, HashMap},
+    collections::BTreeMap,
     fmt,
     net::{IpAddr, Ipv6Addr},
     str::FromStr,
 };
 
 pub(crate) fn extract_value(any: &PyAny) -> PyResult<Value> {
     if let Ok(s) = any.extract::<String>() {
@@ -50,15 +49,15 @@
         return Ok(Value::Facet(facet.inner));
     }
     if let Ok(b) = any.extract::<Vec<u8>>() {
         return Ok(Value::Bytes(b));
     }
     if let Ok(dict) = any.downcast::<PyDict>() {
         if let Ok(json) = pythonize::depythonize(dict) {
-            return Ok(Value::JsonObject(json));
+            return Ok(Value::Object(json));
         }
     }
     Err(to_pyerr(format!("Value unsupported {any:?}")))
 }
 
 pub(crate) fn extract_value_for_type(
     any: &PyAny,
@@ -115,21 +114,21 @@
         tv::schema::Type::Bytes => Value::Bytes(
             any.extract::<Vec<u8>>()
                 .map_err(to_pyerr_for_type("Bytes", field_name, any))?,
         ),
         tv::schema::Type::Json => {
             if let Ok(json_str) = any.extract::<&str>() {
                 return serde_json::from_str(json_str)
-                    .map(Value::JsonObject)
+                    .map(Value::Object)
                     .map_err(to_pyerr_for_type("Json", field_name, any));
             }
 
-            Value::JsonObject(
+            Value::Object(
                 any.downcast::<PyDict>()
-                    .map(|dict| pythonize::depythonize(&dict))
+                    .map(|dict| pythonize::depythonize(dict))
                     .map_err(to_pyerr_for_type("Json", field_name, any))?
                     .map_err(to_pyerr_for_type("Json", field_name, any))?,
             )
         }
         tv::schema::Type::IpAddr => {
             let val = any
                 .extract::<&str>()
@@ -188,40 +187,28 @@
             any,
             field_type.value_type(),
             field_name,
         )?])
     }
 }
 
-fn value_to_object(val: &JsonValue, py: Python<'_>) -> PyObject {
-    match val {
-        JsonValue::Null => py.None(),
-        JsonValue::Bool(b) => b.to_object(py),
-        JsonValue::Number(n) => match n {
-            n if n.is_i64() => n.as_i64().to_object(py),
-            n if n.is_u64() => n.as_u64().to_object(py),
-            n if n.is_f64() => n.as_f64().to_object(py),
-            _ => panic!("number too large"),
-        },
-        JsonValue::String(s) => s.to_object(py),
-        JsonValue::Array(v) => {
-            let inner: Vec<_> =
-                v.iter().map(|x| value_to_object(x, py)).collect();
-            inner.to_object(py)
-        }
-        JsonValue::Object(m) => {
-            let inner: HashMap<_, _> =
-                m.iter().map(|(k, v)| (k, value_to_object(v, py))).collect();
-            inner.to_object(py)
-        }
+fn object_to_py(
+    py: Python,
+    obj: &BTreeMap<String, Value>,
+) -> PyResult<PyObject> {
+    let dict = PyDict::new(py);
+    for (k, v) in obj.iter() {
+        dict.set_item(k, value_to_py(py, v)?)?;
     }
+    Ok(dict.into())
 }
 
 fn value_to_py(py: Python, value: &Value) -> PyResult<PyObject> {
     Ok(match value {
+        Value::Null => py.None(),
         Value::Str(text) => text.into_py(py),
         Value::U64(num) => (*num).into_py(py),
         Value::I64(num) => (*num).into_py(py),
         Value::F64(num) => (*num).into_py(py),
         Value::Bytes(b) => b.to_object(py),
         Value::PreTokStr(_pretoken) => {
             // TODO implement me
@@ -239,40 +226,43 @@
                 utc.second(),
                 utc.microsecond(),
                 None,
             )?
             .into_py(py)
         }
         Value::Facet(f) => Facet { inner: f.clone() }.into_py(py),
-        Value::JsonObject(json_object) => {
-            let inner: HashMap<_, _> = json_object
-                .iter()
-                .map(|(k, v)| (k, value_to_object(v, py)))
-                .collect();
-            inner.to_object(py)
+        Value::Array(_arr) => {
+            // TODO implement me
+            unimplemented!();
         }
+        Value::Object(obj) => object_to_py(py, obj)?,
         Value::Bool(b) => b.into_py(py),
         Value::IpAddr(i) => (*i).to_string().into_py(py),
     })
 }
 
 fn value_to_string(value: &Value) -> String {
     match value {
+        Value::Null => format!("{:?}", value),
         Value::Str(text) => text.clone(),
         Value::U64(num) => format!("{num}"),
         Value::I64(num) => format!("{num}"),
         Value::F64(num) => format!("{num}"),
         Value::Bytes(bytes) => format!("{bytes:?}"),
         Value::Date(d) => format!("{d:?}"),
         Value::Facet(facet) => facet.to_string(),
         Value::PreTokStr(_pretok) => {
             // TODO implement me
             unimplemented!();
         }
-        Value::JsonObject(json_object) => {
+        Value::Array(arr) => {
+            let inner: Vec<_> = arr.iter().map(value_to_string).collect();
+            format!("{inner:?}")
+        }
+        Value::Object(json_object) => {
             serde_json::to_string(&json_object).unwrap()
         }
         Value::Bool(b) => format!("{b}"),
         Value::IpAddr(i) => format!("{}", *i),
     }
 }
 
@@ -304,14 +294,16 @@
 /// implementation, it uses tagging in its serialization and deserialization to differentiate
 /// between different integer types.
 ///
 /// [`BorrowedSerdeValue`] is often used for the serialization path, as owning the data is not
 /// necessary for serialization.
 #[derive(Deserialize, Serialize)]
 enum SerdeValue {
+    /// Null
+    Null,
     /// The str type is used for any text information.
     Str(String),
     /// Pre-tokenized str type,
     PreTokStr(tv::tokenizer::PreTokenizedString),
     /// Unsigned 64-bits Integer `u64`
     U64(u64),
     /// Signed 64-bits Integer `i64`
@@ -326,60 +318,68 @@
     )]
     /// Date/time with microseconds precision
     Date(tv::DateTime),
     /// Facet
     Facet(tv::schema::Facet),
     /// Arbitrarily sized byte array
     Bytes(Vec<u8>),
-    /// Json object value.
-    JsonObject(serde_json::Map<String, serde_json::Value>),
+    /// Array
+    Array(Vec<Value>),
+    /// Object value.
+    Object(BTreeMap<String, Value>),
     /// IpV6 Address. Internally there is no IpV4, it needs to be converted to `Ipv6Addr`.
     IpAddr(Ipv6Addr),
 }
 
 impl From<SerdeValue> for Value {
     fn from(value: SerdeValue) -> Self {
         match value {
+            SerdeValue::Null => Self::Null,
             SerdeValue::Str(v) => Self::Str(v),
             SerdeValue::PreTokStr(v) => Self::PreTokStr(v),
             SerdeValue::U64(v) => Self::U64(v),
             SerdeValue::I64(v) => Self::I64(v),
             SerdeValue::F64(v) => Self::F64(v),
             SerdeValue::Date(v) => Self::Date(v),
             SerdeValue::Facet(v) => Self::Facet(v),
             SerdeValue::Bytes(v) => Self::Bytes(v),
-            SerdeValue::JsonObject(v) => Self::JsonObject(v),
+            SerdeValue::Array(v) => Self::Array(v),
+            SerdeValue::Object(v) => Self::Object(v),
             SerdeValue::Bool(v) => Self::Bool(v),
             SerdeValue::IpAddr(v) => Self::IpAddr(v),
         }
     }
 }
 
 impl From<Value> for SerdeValue {
     fn from(value: Value) -> Self {
         match value {
+            Value::Null => Self::Null,
             Value::Str(v) => Self::Str(v),
             Value::PreTokStr(v) => Self::PreTokStr(v),
             Value::U64(v) => Self::U64(v),
             Value::I64(v) => Self::I64(v),
             Value::F64(v) => Self::F64(v),
             Value::Date(v) => Self::Date(v),
             Value::Facet(v) => Self::Facet(v),
             Value::Bytes(v) => Self::Bytes(v),
-            Value::JsonObject(v) => Self::JsonObject(v),
+            Value::Array(v) => Self::Array(v),
+            Value::Object(v) => Self::Object(v),
             Value::Bool(v) => Self::Bool(v),
             Value::IpAddr(v) => Self::IpAddr(v),
         }
     }
 }
 
 /// A non-owning version of [`SerdeValue`]. This is used in serialization to avoid unnecessary
 /// cloning.
 #[derive(Serialize)]
 enum BorrowedSerdeValue<'a> {
+    /// Null
+    Null,
     /// The str type is used for any text information.
     Str(&'a str),
     /// Pre-tokenized str type,
     PreTokStr(&'a tv::tokenizer::PreTokenizedString),
     /// Unsigned 64-bits Integer `u64`
     U64(&'a u64),
     /// Signed 64-bits Integer `i64`
@@ -391,32 +391,36 @@
     #[serde(serialize_with = "serialize_datetime")]
     /// Date/time with microseconds precision
     Date(&'a tv::DateTime),
     /// Facet
     Facet(&'a tv::schema::Facet),
     /// Arbitrarily sized byte array
     Bytes(&'a [u8]),
+    /// Array
+    Array(&'a Vec<Value>),
     /// Json object value.
-    JsonObject(&'a serde_json::Map<String, serde_json::Value>),
+    Object(&'a BTreeMap<String, Value>),
     /// IpV6 Address. Internally there is no IpV4, it needs to be converted to `Ipv6Addr`.
     IpAddr(&'a Ipv6Addr),
 }
 
 impl<'a> From<&'a Value> for BorrowedSerdeValue<'a> {
     fn from(value: &'a Value) -> Self {
         match value {
+            Value::Null => Self::Null,
             Value::Str(v) => Self::Str(v),
             Value::PreTokStr(v) => Self::PreTokStr(v),
             Value::U64(v) => Self::U64(v),
             Value::I64(v) => Self::I64(v),
             Value::F64(v) => Self::F64(v),
             Value::Date(v) => Self::Date(v),
             Value::Facet(v) => Self::Facet(v),
             Value::Bytes(v) => Self::Bytes(v),
-            Value::JsonObject(v) => Self::JsonObject(v),
+            Value::Array(v) => Self::Array(v),
+            Value::Object(v) => Self::Object(v),
             Value::Bool(v) => Self::Bool(v),
             Value::IpAddr(v) => Self::IpAddr(v),
         }
     }
 }
 
 /// Tantivy's Document is the object that can be indexed and then searched for.
@@ -459,15 +463,15 @@
 ///     ...         .add_float_field("float")
 ///     ...         .build()
 ///     ... )
 ///     >>> doc = tantivy.Document.from_dict(
 ///     ...     {"unsigned": 1000, "signed": -5, "float": 0.4},
 ///     ...     schema,
 ///     ... )
-#[pyclass(module = "tantivy")]
+#[pyclass(module = "tantivy.tantivy")]
 #[derive(Clone, Default, PartialEq)]
 pub(crate) struct Document {
     pub(crate) field_values: BTreeMap<String, Vec<Value>>,
 }
 
 impl fmt::Debug for Document {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
@@ -555,16 +559,15 @@
     }
 
     #[staticmethod]
     fn from_dict(
         py_dict: &PyDict,
         schema: Option<&Schema>,
     ) -> PyResult<Document> {
-        let mut field_values: BTreeMap<String, Vec<tv::schema::Value>> =
-            BTreeMap::new();
+        let mut field_values: BTreeMap<String, Vec<Value>> = BTreeMap::new();
         Document::extract_py_values_from_dict(
             py_dict,
             schema,
             &mut field_values,
         )?;
         Ok(Document { field_values })
     }
@@ -670,27 +673,36 @@
     /// Args:
     ///     field_name (str): The field for which we are adding the bytes.
     ///     value (bytes): The bytes that will be added to the document.
     fn add_bytes(&mut self, field_name: String, bytes: Vec<u8>) {
         self.add_value(field_name, bytes);
     }
 
-    /// Add a bytes value to the document.
+    /// Add a JSON value to the document.
     ///
     /// Args:
     ///     field_name (str): The field for which we are adding the bytes.
-    ///     value (str): The json object that will be added to the document.
+    ///     value (str | Dict[str, Any]): The JSON object that will be added
+    ///         to the document.
     ///
-    /// Raises a ValueError if the json is invalid.
-    fn add_json(&mut self, field_name: String, json: &str) -> PyResult<()> {
-        let json_object: serde_json::Value =
-            serde_json::from_str(json).map_err(to_pyerr)?;
-        self.add_value(field_name, json_object);
-
-        Ok(())
+    /// Raises a ValueError if the JSON is invalid.
+    fn add_json(&mut self, field_name: String, value: &PyAny) -> PyResult<()> {
+        type JsonMap = serde_json::Map<String, serde_json::Value>;
+
+        if let Ok(json_str) = value.extract::<&str>() {
+            let json_map: JsonMap =
+                serde_json::from_str(json_str).map_err(to_pyerr)?;
+            self.add_value(field_name, json_map);
+            Ok(())
+        } else if let Ok(json_map) = pythonize::depythonize::<JsonMap>(value) {
+            self.add_value(field_name, json_map);
+            Ok(())
+        } else {
+            Err(to_pyerr("Invalid JSON object. Expected valid JSON string or Dict[str, Any]."))
+        }
     }
 
     /// Returns the number of added fields that have been added to the document
     #[getter]
     fn num_fields(&self) -> usize {
         self.field_values.len()
     }
@@ -796,15 +808,15 @@
             .or_default()
             .push(Value::from(value));
     }
 
     fn extract_py_values_from_dict(
         py_dict: &PyDict,
         schema: Option<&Schema>,
-        out_field_values: &mut BTreeMap<String, Vec<tv::schema::Value>>,
+        out_field_values: &mut BTreeMap<String, Vec<Value>>,
     ) -> PyResult<()> {
         // TODO: Reserve when https://github.com/rust-lang/rust/issues/72631 is stable.
         // out_field_values.reserve(py_dict.len());
 
         for key_value_any in py_dict.items() {
             if let Ok(key_value) = key_value_any.downcast::<PyTuple>() {
                 if key_value.len() != 2 {
```

### Comparing `tantivy-0.21.0/src/facet.rs` & `tantivy-0.22.0/src/facet.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 /// They are typically represented similarly to a filepath. For instance, an
 /// e-commerce website could have a Facet for /electronics/tv_and_video/led_tv.
 ///
 /// A document can be associated to any number of facets. The hierarchy
 /// implicitely imply that a document belonging to a facet also belongs to the
 /// ancestor of its facet. In the example above, /electronics/tv_and_video/
 /// and /electronics.
-#[pyclass(frozen, module = "tantivy")]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 #[derive(Clone, Deserialize, PartialEq, Serialize)]
 pub(crate) struct Facet {
     pub(crate) inner: schema::Facet,
 }
 
 #[pymethods]
 impl Facet {
```

### Comparing `tantivy-0.21.0/src/index.rs` & `tantivy-0.22.0/src/index.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 #![allow(clippy::new_ret_no_self)]
 
+use std::collections::HashMap;
+
 use pyo3::{exceptions, prelude::*, types::PyAny};
 
 use crate::{
     document::{extract_value, Document},
     get_field,
     parser_error::QueryParserErrorIntoPy,
     query::Query,
     schema::Schema,
     searcher::Searcher,
     to_pyerr,
 };
 use tantivy as tv;
 use tantivy::{
     directory::MmapDirectory,
-    schema::{NamedFieldDocument, Term, Value},
+    schema::{
+        document::TantivyDocument, NamedFieldDocument, OwnedValue as Value,
+        Term,
+    },
     tokenizer::{
         Language, LowerCaser, RemoveLongFilter, SimpleTokenizer, Stemmer,
         TextAnalyzer,
     },
 };
 
 const RELOAD_POLICY: &str = "commit";
 
 /// IndexWriter is the user entry-point to add documents to the index.
 ///
 /// To create an IndexWriter first create an Index and call the writer() method
 /// on the index object.
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct IndexWriter {
     inner_index_writer: Option<tv::IndexWriter>,
     schema: tv::schema::Schema,
 }
 
 impl IndexWriter {
     fn inner(&self) -> PyResult<&tv::IndexWriter> {
@@ -67,28 +72,30 @@
     ///
     /// Returns an `opstamp`, which is an increasing integer that can be used
     /// by the client to align commits with its own document queue.
     /// The `opstamp` represents the number of documents that have been added
     /// since the creation of the index.
     pub fn add_document(&mut self, doc: &Document) -> PyResult<u64> {
         let named_doc = NamedFieldDocument(doc.field_values.clone());
-        let doc = self.schema.convert_named_doc(named_doc).map_err(to_pyerr)?;
+        let doc = TantivyDocument::convert_named_doc(&self.schema, named_doc)
+            .map_err(to_pyerr)?;
         self.inner()?.add_document(doc).map_err(to_pyerr)
     }
 
     /// Helper for the `add_document` method, but passing a json string.
     ///
     /// If the indexing pipeline is full, this call may block.
     ///
     /// Returns an `opstamp`, which is an increasing integer that can be used
     /// by the client to align commits with its own document queue.
     /// The `opstamp` represents the number of documents that have been added
     /// since the creation of the index.
     pub fn add_json(&mut self, json: &str) -> PyResult<u64> {
-        let doc = self.schema.parse_document(json).map_err(to_pyerr)?;
+        let doc = TantivyDocument::parse_json(&self.schema, json)
+            .map_err(to_pyerr)?;
         let opstamp = self.inner()?.add_document(doc);
         opstamp.map_err(to_pyerr)
     }
 
     /// Commits all of the pending changes
     ///
     /// A call to commit blocks. After it returns, all of the document that
@@ -148,14 +155,19 @@
         &mut self,
         field_name: &str,
         field_value: &PyAny,
     ) -> PyResult<u64> {
         let field = get_field(&self.schema, field_name)?;
         let value = extract_value(field_value)?;
         let term = match value {
+            Value::Null => {
+                return Err(exceptions::PyValueError::new_err(format!(
+                    "Field `{field_name}` is null type not deletable."
+                )))
+            },
             Value::Str(text) => Term::from_field_text(field, &text),
             Value::U64(num) => Term::from_field_u64(field, num),
             Value::I64(num) => Term::from_field_i64(field, num),
             Value::F64(num) => Term::from_field_f64(field, num),
             Value::Date(d) => Term::from_field_date(field, d),
             Value::Facet(facet) => Term::from_facet(field, &facet),
             Value::Bytes(_) => {
@@ -164,15 +176,20 @@
                 )))
             }
             Value::PreTokStr(_pretok) => {
                 return Err(exceptions::PyValueError::new_err(format!(
                     "Field `{field_name}` is pretokenized. This is not authorized for delete."
                 )))
             }
-            Value::JsonObject(_) => {
+            Value::Array(_) => {
+                return Err(exceptions::PyValueError::new_err(format!(
+                    "Field `{field_name}` is array type not deletable."
+                )))
+            }
+            Value::Object(_) => {
                 return Err(exceptions::PyValueError::new_err(format!(
                     "Field `{field_name}` is json object type not deletable."
                 )))
             },
             Value::Bool(b) => Term::from_field_bool(field, b),
             Value::IpAddr(i) => Term::from_field_ip_addr(field, i)
         };
@@ -196,15 +213,15 @@
 ///     path (str, optional): The path where the index should be stored. If
 ///         no path is provided, the index will be stored in memory.
 ///     reuse (bool, optional): Should we open an existing index if one exists
 ///         or always create a new one.
 ///
 /// If an index already exists it will be opened and reused. Raises OSError
 /// if there was a problem during the opening or creation of the index.
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct Index {
     pub(crate) index: tv::Index,
     reader: tv::IndexReader,
 }
 
 #[pymethods]
 impl Index {
@@ -291,17 +308,17 @@
     fn config_reader(
         &mut self,
         reload_policy: &str,
         num_warmers: usize,
     ) -> Result<(), PyErr> {
         let reload_policy = reload_policy.to_lowercase();
         let reload_policy = match reload_policy.as_ref() {
-            "commit" => tv::ReloadPolicy::OnCommit,
-            "on-commit" => tv::ReloadPolicy::OnCommit,
-            "oncommit" => tv::ReloadPolicy::OnCommit,
+            "commit" => tv::ReloadPolicy::OnCommitWithDelay,
+            "on-commit" => tv::ReloadPolicy::OnCommitWithDelay,
+            "oncommit" => tv::ReloadPolicy::OnCommitWithDelay,
             "manual" => tv::ReloadPolicy::Manual,
             _ => return Err(exceptions::PyValueError::new_err(
                 "Invalid reload policy, valid choices are: 'manual' and 'OnCommit'"
             ))
         };
         let builder = self.index.reader_builder();
         let builder = builder.reload_policy(reload_policy);
@@ -354,124 +371,155 @@
         self.reader.reload().map_err(to_pyerr)
     }
 
     /// Parse a query
     ///
     /// Args:
     ///     query: the query, following the tantivy query language.
+    ///
     ///     default_fields_names (List[Field]): A list of fields used to search if no
     ///         field is specified in the query.
     ///
-    #[pyo3(signature = (query, default_field_names = None))]
+    ///     field_boosts: A dictionary keyed on field names which provides default boosts
+    ///         for the query constructed by this method.
+    ///
+    ///     fuzzy_fields: A dictionary keyed on field names which provides (prefix, distance, transpose_cost_one)
+    ///         triples making queries constructed by this method fuzzy against the given fields
+    ///         and using the given parameters.
+    ///         `prefix` determines if terms which are prefixes of the given term match the query.
+    ///         `distance` determines the maximum Levenshtein distance between terms matching the query and the given term.
+    ///         `transpose_cost_one` determines if transpositions of neighbouring characters are counted only once against the Levenshtein distance.
+    #[pyo3(signature = (query, default_field_names = None, field_boosts = HashMap::new(), fuzzy_fields = HashMap::new()))]
     pub fn parse_query(
         &self,
         query: &str,
         default_field_names: Option<Vec<String>>,
+        field_boosts: HashMap<String, tv::Score>,
+        fuzzy_fields: HashMap<String, (bool, u8, bool)>,
     ) -> PyResult<Query> {
-        let mut default_fields = vec![];
-        let schema = self.index.schema();
-        if let Some(default_field_names_vec) = default_field_names {
-            for default_field_name in &default_field_names_vec {
-                if let Ok(field) = schema.get_field(default_field_name) {
-                    let field_entry = schema.get_field_entry(field);
-                    if !field_entry.is_indexed() {
-                        return Err(exceptions::PyValueError::new_err(
-                            format!(
-                            "Field `{default_field_name}` is not set as indexed in the schema."
-                        ),
-                        ));
-                    }
-                    default_fields.push(field);
-                } else {
-                    return Err(exceptions::PyValueError::new_err(format!(
-                        "Field `{default_field_name}` is not defined in the schema."
-                    )));
-                }
-            }
-        } else {
-            for (field, field_entry) in self.index.schema().fields() {
-                if field_entry.is_indexed() {
-                    default_fields.push(field);
-                }
-            }
-        }
-        let parser =
-            tv::query::QueryParser::for_index(&self.index, default_fields);
+        let parser = self.prepare_query_parser(
+            default_field_names,
+            field_boosts,
+            fuzzy_fields,
+        )?;
+
         let query = parser.parse_query(query).map_err(to_pyerr)?;
 
         Ok(Query { inner: query })
     }
 
     /// Parse a query leniently.
     ///
     /// This variant parses invalid query on a best effort basis. If some part of the query can't
     /// reasonably be executed (range query without field, searching on a non existing field,
     /// searching without precising field when no default field is provided...), they may get turned
     /// into a "match-nothing" subquery.
     ///
     /// Args:
     ///     query: the query, following the tantivy query language.
+    ///
     ///     default_fields_names (List[Field]): A list of fields used to search if no
     ///         field is specified in the query.
     ///
+    ///     field_boosts: A dictionary keyed on field names which provides default boosts
+    ///         for the query constructed by this method.
+    ///
+    ///     fuzzy_fields: A dictionary keyed on field names which provides (prefix, distance, transpose_cost_one)
+    ///         triples making queries constructed by this method fuzzy against the given fields
+    ///         and using the given parameters.
+    ///         `prefix` determines if terms which are prefixes of the given term match the query.
+    ///         `distance` determines the maximum Levenshtein distance between terms matching the query and the given term.
+    ///         `transpose_cost_one` determines if transpositions of neighbouring characters are counted only once against the Levenshtein distance.
+    ///
     /// Returns a tuple containing the parsed query and a list of errors.
     ///
     /// Raises ValueError if a field in `default_field_names` is not defined or marked as indexed.
-    #[pyo3(signature = (query, default_field_names = None))]
+    #[pyo3(signature = (query, default_field_names = None, field_boosts = HashMap::new(), fuzzy_fields = HashMap::new()))]
     pub fn parse_query_lenient(
         &self,
         query: &str,
         default_field_names: Option<Vec<String>>,
+        field_boosts: HashMap<String, tv::Score>,
+        fuzzy_fields: HashMap<String, (bool, u8, bool)>,
+        py: Python,
     ) -> PyResult<(Query, Vec<PyObject>)> {
+        let parser = self.prepare_query_parser(
+            default_field_names,
+            field_boosts,
+            fuzzy_fields,
+        )?;
+
+        let (query, errors) = parser.parse_query_lenient(query);
+        let errors = errors.into_iter().map(|err| err.into_py(py)).collect();
+
+        Ok((Query { inner: query }, errors))
+    }
+}
+
+impl Index {
+    fn prepare_query_parser(
+        &self,
+        default_field_names: Option<Vec<String>>,
+        field_boosts: HashMap<String, tv::Score>,
+        fuzzy_fields: HashMap<String, (bool, u8, bool)>,
+    ) -> PyResult<tv::query::QueryParser> {
         let schema = self.index.schema();
 
-        let default_fields = if let Some(default_field_names_vec) =
+        let default_fields = if let Some(default_field_names) =
             default_field_names
         {
-            default_field_names_vec
-                .iter()
-                .map(|field_name| {
-                    schema
-                        .get_field(field_name)
-                        .map_err(|_err| {
-                            exceptions::PyValueError::new_err(format!(
-                                "Field `{field_name}` is not defined in the schema."
-                            ))
-                        })
-                        .and_then(|field| {
-                            schema.get_field_entry(field).is_indexed().then_some(field).ok_or(
-                                exceptions::PyValueError::new_err(
-                                    format!(
-                                        "Field `{field_name}` is not set as indexed in the schema."
-                                    ),
-                                ))
-                        })
-                }).collect::<Result<Vec<_>, _>>()?
+            default_field_names.iter().map(|field_name| {
+                let field = schema.get_field(field_name).map_err(|_err| {
+                    exceptions::PyValueError::new_err(format!(
+                        "Field `{field_name}` is not defined in the schema."
+                    ))
+                })?;
+
+                let field_entry = schema.get_field_entry(field);
+                if !field_entry.is_indexed() {
+                    return Err(exceptions::PyValueError::new_err(
+                        format!("Field `{field_name}` is not set as indexed in the schema.")
+                    ));
+                }
+
+                Ok(field)
+            }).collect::<PyResult<_>>()?
         } else {
-            self.index
-                .schema()
+            schema
                 .fields()
-                .filter_map(|(f, fe)| fe.is_indexed().then_some(f))
-                .collect::<Vec<_>>()
+                .filter(|(_, field_entry)| field_entry.is_indexed())
+                .map(|(field, _)| field)
+                .collect()
         };
 
-        let parser =
+        let mut parser =
             tv::query::QueryParser::for_index(&self.index, default_fields);
-        let (query, errors) = parser.parse_query_lenient(query);
 
-        Python::with_gil(|py| {
-            let errors =
-                errors.into_iter().map(|err| err.into_py(py)).collect();
+        for (field_name, boost) in field_boosts {
+            let field = schema.get_field(&field_name).map_err(|_err| {
+                exceptions::PyValueError::new_err(format!(
+                    "Field `{field_name}` is not defined in the schema."
+                ))
+            })?;
+            parser.set_field_boost(field, boost);
+        }
 
-            Ok((Query { inner: query }, errors))
-        })
+        for (field_name, (prefix, distance, transpose_cost_one)) in fuzzy_fields
+        {
+            let field = schema.get_field(&field_name).map_err(|_err| {
+                exceptions::PyValueError::new_err(format!(
+                    "Field `{field_name}` is not defined in the schema."
+                ))
+            })?;
+            parser.set_field_fuzzy(field, prefix, distance, transpose_cost_one);
+        }
+
+        Ok(parser)
     }
-}
 
-impl Index {
     fn register_custom_text_analyzers(index: &tv::Index) {
         let analyzers = [
             ("ar_stem", Language::Arabic),
             ("da_stem", Language::Danish),
             ("nl_stem", Language::Dutch),
             ("fi_stem", Language::Finnish),
             ("fr_stem", Language::French),
```

### Comparing `tantivy-0.21.0/src/lib.rs` & `tantivy-0.22.0/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use ::tantivy as tv;
+use ::tantivy::schema::{OwnedValue as Value, Term};
 use pyo3::{exceptions, prelude::*, wrap_pymodule};
 
 mod document;
 mod facet;
 mod index;
 mod parser_error;
 mod query;
@@ -10,20 +11,22 @@
 mod schemabuilder;
 mod searcher;
 mod snippet;
 
 use document::Document;
 use facet::Facet;
 use index::Index;
-use query::Query;
+use query::{Occur, Query};
 use schema::Schema;
 use schemabuilder::SchemaBuilder;
 use searcher::{DocAddress, Order, SearchResult, Searcher};
 use snippet::{Snippet, SnippetGenerator};
 
+use crate::document::extract_value;
+
 /// Python bindings for the search engine library Tantivy.
 ///
 /// Tantivy is a full text search engine library written in rust.
 ///
 /// It is closer to Apache Lucene than to Elasticsearch and Apache Solr in
 /// the sense it is not an off-the-shelf search engine server, but rather
 /// a library that can be used to build such a search engine.
@@ -80,14 +83,15 @@
     m.add_class::<Document>()?;
     m.add_class::<Index>()?;
     m.add_class::<DocAddress>()?;
     m.add_class::<Facet>()?;
     m.add_class::<Query>()?;
     m.add_class::<Snippet>()?;
     m.add_class::<SnippetGenerator>()?;
+    m.add_class::<Occur>()?;
 
     m.add_wrapped(wrap_pymodule!(query_parser_error))?;
 
     Ok(())
 }
 
 /// Submodule containing all the possible errors that can be raised during
@@ -149,7 +153,33 @@
         exceptions::PyValueError::new_err(format!(
             "Field `{field_name}` is not defined in the schema."
         ))
     })?;
 
     Ok(field)
 }
+
+pub(crate) fn make_term(
+    schema: &tv::schema::Schema,
+    field_name: &str,
+    field_value: &PyAny,
+) -> PyResult<tv::Term> {
+    let field = get_field(schema, field_name)?;
+    let value = extract_value(field_value)?;
+    let term = match value {
+        Value::Str(text) => Term::from_field_text(field, &text),
+        Value::U64(num) => Term::from_field_u64(field, num),
+        Value::I64(num) => Term::from_field_i64(field, num),
+        Value::F64(num) => Term::from_field_f64(field, num),
+        Value::Date(d) => Term::from_field_date(field, d),
+        Value::Facet(facet) => Term::from_facet(field, &facet),
+        Value::Bool(b) => Term::from_field_bool(field, b),
+        Value::IpAddr(i) => Term::from_field_ip_addr(field, i),
+        _ => {
+            return Err(exceptions::PyValueError::new_err(format!(
+                "Can't create a term for Field `{field_name}` with value `{field_value}`."
+            )))
+        }
+    };
+
+    Ok(term)
+}
```

### Comparing `tantivy-0.21.0/src/parser_error.rs` & `tantivy-0.22.0/src/parser_error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 IpFormatError { addr_parse_error }.into_py(py)
             }
         }
     }
 }
 
 /// Error in the query syntax.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct SyntaxError {
     message: String,
 }
 
 #[pymethods]
 impl SyntaxError {
     #[getter]
@@ -127,15 +127,15 @@
             }
             _ => Err(format!("{error} is not a SyntaxError")),
         }
     }
 }
 
 /// This query is unsupported.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct UnsupportedQueryError {
     message: String,
 }
 
 #[pymethods]
 impl UnsupportedQueryError {
     #[getter]
@@ -176,15 +176,15 @@
             }
             _ => Err(format!("{error} is not an UnsupportedQuery error")),
         }
     }
 }
 
 /// The query references a field that is not in the schema.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub struct FieldDoesNotExistError {
     field: String,
 }
 
 #[pymethods]
 impl FieldDoesNotExistError {
     /// The name of the field causing the error.
@@ -226,15 +226,15 @@
             }
             _ => Err(format!("{error} is not a FieldDoesNotExist error")),
         }
     }
 }
 
 /// The query contains a term for a `u64` or `i64`-field, but the value is neither.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct ExpectedIntError {
     parse_int_error: ParseIntError,
 }
 
 #[pymethods]
 impl ExpectedIntError {
     /// If `true`, the value being parsed was empty.
@@ -290,55 +290,49 @@
             }
             _ => Err(format!("{error} is not an ExpectedInt error")),
         }
     }
 }
 
 /// The query contains a term for a bytes field, but the value is not valid base64.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct ExpectedBase64Error {
     decode_error: base64::DecodeError,
 }
 
 #[pymethods]
 impl ExpectedBase64Error {
     /// If `true`, an invalid byte was found in the query. Padding characters (`=`) interspersed in
     /// the encoded form will be treated as invalid bytes.
     fn caused_by_invalid_byte(&self) -> bool {
-        match self.decode_error {
-            base64::DecodeError::InvalidByte { .. } => true,
-            _ => false,
-        }
+        matches!(self.decode_error, base64::DecodeError::InvalidByte { .. })
     }
 
     /// If the error was caused by an invalid byte, returns the offset and offending byte.
     fn invalid_byte_info(&self) -> Option<(usize, u8)> {
         match self.decode_error {
             base64::DecodeError::InvalidByte(position, byte) => {
                 Some((position, byte))
             }
             _ => None,
         }
     }
 
     /// If `true`, the length of the base64 string was invalid.
     fn caused_by_invalid_length(&self) -> bool {
-        match self.decode_error {
-            base64::DecodeError::InvalidLength => true,
-            _ => false,
-        }
+        matches!(self.decode_error, base64::DecodeError::InvalidLength(_))
     }
 
     /// The last non-padding input symbol's encoded 6 bits have nonzero bits that will be discarded.
     /// If `true`, this is indicative of corrupted or truncated Base64.
     fn caused_by_invalid_last_symbol(&self) -> bool {
-        match self.decode_error {
-            base64::DecodeError::InvalidLastSymbol { .. } => true,
-            _ => false,
-        }
+        matches!(
+            self.decode_error,
+            base64::DecodeError::InvalidLastSymbol { .. }
+        )
     }
 
     /// If the error was caused by an invalid last symbol, returns the offset and offending byte.
     fn invalid_last_symbol_info(&self) -> Option<(usize, u8)> {
         match self.decode_error {
             base64::DecodeError::InvalidLastSymbol(position, byte) => {
                 Some((position, byte))
@@ -346,18 +340,15 @@
             _ => None,
         }
     }
 
     /// The nature of the padding was not as configured: absent or incorrect when it must be
     /// canonical, or present when it must be absent, etc.
     fn caused_by_invalid_padding(&self) -> bool {
-        match self.decode_error {
-            base64::DecodeError::InvalidPadding => true,
-            _ => false,
-        }
+        matches!(self.decode_error, base64::DecodeError::InvalidPadding)
     }
 
     fn __repr__(&self) -> String {
         self.full_message()
     }
 
     fn __str__(&self) -> String {
@@ -389,15 +380,15 @@
             }
             _ => Err(format!("{error} is not an ExpectedBase64 error")),
         }
     }
 }
 
 /// The query contains a term for a `f64`-field, but the value is not a f64.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct ExpectedFloatError {
     parse_float_error: ParseFloatError,
 }
 
 #[pymethods]
 impl ExpectedFloatError {
     fn __repr__(&self) -> String {
@@ -433,15 +424,15 @@
             }
             _ => Err(format!("{error} is not an ExpectedFloat error")),
         }
     }
 }
 
 /// The query contains a term for a `bool`-field, but the value is not a bool.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct ExpectedBoolError {
     parse_bool_error: ParseBoolError,
 }
 
 #[pymethods]
 impl ExpectedBoolError {
     fn __repr__(&self) -> String {
@@ -477,15 +468,15 @@
             }
             _ => Err(format!("{error} is not an ExpectedBool error")),
         }
     }
 }
 
 /// It is forbidden queries that are only "excluding". (e.g. -title:pop)
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct AllButQueryForbiddenError;
 
 #[pymethods]
 impl AllButQueryForbiddenError {
     fn __repr__(&self) -> String {
         self.full_message()
     }
@@ -517,15 +508,15 @@
             tv::query::QueryParserError::AllButQueryForbidden => Ok(Self {}),
             _ => Err(format!("{error} is not an AllButQueryForbidden error")),
         }
     }
 }
 
 /// If no default field is declared, running a query without any field specified is forbbidden.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct NoDefaultFieldDeclaredError;
 
 #[pymethods]
 impl NoDefaultFieldDeclaredError {
     fn __repr__(&self) -> String {
         self.full_message()
     }
@@ -557,15 +548,15 @@
             tv::query::QueryParserError::NoDefaultFieldDeclared => Ok(Self {}),
             _ => Err(format!("{error} is not a NoDefaultFieldDeclared error")),
         }
     }
 }
 
 /// The field searched for is not declared as indexed in the schema.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct FieldNotIndexedError {
     field: String,
 }
 
 #[pymethods]
 impl FieldNotIndexedError {
     fn field(&self) -> &str {
@@ -605,15 +596,15 @@
             }
             _ => Err(format!("{error} is not an FieldNotIndexed error")),
         }
     }
 }
 
 /// A phrase query was requested for a field that does not have any positions indexed.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct FieldDoesNotHavePositionsIndexedError {
     field: String,
 }
 
 #[pymethods]
 impl FieldDoesNotHavePositionsIndexedError {
     fn field(&self) -> &str {
@@ -664,15 +655,15 @@
                 "{error} is not a FieldDoesNotHavePositionsIndexed error"
             )),
         }
     }
 }
 
 /// A phrase-prefix query requires at least two terms
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct PhrasePrefixRequiresAtLeastTwoTermsError {
     /// The phrase which triggered the issue.
     phrase: String,
     /// The tokenizer configured for the field.
     tokenizer: String,
 }
 
@@ -732,15 +723,15 @@
                 "{error} is not a PhrasePrefixRequiresAtLeastTwoTerms error"
             )),
         }
     }
 }
 
 /// The tokenizer for the given field is unknown.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct UnknownTokenizerError {
     /// The name of the tokenizer.
     tokenizer: String,
     /// The field name.
     field: String,
 }
 
@@ -795,15 +786,15 @@
             _ => Err(format!("{error} is not an UnknownTokenizer error")),
         }
     }
 }
 
 /// The query contains a range query with a phrase as one of the bounds. Only terms can be used as
 /// bounds.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct RangeMustNotHavePhraseError;
 
 #[pymethods]
 impl RangeMustNotHavePhraseError {
     fn __repr__(&self) -> String {
         self.full_message()
     }
@@ -835,15 +826,15 @@
             tv::query::QueryParserError::RangeMustNotHavePhrase => Ok(Self {}),
             _ => Err(format!("{error} is not a RangeMustNotHavePhrase error")),
         }
     }
 }
 
 /// The format for the date field is not RFC 3339 compliant.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct DateFormatError {
     // Keep around the entire `QueryParserError` to avoid importing the `time` crate.
     inner: tv::query::QueryParserError,
 }
 
 #[pymethods]
 impl DateFormatError {
@@ -880,15 +871,15 @@
             }
             _ => Err(format!("{error} is not a DateFormatError")),
         }
     }
 }
 
 /// The format for the facet field is invalid.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct FacetFormatError {
     facet_parse_error: FacetParseError,
 }
 
 #[pymethods]
 impl FacetFormatError {
     fn __repr__(&self) -> String {
@@ -924,15 +915,15 @@
             ) => Ok(Self { facet_parse_error }),
             _ => Err(format!("{error} is not a FacetFormatError")),
         }
     }
 }
 
 /// The format for the ip field is invalid.
-#[pyclass(frozen)]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 pub(crate) struct IpFormatError {
     addr_parse_error: AddrParseError,
 }
 
 #[pymethods]
 impl IpFormatError {
     fn __repr__(&self) -> String {
```

### Comparing `tantivy-0.21.0/src/schema.rs` & `tantivy-0.22.0/src/schema.rs`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use serde::{Deserialize, Serialize};
 use tantivy as tv;
 
 /// Tantivy schema.
 ///
 /// The schema is very strict. To build the schema the `SchemaBuilder` class is
 /// provided.
-#[pyclass(frozen, module = "tantivy")]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 #[derive(Deserialize, PartialEq, Serialize)]
 pub(crate) struct Schema {
     pub(crate) inner: tv::schema::Schema,
 }
 
 #[pymethods]
 impl Schema {
```

### Comparing `tantivy-0.21.0/src/schemabuilder.rs` & `tantivy-0.22.0/src/schemabuilder.rs`

 * *Files 9% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 ///
 ///     >>> builder = tantivy.SchemaBuilder()
 ///
 ///     >>> title = builder.add_text_field("title", stored=True)
 ///     >>> body = builder.add_text_field("body")
 ///
 ///     >>> schema = builder.build()
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 #[derive(Clone)]
 pub(crate) struct SchemaBuilder {
     pub(crate) builder: Arc<RwLock<Option<schema::SchemaBuilder>>>,
 }
 
+const NO_TOKENIZER_NAME: &str = "raw";
 const TOKENIZER: &str = "default";
 const RECORD: &str = "position";
 
 #[pymethods]
 impl SchemaBuilder {
     #[new]
     fn new() -> Self {
@@ -49,14 +50,22 @@
     /// Add a new text field to the schema.
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
+    ///     fast (bool, optional): Set the text options as a fast field. A
+    ///         fast field is a column-oriented fashion storage for tantivy.
+    ///         Text fast fields will have the term ids stored in the fast
+    ///         field. The fast field will be a multivalued fast field.
+    ///         It is recommended to use the "raw" tokenizer, since it will
+    ///         store the original text unchanged. The "default" tokenizer will
+    ///         store the terms as lower case and this will be reflected in the
+    ///         dictionary.
     ///     tokenizer_name (str, optional): The name of the tokenizer that
     ///         should be used to process the field. Defaults to 'default'
     ///     index_option (str, optional): Sets which information should be
     ///         indexed with the tokens. Can be one of 'position', 'freq' or
     ///         'basic'. Defaults to 'position'. The 'basic' index_option
     ///         records only the document ID, the 'freq' option records the
     ///         document id and the term frequency, while the 'position' option
@@ -64,27 +73,30 @@
     ///         the term occurrences in the document.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (
         name,
         stored = false,
+        fast = false,
         tokenizer_name = TOKENIZER,
         index_option = RECORD
     ))]
     fn add_text_field(
         &mut self,
         name: &str,
         stored: bool,
+        fast: bool,
         tokenizer_name: &str,
         index_option: &str,
     ) -> PyResult<Self> {
         let builder = &mut self.builder;
         let options = SchemaBuilder::build_text_option(
             stored,
+            fast,
             tokenizer_name,
             index_option,
         )?;
 
         if let Some(builder) = builder.write().unwrap().as_mut() {
             builder.add_text_field(name, options);
         } else {
@@ -99,15 +111,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the numeric options as a fast field. A
+    ///     fast (bool, optional): Set the numeric options as a fast field. A
     ///         fast field is a column-oriented fashion storage for tantivy.
     ///         It is designed for the fast random access of some document
     ///         fields given a document id.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (name, stored = false, indexed = false, fast = false))]
@@ -136,15 +148,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the numeric options as a fast field. A
+    ///     fast (bool, optional): Set the numeric options as a fast field. A
     ///         fast field is a column-oriented fashion storage for tantivy.
     ///         It is designed for the fast random access of some document
     ///         fields given a document id.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (name, stored = false, indexed = false, fast = false))]
@@ -173,15 +185,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the numeric options as a fast field. A
+    ///     fast (bool, optional): Set the numeric options as a fast field. A
     ///         fast field is a column-oriented fashion storage for tantivy.
     ///         It is designed for the fast random access of some document
     ///         fields given a document id.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (name, stored = false, indexed = false, fast = false))]
@@ -210,15 +222,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the numeric options as a fast field. A
+    ///     fast (bool, optional): Set the numeric options as a fast field. A
     ///         fast field is a column-oriented fashion storage for tantivy.
     ///         It is designed for the fast random access of some document
     ///         fields given a document id.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (name, stored = false, indexed = false, fast = false))]
@@ -247,15 +259,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the date options as a fast field. A fast
+    ///     fast (bool, optional): Set the date options as a fast field. A fast
     ///         field is a column-oriented fashion storage for tantivy. It is
     ///         designed for the fast random access of some document fields
     ///         given a document id.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (name, stored = false, indexed = false, fast = false))]
@@ -292,14 +304,22 @@
     /// Add a new json field to the schema.
     ///
     /// Args:
     ///     name (str): the name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
+    ///     fast (bool, optional): Set the text options as a fast field. A
+    ///         fast field is a column-oriented fashion storage for tantivy.
+    ///         Text fast fields will have the term ids stored in the fast
+    ///         field. The fast field will be a multivalued fast field.
+    ///         It is recommended to use the "raw" tokenizer, since it will
+    ///         store the original text unchanged. The "default" tokenizer will
+    ///         store the terms as lower case and this will be reflected in the
+    ///         dictionary.
     ///     tokenizer_name (str, optional): The name of the tokenizer that
     ///         should be used to process the field. Defaults to 'default'
     ///     index_option (str, optional): Sets which information should be
     ///         indexed with the tokens. Can be one of 'position', 'freq' or
     ///         'basic'. Defaults to 'position'. The 'basic' index_option
     ///         records only the document ID, the 'freq' option records the
     ///         document id and the term frequency, while the 'position' option
@@ -307,27 +327,30 @@
     ///         the term occurrences in the document.
     ///
     /// Returns the associated field handle.
     /// Raises a ValueError if there was an error with the field creation.
     #[pyo3(signature = (
         name,
         stored = false,
+        fast = false,
         tokenizer_name = TOKENIZER,
         index_option = RECORD
     ))]
     fn add_json_field(
         &mut self,
         name: &str,
         stored: bool,
+        fast: bool,
         tokenizer_name: &str,
         index_option: &str,
     ) -> PyResult<Self> {
         let builder = &mut self.builder;
         let options = SchemaBuilder::build_text_option(
             stored,
+            fast,
             tokenizer_name,
             index_option,
         )?;
 
         if let Some(builder) = builder.write().unwrap().as_mut() {
             builder.add_json_field(name, options);
         } else {
@@ -359,15 +382,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the bytes options as a fast field. A fast
+    ///     fast (bool, optional): Set the bytes options as a fast field. A fast
     ///         field is a column-oriented fashion storage for tantivy. It is
     ///         designed for the fast random access of some document fields
     ///         given a document id.
     #[pyo3(signature = (
         name,
         stored = false,
         indexed = false,
@@ -406,15 +429,15 @@
     ///
     /// Args:
     ///     name (str): The name of the field.
     ///     stored (bool, optional): If true sets the field as stored, the
     ///         content of the field can be later restored from a Searcher.
     ///         Defaults to False.
     ///     indexed (bool, optional): If true sets the field to be indexed.
-    ///     fast (str, optional): Set the IP address options as a fast field. A
+    ///     fast (bool, optional): Set the IP address options as a fast field. A
     ///         fast field is a column-oriented fashion storage for tantivy. It
     ///         is designed for the fast random access of some document fields
     ///         given a document id.
     #[pyo3(signature = (
         name,
         stored = false,
         indexed = false,
@@ -478,14 +501,15 @@
         let opts = if indexed { opts.set_indexed() } else { opts };
         let opts = if fast { opts.set_fast() } else { opts };
         Ok(opts)
     }
 
     fn build_text_option(
         stored: bool,
+        fast: bool,
         tokenizer_name: &str,
         index_option: &str,
     ) -> PyResult<schema::TextOptions> {
         let index_option = match index_option {
             "position" => schema::IndexRecordOption::WithFreqsAndPositions,
             "freq" => schema::IndexRecordOption::WithFreqs,
             "basic" => schema::IndexRecordOption::Basic,
@@ -502,10 +526,21 @@
             schema::TextOptions::default().set_indexing_options(indexing);
         let options = if stored {
             options.set_stored()
         } else {
             options
         };
 
+        let options = if fast {
+            let text_tokenizer = if tokenizer_name != NO_TOKENIZER_NAME {
+                Some(tokenizer_name)
+            } else {
+                None
+            };
+            options.set_fast(text_tokenizer)
+        } else {
+            options
+        };
+
         Ok(options)
     }
 }
```

### Comparing `tantivy-0.21.0/src/searcher.rs` & `tantivy-0.22.0/src/searcher.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 #![allow(clippy::new_ret_no_self)]
 
 use crate::{document::Document, query::Query, to_pyerr};
 use pyo3::{basic::CompareOp, exceptions::PyValueError, prelude::*};
 use serde::{Deserialize, Serialize};
 use tantivy as tv;
 use tantivy::collector::{Count, MultiCollector, TopDocs};
+use tantivy::TantivyDocument;
+// Bring the trait into scope. This is required for the `to_named_doc` method.
+// However, tantivy-py declares its own `Document` class, so we need to avoid
+// introduce the `Document` trait into the namespace.
+use tantivy::Document as _;
 
 /// Tantivy's Searcher class
 ///
 /// A Searcher is used to search the index given a prepared Query.
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct Searcher {
     pub(crate) inner: tv::Searcher,
 }
 
 #[derive(Clone, Deserialize, FromPyObject, PartialEq, Serialize)]
 enum Fruit {
     #[pyo3(transparent)]
@@ -36,15 +41,15 @@
         match self {
             Fruit::Score(s) => s.to_object(py),
             Fruit::Order(o) => o.to_object(py),
         }
     }
 }
 
-#[pyclass(frozen, module = "tantivy")]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 #[derive(Clone, Copy, Deserialize, PartialEq, Serialize)]
 /// Enum representing the direction in which something should be sorted.
 pub(crate) enum Order {
     /// Ascending. Smaller values appear first.
     Asc,
 
     /// Descending. Larger values appear first.
@@ -56,15 +61,15 @@
         match order {
             Order::Asc => tv::Order::Asc,
             Order::Desc => tv::Order::Desc,
         }
     }
 }
 
-#[pyclass(frozen, module = "tantivy")]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 #[derive(Clone, Default, Deserialize, PartialEq, Serialize)]
 /// Object holding a results successful search.
 pub(crate) struct SearchResult {
     hits: Vec<(Fruit, DocAddress)>,
     #[pyo3(get)]
     /// How many documents matched the query. Only available if `count` was set
     /// to true during the search.
@@ -149,14 +154,15 @@
     ///     order (Order, optional): The order in which the results
     ///         should be sorted. If not specified, defaults to descending.
     ///
     /// Returns `SearchResult` object.
     ///
     /// Raises a ValueError if there was an error with the search.
     #[pyo3(signature = (query, limit = 10, count = true, order_by_field = None, offset = 0, order = Order::Desc))]
+    #[allow(clippy::too_many_arguments)]
     fn search(
         &self,
         py: Python,
         query: &Query,
         limit: usize,
         count: bool,
         order_by_field: Option<&str>,
@@ -172,15 +178,15 @@
                 None
             };
 
             let (mut multifruit, hits) = {
                 if let Some(order_by) = order_by_field {
                     let collector = TopDocs::with_limit(limit)
                         .and_offset(offset)
-                        .order_by_fast_field(order_by, order.into());
+                        .order_by_u64_field(order_by, order.into());
                     let top_docs_handle =
                         multicollector.add_collector(collector);
                     let ret = self.inner.search(query.get(), &multicollector);
 
                     match ret {
                         Ok(mut r) => {
                             let top_docs = top_docs_handle.extract(&mut r);
@@ -243,17 +249,18 @@
     ///
     /// Args:
     ///     doc_address (DocAddress): The DocAddress that is associated with
     ///         the document that we wish to fetch.
     ///
     /// Returns the Document, raises ValueError if the document can't be found.
     fn doc(&self, doc_address: &DocAddress) -> PyResult<Document> {
-        let doc = self.inner.doc(doc_address.into()).map_err(to_pyerr)?;
-        let named_doc = self.inner.schema().to_named_doc(&doc);
-        Ok(Document {
+        let doc: TantivyDocument =
+            self.inner.doc(doc_address.into()).map_err(to_pyerr)?;
+        let named_doc = doc.to_named_doc(self.inner.schema());
+        Ok(crate::document::Document {
             field_values: named_doc.0,
         })
     }
 
     fn __repr__(&self) -> PyResult<String> {
         Ok(format!(
             "Searcher(num_docs={}, num_segments={})",
@@ -265,15 +272,15 @@
 
 /// DocAddress contains all the necessary information to identify a document
 /// given a Searcher object.
 ///
 /// It consists in an id identifying its segment, and its segment-local DocId.
 /// The id used for the segment is actually an ordinal in the list of segment
 /// hold by a Searcher.
-#[pyclass(frozen, module = "tantivy")]
+#[pyclass(frozen, module = "tantivy.tantivy")]
 #[derive(Clone, Debug, Deserialize, PartialEq, Serialize)]
 pub(crate) struct DocAddress {
     pub(crate) segment_ord: tv::SegmentOrdinal,
     pub(crate) doc: tv::DocId,
 }
 
 #[pymethods]
```

### Comparing `tantivy-0.21.0/src/snippet.rs` & `tantivy-0.22.0/src/snippet.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 use crate::to_pyerr;
 use pyo3::prelude::*;
 use tantivy as tv;
+// Bring the trait into scope to use methods like `as_str()` on `OwnedValue`.
+use tantivy::schema::Value;
 
-/// Tantivy schema.
+/// Tantivy Snippet
 ///
-/// The schema is very strict. To build the schema the `SchemaBuilder` class is
-/// provided.
-#[pyclass]
+/// Snippet contains a fragment of a document, and some highlighted
+/// parts inside it.
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct Snippet {
     pub(crate) inner: tv::Snippet,
 }
 
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct Range {
     #[pyo3(get)]
     start: usize,
     #[pyo3(get)]
     end: usize,
 }
 
@@ -34,15 +36,15 @@
                 end: r.end,
             })
             .collect::<Vec<_>>();
         results
     }
 }
 
-#[pyclass]
+#[pyclass(module = "tantivy.tantivy")]
 pub(crate) struct SnippetGenerator {
     pub(crate) field_name: String,
     pub(crate) inner: tv::SnippetGenerator,
 }
 
 #[pymethods]
 impl SnippetGenerator {
@@ -58,24 +60,24 @@
             .get_field(field_name)
             .or(Err("field not found"))
             .map_err(to_pyerr)?;
         let generator =
             tv::SnippetGenerator::create(&searcher.inner, query.get(), field)
                 .map_err(to_pyerr)?;
 
-        return Ok(SnippetGenerator {
+        Ok(SnippetGenerator {
             field_name: field_name.to_string(),
             inner: generator,
-        });
+        })
     }
 
     pub fn snippet_from_doc(&self, doc: &crate::Document) -> crate::Snippet {
         let text: String = doc
             .iter_values_for_field(&self.field_name)
-            .flat_map(tv::schema::Value::as_text)
+            .flat_map(|ov| ov.as_str())
             .collect::<Vec<&str>>()
             .join(" ");
 
         let result = self.inner.snippet(&text);
         Snippet { inner: result }
     }
 }
```

### Comparing `tantivy-0.21.0/Cargo.lock` & `tantivy-0.22.0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
-version = "0.21.5"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -83,17 +83,17 @@
 name = "bitflags"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
 
 [[package]]
 name = "bitpacking"
-version = "0.8.4"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8c7d2ac73c167c06af4a5f37e6e59d84148d57ccbe4480b76f0273eefea82d7"
+checksum = "4c1d3e2bfd8d06048a179f7b17afc3188effa10385e7b00dc65af6aae732ea92"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.14.0"
@@ -114,36 +114,36 @@
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "census"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fafee10a5dd1cffcb5cc560e0d0df8803d7355a2b12272e3557dee57314cb6e"
+checksum = "4f4c707c6a209cbe82d10abd08e1ea8995e9ea937d2550646e02798948992be0"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
@@ -231,15 +231,15 @@
 [[package]]
 name = "errno"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3e13f66a2f95e32a39eaa81f6b95d42878ca0e1db0c7543723dfe12557e860"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "fastdivide"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "25c7df09945d65ea8d70b3321547ed414bbc540aad5bac6883d021b970f35b04"
@@ -254,20 +254,20 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "fs4"
-version = "0.6.6"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2eeb4ed9e12f43b7fa0baae3f9cdda28352770132ef2e09a23760c29cae8bd47"
+checksum = "21dabded2e32cd57ded879041205c60a4a4c4bab47bd0fd2fa8b01f30849f02b"
 dependencies = [
  "rustix",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "futures"
 version = "0.3.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da0290714b38af9b4a7b094b8a37086d1b4e61f2df9122c3cad2577669145335"
@@ -446,26 +446,17 @@
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
-]
-
-[[package]]
-name = "itertools"
-version = "0.11.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.9"
@@ -500,17 +491,23 @@
 name = "levenshtein_automata"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2cdeb66e45e9f36bfad5bbdb4d2384e70936afbee843c6f6543f0c551ebb25"
 
 [[package]]
 name = "libc"
-version = "0.2.149"
+version = "0.2.153"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+
+[[package]]
+name = "libm"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a08173bc88b7955d1b3145aa561539096c421ac8debde8cbc3612ec635fee29b"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da2479e8c062e40bf0066ffa0bc823de0a9368974af99c9f6df941d2c231e03f"
 
@@ -542,17 +539,17 @@
  "scoped-tls",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "lru"
-version = "0.11.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a83fb7698b3643a0e34f9ae6f2e8f0178c0fd42f8b59d493aa271ff3a5bf21"
+checksum = "d3262e75e648fce39813cb56ac41f3c3e3f65217ebf3844d818d1f9398cfb0dc"
 dependencies = [
  "hashbrown",
 ]
 
 [[package]]
 name = "lz4_flex"
 version = "0.11.1"
@@ -582,17 +579,17 @@
 name = "memchr"
 version = "2.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
 
 [[package]]
 name = "memmap2"
-version = "0.7.1"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
+checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
@@ -637,14 +634,15 @@
 [[package]]
 name = "num-traits"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
@@ -672,17 +670,17 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e8a72b918ae8198abb3a18c190288123e1d442b6b9a7d709305fd194688b4b7"
+checksum = "c3a059efb063b8f425b948e042e6b9bd85edfe60e913630ed727b23e2dfcc558"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
@@ -699,15 +697,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
@@ -727,14 +725,20 @@
 [[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
 dependencies = [
  "unicode-ident",
 ]
@@ -817,14 +821,54 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
+name = "rand_distr"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
+dependencies = [
+ "num-traits",
+ "rand",
+]
+
+[[package]]
 name = "rayon"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c27db03db7734835b3f53954b534c91069375ce6ccaa2e065441e07d9b6cdb1"
 dependencies = [
  "either",
  "rayon-core",
@@ -915,15 +959,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b426b0506e5d50a7d8dafcf2e81471400deb602392c7dd110815afb4eaf02a3"
 dependencies = [
  "bitflags 2.4.1",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
@@ -964,17 +1008,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.108"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
+checksum = "cb0652c533506ad7a2e353cce269330d6afd8bdfb6d75e0ace5b35aacbd7b9e9"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1025,55 +1069,54 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tantivy"
-version = "0.21.0"
+version = "0.22.0"
 dependencies = [
  "base64",
  "chrono",
  "futures",
- "itertools 0.10.5",
+ "itertools",
  "pyo3",
  "pyo3-build-config",
  "pythonize",
  "serde",
  "serde_json",
- "tantivy 0.21.1",
+ "tantivy 0.22.0 (registry+https://github.com/rust-lang/crates.io-index)",
 ]
 
 [[package]]
 name = "tantivy"
-version = "0.21.1"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6083cd777fa94271b8ce0fe4533772cb8110c3044bab048d20f70108329a1f2"
+checksum = "f8d0582f186c0a6d55655d24543f15e43607299425c5ad8352c242b914b31856"
 dependencies = [
  "aho-corasick",
  "arc-swap",
- "async-trait",
  "base64",
  "bitpacking",
  "byteorder",
  "census",
  "crc32fast",
  "crossbeam-channel",
  "downcast-rs",
  "fastdivide",
+ "fnv",
  "fs4",
  "htmlescape",
- "itertools 0.11.0",
+ "itertools",
  "levenshtein_automata",
  "log",
  "lru",
  "lz4_flex",
  "measure_time",
  "memmap2",
- "murmurhash32",
  "num_cpus",
  "once_cell",
  "oneshot",
  "rayon",
  "regex",
  "rust-stemmers",
  "rustc-hash",
@@ -1093,96 +1136,98 @@
  "time",
  "uuid",
  "winapi",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cecb164321482301f514dd582264fa67f70da2d7eb01872ccd71e35e0d96655a"
+checksum = "284899c2325d6832203ac6ff5891b297fc5239c3dc754c5bc1977855b23c10df"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d85f8019af9a78b3118c11298b36ffd21c2314bd76bbcd9d12e00124cbb7e70"
+checksum = "12722224ffbe346c7fec3275c699e508fd0d4710e629e933d5736ec524a1f44e"
 dependencies = [
+ "downcast-rs",
  "fastdivide",
- "fnv",
- "itertools 0.11.0",
+ "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af4a3a975e604a2aba6b1106a04505e1e7a025e6def477fab6e410b4126471e1"
+checksum = "8019e3cabcfd20a1380b491e13ff42f57bb38bf97c3d5fa5c07e50816e0621f4"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
 
 [[package]]
 name = "tantivy-fst"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc3c506b1a8443a3a65352df6382a1fb6a7afe1a02e871cee0d25e2c3d5f3944"
+checksum = "d60769b80ad7953d8a7b2c70cdfe722bbcdcac6bccc8ac934c40c034d866fc18"
 dependencies = [
  "byteorder",
- "regex-syntax 0.6.29",
+ "regex-syntax 0.8.2",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d39c5a03100ac10c96e0c8b07538e2ab8b17da56434ab348309b31f23fada77"
+checksum = "847434d4af57b32e309f4ab1b4f1707a6c566656264caa427ff4285c4d9d0b82"
 dependencies = [
  "nom",
 ]
 
 [[package]]
 name = "tantivy-sstable"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc0c1bb43e5e8b8e05eb8009610344dbf285f06066c844032fbb3e546b3c71df"
+checksum = "c69578242e8e9fc989119f522ba5b49a38ac20f576fc778035b96cc94f41f98e"
 dependencies = [
+ "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-fst",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2c078595413f13f218cf6f97b23dcfd48936838f1d3d13a1016e05acd64ed6c"
+checksum = "c56d6ff5591fc332739b3ce7035b57995a3ce29a93ffd6012660e0949c956ea8"
 dependencies = [
  "murmurhash32",
+ "rand_distr",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "347b6fb212b26d3505d224f438e3c4b827ab8bd847fe9953ad5ac6b8f9443b66"
+checksum = "2a0dcade25819a89cfe6f17d932c9cedff11989936bf6dd4f336d50392053b04"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.12"
@@ -1195,15 +1240,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ef1adac450ad7f4b3c28589471ade84f25f731a7a0fe30d71dfa9f60fd808e5"
 dependencies = [
  "cfg-if",
  "fastrand",
  "redox_syscall",
  "rustix",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
@@ -1456,133 +1501,205 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.51.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1f8cf84f35d2db49a46868f947758c7a1138116f7fac3bc844f43ade1292e64"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
 name = "zerocopy"
-version = "0.7.21"
+version = "0.7.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "686b7e407015242119c33dab17b8f61ba6843534de936d94368856528eae4dcc"
+checksum = "1c4061bedbb353041c12f413700357bec76df2c7e2ca8e4df8bac24c6bf68e3d"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.21"
+version = "0.7.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "020f3dfe25dfc38dfea49ce62d5d45ecdd7f0d8a724fa63eb36b6eba4ec76806"
+checksum = "b3c129550b3e6de3fd0ba67ba5c81818f9805e58b8d7fee80a3a59d2c9fc601a"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.4"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.6"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
- "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `tantivy-0.21.0/pyproject.toml` & `tantivy-0.22.0/pyproject.toml`

 * *Files identical despite different names*

