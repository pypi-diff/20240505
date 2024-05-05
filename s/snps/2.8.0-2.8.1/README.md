# Comparing `tmp/snps-2.8.0.tar.gz` & `tmp/snps-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snps-2.8.0.tar", last modified: Tue Mar  5 04:46:54 2024, max compression
+gzip compressed data, was "snps-2.8.1.tar", last modified: Sun May  5 04:28:40 2024, max compression
```

## Comparing `snps-2.8.0.tar` & `snps-2.8.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-05 04:46:46.000000 snps-2.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-03-05 04:46:46.000000 snps-2.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-05 04:46:46.000000 snps-2.8.0/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-05 04:46:46.000000 snps-2.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-03-05 04:46:46.000000 snps-2.8.0/LICENSES-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-05 04:46:46.000000 snps-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-05 04:46:54.666469 snps-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-03-05 04:46:46.000000 snps-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.654469 snps-2.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-05 04:46:46.000000 snps-2.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-05 04:46:46.000000 snps-2.8.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-05 04:46:46.000000 snps-2.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-05 04:46:46.000000 snps-2.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-05 04:46:46.000000 snps-2.8.0/docs/contributors.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.654469 snps-2.8.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    42629 2024-03-05 04:46:46.000000 snps-2.8.0/docs/images/snps_banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-05 04:46:46.000000 snps-2.8.0/docs/images/snps_banner.svg
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-05 04:46:46.000000 snps-2.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-05 04:46:46.000000 snps-2.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-05 04:46:46.000000 snps-2.8.0/docs/output_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-05 04:46:46.000000 snps-2.8.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 04:46:46.000000 snps-2.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-05 04:46:46.000000 snps-2.8.0/docs/snps.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-05 04:46:46.000000 snps-2.8.0/docs/snps_banner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-05 04:46:46.000000 snps-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-05 04:46:54.666469 snps-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-05 04:46:46.000000 snps-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.646469 snps-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.654469 snps-2.8.0/src/snps/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-05 04:46:54.670469 snps-2.8.0/src/snps/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/ensembl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.658469 snps-2.8.0/src/snps/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48161 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14261 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/io/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34947 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    71068 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/snps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-03-05 04:46:46.000000 snps-2.8.0/src/snps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/src/snps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-03-05 04:46:54.000000 snps-2.8.0/src/snps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-03-05 04:46:54.000000 snps-2.8.0/src/snps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 04:46:54.000000 snps-2.8.0/src/snps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-05 04:46:54.000000 snps-2.8.0/src/snps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-05 04:46:54.000000 snps-2.8.0/src/snps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.658469 snps-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-03-05 04:46:46.000000 snps-2.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/tests/input/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/23andme.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/23andme_allele.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/23andme_win.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/DNALand.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/GRCh37.csv
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/GRCh37_PAR.csv
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/GRCh38.csv
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/NCBI36.csv
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/ancestry.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/ancestry_mt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/ancestry_multi_sep.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/chromosomes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/circledna.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/codigo46.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/discrepant_snps.csv
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/duplicate_rsids.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/ftdna.csv
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/ftdna_famfinder.csv
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic.csv
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic.fa
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic_extra_column.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic_header_comment.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic_multi_rsid.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic_no_header.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/generic_non_standard_columns.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/genesforgood.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/livingdna.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/mapmygenome.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/mapmygenome_alt_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/myheritage.csv
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/myheritage_extra_quotes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/sano.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/tellmeGen.txt
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/testvcf.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/testvcf_chr_prefix.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/testvcf_multi_sample.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/testvcf_phased.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-05 04:46:46.000000 snps-2.8.0/tests/input/unannotated_testvcf.vcf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:46.000000 snps-2.8.0/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-03-05 04:46:46.000000 snps-2.8.0/tests/io/test_reader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12750 2024-03-05 04:46:46.000000 snps-2.8.0/tests/io/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/tests/output/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_chrom_prefix_chr.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_generic.vcf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/tests/output/vcf_qc/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_qc/qc_only_F_qc_filter_F.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_qc/qc_only_F_qc_filter_T.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_qc/qc_only_T_qc_filter_F.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-05 04:46:46.000000 snps-2.8.0/tests/output/vcf_qc/qc_only_T_qc_filter_T.vcf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 04:46:54.666469 snps-2.8.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-05 04:46:46.000000 snps-2.8.0/tests/resources/dbsnp_151_37_reverse.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-05 04:46:46.000000 snps-2.8.0/tests/resources/gsa_chrpos_map.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-05 04:46:46.000000 snps-2.8.0/tests/resources/gsa_rsid_map.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-03-05 04:46:46.000000 snps-2.8.0/tests/test_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    49987 2024-03-05 04:46:46.000000 snps-2.8.0/tests/test_snps.py
--rw-r--r--   0 runner    (1001) docker     (127)    86854 2024-03-05 04:46:46.000000 snps-2.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.511691 snps-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-05 04:28:29.000000 snps-2.8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-05 04:28:29.000000 snps-2.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-05 04:28:29.000000 snps-2.8.1/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-05 04:28:29.000000 snps-2.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-05-05 04:28:29.000000 snps-2.8.1/LICENSES-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-05 04:28:29.000000 snps-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-05 04:28:40.511691 snps-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-05-05 04:28:29.000000 snps-2.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.495691 snps-2.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-05 04:28:29.000000 snps-2.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-05 04:28:29.000000 snps-2.8.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-05 04:28:29.000000 snps-2.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 04:28:29.000000 snps-2.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-05 04:28:29.000000 snps-2.8.1/docs/contributors.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.495691 snps-2.8.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    42629 2024-05-05 04:28:29.000000 snps-2.8.1/docs/images/snps_banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-05 04:28:29.000000 snps-2.8.1/docs/images/snps_banner.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-05 04:28:29.000000 snps-2.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-05 04:28:29.000000 snps-2.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-05 04:28:29.000000 snps-2.8.1/docs/output_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 04:28:29.000000 snps-2.8.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 04:28:29.000000 snps-2.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-05 04:28:29.000000 snps-2.8.1/docs/snps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-05 04:28:29.000000 snps-2.8.1/docs/snps_banner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-05 04:28:29.000000 snps-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-05 04:28:40.511691 snps-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-05 04:28:29.000000 snps-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.491691 snps-2.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.499691 snps-2.8.1/src/snps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-05 04:28:40.511691 snps-2.8.1/src/snps/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/ensembl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.499691 snps-2.8.1/src/snps/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48161 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14261 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35395 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71068 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/snps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-05-05 04:28:29.000000 snps-2.8.1/src/snps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.511691 snps-2.8.1/src/snps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-05 04:28:40.000000 snps-2.8.1/src/snps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-05 04:28:40.000000 snps-2.8.1/src/snps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 04:28:40.000000 snps-2.8.1/src/snps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-05 04:28:40.000000 snps-2.8.1/src/snps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 04:28:40.000000 snps-2.8.1/src/snps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.499691 snps-2.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    26942 2024-05-05 04:28:29.000000 snps-2.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.507691 snps-2.8.1/tests/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/23andme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/23andme_allele.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/23andme_win.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/DNALand.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/GRCh37.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/GRCh37_PAR.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/GRCh38.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/NCBI36.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/ancestry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/ancestry_mt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/ancestry_multi_sep.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/chromosomes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/circledna.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/codigo46.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/discrepant_snps.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/duplicate_rsids.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/ftdna.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/ftdna_famfinder.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic_extra_column.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic_header_comment.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic_multi_rsid.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic_no_header.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/generic_non_standard_columns.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/genesforgood.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/livingdna.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/mapmygenome.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/mapmygenome_alt_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/myheritage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/myheritage_extra_quotes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/sano.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/tellmeGen.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/testvcf.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/testvcf_chr_prefix.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/testvcf_multi_sample.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/testvcf_phased.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 04:28:29.000000 snps-2.8.1/tests/input/unannotated_testvcf.vcf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.507691 snps-2.8.1/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:29.000000 snps-2.8.1/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-05-05 04:28:29.000000 snps-2.8.1/tests/io/test_reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12750 2024-05-05 04:28:29.000000 snps-2.8.1/tests/io/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.507691 snps-2.8.1/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_chrom_prefix_chr.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_generic.vcf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.507691 snps-2.8.1/tests/output/vcf_qc/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_qc/qc_only_F_qc_filter_F.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_qc/qc_only_F_qc_filter_T.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_qc/qc_only_T_qc_filter_F.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-05 04:28:29.000000 snps-2.8.1/tests/output/vcf_qc/qc_only_T_qc_filter_T.vcf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 04:28:40.511691 snps-2.8.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-05 04:28:29.000000 snps-2.8.1/tests/resources/dbsnp_151_37_reverse.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-05 04:28:29.000000 snps-2.8.1/tests/resources/gsa_chrpos_map.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-05 04:28:29.000000 snps-2.8.1/tests/resources/gsa_rsid_map.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-05 04:28:29.000000 snps-2.8.1/tests/test_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49987 2024-05-05 04:28:29.000000 snps-2.8.1/tests/test_snps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86854 2024-05-05 04:28:29.000000 snps-2.8.1/versioneer.py
```

### Comparing `snps-2.8.0/CONTRIBUTING.rst` & `snps-2.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/CONTRIBUTORS.rst` & `snps-2.8.1/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/LICENSE.txt` & `snps-2.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/LICENSES-3RD-PARTY.txt` & `snps-2.8.1/LICENSES-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/PKG-INFO` & `snps-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snps
-Version: 2.8.0
+Version: 2.8.1
 Summary: tools for reading, writing, merging, and remapping SNPs
 Home-page: https://github.com/apriha/snps
 Author: Andrew Riha
 Author-email: apriha@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://snps.readthedocs.io/
 Project-URL: Changelog, https://github.com/apriha/snps/releases
```

### Comparing `snps-2.8.0/README.rst` & `snps-2.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/Makefile` & `snps-2.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/conf.py` & `snps-2.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/images/snps_banner.png` & `snps-2.8.1/docs/images/snps_banner.png`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/images/snps_banner.svg` & `snps-2.8.1/docs/images/snps_banner.svg`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/index.rst` & `snps-2.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/installation.rst` & `snps-2.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/output_files.rst` & `snps-2.8.1/docs/output_files.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/snps.rst` & `snps-2.8.1/docs/snps.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/docs/snps_banner.rst` & `snps-2.8.1/docs/snps_banner.rst`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/setup.py` & `snps-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/__init__.py` & `snps-2.8.1/src/snps/__init__.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/ensembl.py` & `snps-2.8.1/src/snps/ensembl.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/io/__init__.py` & `snps-2.8.1/src/snps/io/__init__.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/io/reader.py` & `snps-2.8.1/src/snps/io/reader.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/io/writer.py` & `snps-2.8.1/src/snps/io/writer.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/resources.py` & `snps-2.8.1/src/snps/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,18 +283,22 @@
         References
         ----------
         1. Chang Lu, Bastian Greshake Tzovaras, Julian Gough, A survey of
            direct-to-consumer genotype data, and quality control tool
            (GenomePrep) for research, Computational and Structural
            Biotechnology Journal, Volume 19, 2021, Pages 3747-3754, ISSN
            2001-0370, https://doi.org/10.1016/j.csbj.2021.06.040.
+        2. Lu, Tzovaras, & Gough. (2021). OpenSNP data-freeze of 5,393
+           (19.10.2020) [Data set]. In Computational and Structural
+           Biotechnology Journal. Zenodo.
+           https://doi.org/10.1016/j.csbj.2021.06.040
         """
         if self._chip_clusters is None:
             chip_clusters_path = self._download_file(
-                "https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/the_list.tsv.gz",
+                "https://zenodo.org/records/5047472/files/the_list.tsv.gz",
                 "chip_clusters.tsv.gz",
             )
 
             df = pd.read_csv(
                 chip_clusters_path,
                 sep="\t",
                 names=["locus", "clusters"],
@@ -321,18 +325,22 @@
         References
         ----------
         1. Chang Lu, Bastian Greshake Tzovaras, Julian Gough, A survey of
            direct-to-consumer genotype data, and quality control tool
            (GenomePrep) for research, Computational and Structural
            Biotechnology Journal, Volume 19, 2021, Pages 3747-3754, ISSN
            2001-0370, https://doi.org/10.1016/j.csbj.2021.06.040.
+        2. Lu, Tzovaras, & Gough. (2021). OpenSNP data-freeze of 5,393
+           (19.10.2020) [Data set]. In Computational and Structural
+           Biotechnology Journal. Zenodo.
+           https://doi.org/10.1016/j.csbj.2021.06.040
         """
         if self._low_quality_snps is None:
             low_quality_snps_path = self._download_file(
-                "https://supfam.mrc-lmb.cam.ac.uk/GenomePrep/datadir/badalleles.tsv.gz",
+                "https://zenodo.org/records/5047472/files/badalleles.tsv.gz",
                 "low_quality_snps.tsv.gz",
             )
 
             df = pd.read_csv(
                 low_quality_snps_path,
                 sep="\t",
                 names=["cluster", "loci"],
```

### Comparing `snps-2.8.0/src/snps/snps.py` & `snps-2.8.1/src/snps/snps.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps/utils.py` & `snps-2.8.1/src/snps/utils.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/src/snps.egg-info/PKG-INFO` & `snps-2.8.1/src/snps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snps
-Version: 2.8.0
+Version: 2.8.1
 Summary: tools for reading, writing, merging, and remapping SNPs
 Home-page: https://github.com/apriha/snps
 Author: Andrew Riha
 Author-email: apriha@gmail.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://snps.readthedocs.io/
 Project-URL: Changelog, https://github.com/apriha/snps/releases
```

### Comparing `snps-2.8.0/src/snps.egg-info/SOURCES.txt` & `snps-2.8.1/src/snps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/__init__.py` & `snps-2.8.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/discrepant_snps.csv` & `snps-2.8.1/tests/input/discrepant_snps.csv`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/mapmygenome.txt` & `snps-2.8.1/tests/input/mapmygenome.txt`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/mapmygenome_alt_header.txt` & `snps-2.8.1/tests/input/mapmygenome_alt_header.txt`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/testvcf.vcf` & `snps-2.8.1/tests/input/testvcf.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/testvcf_chr_prefix.vcf` & `snps-2.8.1/tests/input/testvcf_chr_prefix.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/testvcf_multi_sample.vcf` & `snps-2.8.1/tests/input/testvcf_multi_sample.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/input/testvcf_phased.vcf` & `snps-2.8.1/tests/input/testvcf_phased.vcf`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/io/test_reader.py` & `snps-2.8.1/tests/io/test_reader.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/io/test_writer.py` & `snps-2.8.1/tests/io/test_writer.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/test_resources.py` & `snps-2.8.1/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/tests/test_snps.py` & `snps-2.8.1/tests/test_snps.py`

 * *Files identical despite different names*

### Comparing `snps-2.8.0/versioneer.py` & `snps-2.8.1/versioneer.py`

 * *Files identical despite different names*

