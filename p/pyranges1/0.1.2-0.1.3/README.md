# Comparing `tmp/pyranges1-0.1.2.tar.gz` & `tmp/pyranges1-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyranges1-0.1.2.tar", last modified: Sun May  5 10:23:25 2024, max compression
+gzip compressed data, was "pyranges1-0.1.3.tar", last modified: Sun May  5 10:43:17 2024, max compression
```

## Comparing `pyranges1-0.1.2.tar` & `pyranges1-0.1.3.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.526968 pyranges1-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.530968 pyranges1-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/all_checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/build_the_book.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/build_wheels_and_upload_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.github/workflows/hypothesis_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 10:23:21.000000 pyranges1-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 10:23:21.000000 pyranges1-0.1.2/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 10:23:21.000000 pyranges1-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:23:25.558968 pyranges1-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-05 10:23:21.000000 pyranges1-0.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-05 10:23:21.000000 pyranges1-0.1.2/check_typing_linting_and_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-05 10:23:21.000000 pyranges1-0.1.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.534968 pyranges1-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_orfs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_seqs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/extension_stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_columns.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_create.rst
--rw-r--r--   0 runner    (1001) docker     (127)    33804 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_genomic_ops.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_inspect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_pages.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_rows.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_sequences.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/how_to_write.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_extensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/pyranges_objects.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/range_frame.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/todos.rst
--rw-r--r--   0 runner    (1001) docker     (127)    46805 2024-05-05 10:23:21.000000 pyranges1-0.1.2/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.538968 pyranges1-0.1.2/pyranges/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.538968 pyranges1-0.1.2/pyranges/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/loci_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/multioverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_groupby.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)   212529 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/pyranges_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/tostring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.542968 pyranges1-0.1.2/pyranges/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/aorta.bed
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/aorta2.bed
--rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chipseq.bed
--rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chipseq_background.bed
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/chromsizes.bed
--rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/cpg.bed
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ensembl_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/exons.bed
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/f2.bed
--rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/gencode_human.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/lamina.bed
--rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ncbi.gff.gz
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/smaller.bam
--rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/data/ucsc_human.bed.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/docs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.546968 pyranges1-0.1.2/pyranges/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/orfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/ext/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.546968 pyranges1-0.1.2/pyranges/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/combine_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/itergrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/max_disjoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/merge_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/tile_genome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/to_rle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/methods/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/orfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/pyranges/range_frame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/range_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/range_frame/range_frame_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/seqs.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 10:23:21.000000 pyranges1-0.1.2/pyranges/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/pyranges1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 10:23:25.000000 pyranges1-0.1.2/pyranges1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:23:25.558968 pyranges1-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:23:21.000000 pyranges1-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/.fuse_hidden0000017200000002
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/hi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.550968 pyranges1-0.1.2/tests/property_based/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/hypothesis_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/new.py
--rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_do_not_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/property_based/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/run_doctest_tutorial_howto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/test_calculate_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/test_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/chip_10.bed
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/f1.bed
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/f2.bed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/getitem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/getitem/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/hi
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/k_nearest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/new_position/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/new_position/test_new_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/out/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/out/test_out.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/spliced_subsequence/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/spliced_subsequence/test_spliced_subsequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_count_overlaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.554967 pyranges1-0.1.2/tests/unit/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/ensembl.gtf
--rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam
--rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_guessers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_pandas_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/test_tostring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:25.558968 pyranges1-0.1.2/tests/unit/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:23:21.000000 pyranges1-0.1.2/tests/unit/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.207656 pyranges1-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.179655 pyranges1-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.183656 pyranges1-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.github/workflows/all_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.github/workflows/build_the_book.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.github/workflows/build_wheels_and_upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.github/workflows/hypothesis_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 10:43:13.000000 pyranges1-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 10:43:13.000000 pyranges1-0.1.3/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-05 10:43:13.000000 pyranges1-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:43:17.207656 pyranges1-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-05 10:43:13.000000 pyranges1-0.1.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2077 2024-05-05 10:43:13.000000 pyranges1-0.1.3/check_typing_linting_and_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-05 10:43:13.000000 pyranges1-0.1.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.187656 pyranges1-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/extension_orfs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/extension_seqs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/extension_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_columns.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_create.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33804 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_genomic_ops.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_inspect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_pages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_rows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_sequences.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/how_to_write.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/pyranges_extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/pyranges_module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/pyranges_objects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/range_frame.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/todos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    46805 2024-05-05 10:43:13.000000 pyranges1-0.1.3/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.187656 pyranges1-0.1.3/pyranges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.187656 pyranges1-0.1.3/pyranges/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/loci_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/multioverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/pyranges_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/pyranges_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   212529 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/pyranges_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/tostring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.195655 pyranges1-0.1.3/pyranges/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/aorta.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/aorta2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309369 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/chipseq.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   309045 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/chipseq_background.bed
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/chromsizes.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    28209 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/cpg.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    35943 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ensembl_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    64417 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/exons.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/f2.bed
+-rw-r--r--   0 runner    (1001) docker     (127)    81253 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/gencode_human.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    55608 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/lamina.bed
+-rw-r--r--   0 runner    (1001) docker     (127)   387402 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ncbi.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ncbi.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ncbi.gff.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/smaller.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    62555 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/data/ucsc_human.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/docs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.195655 pyranges1-0.1.3/pyranges/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/ext/orfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13762 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/ext/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/ext/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.199655 pyranges1-0.1.3/pyranges/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/combine_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/itergrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/max_disjoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/merge_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/tile_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/to_rle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/methods/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/orfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.199655 pyranges1-0.1.3/pyranges/range_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/range_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/range_frame/range_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/range_frame/range_frame_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/seqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-05 10:43:13.000000 pyranges1-0.1.3/pyranges/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.207656 pyranges1-0.1.3/pyranges1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-05 10:43:17.000000 pyranges1-0.1.3/pyranges1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-05 10:43:17.000000 pyranges1-0.1.3/pyranges1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:43:17.000000 pyranges1-0.1.3/pyranges1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-05 10:43:17.000000 pyranges1-0.1.3/pyranges1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 10:43:17.000000 pyranges1-0.1.3/pyranges1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:43:17.207656 pyranges1-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-05 10:43:13.000000 pyranges1-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.199655 pyranges1-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11164 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/.fuse_hidden0000017200000002
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/hi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.199655 pyranges1-0.1.3/tests/property_based/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/hypothesis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17767 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/test_do_not_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9456 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/property_based/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/run_doctest_tutorial_howto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/test_calculate_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/test_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/chip_10.bed
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/f1.bed
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/f2.bed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/getitem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/getitem/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/hi
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/k_nearest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/new_position/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/new_position/test_new_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/out/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/out/test_out.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/spliced_subsequence/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/spliced_subsequence/test_spliced_subsequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_count_overlaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.203656 pyranges1-0.1.3/tests/unit/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_data/ensembl.gtf
+-rw-r--r--   0 runner    (1001) docker     (127)    71593 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_data/test_sorted.bam
+-rw-r--r--   0 runner    (1001) docker     (127)  1706448 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_data/test_sorted.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_guessers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_pandas_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/test_tostring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:17.207656 pyranges1-0.1.3/tests/unit/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:43:13.000000 pyranges1-0.1.3/tests/unit/unit/__init__.py
```

### Comparing `pyranges1-0.1.2/.github/workflows/all_checks.yml` & `pyranges1-0.1.3/.github/workflows/all_checks.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/.github/workflows/build_the_book.yml` & `pyranges1-0.1.3/.github/workflows/build_the_book.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/.github/workflows/build_wheels_and_upload_to_pypi.yml` & `pyranges1-0.1.3/.github/workflows/build_wheels_and_upload_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/.github/workflows/hypothesis_tests.yml` & `pyranges1-0.1.3/.github/workflows/hypothesis_tests.yml`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/LICENSE` & `pyranges1-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/PKG-INFO` & `pyranges1-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.2
+Version: 0.1.3
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyranges1-0.1.2/README.md` & `pyranges1-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/check_typing_linting_and_formatting.py` & `pyranges1-0.1.3/check_typing_linting_and_formatting.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/conftest.py` & `pyranges1-0.1.3/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/Makefile` & `pyranges1-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/api_reference.rst` & `pyranges1-0.1.3/docs/api_reference.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/conf.py` & `pyranges1-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/developer_guide.rst` & `pyranges1-0.1.3/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_columns.rst` & `pyranges1-0.1.3/docs/how_to_columns.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_create.rst` & `pyranges1-0.1.3/docs/how_to_create.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_genomic_ops.rst` & `pyranges1-0.1.3/docs/how_to_genomic_ops.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_inspect.rst` & `pyranges1-0.1.3/docs/how_to_inspect.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_rows.rst` & `pyranges1-0.1.3/docs/how_to_rows.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_sequences.rst` & `pyranges1-0.1.3/docs/how_to_sequences.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/how_to_write.rst` & `pyranges1-0.1.3/docs/how_to_write.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/index.rst` & `pyranges1-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/installation.rst` & `pyranges1-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/make.bat` & `pyranges1-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/pyranges_module.rst` & `pyranges1-0.1.3/docs/pyranges_module.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/requirements.txt` & `pyranges1-0.1.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/todos.rst` & `pyranges1-0.1.3/docs/todos.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/docs/tutorial.rst` & `pyranges1-0.1.3/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyproject.toml` & `pyranges1-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "cython", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyranges1"
-version = "0.1.2"
+version = "0.1.3"
 description = "GenomicRanges for Python."
 requires-python = ">=3.12.0"
 readme = "README.md"
 authors = [{ name = "Endre Bakken Stovner", email = "endbak@pm.me" }]
 license = { text = "MIT" }
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `pyranges1-0.1.2/pyranges/__init__.py` & `pyranges1-0.1.3/pyranges/__init__.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/empty.py` & `pyranges1-0.1.3/pyranges/core/empty.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/example_data.py` & `pyranges1-0.1.3/pyranges/core/example_data.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/loci_getter.py` & `pyranges1-0.1.3/pyranges/core/loci_getter.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/multioverlap.py` & `pyranges1-0.1.3/pyranges/core/multioverlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/names.py` & `pyranges1-0.1.3/pyranges/core/names.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/options.py` & `pyranges1-0.1.3/pyranges/core/options.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/out.py` & `pyranges1-0.1.3/pyranges/core/out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/parallelism.py` & `pyranges1-0.1.3/pyranges/core/parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/pyranges_groupby.py` & `pyranges1-0.1.3/pyranges/core/pyranges_groupby.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/pyranges_helpers.py` & `pyranges1-0.1.3/pyranges/core/pyranges_helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/pyranges_main.py` & `pyranges1-0.1.3/pyranges/core/pyranges_main.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/random.py` & `pyranges1-0.1.3/pyranges/core/random.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/tostring.py` & `pyranges1-0.1.3/pyranges/core/tostring.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/core/version.py` & `pyranges1-0.1.3/pyranges/core/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import pyranges as pr
 
 logging.basicConfig(level=logging.INFO)
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
-__version__ = importlib.metadata.version("pyranges")
+__version__ = importlib.metadata.version("pyranges1") # note: update when pyranges1 becomes default
 
 
 def version_info() -> None:
     """Print version info for pyranges and its dependencies.
 
     Used for debugging.
     """
```

### Comparing `pyranges1-0.1.2/pyranges/data/chipseq.bed` & `pyranges1-0.1.3/pyranges/data/chipseq.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/chipseq_background.bed` & `pyranges1-0.1.3/pyranges/data/chipseq_background.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/cpg.bed` & `pyranges1-0.1.3/pyranges/data/cpg.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/ensembl.gtf` & `pyranges1-0.1.3/pyranges/data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/ensembl_human.gtf.gz` & `pyranges1-0.1.3/pyranges/data/ensembl_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/exons.bed` & `pyranges1-0.1.3/pyranges/data/exons.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/gencode_human.gtf.gz` & `pyranges1-0.1.3/pyranges/data/gencode_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/lamina.bed` & `pyranges1-0.1.3/pyranges/data/lamina.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/ncbi.fasta` & `pyranges1-0.1.3/pyranges/data/ncbi.fasta`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/ncbi.gff.gz` & `pyranges1-0.1.3/pyranges/data/ncbi.gff.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/smaller.bam` & `pyranges1-0.1.3/pyranges/data/smaller.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/data/ucsc_human.bed.gz` & `pyranges1-0.1.3/pyranges/data/ucsc_human.bed.gz`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/ext/orfs.py` & `pyranges1-0.1.3/pyranges/ext/orfs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/ext/seqs.py` & `pyranges1-0.1.3/pyranges/ext/seqs.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/ext/stats.py` & `pyranges1-0.1.3/pyranges/ext/stats.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/boundaries.py` & `pyranges1-0.1.3/pyranges/methods/boundaries.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/cluster.py` & `pyranges1-0.1.3/pyranges/methods/cluster.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/combine_positions.py` & `pyranges1-0.1.3/pyranges/methods/combine_positions.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/concat.py` & `pyranges1-0.1.3/pyranges/methods/concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/coverage.py` & `pyranges1-0.1.3/pyranges/methods/coverage.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/join.py` & `pyranges1-0.1.3/pyranges/methods/join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/merge.py` & `pyranges1-0.1.3/pyranges/methods/merge.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/nearest.py` & `pyranges1-0.1.3/pyranges/methods/nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/overlap.py` & `pyranges1-0.1.3/pyranges/methods/overlap.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/spliced_subsequence.py` & `pyranges1-0.1.3/pyranges/methods/spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/split.py` & `pyranges1-0.1.3/pyranges/methods/split.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/statistics.py` & `pyranges1-0.1.3/pyranges/methods/statistics.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/subsequence.py` & `pyranges1-0.1.3/pyranges/methods/subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/subtraction.py` & `pyranges1-0.1.3/pyranges/methods/subtraction.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/summary.py` & `pyranges1-0.1.3/pyranges/methods/summary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/tile_genome.py` & `pyranges1-0.1.3/pyranges/methods/tile_genome.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/to_rle.py` & `pyranges1-0.1.3/pyranges/methods/to_rle.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/methods/windows.py` & `pyranges1-0.1.3/pyranges/methods/windows.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/range_frame/range_frame.py` & `pyranges1-0.1.3/pyranges/range_frame/range_frame.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/range_frame/range_frame_validator.py` & `pyranges1-0.1.3/pyranges/range_frame/range_frame_validator.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges/readers.py` & `pyranges1-0.1.3/pyranges/readers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/pyranges1.egg-info/PKG-INFO` & `pyranges1-0.1.3/pyranges1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranges1
-Version: 0.1.2
+Version: 0.1.3
 Summary: GenomicRanges for Python.
 Author-email: Endre Bakken Stovner <endbak@pm.me>
 License: MIT
 Project-URL: Homepage, http://github.com/pyranges/pyranges_1.x
 Keywords: bioinformatics,genomicranges,genomics
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyranges1-0.1.2/pyranges1.egg-info/SOURCES.txt` & `pyranges1-0.1.3/pyranges1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/.fuse_hidden0000017200000002` & `pyranges1-0.1.3/tests/.fuse_hidden0000017200000002`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/helpers.py` & `pyranges1-0.1.3/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/hi` & `pyranges1-0.1.3/tests/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/property_based/hypothesis_helper.py` & `pyranges1-0.1.3/tests/property_based/hypothesis_helper.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/property_based/new.py` & `pyranges1-0.1.3/tests/property_based/new.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/property_based/test_binary.py` & `pyranges1-0.1.3/tests/property_based/test_binary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/property_based/test_do_not_error.py` & `pyranges1-0.1.3/tests/property_based/test_do_not_error.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/property_based/test_unary.py` & `pyranges1-0.1.3/tests/property_based/test_unary.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/test_parallelism.py` & `pyranges1-0.1.3/tests/test_parallelism.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/chip_10.bed` & `pyranges1-0.1.3/tests/unit/chip_10.bed`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/conftest.py` & `pyranges1-0.1.3/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/hi` & `pyranges1-0.1.3/tests/unit/hi`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/k_nearest.py` & `pyranges1-0.1.3/tests/unit/k_nearest.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/out/test_out.py` & `pyranges1-0.1.3/tests/unit/out/test_out.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/spliced_subsequence/test_spliced_subsequence.py` & `pyranges1-0.1.3/tests/unit/spliced_subsequence/test_spliced_subsequence.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_concat.py` & `pyranges1-0.1.3/tests/unit/test_concat.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_count_overlaps.py` & `pyranges1-0.1.3/tests/unit/test_count_overlaps.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_data/ensembl.gtf` & `pyranges1-0.1.3/tests/unit/test_data/ensembl.gtf`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam` & `pyranges1-0.1.3/tests/unit/test_data/test_sorted.bam`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_data/test_sorted.bam.bai` & `pyranges1-0.1.3/tests/unit/test_data/test_sorted.bam.bai`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_guessers.py` & `pyranges1-0.1.3/tests/unit/test_guessers.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_join.py` & `pyranges1-0.1.3/tests/unit/test_join.py`

 * *Files identical despite different names*

### Comparing `pyranges1-0.1.2/tests/unit/test_pandas_overrides.py` & `pyranges1-0.1.3/tests/unit/test_pandas_overrides.py`

 * *Files identical despite different names*

