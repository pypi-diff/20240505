# Comparing `tmp/biobit-0.0.1.tar.gz` & `tmp/biobit-0.0.2.tar.gz`

## Comparing `biobit-0.0.1.tar` & `biobit-0.0.2.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 biobit-0.0.1/modules/py/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/README.md
--rwxr-xr-x   0     1001      127      119 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/__init__.py
--rw-r--r--   0     1001      127       39 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/algo/__init__.py
--rw-r--r--   0     1001      127      577 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/algo/misc.py
--rw-r--r--   0     1001      127        0 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/__init__.py
--rw-r--r--   0     1001      127       65 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/__init__.py
--rw-r--r--   0     1001      127       67 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/fetchngs/__init__.py
--rw-r--r--   0     1001      127     7760 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py
--rw-r--r--   0     1001      127      158 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/__init__.py
--rw-r--r--   0     1001      127     2656 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/descriptor.py
--rw-r--r--   0     1001      127     2408 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/design.py
--rw-r--r--   0     1001      127     2508 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/experiment.py
--rw-r--r--   0     1001      127     1452 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/project.py
--rw-r--r--   0     1001      127      217 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/__init__.py
--rw-r--r--   0     1001      127      203 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/__init__.py
--rw-r--r--   0     1001      127     4370 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/joblib_counter.py
--rw-r--r--   0     1001      127     2215 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/partition.py
--rw-r--r--   0     1001      127     1039 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/reads_counter.py
--rw-r--r--   0     1001      127     5676 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/resolve.py
--rw-r--r--   0     1001      127      192 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/__init__.py
--rw-r--r--   0     1001      127     2162 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/adapters.py
--rw-r--r--   0     1001      127     2440 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/bam.py
--rw-r--r--   0     1001      127     1290 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/source.py
--rw-r--r--   0     1001      127      296 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/__init__.py
--rw-r--r--   0     1001      127       39 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/adapter/__init__.py
--rw-r--r--   0     1001      127     2020 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/adapter/yaml.py
--rw-r--r--   0     1001      127     1941 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/experiment.py
--rw-r--r--   0     1001      127     4260 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/filtering_schema.py
--rw-r--r--   0     1001      127     2404 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/library.py
--rw-r--r--   0     1001      127     4054 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/project.py
--rw-r--r--   0     1001      127     1818 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/sample.py
--rw-r--r--   0     1001      127     4763 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/seqrun.py
--rw-r--r--   0     1001      127      303 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/__init__.py
--rw-r--r--   0     1001      127      231 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/interval.py
--rw-r--r--   0     1001      127     1233 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/orientation.py
--rw-r--r--   0     1001      127     1501 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/range.py
--rw-r--r--   0     1001      127     1100 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/strand.py
--rw-r--r--   0     1001      127     2929 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/core/strdeductor.py
--rw-r--r--   0     1001      127       69 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/__init__.py
--rwxr-xr-x   0     1001      127      145 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/__init__.py
--rw-r--r--   0     1001      127      723 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/abc.py
--rwxr-xr-x   0     1001      127     1051 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/assembly.py
--rwxr-xr-x   0     1001      127      924 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/biomart.py
--rw-r--r--   0     1001      127      108 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/gene/__init__.py
--rw-r--r--   0     1001      127     3322 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/gene/attributes.py
--rw-r--r--   0     1001      127     5168 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/gene/descriptor.py
--rw-r--r--   0     1001      127     5798 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/loader.py
--rw-r--r--   0     1001      127      108 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/transcript/__init__.py
--rw-r--r--   0     1001      127     5072 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/transcript/attributes.py
--rw-r--r--   0     1001      127     5703 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/ensembl/transcript/descriptor.py
--rwxr-xr-x   0     1001      127    56796 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/repmasker/GRCh38.tsv.gz
--rwxr-xr-x   0     1001      127    47795 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/repmasker/GRCm39.tsv.gz
--rwxr-xr-x   0     1001      127      222 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/repmasker/__init__.py
--rwxr-xr-x   0     1001      127      928 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/db/repmasker/repmasker.py
--rw-r--r--   0     1001      127       43 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/ds/__init__.py
--rwxr-xr-x   0     1001      127      154 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/ds/gindex/__init__.py
--rw-r--r--   0     1001      127     4568 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/ds/gindex/genomic_index.py
--rw-r--r--   0     1001      127     2050 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/ds/gindex/overlap.py
--rw-r--r--   0     1001      127       37 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/io/__init__.py
--rwxr-xr-x   0     1001      127     8348 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/io/bam.py
--rwxr-xr-x   0     1001      127      133 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/paths.py
--rw-r--r--   0     1001      127        0 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/python/biobit/plot/__init__.py
--rw-r--r--   0     1001      127      127 2024-05-05 21:16:01.000000 biobit-0.0.1/modules/py/src/lib.rs
--rw-r--r--   0     1001      127    16376 2024-05-05 21:16:05.000000 biobit-0.0.1/Cargo.lock
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 biobit-0.0.1/Cargo.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 biobit-0.0.1/pyproject.toml
--rwxr-xr-x   0     1001      127      133 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/paths.py
--rw-r--r--   0     1001      127     5676 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/resolve.py
--rw-r--r--   0     1001      127     1039 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/counter/reads_counter.py
--rw-r--r--   0     1001      127      203 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/counter/__init__.py
--rw-r--r--   0     1001      127     4370 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/counter/joblib_counter.py
--rw-r--r--   0     1001      127     2215 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/counter/partition.py
--rw-r--r--   0     1001      127      217 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/__init__.py
--rw-r--r--   0     1001      127     3821 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/test_resolution.py
--rw-r--r--   0     1001      127     1290 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/source/source.py
--rw-r--r--   0     1001      127     2162 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/source/adapters.py
--rw-r--r--   0     1001      127      192 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/source/__init__.py
--rw-r--r--   0     1001      127     2440 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/rcount/source/bam.py
--rw-r--r--   0     1001      127     1941 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/experiment.py
--rw-r--r--   0     1001      127     4260 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/filtering_schema.py
--rw-r--r--   0     1001      127     2404 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/library.py
--rw-r--r--   0     1001      127     5371 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/test_seqproj.py
--rw-r--r--   0     1001      127     1818 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/sample.py
--rw-r--r--   0     1001      127     1350 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/adapter/test_adapters.py
--rw-r--r--   0     1001      127       39 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/adapter/__init__.py
--rw-r--r--   0     1001      127     2020 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/adapter/yaml.py
--rw-r--r--   0     1001      127     4054 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/project.py
--rw-r--r--   0     1001      127      296 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/__init__.py
--rw-r--r--   0     1001      127     4763 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/seqproj/seqrun.py
--rw-r--r--   0     1001      127        0 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/__init__.py
--rw-r--r--   0     1001      127     7760 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py
--rw-r--r--   0     1001      127       67 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/fetchngs/__init__.py
--rw-r--r--   0     1001      127       65 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/__init__.py
--rw-r--r--   0     1001      127     2408 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/design.py
--rw-r--r--   0     1001      127     2508 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/experiment.py
--rw-r--r--   0     1001      127     1452 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/project.py
--rw-r--r--   0     1001      127      158 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/__init__.py
--rw-r--r--   0     1001      127     2656 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/descriptor.py
--rw-r--r--   0     1001      127       37 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/io/__init__.py
--rwxr-xr-x   0     1001      127     8348 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/io/bam.py
--rwxr-xr-x   0     1001      127      119 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/__init__.py
--rw-r--r--   0     1001      127       69 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/__init__.py
--rwxr-xr-x   0     1001      127    47795 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/repmasker/GRCm39.tsv.gz
--rw-r--r--   0     1001      127     2012 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/repmasker/test_repmasker.py
--rwxr-xr-x   0     1001      127      222 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/repmasker/__init__.py
--rwxr-xr-x   0     1001      127      928 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/repmasker/repmasker.py
--rwxr-xr-x   0     1001      127    56796 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/repmasker/GRCh38.tsv.gz
--rw-r--r--   0     1001      127     5798 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/loader.py
--rwxr-xr-x   0     1001      127      924 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/biomart.py
--rw-r--r--   0     1001      127     5072 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/transcript/attributes.py
--rw-r--r--   0     1001      127      108 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/transcript/__init__.py
--rw-r--r--   0     1001      127     5703 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/transcript/descriptor.py
--rwxr-xr-x   0     1001      127      145 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/__init__.py
--rw-r--r--   0     1001      127      723 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/abc.py
--rwxr-xr-x   0     1001      127     1051 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/assembly.py
--rw-r--r--   0     1001      127     3322 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/gene/attributes.py
--rw-r--r--   0     1001      127      108 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/gene/__init__.py
--rw-r--r--   0     1001      127     5168 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/db/ensembl/gene/descriptor.py
--rw-r--r--   0     1001      127     4568 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/gindex/genomic_index.py
--rw-r--r--   0     1001      127     3813 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/gindex/test_index.py
--rw-r--r--   0     1001      127     3699 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/gindex/test_overlap.py
--rwxr-xr-x   0     1001      127      154 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/gindex/__init__.py
--rw-r--r--   0     1001      127     2050 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/gindex/overlap.py
--rw-r--r--   0     1001      127       43 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/ds/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/plot/__init__.py
--rw-r--r--   0     1001      127     2077 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/test_range.py
--rw-r--r--   0     1001      127     1501 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/range.py
--rw-r--r--   0     1001      127     1100 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/strand.py
--rw-r--r--   0     1001      127     1233 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/orientation.py
--rw-r--r--   0     1001      127      303 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/__init__.py
--rw-r--r--   0     1001      127     1456 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/test_strdeductor.py
--rw-r--r--   0     1001      127      231 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/interval.py
--rw-r--r--   0     1001      127     2929 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/strdeductor.py
--rw-r--r--   0     1001      127     1030 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/core/test_orientation.py
--rw-r--r--   0     1001      127      577 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/algo/misc.py
--rw-r--r--   0     1001      127       39 2024-05-05 21:16:01.000000 biobit-0.0.1/python/biobit/algo/__init__.py
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 biobit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 biobit-0.0.2/modules/py/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/README.md
+-rwxr-xr-x   0     1001      127      119 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/__init__.py
+-rw-r--r--   0     1001      127       39 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/algo/__init__.py
+-rw-r--r--   0     1001      127      577 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/algo/misc.py
+-rw-r--r--   0     1001      127        0 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/__init__.py
+-rw-r--r--   0     1001      127       65 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/__init__.py
+-rw-r--r--   0     1001      127       67 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/fetchngs/__init__.py
+-rw-r--r--   0     1001      127     7760 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py
+-rw-r--r--   0     1001      127      158 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/__init__.py
+-rw-r--r--   0     1001      127     2656 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/descriptor.py
+-rw-r--r--   0     1001      127     2408 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/design.py
+-rw-r--r--   0     1001      127     2508 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/experiment.py
+-rw-r--r--   0     1001      127     1452 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/project.py
+-rw-r--r--   0     1001      127      217 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/__init__.py
+-rw-r--r--   0     1001      127      203 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/__init__.py
+-rw-r--r--   0     1001      127     4370 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/joblib_counter.py
+-rw-r--r--   0     1001      127     2215 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/partition.py
+-rw-r--r--   0     1001      127     1039 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/reads_counter.py
+-rw-r--r--   0     1001      127     5676 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/resolve.py
+-rw-r--r--   0     1001      127      192 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/__init__.py
+-rw-r--r--   0     1001      127     2162 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/adapters.py
+-rw-r--r--   0     1001      127     2440 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/bam.py
+-rw-r--r--   0     1001      127     1290 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/source.py
+-rw-r--r--   0     1001      127      296 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/__init__.py
+-rw-r--r--   0     1001      127       39 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/adapter/__init__.py
+-rw-r--r--   0     1001      127     2020 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/adapter/yaml.py
+-rw-r--r--   0     1001      127     1941 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/experiment.py
+-rw-r--r--   0     1001      127     4260 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/filtering_schema.py
+-rw-r--r--   0     1001      127     2404 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/library.py
+-rw-r--r--   0     1001      127     4054 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/project.py
+-rw-r--r--   0     1001      127     1818 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/sample.py
+-rw-r--r--   0     1001      127     4763 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/seqrun.py
+-rw-r--r--   0     1001      127      303 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/__init__.py
+-rw-r--r--   0     1001      127      231 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/interval.py
+-rw-r--r--   0     1001      127     1233 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/orientation.py
+-rw-r--r--   0     1001      127     1501 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/range.py
+-rw-r--r--   0     1001      127     1100 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/strand.py
+-rw-r--r--   0     1001      127     2929 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/core/strdeductor.py
+-rw-r--r--   0     1001      127       69 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/__init__.py
+-rwxr-xr-x   0     1001      127      145 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/__init__.py
+-rw-r--r--   0     1001      127      723 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/abc.py
+-rwxr-xr-x   0     1001      127     1051 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/assembly.py
+-rwxr-xr-x   0     1001      127      924 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/biomart.py
+-rw-r--r--   0     1001      127      108 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/gene/__init__.py
+-rw-r--r--   0     1001      127     3322 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/gene/attributes.py
+-rw-r--r--   0     1001      127     5168 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/gene/descriptor.py
+-rw-r--r--   0     1001      127     5798 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/loader.py
+-rw-r--r--   0     1001      127      108 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/transcript/__init__.py
+-rw-r--r--   0     1001      127     5072 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/transcript/attributes.py
+-rw-r--r--   0     1001      127     5703 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/ensembl/transcript/descriptor.py
+-rwxr-xr-x   0     1001      127    56796 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/repmasker/GRCh38.tsv.gz
+-rwxr-xr-x   0     1001      127    47795 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/repmasker/GRCm39.tsv.gz
+-rwxr-xr-x   0     1001      127      222 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/repmasker/__init__.py
+-rwxr-xr-x   0     1001      127      928 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/db/repmasker/repmasker.py
+-rw-r--r--   0     1001      127       43 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/ds/__init__.py
+-rwxr-xr-x   0     1001      127      154 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/ds/gindex/__init__.py
+-rw-r--r--   0     1001      127     4568 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/ds/gindex/genomic_index.py
+-rw-r--r--   0     1001      127     2050 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/ds/gindex/overlap.py
+-rw-r--r--   0     1001      127       37 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/io/__init__.py
+-rwxr-xr-x   0     1001      127     8348 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/io/bam.py
+-rwxr-xr-x   0     1001      127      133 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/paths.py
+-rw-r--r--   0     1001      127        0 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/python/biobit/plot/__init__.py
+-rw-r--r--   0     1001      127      127 2024-05-05 21:21:31.000000 biobit-0.0.2/modules/py/src/lib.rs
+-rw-r--r--   0     1001      127    16376 2024-05-05 21:21:37.000000 biobit-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 biobit-0.0.2/Cargo.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 biobit-0.0.2/pyproject.toml
+-rwxr-xr-x   0     1001      127      133 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/paths.py
+-rw-r--r--   0     1001      127     5676 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/resolve.py
+-rw-r--r--   0     1001      127     1039 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/counter/reads_counter.py
+-rw-r--r--   0     1001      127      203 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/counter/__init__.py
+-rw-r--r--   0     1001      127     4370 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/counter/joblib_counter.py
+-rw-r--r--   0     1001      127     2215 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/counter/partition.py
+-rw-r--r--   0     1001      127      217 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/__init__.py
+-rw-r--r--   0     1001      127     3821 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/test_resolution.py
+-rw-r--r--   0     1001      127     1290 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/source/source.py
+-rw-r--r--   0     1001      127     2162 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/source/adapters.py
+-rw-r--r--   0     1001      127      192 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/source/__init__.py
+-rw-r--r--   0     1001      127     2440 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/rcount/source/bam.py
+-rw-r--r--   0     1001      127     1941 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/experiment.py
+-rw-r--r--   0     1001      127     4260 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/filtering_schema.py
+-rw-r--r--   0     1001      127     2404 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/library.py
+-rw-r--r--   0     1001      127     5371 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/test_seqproj.py
+-rw-r--r--   0     1001      127     1818 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/sample.py
+-rw-r--r--   0     1001      127     1350 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/adapter/test_adapters.py
+-rw-r--r--   0     1001      127       39 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/adapter/__init__.py
+-rw-r--r--   0     1001      127     2020 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/adapter/yaml.py
+-rw-r--r--   0     1001      127     4054 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/project.py
+-rw-r--r--   0     1001      127      296 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/__init__.py
+-rw-r--r--   0     1001      127     4763 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/seqproj/seqrun.py
+-rw-r--r--   0     1001      127        0 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/__init__.py
+-rw-r--r--   0     1001      127     7760 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py
+-rw-r--r--   0     1001      127       67 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/fetchngs/__init__.py
+-rw-r--r--   0     1001      127       65 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/__init__.py
+-rw-r--r--   0     1001      127     2408 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/design.py
+-rw-r--r--   0     1001      127     2508 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/experiment.py
+-rw-r--r--   0     1001      127     1452 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/project.py
+-rw-r--r--   0     1001      127      158 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/__init__.py
+-rw-r--r--   0     1001      127     2656 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/descriptor.py
+-rw-r--r--   0     1001      127       37 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/io/__init__.py
+-rwxr-xr-x   0     1001      127     8348 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/io/bam.py
+-rwxr-xr-x   0     1001      127      119 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/__init__.py
+-rw-r--r--   0     1001      127       69 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/__init__.py
+-rwxr-xr-x   0     1001      127    47795 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/repmasker/GRCm39.tsv.gz
+-rw-r--r--   0     1001      127     2012 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/repmasker/test_repmasker.py
+-rwxr-xr-x   0     1001      127      222 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/repmasker/__init__.py
+-rwxr-xr-x   0     1001      127      928 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/repmasker/repmasker.py
+-rwxr-xr-x   0     1001      127    56796 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/repmasker/GRCh38.tsv.gz
+-rw-r--r--   0     1001      127     5798 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/loader.py
+-rwxr-xr-x   0     1001      127      924 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/biomart.py
+-rw-r--r--   0     1001      127     5072 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/transcript/attributes.py
+-rw-r--r--   0     1001      127      108 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/transcript/__init__.py
+-rw-r--r--   0     1001      127     5703 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/transcript/descriptor.py
+-rwxr-xr-x   0     1001      127      145 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/__init__.py
+-rw-r--r--   0     1001      127      723 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/abc.py
+-rwxr-xr-x   0     1001      127     1051 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/assembly.py
+-rw-r--r--   0     1001      127     3322 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/gene/attributes.py
+-rw-r--r--   0     1001      127      108 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/gene/__init__.py
+-rw-r--r--   0     1001      127     5168 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/db/ensembl/gene/descriptor.py
+-rw-r--r--   0     1001      127     4568 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/gindex/genomic_index.py
+-rw-r--r--   0     1001      127     3813 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/gindex/test_index.py
+-rw-r--r--   0     1001      127     3699 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/gindex/test_overlap.py
+-rwxr-xr-x   0     1001      127      154 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/gindex/__init__.py
+-rw-r--r--   0     1001      127     2050 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/gindex/overlap.py
+-rw-r--r--   0     1001      127       43 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/ds/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/plot/__init__.py
+-rw-r--r--   0     1001      127     2077 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/test_range.py
+-rw-r--r--   0     1001      127     1501 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/range.py
+-rw-r--r--   0     1001      127     1100 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/strand.py
+-rw-r--r--   0     1001      127     1233 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/orientation.py
+-rw-r--r--   0     1001      127      303 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/__init__.py
+-rw-r--r--   0     1001      127     1456 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/test_strdeductor.py
+-rw-r--r--   0     1001      127      231 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/interval.py
+-rw-r--r--   0     1001      127     2929 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/strdeductor.py
+-rw-r--r--   0     1001      127     1030 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/core/test_orientation.py
+-rw-r--r--   0     1001      127      577 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/algo/misc.py
+-rw-r--r--   0     1001      127       39 2024-05-05 21:21:31.000000 biobit-0.0.2/python/biobit/algo/__init__.py
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 biobit-0.0.2/PKG-INFO
```

### Comparing `biobit-0.0.1/modules/py/Cargo.toml` & `biobit-0.0.2/modules/py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/algo/misc.py` & `biobit-0.0.2/modules/py/python/biobit/algo/misc.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/descriptor.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/design.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/design.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/experiment.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/experiment.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/nfcore/rnaseq/project.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/nfcore/rnaseq/project.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/joblib_counter.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/joblib_counter.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/partition.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/partition.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/counter/reads_counter.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/counter/reads_counter.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/resolve.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/resolve.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/adapters.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/adapters.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/bam.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/bam.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/rcount/source/source.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/rcount/source/source.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/adapter/yaml.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/adapter/yaml.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/experiment.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/experiment.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/filtering_schema.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/filtering_schema.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/library.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/library.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/project.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/project.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/sample.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/sample.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/analysis/seqproj/seqrun.py` & `biobit-0.0.2/modules/py/python/biobit/analysis/seqproj/seqrun.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/core/orientation.py` & `biobit-0.0.2/modules/py/python/biobit/core/orientation.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/core/range.py` & `biobit-0.0.2/modules/py/python/biobit/core/range.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/core/strand.py` & `biobit-0.0.2/modules/py/python/biobit/core/strand.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/core/strdeductor.py` & `biobit-0.0.2/modules/py/python/biobit/core/strdeductor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/abc.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/abc.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/assembly.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/assembly.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/biomart.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/biomart.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/gene/attributes.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/gene/attributes.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/gene/descriptor.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/gene/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/loader.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/loader.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/transcript/attributes.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/transcript/attributes.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/ensembl/transcript/descriptor.py` & `biobit-0.0.2/modules/py/python/biobit/db/ensembl/transcript/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/repmasker/GRCh38.tsv.gz` & `biobit-0.0.2/modules/py/python/biobit/db/repmasker/GRCh38.tsv.gz`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/repmasker/GRCm39.tsv.gz` & `biobit-0.0.2/modules/py/python/biobit/db/repmasker/GRCm39.tsv.gz`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/db/repmasker/repmasker.py` & `biobit-0.0.2/modules/py/python/biobit/db/repmasker/repmasker.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/ds/gindex/genomic_index.py` & `biobit-0.0.2/modules/py/python/biobit/ds/gindex/genomic_index.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/ds/gindex/overlap.py` & `biobit-0.0.2/modules/py/python/biobit/ds/gindex/overlap.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/modules/py/python/biobit/io/bam.py` & `biobit-0.0.2/modules/py/python/biobit/io/bam.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/Cargo.lock` & `biobit-0.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -33,25 +33,25 @@
 name = "autocfg"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "biobit"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "eyre",
  "geo",
  "itertools 0.12.1",
  "num",
 ]
 
 [[package]]
 name = "biobit-py"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "eyre",
  "itertools 0.12.1",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `biobit-0.0.1/Cargo.toml` & `biobit-0.0.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["modules/*"]
 resolver = "2"
 
 [workspace.package]
-version = "0.0.1"
+version = "0.0.2"
 edition = "2021"
 rust-version = "1.77.2"
 authors = ["Aleksandr Fedorov"]
 description = "Rust library for bioinformatics"
 readme = "README.md"
 documentation = "https://github.com/terabio"
 homepage = "https://github.com/terabio"
```

### Comparing `biobit-0.0.1/pyproject.toml` & `biobit-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/resolve.py` & `biobit-0.0.2/python/biobit/analysis/rcount/resolve.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/counter/reads_counter.py` & `biobit-0.0.2/python/biobit/analysis/rcount/counter/reads_counter.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/counter/joblib_counter.py` & `biobit-0.0.2/python/biobit/analysis/rcount/counter/joblib_counter.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/counter/partition.py` & `biobit-0.0.2/python/biobit/analysis/rcount/counter/partition.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/test_resolution.py` & `biobit-0.0.2/python/biobit/analysis/rcount/test_resolution.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/source/source.py` & `biobit-0.0.2/python/biobit/analysis/rcount/source/source.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/source/adapters.py` & `biobit-0.0.2/python/biobit/analysis/rcount/source/adapters.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/rcount/source/bam.py` & `biobit-0.0.2/python/biobit/analysis/rcount/source/bam.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/experiment.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/experiment.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/filtering_schema.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/filtering_schema.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/library.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/library.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/test_seqproj.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/test_seqproj.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/sample.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/sample.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/adapter/test_adapters.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/adapter/test_adapters.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/adapter/yaml.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/adapter/yaml.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/project.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/project.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/seqproj/seqrun.py` & `biobit-0.0.2/python/biobit/analysis/seqproj/seqrun.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py` & `biobit-0.0.2/python/biobit/analysis/nfcore/fetchngs/load_bioproj.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/design.py` & `biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/design.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/experiment.py` & `biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/experiment.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/project.py` & `biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/project.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/analysis/nfcore/rnaseq/descriptor.py` & `biobit-0.0.2/python/biobit/analysis/nfcore/rnaseq/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/io/bam.py` & `biobit-0.0.2/python/biobit/io/bam.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/repmasker/GRCm39.tsv.gz` & `biobit-0.0.2/python/biobit/db/repmasker/GRCm39.tsv.gz`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/repmasker/test_repmasker.py` & `biobit-0.0.2/python/biobit/db/repmasker/test_repmasker.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/repmasker/repmasker.py` & `biobit-0.0.2/python/biobit/db/repmasker/repmasker.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/repmasker/GRCh38.tsv.gz` & `biobit-0.0.2/python/biobit/db/repmasker/GRCh38.tsv.gz`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/loader.py` & `biobit-0.0.2/python/biobit/db/ensembl/loader.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/biomart.py` & `biobit-0.0.2/python/biobit/db/ensembl/biomart.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/transcript/attributes.py` & `biobit-0.0.2/python/biobit/db/ensembl/transcript/attributes.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/transcript/descriptor.py` & `biobit-0.0.2/python/biobit/db/ensembl/transcript/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/abc.py` & `biobit-0.0.2/python/biobit/db/ensembl/abc.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/assembly.py` & `biobit-0.0.2/python/biobit/db/ensembl/assembly.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/gene/attributes.py` & `biobit-0.0.2/python/biobit/db/ensembl/gene/attributes.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/db/ensembl/gene/descriptor.py` & `biobit-0.0.2/python/biobit/db/ensembl/gene/descriptor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/ds/gindex/genomic_index.py` & `biobit-0.0.2/python/biobit/ds/gindex/genomic_index.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/ds/gindex/test_index.py` & `biobit-0.0.2/python/biobit/ds/gindex/test_index.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/ds/gindex/test_overlap.py` & `biobit-0.0.2/python/biobit/ds/gindex/test_overlap.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/ds/gindex/overlap.py` & `biobit-0.0.2/python/biobit/ds/gindex/overlap.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/test_range.py` & `biobit-0.0.2/python/biobit/core/test_range.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/range.py` & `biobit-0.0.2/python/biobit/core/range.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/strand.py` & `biobit-0.0.2/python/biobit/core/strand.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/orientation.py` & `biobit-0.0.2/python/biobit/core/orientation.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/test_strdeductor.py` & `biobit-0.0.2/python/biobit/core/test_strdeductor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/strdeductor.py` & `biobit-0.0.2/python/biobit/core/strdeductor.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/core/test_orientation.py` & `biobit-0.0.2/python/biobit/core/test_orientation.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/python/biobit/algo/misc.py` & `biobit-0.0.2/python/biobit/algo/misc.py`

 * *Files identical despite different names*

### Comparing `biobit-0.0.1/PKG-INFO` & `biobit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: biobit
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: attrs >=23.2.0, <24
 Requires-Dist: cattrs[pyyaml] >=23.2.3, <24
 Requires-Dist: pysam >=0.21.0, <1
```

