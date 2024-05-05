# Comparing `tmp/ReplayTables_andnp-6.2.16.tar.gz` & `tmp/ReplayTables_andnp-6.3.0.tar.gz`

## Comparing `ReplayTables_andnp-6.2.16.tar` & `ReplayTables_andnp-6.3.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.2.16/Cargo.toml
--rw-r--r--   0     1001      127      693 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/dependabot.yml
--rw-r--r--   0     1001      127     1003 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/workflows/benchmark.yml
--rw-r--r--   0     1001      127     1099 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/workflows/pr_benchmark.yml
--rw-r--r--   0     1001      127     2233 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      834 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/workflows/tag.yml
--rw-r--r--   0     1001      127      861 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.github/workflows/test.yml
--rw-r--r--   0     1001      127      148 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.gitignore
--rw-r--r--   0     1001      127      265 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     2350 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/README.md
--rw-r--r--   0     1001      127      748 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/BackwardsReplay.py
--rw-r--r--   0     1001      127     6094 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/Distributions.py
--rw-r--r--   0     1001      127     2476 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/PER.py
--rw-r--r--   0     1001      127     2582 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/PSER.py
--rw-r--r--   0     1001      127     4358 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ReplayBuffer.py
--rw-r--r--   0     1001      127     8237 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/Table.py
--rw-r--r--   0     1001      127     6193 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0     1001      127     1772 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/RandDict.py
--rw-r--r--   0     1001      127     2679 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/SamplableSet.py
--rw-r--r--   0     1001      127     2373 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/SumTree.py
--rw-r--r--   0     1001      127        0 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/__init__.py
--rw-r--r--   0     1001      127     1523 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/jit.py
--rw-r--r--   0     1001      127       58 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/logger.py
--rw-r--r--   0     1001      127      502 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/_utils/np.py
--rw-r--r--   0     1001      127      850 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ingress/CircularMapper.py
--rw-r--r--   0     1001      127      599 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ingress/IndexMapper.py
--rw-r--r--   0     1001      127     3193 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ingress/LagBuffer.py
--rw-r--r--   0     1001      127     1788 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ingress/MinHeapMapper.py
--rw-r--r--   0     1001      127      956 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/ingress/Trackers.py
--rw-r--r--   0     1001      127     1509 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/interface.py
--rw-r--r--   0     1001      127     1099 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/registry.py
--rw-r--r--   0     1001      127     2190 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/BackwardsSampler.py
--rw-r--r--   0     1001      127     1292 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/IndexSampler.py
--rw-r--r--   0     1001      127     1996 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/PrioritySampler.py
--rw-r--r--   0     1001      127     5388 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/PrioritySequenceSampler.py
--rw-r--r--   0     1001      127      947 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/UniformSampler.py
--rw-r--r--   0     1001      127      460 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/sampling/tools.py
--rw-r--r--   0     1001      127     4804 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/storage/BasicStorage.py
--rw-r--r--   0     1001      127     2045 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/storage/CompressedStorage.py
--rw-r--r--   0     1001      127      951 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/storage/MetadataStorage.py
--rw-r--r--   0     1001      127      969 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/storage/NonArrayStorage.py
--rw-r--r--   0     1001      127      974 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/ReplayTables/storage/Storage.py
--rwxr-xr-x   0     1001      127      105 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/dev-setup.sh
--rw-r--r--   0     1001      127     1534 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/requirements.txt
--rwxr-xr-x   0     1001      127      511 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/scripts/publish.sh
--rwxr-xr-x   0     1001      127       47 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/scripts/run_tests.sh
--rw-r--r--   0     1001      127      119 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/setup.cfg
--rw-r--r--   0     1001      127      385 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/lib.rs
--rw-r--r--   0     1001      127     4954 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/storage/metadata_storage.rs
--rw-r--r--   0     1001      127       26 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/storage.rs
--rw-r--r--   0     1001      127     3008 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/utils/ref_count.rs
--rw-r--r--   0     1001      127     5256 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/utils/sumtree.rs
--rw-r--r--   0     1001      127       36 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/src/utils.rs
--rw-r--r--   0     1001      127      247 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/test.py
--rw-r--r--   0     1001      127        0 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/__init__.py
--rw-r--r--   0     1001      127     4137 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/_utils/fake_data.py
--rw-r--r--   0     1001      127      998 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/rust/test_RefCount.py
--rw-r--r--   0     1001      127        0 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/sampling/__init__.py
--rw-r--r--   0     1001      127     2584 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/sampling/test_PrioritizedSequenceSampler.py
--rw-r--r--   0     1001      127     1216 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/storage/test_BasicStorage.py
--rw-r--r--   0     1001      127     6419 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/storage/test_Storage.py
--rw-r--r--   0     1001      127     2947 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_LagBuffer.py
--rw-r--r--   0     1001      127     4955 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_PER.py
--rw-r--r--   0     1001      127     5158 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_ReplayBuffer.py
--rw-r--r--   0     1001      127     1422 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_Table.py
--rw-r--r--   0     1001      127     5453 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_View.py
--rw-r--r--   0     1001      127     2392 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_fuzz.py
--rw-r--r--   0     1001      127     1657 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/test_integration.py
--rw-r--r--   0     1001      127        0 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/utils/__init__.py
--rw-r--r--   0     1001      127      981 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0     1001      127     3285 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/tests/utils/test_SumTree.py
--rw-r--r--   0     1001      127        0 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/ReplayTables/__init__.pyi
--rw-r--r--   0     1001      127     1413 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/ReplayTables/rust/__init__.pyi
--rw-r--r--   0     1001      127      108 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/lz4/frame/__init__.pyi
--rw-r--r--   0     1001      127      491 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/numba/__init__.pyi
--rw-r--r--   0     1001      127       55 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/numba/core/errors/__init__.pyi
--rw-r--r--   0     1001      127       38 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/numba/experimental/__init__.pyi
--rw-r--r--   0     1001      127      153 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/numba/typed/__init__.pyi
--rw-r--r--   0     1001      127       34 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/typings/numba/types/__init__.pyi
--rw-r--r--   0     1001      127    12392 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-03-14 01:42:59.000000 ReplayTables_andnp-6.2.16/pyproject.toml
--rw-r--r--   0        0        0     3334 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.2.16/PKG-INFO
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.3.0/Cargo.toml
+-rw-r--r--   0     1001      127      888 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/dependabot.yml
+-rw-r--r--   0     1001      127     1003 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/workflows/benchmark.yml
+-rw-r--r--   0     1001      127     1099 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/workflows/pr_benchmark.yml
+-rw-r--r--   0     1001      127     2233 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      834 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/workflows/tag.yml
+-rw-r--r--   0     1001      127      861 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      148 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.gitignore
+-rw-r--r--   0     1001      127      265 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     2350 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/README.md
+-rw-r--r--   0     1001      127      748 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/BackwardsReplay.py
+-rw-r--r--   0     1001      127     6094 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/Distributions.py
+-rw-r--r--   0     1001      127     2476 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/PER.py
+-rw-r--r--   0     1001      127     2582 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/PSER.py
+-rw-r--r--   0     1001      127      803 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/PrototypeBuffer.py
+-rw-r--r--   0     1001      127     4358 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0     1001      127     6193 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0     1001      127     1772 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0     1001      127     2679 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/SamplableSet.py
+-rw-r--r--   0     1001      127     2373 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0     1001      127        0 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/__init__.py
+-rw-r--r--   0     1001      127     1523 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/jit.py
+-rw-r--r--   0     1001      127       58 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/logger.py
+-rw-r--r--   0     1001      127      502 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/_utils/np.py
+-rw-r--r--   0     1001      127      850 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/CircularMapper.py
+-rw-r--r--   0     1001      127      599 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/IndexMapper.py
+-rw-r--r--   0     1001      127     3193 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/LagBuffer.py
+-rw-r--r--   0     1001      127     1788 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/MinHeapMapper.py
+-rw-r--r--   0     1001      127     1295 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/RandomIndexer.py
+-rw-r--r--   0     1001      127      956 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/ingress/Trackers.py
+-rw-r--r--   0     1001      127     1509 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/interface.py
+-rw-r--r--   0     1001      127     1255 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/registry.py
+-rw-r--r--   0     1001      127     2190 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/BackwardsSampler.py
+-rw-r--r--   0     1001      127     1292 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/IndexSampler.py
+-rw-r--r--   0     1001      127     1996 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/PrioritySampler.py
+-rw-r--r--   0     1001      127     5388 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/PrioritySequenceSampler.py
+-rw-r--r--   0     1001      127      947 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/UniformSampler.py
+-rw-r--r--   0     1001      127      460 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/sampling/tools.py
+-rw-r--r--   0     1001      127     4804 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/storage/BasicStorage.py
+-rw-r--r--   0     1001      127     2045 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/storage/CompressedStorage.py
+-rw-r--r--   0     1001      127      951 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/storage/MetadataStorage.py
+-rw-r--r--   0     1001      127      969 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/storage/NonArrayStorage.py
+-rw-r--r--   0     1001      127      974 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/ReplayTables/storage/Storage.py
+-rwxr-xr-x   0     1001      127      105 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/dev-setup.sh
+-rw-r--r--   0     1001      127     1534 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/requirements.txt
+-rwxr-xr-x   0     1001      127      511 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/scripts/publish.sh
+-rwxr-xr-x   0     1001      127       47 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/scripts/run_tests.sh
+-rw-r--r--   0     1001      127      119 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/setup.cfg
+-rw-r--r--   0     1001      127      385 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/lib.rs
+-rw-r--r--   0     1001      127     4954 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/storage/metadata_storage.rs
+-rw-r--r--   0     1001      127       26 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/storage.rs
+-rw-r--r--   0     1001      127     3008 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/utils/ref_count.rs
+-rw-r--r--   0     1001      127     5256 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/utils/sumtree.rs
+-rw-r--r--   0     1001      127       36 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/src/utils.rs
+-rw-r--r--   0     1001      127      247 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/test.py
+-rw-r--r--   0     1001      127        0 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/__init__.py
+-rw-r--r--   0     1001      127     4137 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/_utils/fake_data.py
+-rw-r--r--   0     1001      127     1219 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/ingress/test_RandomIndexer.py
+-rw-r--r--   0     1001      127      998 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/rust/test_RefCount.py
+-rw-r--r--   0     1001      127        0 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/sampling/__init__.py
+-rw-r--r--   0     1001      127     2584 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/sampling/test_PrioritizedSequenceSampler.py
+-rw-r--r--   0     1001      127     1216 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/storage/test_BasicStorage.py
+-rw-r--r--   0     1001      127     6419 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/storage/test_Storage.py
+-rw-r--r--   0     1001      127     2947 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_LagBuffer.py
+-rw-r--r--   0     1001      127     4955 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_PER.py
+-rw-r--r--   0     1001      127     2174 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_PrototypeBuffer.py
+-rw-r--r--   0     1001      127     5158 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_ReplayBuffer.py
+-rw-r--r--   0     1001      127     2392 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_fuzz.py
+-rw-r--r--   0     1001      127     1657 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/test_integration.py
+-rw-r--r--   0     1001      127        0 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/utils/__init__.py
+-rw-r--r--   0     1001      127      981 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0     1001      127     3285 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/tests/utils/test_SumTree.py
+-rw-r--r--   0     1001      127        0 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/typings/ReplayTables/__init__.pyi
+-rw-r--r--   0     1001      127     1413 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/ReplayTables/rust/__init__.pyi
+-rw-r--r--   0     1001      127      108 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/lz4/frame/__init__.pyi
+-rw-r--r--   0     1001      127      491 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/numba/__init__.pyi
+-rw-r--r--   0     1001      127       55 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/numba/core/errors/__init__.pyi
+-rw-r--r--   0     1001      127       38 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/numba/experimental/__init__.pyi
+-rw-r--r--   0     1001      127      153 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/numba/typed/__init__.pyi
+-rw-r--r--   0     1001      127       34 2024-05-05 01:18:32.000000 ReplayTables_andnp-6.3.0/typings/numba/types/__init__.pyi
+-rw-r--r--   0     1001      127    12392 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/Cargo.lock
+-rw-r--r--   0     1001      127     1152 2024-05-05 01:18:31.000000 ReplayTables_andnp-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 ReplayTables_andnp-6.3.0/PKG-INFO
```

### Comparing `ReplayTables_andnp-6.2.16/Cargo.toml` & `ReplayTables_andnp-6.3.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ReplayTables"
 crate-type = ["cdylib"]
 
 [dependencies]
 bincode = "1.3.3"
-hashbrown = { version = "0.14.3", features = ["serde"] }
+hashbrown = { version = "0.14.5", features = ["serde"] }
 ndarray = { version = "0.15.6", features = ["serde"] }
 numpy = "0.20.0"
 pyo3 = { version = "0.20.3", features = ["extension-module", "generate-import-lib"] }
-serde = { version = "1.0.197", features = ["derive"] }
+serde = { version = "1.0.199", features = ["derive"] }
```

### Comparing `ReplayTables_andnp-6.2.16/.github/dependabot.yml` & `ReplayTables_andnp-6.3.0/.github/dependabot.yml`

 * *Files 24% similar despite different names*

```diff
@@ -5,12 +5,23 @@
 
 version: 2
 updates:
   - package-ecosystem: "cargo" # See documentation for possible values
     directory: "/" # Location of package manifests
     schedule:
       interval: "weekly"
-      
+    groups:
+      rust-deps:
+        applies-to: version-updates
+        patterns:
+          - "*"
+
   - package-ecosystem: "pip" # See documentation for possible values
     directory: "/" # Location of package manifests
     schedule:
       interval: "weekly"
+
+    groups:
+      python-deps:
+        applies-to: version-updates
+        patterns:
+          - "*"
```

### Comparing `ReplayTables_andnp-6.2.16/.github/workflows/benchmark.yml` & `ReplayTables_andnp-6.3.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/.github/workflows/pr_benchmark.yml` & `ReplayTables_andnp-6.3.0/.github/workflows/pr_benchmark.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/.github/workflows/publish.yml` & `ReplayTables_andnp-6.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/.github/workflows/tag.yml` & `ReplayTables_andnp-6.3.0/.github/workflows/tag.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/.github/workflows/test.yml` & `ReplayTables_andnp-6.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/README.md` & `ReplayTables_andnp-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/BackwardsReplay.py` & `ReplayTables_andnp-6.3.0/ReplayTables/BackwardsReplay.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/Distributions.py` & `ReplayTables_andnp-6.3.0/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/PER.py` & `ReplayTables_andnp-6.3.0/ReplayTables/PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/PSER.py` & `ReplayTables_andnp-6.3.0/ReplayTables/PSER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ReplayBuffer.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables_andnp-6.3.0/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/_utils/RandDict.py` & `ReplayTables_andnp-6.3.0/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/_utils/SamplableSet.py` & `ReplayTables_andnp-6.3.0/ReplayTables/_utils/SamplableSet.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/_utils/SumTree.py` & `ReplayTables_andnp-6.3.0/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/_utils/jit.py` & `ReplayTables_andnp-6.3.0/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ingress/CircularMapper.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ingress/CircularMapper.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ingress/IndexMapper.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ingress/IndexMapper.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ingress/LagBuffer.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ingress/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ingress/MinHeapMapper.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ingress/MinHeapMapper.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/ingress/Trackers.py` & `ReplayTables_andnp-6.3.0/ReplayTables/ingress/Trackers.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/interface.py` & `ReplayTables_andnp-6.3.0/ReplayTables/interface.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/registry.py` & `ReplayTables_andnp-6.3.0/ReplayTables/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from typing import Any, Dict
 from ReplayTables.ReplayBuffer import ReplayBuffer
 
 from ReplayTables.BackwardsReplay import BackwardsReplay, BackwardsReplayConfig
 from ReplayTables.PER import PrioritizedReplay, PERConfig
 from ReplayTables.PSER import PrioritizedSequenceReplay, PSERConfig
+from ReplayTables.PrototypeBuffer import RandomEgressBuffer
 
 def build_buffer(buffer_type: str, max_size: int, lag: int, rng: np.random.Generator, config: Dict[str, Any]) -> ReplayBuffer:
     buffer_type = buffer_type.lower()
 
     # TODO: remove once mypy fixes typing inference
     c: Any = None
 
@@ -23,8 +24,11 @@
         c = PERConfig(**config)
         return PrioritizedReplay(max_size, lag, rng, c)
 
     elif buffer_type == 'pser':
         c = PSERConfig(**config)
         return PrioritizedSequenceReplay(max_size, lag, rng, c)
 
+    elif buffer_type == 'random_egress':
+        return RandomEgressBuffer(max_size, lag, rng)
+
     raise Exception('Unable to determine type of buffer')
```

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/sampling/BackwardsSampler.py` & `ReplayTables_andnp-6.3.0/ReplayTables/sampling/BackwardsSampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/sampling/IndexSampler.py` & `ReplayTables_andnp-6.3.0/ReplayTables/sampling/IndexSampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/sampling/PrioritySampler.py` & `ReplayTables_andnp-6.3.0/ReplayTables/sampling/PrioritySampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/sampling/PrioritySequenceSampler.py` & `ReplayTables_andnp-6.3.0/ReplayTables/sampling/PrioritySequenceSampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/sampling/UniformSampler.py` & `ReplayTables_andnp-6.3.0/ReplayTables/sampling/UniformSampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/storage/BasicStorage.py` & `ReplayTables_andnp-6.3.0/ReplayTables/storage/BasicStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/storage/CompressedStorage.py` & `ReplayTables_andnp-6.3.0/ReplayTables/storage/CompressedStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/storage/MetadataStorage.py` & `ReplayTables_andnp-6.3.0/ReplayTables/storage/MetadataStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/storage/NonArrayStorage.py` & `ReplayTables_andnp-6.3.0/ReplayTables/storage/NonArrayStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/ReplayTables/storage/Storage.py` & `ReplayTables_andnp-6.3.0/ReplayTables/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/requirements.txt` & `ReplayTables_andnp-6.3.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,77 +4,77 @@
     # via commitizen
 cfgv==3.4.0
     # via pre-commit
 charset-normalizer==3.3.2
     # via commitizen
 colorama==0.4.6
     # via commitizen
-commitizen==3.18.0
+commitizen==3.21.3
 decli==0.6.1
     # via commitizen
 distlib==0.3.8
     # via virtualenv
 filelock==3.13.1
     # via virtualenv
 identify==2.5.35
     # via pre-commit
-importlib-metadata==7.0.1
+importlib-metadata==7.1.0
     # via commitizen
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.3
     # via commitizen
 llvmlite==0.42.0
     # via numba
 lz4==4.3.3
 markupsafe==2.1.5
     # via jinja2
-maturin==1.4.0
+maturin==1.5.0
 mypy==1.9.0
 mypy-extensions==1.0.0
     # via mypy
 nodeenv==1.8.0
     # via pre-commit
-numba==0.59.0
+numba==0.59.1
 numpy==1.26.4
     # via
     #   numba
     #   scipy
 packaging==24.0
     # via
     #   commitizen
     #   pytest
 pip==24.0
 platformdirs==4.2.0
     # via virtualenv
 pluggy==1.4.0
     # via pytest
-pre-commit==3.6.2
+pre-commit==3.7.0
 prompt-toolkit==3.0.36
     # via questionary
 py-cpuinfo==9.0.0
     # via pytest-benchmark
-pytest==8.1.0
+pytest==8.1.1
     # via pytest-benchmark
 pytest-benchmark==4.0.0
 pyyaml==6.0.1
     # via
     #   commitizen
     #   pre-commit
 questionary==2.0.1
     # via commitizen
-ruff==0.3.0
+ruff==0.3.4
 scipy==1.12.0
-setuptools==69.1.1
+setuptools==69.2.0
     # via nodeenv
 termcolor==2.4.0
     # via commitizen
 tomlkit==0.12.4
     # via commitizen
 typing-extensions==4.10.0
     # via mypy
 virtualenv==20.25.1
     # via pre-commit
 wcwidth==0.2.13
     # via prompt-toolkit
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `ReplayTables_andnp-6.2.16/src/storage/metadata_storage.rs` & `ReplayTables_andnp-6.3.0/src/storage/metadata_storage.rs`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/src/utils/ref_count.rs` & `ReplayTables_andnp-6.3.0/src/utils/ref_count.rs`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/src/utils/sumtree.rs` & `ReplayTables_andnp-6.3.0/src/utils/sumtree.rs`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/_utils/fake_data.py` & `ReplayTables_andnp-6.3.0/tests/_utils/fake_data.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/rust/test_RefCount.py` & `ReplayTables_andnp-6.3.0/tests/rust/test_RefCount.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/sampling/test_PrioritizedSequenceSampler.py` & `ReplayTables_andnp-6.3.0/tests/sampling/test_PrioritizedSequenceSampler.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/storage/test_BasicStorage.py` & `ReplayTables_andnp-6.3.0/tests/storage/test_BasicStorage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/storage/test_Storage.py` & `ReplayTables_andnp-6.3.0/tests/storage/test_Storage.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/test_LagBuffer.py` & `ReplayTables_andnp-6.3.0/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/test_PER.py` & `ReplayTables_andnp-6.3.0/tests/test_PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/test_ReplayBuffer.py` & `ReplayTables_andnp-6.3.0/tests/test_ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/test_fuzz.py` & `ReplayTables_andnp-6.3.0/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/test_integration.py` & `ReplayTables_andnp-6.3.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/utils/test_MinMaxHeap.py` & `ReplayTables_andnp-6.3.0/tests/utils/test_MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/tests/utils/test_SumTree.py` & `ReplayTables_andnp-6.3.0/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/typings/ReplayTables/rust/__init__.pyi` & `ReplayTables_andnp-6.3.0/typings/ReplayTables/rust/__init__.pyi`

 * *Files identical despite different names*

### Comparing `ReplayTables_andnp-6.2.16/Cargo.lock` & `ReplayTables_andnp-6.3.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
  "serde",
 ]
 
 [[package]]
@@ -333,26 +333,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
```

### Comparing `ReplayTables_andnp-6.2.16/pyproject.toml` & `ReplayTables_andnp-6.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.2.16"
+version = "6.3.0"
 tag_format = "$version"
 version_files = ["pyproject.toml"]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [tool.maturin]
@@ -13,15 +13,15 @@
 module-name = "ReplayTables.rust"
 
 [tool.ruff.lint]
 ignore = ['E701']
 
 [project]
 name = "ReplayTables-andnp"
-version = "6.2.16"
+version = "6.3.0"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     {name = "Andy Patterson", email = "andnpatterson@gmail.com"},
 ]
 dependencies = [
     "numba~=0.57",
     "numpy~=1.23",
@@ -43,13 +43,13 @@
     "pip",
     "mypy",
     "ruff",
     "commitizen",
     "pre-commit",
     "pytest>=7.3,<9.0",
     "pytest-benchmark~=4.0",
-    "maturin~=1.4.0",
+    "maturin>=1.4,<1.6",
 ]
 
 [build-system]
 requires = ["maturin>=1.4,<2.0"]
 build-backend = "maturin"
```

### Comparing `ReplayTables_andnp-6.2.16/PKG-INFO` & `ReplayTables_andnp-6.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.3
 Name: ReplayTables-andnp
-Version: 6.2.16
+Version: 6.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numba ~=0.57
 Requires-Dist: numpy ~=1.23
 Requires-Dist: scipy ~=1.9
 Requires-Dist: lz4 ~=4.3.2
 Requires-Dist: pip ; extra == 'dev'
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
 Requires-Dist: commitizen ; extra == 'dev'
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: pytest >=7.3, <9.0 ; extra == 'dev'
 Requires-Dist: pytest-benchmark ~=4.0 ; extra == 'dev'
-Requires-Dist: maturin ~=1.4.0 ; extra == 'dev'
+Requires-Dist: maturin >=1.4, <1.6 ; extra == 'dev'
 Provides-Extra: dev
 Summary: A simple replay buffer implementation in python for sampling n-step trajectories
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 License: MIT
 Requires-Python: >=3.10, <3.13
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

