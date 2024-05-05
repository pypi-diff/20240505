# Comparing `tmp/pyranges1-0.1.1.tar.gz` & `tmp/pyranges1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyranges1-0.1.1.tar", last modified: Wed May  1 12:11:43 2024, max compression
+gzip compressed data, was "pyranges1-0.1.2.tar", last modified: Sun May  5 10:23:25 2024, max compression
```

## Comparing `pyranges1-0.1.1.tar` & `pyranges1-0.1.2.tar`

### file list

```diff
@@ -1,168 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.879408 pyranges1-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.847409 pyranges1-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.851409 pyranges1-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/all_checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/build_the_book.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/build_wheels_and_upload_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.github/workflows/hypothesis_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 12:11:38.000000 pyranges1-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 12:11:38.000000 pyranges1-0.1.1/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 12:11:38.000000 pyranges1-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-01 12:11:43.879408 pyranges1-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-01 12:11:38.000000 pyranges1-0.1.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-01 12:11:38.000000 pyranges1-0.1.1/check_typing_linting_and_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-01 12:11:38.000000 pyranges1-0.1.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.855409 pyranges1-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_orfs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_seqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/extension_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_columns.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_create.rst
--rw-r--r--   0 runner    (1001) docker     (127)    33827 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_genomic_ops.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_pages.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_rows.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_sequences.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/how_to_write.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/pyranges_objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/range_frame.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/todos.rst
--rw-r--r--   0 runner    (1001) docker     (127)    46812 2024-05-01 12:11:38.000000 pyranges1-0.1.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.859408 pyranges1-0.1.1/pyranges/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.859408 pyranges1-0.1.1/pyranges/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/loci_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/multioverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_groupby.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   213034 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/pyranges_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/tostring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.863409 pyranges1-0.1.1/pyranges/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/aorta.bed
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/aorta2.bed
--rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chipseq.bed
--rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chipseq_background.bed
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/chromsizes.bed
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/cpg.bed
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ensembl_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/exons.bed
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/f2.bed
--rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/gencode_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/lamina.bed
--rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ncbi.gff.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/smaller.bam
--rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/data/ucsc_human.bed.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/docs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.863409 pyranges1-0.1.1/pyranges/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/orfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/ext/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.867409 pyranges1-0.1.1/pyranges/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/combine_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/itergrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/max_disjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/merge_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/tile_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/to_rle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/methods/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/orfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.867409 pyranges1-0.1.1/pyranges/range_frame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/range_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/range_frame/range_frame_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 12:11:38.000000 pyranges1-0.1.1/pyranges/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/pyranges1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 12:11:43.000000 pyranges1-0.1.1/pyranges1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:11:43.879408 pyranges1-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-01 12:11:38.000000 pyranges1-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/.fuse_hidden0000017200000002
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/hi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/property_based/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/hypothesis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/new.py
--rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_do_not_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/property_based/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/run_doctest_tutorial_howto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/test_calculate_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/test_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/chip_10.bed
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/f2.bed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/getitem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/getitem/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/hi
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/k_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.871409 pyranges1-0.1.1/tests/unit/new_position/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/new_position/test_new_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/out/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/out/test_out.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/spliced_subsequence/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_count_overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam
--rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_guessers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_pandas_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/test_tostring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:43.875409 pyranges1-0.1.1/tests/unit/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:11:38.000000 pyranges1-0.1.1/tests/unit/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.526968 pyranges1-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.530968 pyranges1-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/all_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/build_the_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/build_wheels_and_upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/hypothesis_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 10:23:21.000000 pyranges1-0.1.2/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 10:23:21.000000 pyranges1-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:23:25.558968 pyranges1-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-05 10:23:21.000000 pyranges1-0.1.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-05 10:23:21.000000 pyranges1-0.1.2/check_typing_linting_and_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-05 10:23:21.000000 pyranges1-0.1.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.534968 pyranges1-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_orfs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_seqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_columns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33804 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_genomic_ops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_rows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_write.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/range_frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/todos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46805 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.538968 pyranges1-0.1.2/pyranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.538968 pyranges1-0.1.2/pyranges/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/loci_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/multioverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212529 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/tostring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.542968 pyranges1-0.1.2/pyranges/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/aorta.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/aorta2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chipseq.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chipseq_background.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chromsizes.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/cpg.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ensembl_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/exons.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/f2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/gencode_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/lamina.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.gff.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/smaller.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ucsc_human.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/docs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.546968 pyranges1-0.1.2/pyranges/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/orfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.546968 pyranges1-0.1.2/pyranges/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/combine_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/itergrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/max_disjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/merge_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/tile_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/to_rle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/orfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/pyranges/range_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/range_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/range_frame_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/pyranges1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:23:25.558968 pyranges1-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:23:21.000000 pyranges1-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/.fuse_hidden0000017200000002
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/hi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/tests/property_based/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/hypothesis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_do_not_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/run_doctest_tutorial_howto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/test_calculate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/test_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/chip_10.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/f2.bed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/getitem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/getitem/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/hi
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/k_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/new_position/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/new_position/test_new_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/out/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/out/test_out.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/spliced_subsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/spliced_subsequence/test_spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_count_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam
+-rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_guessers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_pandas_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_tostring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/tests/unit/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/unit/__init__.py
```

### Comparing `pyranges1-0.1.1/.github/workflows/all_checks.yml` & `pyranges1-0.1.2/.github/workflows/all_checks.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/.github/workflows/build_the_book.yml` & `pyranges1-0.1.2/.github/workflows/build_the_book.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/.github/workflows/build_wheels_and_upload_to_pypi.yml` & `pyranges1-0.1.2/.github/workflows/build_wheels_and_upload_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/.github/workflows/hypothesis_tests.yml` & `pyranges1-0.1.2/.github/workflows/hypothesis_tests.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/LICENSE` & `pyranges1-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/PKG-INFO` & `pyranges1-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.1
+Version: 0.1.2
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: ncls>=0.0.63
 Requires-Dist: tabulate
 Requires-Dist: sorted_nearest>=0.0.33
 Requires-Dist: natsort
@@ -47,54 +47,69 @@
 Provides-Extra: all
 Requires-Dist: pyranges[add-ons]; extra == "all"
 Requires-Dist: pyranges[dev]; extra == "all"
 Requires-Dist: pyranges[docs]; extra == "all"
 
 # pyranges
 
-[![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
+## Introduction
+
+PyRanges is a Python library for efficient and intuitive manipulation of genomics data,
+particularly genomic intervals (like genes, genomic features, or reads).
+The library is optimized for fast querying and manipulation of genomic annotations.
+It enables intuitive and highly efficient pipelines for genomic analysis.
+
+*"Finally ... This was what Python badly needed for years."* - Heng Li
+
+## Version 1.x
+This is version 1.x of pyranges. It is a complete rewrite of the original pyranges library, 
+that will replace the "default" (version 0) sometime in 2024.
 
 ## Install
 
+Pyranges 1.x requires python ≥3.12. Minimal installation: 
+
 ```bash
 pip install pyranges1
 ```
 
-## Introduction
+Installation including all optional dependencies:
 
-PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
-particularly genomic intervals (like genes, genomic features, or reads).
-The library is optimized for fast querying and manipulation of genomic annotations.
+```bash
+pip install pyranges1[all]
+```
 
-*"Finally ... This was what Python badly needed for years."* - Heng Li
+Details at https://pyranges1.readthedocs.io/en/latest/installation.html
 
 ## Documentation
 
-The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, will soon become available.
+The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, is 
+available at https://pyranges1.readthedocs.io/
 
 ## Features
 
   - fast
   - memory-efficient
   - featureful
   - pythonic/pandastic
-  - supports chaining with a terse syntax
-  - is a proper subclass of Pandas DataFrames
 
 ## Paper/Cite
 
-Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. *Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
+Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. 
+*Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
 
 ## Supporting pyranges
 
   - most importantly, cite pyranges if you use it. It is the main metric funding sources care about.
   - use pyranges in Stack Overflow/biostars questions and answers
   - star the repo (possibly important for github visibility and as a proxy for project popularity)
 
 ## Asking for help
 
-If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
+If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, 
+or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
 
 ## Contributing to pyranges
 
-Pyranges accepts code contributions in form of pull request. For details, visit https://pyranges.readthedocs.io/developer_guide.html
+Pyranges accepts code contributions in form of pull request. 
+For details, visit https://pyranges1.readthedocs.io/developer_guide.html
```

### Comparing `pyranges1-0.1.1/README.md` & `pyranges1-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 # pyranges
 
-[![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
+## Introduction
+
+PyRanges is a Python library for efficient and intuitive manipulation of genomics data,
+particularly genomic intervals (like genes, genomic features, or reads).
+The library is optimized for fast querying and manipulation of genomic annotations.
+It enables intuitive and highly efficient pipelines for genomic analysis.
+
+*"Finally ... This was what Python badly needed for years."* - Heng Li
+
+## Version 1.x
+This is version 1.x of pyranges. It is a complete rewrite of the original pyranges library, 
+that will replace the "default" (version 0) sometime in 2024.
 
 ## Install
 
+Pyranges 1.x requires python ≥3.12. Minimal installation: 
+
 ```bash
 pip install pyranges1
 ```
 
-## Introduction
+Installation including all optional dependencies:
 
-PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
-particularly genomic intervals (like genes, genomic features, or reads).
-The library is optimized for fast querying and manipulation of genomic annotations.
+```bash
+pip install pyranges1[all]
+```
 
-*"Finally ... This was what Python badly needed for years."* - Heng Li
+Details at https://pyranges1.readthedocs.io/en/latest/installation.html
 
 ## Documentation
 
-The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, will soon become available.
+The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, is 
+available at https://pyranges1.readthedocs.io/
 
 ## Features
 
   - fast
   - memory-efficient
   - featureful
   - pythonic/pandastic
-  - supports chaining with a terse syntax
-  - is a proper subclass of Pandas DataFrames
 
 ## Paper/Cite
 
-Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. *Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
+Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. 
+*Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
 
 ## Supporting pyranges
 
   - most importantly, cite pyranges if you use it. It is the main metric funding sources care about.
   - use pyranges in Stack Overflow/biostars questions and answers
   - star the repo (possibly important for github visibility and as a proxy for project popularity)
 
 ## Asking for help
 
-If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
+If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, 
+or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
 
 ## Contributing to pyranges
 
-Pyranges accepts code contributions in form of pull request. For details, visit https://pyranges.readthedocs.io/developer_guide.html
+Pyranges accepts code contributions in form of pull request. 
+For details, visit https://pyranges1.readthedocs.io/developer_guide.html
```

### Comparing `pyranges1-0.1.1/check_typing_linting_and_formatting.py` & `pyranges1-0.1.2/check_typing_linting_and_formatting.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/conftest.py` & `pyranges1-0.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/Makefile` & `pyranges1-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/api_reference.rst` & `pyranges1-0.1.2/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/conf.py` & `pyranges1-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/developer_guide.rst` & `pyranges1-0.1.2/docs/developer_guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Developer guide
 ===============
 
 Pyranges was originally written by Endre Bakken Stovner under supervision of Pål Sætrom.
 It is now mainly developed by Endre Bakken Stovner and by the Comparative Genomics lab of
 Marco Mariotti. It follows the guidelines for open source software, and external contributors
-are welcome. The code is centralized on github, at https://github.com/pyranges/pyranges
+are welcome. The code is centralized on github, at https://github.com/pyranges/pyranges_1.x
 
 Bugs and feature requests can be reported as github issues. You may also contribute by submitting
 your own code edits, either to deal with issues or to add new functionalities. Please discuss new
 features with the team before making a PR. The code will be reviewed by the core development team,
 which may integrate it in the main repository. Contributions are tracked by github and are publicly
 visible.
 
 Below, we sketch a guide to contribute to Pyranges. It assumes familiarity with python and with the
-terminal, and minimal experience with git/github. Before the actual list of steps follow (Task
-sequence), we go over some essential concepts used in the "continuous integration" system in place
+terminal, and minimal experience with git/github. Before the actual list of steps follow (:ref:`Task
+sequence <task_sequence>`), we go over some essential concepts used in the "continuous integration" system in place
 to maintain and evolve Pyranges.
 
 
 
+
 Tests
 ~~~~~
 
 Tests are an essential part of continuous integration. Briefly, they ensure that code edits do not
 break existing functions. Various layers of tests are implemented in Pyranges:
 
 - **unit tests**: quick and compulsory tests about the main Pyranges functionalities
@@ -82,20 +83,22 @@
 
 .. code:: python
 
     def add(a: int, b: int) -> int:
         return a + b
 
 For more detailed guidance on typing in Python, see the
-[official Python documentation](https://docs.python.org/3/library/typing.html).
+`official Python documentation <https://docs.python.org/3/library/typing.html>`_.
 
 We encourage contributions to Pyranges, even if they involve partial typing. If you're new
 to typing or have any questions, feel free to ask for help. We're committed to supporting
 our community in enhancing Pyranges together.
 
+.. _task_sequence:
+
 Task sequence
 ~~~~~~~~~~~~~
 
 1. Create and download your own Pyranges fork
 ------------------------------------------
 
 The easiest way to do this is through github. Login into the github website if you aren't already,
@@ -314,15 +317,15 @@
 11. Core team only: upload to PyPI
 ---------------------------------
 
 Every now and then, the core development team considers that a new pyranges version should be
 released. To do so:
 
 - Update the version number in the pyproject.toml file
-- Find the "Build and upload to PyPI" workflow in the left menu of the github actions at `https://github.com/pyranges/pyranges/actions/ <https://github.com/pyranges/pyranges/actions/>`_
+- Find the "Build and upload to PyPI" workflow in the left menu of the github actions at `https://github.com/pyranges/pyranges_1.x/actions/ <https://github.com/pyranges/pyranges_1.x/actions/>`_
 - Click the "Run workflow" button on the right
 
 Next, check that everything worked correctly, by confirming that a new pyranges installation via
 pip selects the new version.
 
 Finally, the pyranges conda package at Bioconda is updated automatically upon pip upload. Check
 that this is updated correctly.
```

### Comparing `pyranges1-0.1.1/docs/how_to_columns.rst` & `pyranges1-0.1.2/docs/how_to_columns.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Columns operations
 ~~~~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
 
 
 
 Fetching or writing a column
 ----------------------------
 Most column operations are analogous to pandas.
 A single PyRanges column (which are pandas Series) can be extracted through the dot notation, when reading it:
```

### Comparing `pyranges1-0.1.1/docs/how_to_create.rst` & `pyranges1-0.1.2/docs/how_to_create.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Loading/Creating PyRanges
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
 
 
 A PyRanges object can be built like a Pandas DataFrame, but genomic location columns (Chromosome, Start, End) are
 mandatory. Refer to https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html for more information on how
 to create a DataFrame. In alternative, PyRanges can be read from a file in bed, gtf, gff3 or bam format.
 
 PyRanges are created in the following ways:
```

### Comparing `pyranges1-0.1.1/docs/how_to_genomic_ops.rst` & `pyranges1-0.1.2/docs/how_to_genomic_ops.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Operating on coordinates
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
-
 
 Modifying coordinates
 ---------------------
 Interval coordinates (Start, End) can be directly modified like any Series in dataframes.
 Let's get some data:
 
   >>> import pyranges as pr
```

### Comparing `pyranges1-0.1.1/docs/how_to_inspect.rst` & `pyranges1-0.1.2/docs/how_to_inspect.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Inspecting PyRanges
 ~~~~~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
-
 
 String representation
 ---------------------
 
 Print a PyRanges object for an overview of its data:
 
   >>> import pyranges as pr
```

### Comparing `pyranges1-0.1.1/docs/how_to_rows.rst` & `pyranges1-0.1.2/docs/how_to_rows.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Rows operations
 ~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
 
 
 Indexing with iloc, loc
 -----------------------
 
 PyRanges inherits all the indexing and slicing capabilities of pandas, e.g. boolean Series indexing,
 ``iloc``, ``loc``, ``at``, ``iat``.
```

### Comparing `pyranges1-0.1.1/docs/how_to_sequences.rst` & `pyranges1-0.1.2/docs/how_to_sequences.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 
 Working with sequences
 ~~~~~~~~~~~~~~~~~~~~~~
 
+.. contents::
+   :local:
+   :depth: 2
+
 Fetching sequences per interval
 -------------------------------
 
 A common operation is to fetch the sequences corresponding to the intervals
 represented in the PyRanges object. Let's see an example with built-in data.
 
   >>> import pyranges as pr
```

### Comparing `pyranges1-0.1.1/docs/how_to_write.rst` & `pyranges1-0.1.2/docs/how_to_write.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Writing to disk
 ~~~~~~~~~~~~~~~
 
 .. contents::
    :local:
    :depth: 2
-   :caption: Contents
-
 
 
 The PyRanges can be written to several formats, namely csv, gtf, gff3 and bigwig.
 If no path-argument is given, the string representation of the data is returned. (It may potentially be very large.)
 If a path is given, it is taken as the path to the file to be written; in this case, the return value is the object
 itself, to allow inserting write methods into method call chains.
```

### Comparing `pyranges1-0.1.1/docs/index.rst` & `pyranges1-0.1.2/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 .. pyranges documentation master file, created by
    sphinx-quickstart.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 
-The PyRanges documentation
+The pyranges documentation
 ==========================
-PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
+Pyranges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
 particularly genomic intervals (like genes, genomic features, or reads).
 The library is optimized for fast querying and manipulation of genomic annotations.
 
-Pyranges is open source, and hosted at github: https://github.com/pyranges/pyranges
+Pyranges is open source, and hosted at github: https://github.com/pyranges/pyranges_1.x/
 
 Pyranges is developed by Endre Bakken Stovner and by
 `Marco Mariotti's lab <https://www.mariottigenomicslab.com/>`_.
 
-
+**This documentation refers to the version 1 of pyranges**, which introduces a new API and a new data structure
+compared to version 0, still the 'default', soon to be deprecated. **Version 0** is available at
+https://github.com/pyranges/pyranges and https://pyranges.readthedocs.io/
 
 
 Citation
 ~~~~~~~~
 
 Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. *Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
```

### Comparing `pyranges1-0.1.1/docs/make.bat` & `pyranges1-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/pyranges_module.rst` & `pyranges1-0.1.2/docs/pyranges_module.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/todos.rst` & `pyranges1-0.1.2/docs/todos.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/docs/tutorial.rst` & `pyranges1-0.1.2/docs/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,20 +30,20 @@
    :depth: 3
 
 
 Getting started
 ~~~~~~~~~~~~~~~
 
 We recommend using `ipython <https://ipython.readthedocs.io/>`_ or `Jupyter <https://jupyter.org/>`_ for this tutorial.
-Besides pyranges and some of its dependencies, we will use optional module (e.g. **pyfaidx**).
-To install all optional dependencies, use:
+Besides pyranges and pandas, we will use optional modules (e.g. **pyfaidx**).
+If you haven't already, install the optional add-ons with:
 
 .. code-block:: shell
 
-      pip install pyranges1_alpha[add-ons]
+      pip install pyranges1[add-ons]
 
 
 Loading and accessing pyranges objects
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Let's import libraries, and load in memory an example annotation in GFF3 format, consisting of a portion of the genome
 annotation of the worm *Dimorphilus gyrociliatus*.
```

### Comparing `pyranges1-0.1.1/pyproject.toml` & `pyranges1-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "cython", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyranges1"
-version = "0.1.1"
+version = "0.1.2"
 description = "GenomicRanges for Python."
-requires-python = ">=3.11.0"
+requires-python = ">=3.12.0"
 readme = "README.md"
 authors = [{ name = "Endre Bakken Stovner", email = "endbak@pm.me" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta", "Environment :: Other Environment",
     "Intended Audience :: Developers",
```

### Comparing `pyranges1-0.1.1/pyranges/__init__.py` & `pyranges1-0.1.2/pyranges/__init__.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/empty.py` & `pyranges1-0.1.2/pyranges/core/empty.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/example_data.py` & `pyranges1-0.1.2/pyranges/core/example_data.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/loci_getter.py` & `pyranges1-0.1.2/pyranges/core/loci_getter.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/multioverlap.py` & `pyranges1-0.1.2/pyranges/core/multioverlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/names.py` & `pyranges1-0.1.2/pyranges/core/names.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/options.py` & `pyranges1-0.1.2/pyranges/core/options.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/out.py` & `pyranges1-0.1.2/pyranges/core/out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/parallelism.py` & `pyranges1-0.1.2/pyranges/core/parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/pyranges_groupby.py` & `pyranges1-0.1.2/pyranges/core/pyranges_groupby.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/pyranges_helpers.py` & `pyranges1-0.1.2/pyranges/core/pyranges_helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/pyranges_main.py` & `pyranges1-0.1.2/pyranges/core/pyranges_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     NEAREST_UPSTREAM,
     OVERLAP_CONTAINMENT,
     OVERLAP_FIRST,
     PANDAS_COMPRESSION_TYPE,
     RANGE_COLS,
     SKIP_IF_EMPTY_LEFT,
     START_COL,
-    STRAND_BEHAVIOR_DEFAULT,
     STRAND_BEHAVIOR_OPPOSITE,
     STRAND_COL,
     TEMP_END_SLACK_COL,
     TEMP_NAME_COL,
     TEMP_NUM_COL,
     TEMP_START_SLACK_COL,
     TEMP_STRAND_COL,
@@ -870,14 +869,16 @@
         self,
         other: "PyRanges",
         strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
         *,
         match_by: str | list[str] | None = None,
         overlap_col: str = "NumberOverlaps",
         keep_nonoverlapping: bool = True,
+        calculate_coverage: bool = False,
+        coverage_col: str = "CoverageOverlaps",
     ) -> "PyRanges":
         """Count number of overlaps per interval.
 
         For each interval in self, report how many intervals in 'other' overlap with it.
 
         Parameters
         ----------
@@ -894,22 +895,27 @@
 
         keep_nonoverlapping : bool, default True
             Keep intervals without overlaps.
 
         overlap_col : str, default "NumberOverlaps"
             Name of column with overlap counts.
 
+        calculate_coverage : bool, default False
+            Whether to compute the fraction of each interval overlapped by other intervals, added as a new column.
+
+        coverage_col: str = "CoverageOverlaps"
+            If coverage is True, the name of the column with the fraction of overlaps to be added.
+
         Returns
         -------
         PyRanges
             PyRanges with a column of overlaps added.
 
         See Also
         --------
-        PyRanges.coverage: find coverage of PyRanges
         pyranges.count_overlaps: count overlaps from multiple PyRanges
 
         Examples
         --------
         >>> f1 = pr.example_data.f1.remove_nonloc_columns()
         >>> f1
           index  |    Chromosome      Start      End  Strand
@@ -937,131 +943,77 @@
         -------  ---  ------------  -------  -------  ----------  -------
               0  |    chr1                3        6  +                 0
               2  |    chr1                8        9  +                 0
               1  |    chr1                5        7  -                 1
         PyRanges with 3 rows, 5 columns, and 1 index columns.
         Contains 1 chromosomes and 2 strands.
 
+        >>> f1.count_overlaps(f2, overlap_col="C", calculate_coverage=True, coverage_col="F")
+          index  |    Chromosome      Start      End  Strand              F
+          int64  |    category        int64    int64  category      float64
+        -------  ---  ------------  -------  -------  ----------  ---------
+              0  |    chr1                3        6  +                 0
+              2  |    chr1                8        9  +                 0
+              1  |    chr1                5        7  -                 0.5
+        PyRanges with 3 rows, 5 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
+        >>> annotation = pr.example_data.ensembl_gtf.get_with_loc_columns(['transcript_id', 'Feature'])
+        >>> reads = pr.random(1000, chromsizes={'1':150000}, strand=False, seed=123)
+        >>> annotation.count_overlaps(reads)
+        index    |    Chromosome    Start    End      Strand      transcript_id    Feature     NumberOverlaps
+        int64    |    category      int64    int64    category    object           category    int64
+        -------  ---  ------------  -------  -------  ----------  ---------------  ----------  ----------------
+        0        |    1             11868    14409    +           nan              gene        20
+        1        |    1             11868    14409    +           ENST00000456328  transcript  20
+        2        |    1             11868    12227    +           ENST00000456328  exon        3
+        3        |    1             12612    12721    +           ENST00000456328  exon        3
+        ...      |    ...           ...      ...      ...         ...              ...         ...
+        7        |    1             120724   133723   -           ENST00000610542  transcript  85
+        8        |    1             133373   133723   -           ENST00000610542  exon        2
+        9        |    1             129054   129223   -           ENST00000610542  exon        1
+        10       |    1             120873   120932   -           ENST00000610542  exon        1
+        PyRanges with 11 rows, 7 columns, and 1 index columns.
+        Contains 1 chromosomes and 2 strands.
+
         """
         from pyranges.methods.coverage import _number_overlapping
 
-        return self.apply_pair(
+        strand_behavior = validate_and_convert_strand_behavior(self, other, strand_behavior)
+        if coverage_col != "CoverageOverlaps" and not calculate_coverage:
+            msg = "coverage_col can only be provided if calculate_coverage is True."
+            raise ValueError(msg)
+
+        result = self.apply_pair(
             other,
             _number_overlapping,
             strand_behavior=strand_behavior,
             by=match_by,
             keep_nonoverlapping=keep_nonoverlapping,
             overlap_col=overlap_col,
             skip_if_empty=not keep_nonoverlapping,
         )
 
-    def coverage(
-        self,
-        other: "PyRanges",
-        strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
-        *,
-        overlap_col: str = "NumberOverlaps",
-        fraction_col: str = "FractionOverlaps",
-        match_by: VALID_BY_TYPES = None,
-        keep_nonoverlapping: bool = True,
-    ) -> "PyRanges":
-        """Count number of overlaps and their fraction per interval.
-
-        Count how many intervals in self overlap with those in other.
-
-        Parameters
-        ----------
-        other: PyRanges
-            Count overlaps from this PyRanges.
-
-        match_by : str or list, default None
-            If provided, only intervals with an equal value in column(s) `match_by` may be considered as overlapping.
-
-        strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
-            Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
-            information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
-            otherwise ignore the strand information.
-
-        keep_nonoverlapping : bool, default True
-            Keep intervals without overlaps.
-
-        overlap_col : str, default "NumberOverlaps"
-            Name of column with overlap counts.
-
-        fraction_col : str, default "FractionOverlaps"
-            Name of column with fraction of counts.
-
-
-        Returns
-        -------
-        PyRanges
-            PyRanges with a column of overlaps added.
-
-        See Also
-        --------
-        pyranges.count_overlaps: count overlaps from multiple PyRanges
-
-        Examples
-        --------
-        >>> f1 = pr.PyRanges({"Chromosome": [1, 1, 1], "Start": [3, 8, 5],
-        ...                    "End": [6,  9, 7]})
-        >>> f1
-          index  |      Chromosome    Start      End
-          int64  |           int64    int64    int64
-        -------  ---  ------------  -------  -------
-              0  |               1        3        6
-              1  |               1        8        9
-              2  |               1        5        7
-        PyRanges with 3 rows, 3 columns, and 1 index columns.
-        Contains 1 chromosomes.
-
-        >>> f2 = pr.PyRanges({"Chromosome": [1, 1], "Start": [1, 6],
-        ...                    "End": [2, 7]})
-        >>> f2
-          index  |      Chromosome    Start      End
-          int64  |           int64    int64    int64
-        -------  ---  ------------  -------  -------
-              0  |               1        1        2
-              1  |               1        6        7
-        PyRanges with 2 rows, 3 columns, and 1 index columns.
-        Contains 1 chromosomes.
-
-        >>> f1.coverage(f2, overlap_col="C", fraction_col="F")
-          index  |      Chromosome    Start      End        C          F
-          int64  |           int64    int64    int64    int64    float64
-        -------  ---  ------------  -------  -------  -------  ---------
-              0  |               1        3        6        0        0
-              1  |               1        8        9        0        0
-              2  |               1        5        7        1        0.5
-        PyRanges with 3 rows, 5 columns, and 1 index columns.
-        Contains 1 chromosomes.
-
-        """
-        counts = self.count_overlaps(
-            other,
-            keep_nonoverlapping=True,
-            overlap_col=overlap_col,
-            strand_behavior=strand_behavior,
-        )
-
-        strand = strand_behavior != STRAND_BEHAVIOR_DEFAULT
-        other = other.merge_overlaps(use_strand=strand, count_col="Count")
+        if calculate_coverage:
+            from pyranges.methods.coverage import _coverage
 
-        from pyranges.methods.coverage import _coverage
+            use_strand = use_strand_from_validated_strand_behavior(self, other, strand_behavior)
+            other = other.merge_overlaps(use_strand=use_strand, match_by=match_by, count_col="Count")
 
-        return counts.apply_pair(
-            other,
-            _coverage,
-            strand_behavior=strand_behavior,
-            by=match_by,
-            fraction_col=fraction_col,
-            keep_nonoverlapping=keep_nonoverlapping,
-            overlap_col=overlap_col,
-            skip_if_empty=not keep_nonoverlapping,
-        )
+            result = self.copy().apply_pair(
+                other,
+                _coverage,
+                strand_behavior=strand_behavior,
+                by=match_by,
+                fraction_col=coverage_col,
+                keep_nonoverlapping=keep_nonoverlapping,
+                overlap_col=overlap_col,
+                skip_if_empty=not keep_nonoverlapping,
+            )
+        return result
 
     # to do: optimize, doesn't need to split by chromosome, only strand and only if ext_3/5
     def extend(
         self,
         ext: int | None = None,
         ext_3: int | None = None,
         ext_5: int | None = None,
```

### Comparing `pyranges1-0.1.1/pyranges/core/random.py` & `pyranges1-0.1.2/pyranges/core/random.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/tostring.py` & `pyranges1-0.1.2/pyranges/core/tostring.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/core/version.py` & `pyranges1-0.1.2/pyranges/core/version.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/chipseq.bed` & `pyranges1-0.1.2/pyranges/data/chipseq.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/chipseq_background.bed` & `pyranges1-0.1.2/pyranges/data/chipseq_background.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/cpg.bed` & `pyranges1-0.1.2/pyranges/data/cpg.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/ensembl.gtf` & `pyranges1-0.1.2/pyranges/data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/ensembl_human.gtf.gz` & `pyranges1-0.1.2/pyranges/data/ensembl_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/exons.bed` & `pyranges1-0.1.2/pyranges/data/exons.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/gencode_human.gtf.gz` & `pyranges1-0.1.2/pyranges/data/gencode_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/lamina.bed` & `pyranges1-0.1.2/pyranges/data/lamina.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/ncbi.fasta` & `pyranges1-0.1.2/pyranges/data/ncbi.fasta`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/ncbi.gff.gz` & `pyranges1-0.1.2/pyranges/data/ncbi.gff.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/smaller.bam` & `pyranges1-0.1.2/pyranges/data/smaller.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/data/ucsc_human.bed.gz` & `pyranges1-0.1.2/pyranges/data/ucsc_human.bed.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/ext/orfs.py` & `pyranges1-0.1.2/pyranges/ext/orfs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/ext/seqs.py` & `pyranges1-0.1.2/pyranges/ext/seqs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/ext/stats.py` & `pyranges1-0.1.2/pyranges/ext/stats.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/boundaries.py` & `pyranges1-0.1.2/pyranges/methods/boundaries.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/cluster.py` & `pyranges1-0.1.2/pyranges/methods/cluster.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/combine_positions.py` & `pyranges1-0.1.2/pyranges/methods/combine_positions.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/concat.py` & `pyranges1-0.1.2/pyranges/methods/concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/coverage.py` & `pyranges1-0.1.2/pyranges/methods/coverage.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/join.py` & `pyranges1-0.1.2/pyranges/methods/join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/merge.py` & `pyranges1-0.1.2/pyranges/methods/merge.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/nearest.py` & `pyranges1-0.1.2/pyranges/methods/nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/overlap.py` & `pyranges1-0.1.2/pyranges/methods/overlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/spliced_subsequence.py` & `pyranges1-0.1.2/pyranges/methods/spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/split.py` & `pyranges1-0.1.2/pyranges/methods/split.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/statistics.py` & `pyranges1-0.1.2/pyranges/methods/statistics.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/subsequence.py` & `pyranges1-0.1.2/pyranges/methods/subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/subtraction.py` & `pyranges1-0.1.2/pyranges/methods/subtraction.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/summary.py` & `pyranges1-0.1.2/pyranges/methods/summary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/tile_genome.py` & `pyranges1-0.1.2/pyranges/methods/tile_genome.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/to_rle.py` & `pyranges1-0.1.2/pyranges/methods/to_rle.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/methods/windows.py` & `pyranges1-0.1.2/pyranges/methods/windows.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/range_frame/range_frame.py` & `pyranges1-0.1.2/pyranges/range_frame/range_frame.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/range_frame/range_frame_validator.py` & `pyranges1-0.1.2/pyranges/range_frame/range_frame_validator.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges/readers.py` & `pyranges1-0.1.2/pyranges/readers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/pyranges1.egg-info/PKG-INFO` & `pyranges1-0.1.2/pyranges1.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.1
+Version: 0.1.2
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: ncls>=0.0.63
 Requires-Dist: tabulate
 Requires-Dist: sorted_nearest>=0.0.33
 Requires-Dist: natsort
@@ -47,54 +47,69 @@
 Provides-Extra: all
 Requires-Dist: pyranges[add-ons]; extra == "all"
 Requires-Dist: pyranges[dev]; extra == "all"
 Requires-Dist: pyranges[docs]; extra == "all"
 
 # pyranges
 
-[![Coverage Status](https://img.shields.io/coveralls/github/biocore-ntnu/pyranges.svg)](https://coveralls.io/github/biocore-ntnu/pyranges?branch=master) [![hypothesis tested](graphs/hypothesis-tested-brightgreen.svg)](http://hypothesis.readthedocs.io/) [![PyPI version](https://badge.fury.io/py/pyranges.svg)](https://badge.fury.io/py/pyranges) [![MIT](https://img.shields.io/pypi/l/pyranges.svg?color=green)](https://opensource.org/licenses/MIT) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyranges.svg) [![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/pyranges/README.html)
+## Introduction
+
+PyRanges is a Python library for efficient and intuitive manipulation of genomics data,
+particularly genomic intervals (like genes, genomic features, or reads).
+The library is optimized for fast querying and manipulation of genomic annotations.
+It enables intuitive and highly efficient pipelines for genomic analysis.
+
+*"Finally ... This was what Python badly needed for years."* - Heng Li
+
+## Version 1.x
+This is version 1.x of pyranges. It is a complete rewrite of the original pyranges library, 
+that will replace the "default" (version 0) sometime in 2024.
 
 ## Install
 
+Pyranges 1.x requires python ≥3.12. Minimal installation: 
+
 ```bash
 pip install pyranges1
 ```
 
-## Introduction
+Installation including all optional dependencies:
 
-PyRanges is a Python library specifically designed for efficient and intuitive manipulation of genomics data,
-particularly genomic intervals (like genes, genomic features, or reads).
-The library is optimized for fast querying and manipulation of genomic annotations.
+```bash
+pip install pyranges1[all]
+```
 
-*"Finally ... This was what Python badly needed for years."* - Heng Li
+Details at https://pyranges1.readthedocs.io/en/latest/installation.html
 
 ## Documentation
 
-The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, will soon become available.
+The pyranges documentation, including installation instructions, API, tutorial, and how-to-pages, is 
+available at https://pyranges1.readthedocs.io/
 
 ## Features
 
   - fast
   - memory-efficient
   - featureful
   - pythonic/pandastic
-  - supports chaining with a terse syntax
-  - is a proper subclass of Pandas DataFrames
 
 ## Paper/Cite
 
-Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. *Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
+Stovner EB, Sætrom P (2020) PyRanges: efficient comparison of genomic intervals in Python. 
+*Bioinformatics 36(3):918-919*  http://dx.doi.org/10.1093/bioinformatics/btz615
 
 ## Supporting pyranges
 
   - most importantly, cite pyranges if you use it. It is the main metric funding sources care about.
   - use pyranges in Stack Overflow/biostars questions and answers
   - star the repo (possibly important for github visibility and as a proxy for project popularity)
 
 ## Asking for help
 
-If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
+If you encounter bugs, or the documentation is not enough a cannot accomplish a specific task of interest, 
+or if you'd like new features implemented, open an Issue at github: https://github.com/pyranges/pyranges/issues
 
 ## Contributing to pyranges
 
-Pyranges accepts code contributions in form of pull request. For details, visit https://pyranges.readthedocs.io/developer_guide.html
+Pyranges accepts code contributions in form of pull request. 
+For details, visit https://pyranges1.readthedocs.io/developer_guide.html
```

### Comparing `pyranges1-0.1.1/pyranges1.egg-info/SOURCES.txt` & `pyranges1-0.1.2/pyranges1.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 CHANGELOG.txt
 LICENSE
 README.md
 check_typing_linting_and_formatting.py
 conftest.py
 pyproject.toml
 setup.py
```

### Comparing `pyranges1-0.1.1/tests/.fuse_hidden0000017200000002` & `pyranges1-0.1.2/tests/.fuse_hidden0000017200000002`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/helpers.py` & `pyranges1-0.1.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/hi` & `pyranges1-0.1.2/tests/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/property_based/hypothesis_helper.py` & `pyranges1-0.1.2/tests/property_based/hypothesis_helper.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/property_based/new.py` & `pyranges1-0.1.2/tests/property_based/new.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/property_based/test_binary.py` & `pyranges1-0.1.2/tests/property_based/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/property_based/test_do_not_error.py` & `pyranges1-0.1.2/tests/property_based/test_do_not_error.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/property_based/test_unary.py` & `pyranges1-0.1.2/tests/property_based/test_unary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/test_parallelism.py` & `pyranges1-0.1.2/tests/test_parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/chip_10.bed` & `pyranges1-0.1.2/tests/unit/chip_10.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/conftest.py` & `pyranges1-0.1.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/hi` & `pyranges1-0.1.2/tests/unit/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/k_nearest.py` & `pyranges1-0.1.2/tests/unit/k_nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/out/test_out.py` & `pyranges1-0.1.2/tests/unit/out/test_out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/spliced_subsequence/test_spliced_subsequence.py` & `pyranges1-0.1.2/tests/unit/spliced_subsequence/test_spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_concat.py` & `pyranges1-0.1.2/tests/unit/test_concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_count_overlaps.py` & `pyranges1-0.1.2/tests/unit/test_count_overlaps.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_data/ensembl.gtf` & `pyranges1-0.1.2/tests/unit/test_data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam` & `pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_data/test_sorted.bam.bai` & `pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam.bai`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_guessers.py` & `pyranges1-0.1.2/tests/unit/test_guessers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_join.py` & `pyranges1-0.1.2/tests/unit/test_join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.1/tests/unit/test_pandas_overrides.py` & `pyranges1-0.1.2/tests/unit/test_pandas_overrides.py`

 * *Files identical despite different names*

