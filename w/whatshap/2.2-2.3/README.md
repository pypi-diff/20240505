# Comparing `tmp/whatshap-2.2.tar.gz` & `tmp/whatshap-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatshap-2.2.tar", last modified: Fri Jan 26 14:51:28 2024, max compression
+gzip compressed data, was "whatshap-2.3.tar", last modified: Sun May  5 12:11:50 2024, max compression
```

## Comparing `whatshap-2.2.tar` & `whatshap-2.3.tar`

### file list

```diff
@@ -1,460 +1,466 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.250504 whatshap-2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 14:45:49.000000 whatshap-2.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.166504 whatshap-2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-01-26 14:45:49.000000 whatshap-2.2/.github/issue_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.166504 whatshap-2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-01-26 14:45:49.000000 whatshap-2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-26 14:45:49.000000 whatshap-2.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-26 14:45:49.000000 whatshap-2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-26 14:45:49.000000 whatshap-2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-01-26 14:45:49.000000 whatshap-2.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-01-26 14:45:49.000000 whatshap-2.2/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-01-26 14:45:49.000000 whatshap-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-26 14:45:49.000000 whatshap-2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-01-26 14:51:28.250504 whatshap-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-26 14:45:49.000000 whatshap-2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.166504 whatshap-2.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-01-26 14:45:49.000000 whatshap-2.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-26 14:45:49.000000 whatshap-2.2/doc/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.170503 whatshap-2.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-01-26 14:45:49.000000 whatshap-2.2/doc/_static/gtf.png
--rw-r--r--   0 runner    (1001) docker     (127)    29982 2024-01-26 14:45:49.000000 whatshap-2.2/doc/_static/haplotagged-HP.png
--rw-r--r--   0 runner    (1001) docker     (127)    66512 2024-01-26 14:45:49.000000 whatshap-2.2/doc/_static/haplotagged-PS.png
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-26 14:45:49.000000 whatshap-2.2/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-26 14:45:49.000000 whatshap-2.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-01-26 14:45:49.000000 whatshap-2.2/doc/develop.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-26 14:45:49.000000 whatshap-2.2/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50487 2024-01-26 14:45:49.000000 whatshap-2.2/doc/guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-26 14:45:49.000000 whatshap-2.2/doc/howtocite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-26 14:45:49.000000 whatshap-2.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-01-26 14:45:49.000000 whatshap-2.2/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-26 14:45:49.000000 whatshap-2.2/doc/notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-26 14:45:49.000000 whatshap-2.2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.170503 whatshap-2.2/logo/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-26 14:45:49.000000 whatshap-2.2/logo/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-26 14:45:49.000000 whatshap-2.2/logo/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo_notext.png
--rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo_notext.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-01-26 14:45:49.000000 whatshap-2.2/logo/whatshap_logo_text.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.170503 whatshap-2.2/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-26 14:45:49.000000 whatshap-2.2/misc/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-01-26 14:45:49.000000 whatshap-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 14:51:28.250504 whatshap-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-01-26 14:45:49.000000 whatshap-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.178504 whatshap-2.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-01-26 14:45:49.000000 whatshap-2.2/src/backwardcolumniterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-26 14:45:49.000000 whatshap-2.2/src/backwardcolumniterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-26 14:45:49.000000 whatshap-2.2/src/binomial.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-01-26 14:45:49.000000 whatshap-2.2/src/binomial.h
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-01-26 14:45:49.000000 whatshap-2.2/src/caller.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-01-26 14:45:49.000000 whatshap-2.2/src/caller.h
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-01-26 14:45:49.000000 whatshap-2.2/src/columnindexingiterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-26 14:45:49.000000 whatshap-2.2/src/columnindexingiterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-01-26 14:45:49.000000 whatshap-2.2/src/columnindexingscheme.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-26 14:45:49.000000 whatshap-2.2/src/columnindexingscheme.h
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-01-26 14:45:49.000000 whatshap-2.2/src/columniterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-01-26 14:45:49.000000 whatshap-2.2/src/columniterator.h
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-26 14:45:49.000000 whatshap-2.2/src/entry.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-26 14:45:49.000000 whatshap-2.2/src/entry.h
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotype.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotype.h
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypecolumncostcomputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypecolumncostcomputer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypedistribution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypedistribution.h
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypedptable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotypedptable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotyper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-26 14:45:49.000000 whatshap-2.2/src/genotyper.h
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-26 14:45:49.000000 whatshap-2.2/src/graycodes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-01-26 14:45:49.000000 whatshap-2.2/src/graycodes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.182504 whatshap-2.2/src/hapchat/
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/balancedcombinations.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/balancedcombinations.h
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/basictypes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/basictypes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/binomialcoefficient.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/binomialcoefficient.h
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/combinations.h
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/hapchatcolumniterator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    51459 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/hapchatcore.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-01-26 14:45:49.000000 whatshap-2.2/src/hapchat/log.h
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-01-26 14:45:49.000000 whatshap-2.2/src/indexset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-26 14:45:49.000000 whatshap-2.2/src/indexset.h
--rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-01-26 14:45:49.000000 whatshap-2.2/src/mecheader.h
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-01-26 14:45:49.000000 whatshap-2.2/src/multinomial.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-01-26 14:45:49.000000 whatshap-2.2/src/multinomial.h
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigree.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigree.h
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreecolumncostcomputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreecolumncostcomputer.h
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreedptable.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreedptable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreepartitions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedigreepartitions.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    26689 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedmecheuristic.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     8957 2024-01-26 14:45:49.000000 whatshap-2.2/src/pedmecheuristic.h
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-26 14:45:49.000000 whatshap-2.2/src/phredgenotypelikelihoods.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-26 14:45:49.000000 whatshap-2.2/src/phredgenotypelikelihoods.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.186504 whatshap-2.2/src/polyphase/
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/allelematrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/allelematrix.h
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/clustereditingsolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/clustereditingsolution.h
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/clustereditingsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/clustereditingsolver.h
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/edgeheap.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/edgeheap.h
--rw-r--r--   0 runner    (1001) docker     (127)    17768 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/haplothreader.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/haplothreader.h
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/inducedcostheuristic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/inducedcostheuristic.h
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/progenygenotypelikelihoods.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/progenygenotypelikelihoods.h
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/readscoring.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/readscoring.h
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/staticsparsegraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/staticsparsegraph.h
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/switchflipcalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/switchflipcalculator.h
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/trianglesparsematrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/trianglesparsematrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/tuple.h
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/tupleconverter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-01-26 14:45:49.000000 whatshap-2.2/src/polyphase/tupleconverter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-01-26 14:45:49.000000 whatshap-2.2/src/read.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-01-26 14:45:49.000000 whatshap-2.2/src/read.h
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-26 14:45:49.000000 whatshap-2.2/src/readset.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-01-26 14:45:49.000000 whatshap-2.2/src/readset.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.186504 whatshap-2.2/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-01-26 14:45:49.000000 whatshap-2.2/src/testing/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   384567 2024-01-26 14:45:49.000000 whatshap-2.2/src/testing/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-01-26 14:45:49.000000 whatshap-2.2/src/testing/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-01-26 14:45:49.000000 whatshap-2.2/src/transitionprobabilitycomputer.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-26 14:45:49.000000 whatshap-2.2/src/transitionprobabilitycomputer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-01-26 14:45:49.000000 whatshap-2.2/src/vector2d.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.194504 whatshap-2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.226504 whatshap-2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.01.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.01.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.02.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.02.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.03.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.03.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.04.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.04.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.05.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.05.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.biallelic.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.multiallelic.01.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.multiallelic.01.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/alleledetection.multiallelic.vcf
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/chr-lengths.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/duplicate-positions.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/empty_format.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/expected-calls.vcf
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/genetic-haplotyping.ped
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/genetic-haplotyping.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/genotype-likelihoods.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    71353 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X.bam
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X_2.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X_2.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X_3.bam
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.10X_3.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)   415843 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.bam
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.2.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.2.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)   602971 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.bam
--rw-r--r--   0 runner    (1001) docker     (127)   120912 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.large.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.missing_chr.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.missing_chr.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)   327193 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.supplementary.bam
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.supplementary.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.supplementary.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.supplementary.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.without_chr2.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag.without_chr2.vcf.gz.csi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_1.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_1.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_2.bcf
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_2.bcf.csi
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_2.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_2.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)   417657 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noRG.bam
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noRG.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noRG.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noRG.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)   396326 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noSM.bam
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_noSM.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)    84048 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_poly.bam
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_poly.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_poly.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_poly.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_sample.bam
--rw-r--r--   0 runner    (1001) docker     (127)   120608 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_sample.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_sample.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_sample.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)    59894 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_triploid.bam
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_triploid.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_triploid.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_triploid.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_with_csi_index.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/haplotag_with_csi_index.vcf.gz.csi
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/hexadecaploid.chr22.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/indels.sam
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/indels.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/missing-headers.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/multiallelic.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/multisample.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/no-readgroup.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/no-readgroup.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/not-indexed.bam
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/not-indexed.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread-readgroup-without-sample.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread-readgroup-without-sample.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread-ref.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread-ref.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread.crai
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/oneread.cram
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/onevariant.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/onevariant.vcf.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.230504 whatshap-2.2/tests/data/pacbio/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/hapcut.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/haplotags.txt
--rw-r--r--   0 runner    (1001) docker     (127)    90590 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/pacbio.bam
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/pacbio.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/pacbio.crai
--rw-r--r--   0 runner    (1001) docker     (127)    38094 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/pacbio.cram
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/phased.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/phased.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/phased.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/phased_hapchat.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/reference.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/reference.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pacbio/variants.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/paired_end.sorted.sam
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/paired_end.sorted.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    43180 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/ped_samples.bam
--rw-r--r--   0 runner    (1001) docker     (127)    30504 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/ped_samples.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/ped_samples.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/pedigree.ped
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-blocks.blocks.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    99666 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-blocks.reads.bam
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-blocks.reads.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-blocks.variants.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-via-HP-polyploid.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-via-HP.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-via-PS-polyploid.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-via-PS.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased-via-mixed-HP-PS.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased.poly1.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased.poly2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased.poly3.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased1.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased3.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased_overlapping.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased_single_sample1.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phased_single_sample2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/phasedinput.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyphasegenetic.ped1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyphasegenetic.ped2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyphasegenetic.test.parents.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyphasegenetic.test.progeny.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyphasegenetic.test.progeny.vcf.gz.csi
--rw-r--r--   0 runner    (1001) docker     (127)   370565 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.42M.12k.bam
--rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.42M.12k.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.42M.12k.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.inconsistent.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.phased.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.chr22.unphased.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.cuts.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.cuts.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.cuts.vcf
--rw-r--r--   0 runner    (1001) docker     (127)   369929 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.human1.chr22.42M.5k.bam
--rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.human1.chr22.42M.5k.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)   426086 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.human2.chr22.42M.5k.bam
--rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.human2.chr22.42M.5k.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.indels.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.indels.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.indels.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/polyploid.multisample.chr22.42M.5k.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/quartet.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/quartet.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/quartet2.ped
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/quartet2.sam
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/quartet2.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/random0.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/random0.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/reads-no-sequence.bam
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/reads-no-sequence.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/reads-no-sequence.haplotags.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/recombination_breaks.map
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/recombination_breaks.ped
--rw-r--r--   0 runner    (1001) docker     (127)   315878 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/recombination_breaks.sorted.sam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.230504 whatshap-2.2/tests/data/short-genome/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.234504 whatshap-2.2/tests/data/short-genome/learn-data/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/expected.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/short-reads.bam
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/short-reads.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/short-reads.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/short_ref.fasta
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/short_ref.fasta.fai
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/learn-data/variant.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short-hap1.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short-hap2.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short-one-read-duplicate.sam
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short-reads.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short-ref.fasta
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short.sam
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/short.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/short-genome/wrongchromosome.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/string_typed_ps_tag.vcf
--rw-r--r--   0 runner    (1001) docker     (127)    45367 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/test_dist_geno.sam
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/test_dist_geno.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-mendelian-conflict.vcf
--rw-r--r--   0 runner    (1001) docker     (127)   732306 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-merged-blocks.sam
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-merged-blocks.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-missing-genotypes.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-symbolic-alt.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio-two-chromosomes.vcf
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio.map
--rw-r--r--   0 runner    (1001) docker     (127)    95067 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio.pacbio.sam
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio.ped
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio.vcf
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio_genotype_likelihoods.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio_genotype_log_likelihoods.vcf
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/trio_paired_end.ped
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/unknown-genotype.vcf
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/unmapped.bam
--rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/unmapped.bam.bai
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/unphased.vcf
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-26 14:45:49.000000 whatshap-2.2/tests/data/zero-genetic-distance.map
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test.matrix
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_allelematrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_bam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_clusterediting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_geneticmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_genotyping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_kmeralign.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_merge_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_offspringscoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)    28061 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_pedigreegenotyping.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_pedigreephasing.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_pedreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_phasing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_polyphasegenetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_priorityqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_readscoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_readselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_readsetreader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_find_snv_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_genotype.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_hapcut2vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_haplotag.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_learn.py
--rw-r--r--   0 runner    (1001) docker     (127)    35775 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_polyphase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_run_unphase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_variantselection.py
--rw-r--r--   0 runner    (1001) docker     (127)    21185 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-26 14:45:49.000000 whatshap-2.2/tests/test_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-26 14:45:49.000000 whatshap-2.2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.242504 whatshap-2.2/whatshap/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   472288 2024-01-26 14:51:25.000000 whatshap-2.2/whatshap/_variants.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/_variants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/_variants.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   955627 2024-01-26 14:51:25.000000 whatshap-2.2/whatshap/align.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/align.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/align.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/bam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.246504 whatshap-2.2/whatshap/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40497 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/find_snv_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/genotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/hapcut2vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    27057 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/haplotag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)    51385 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)    20351 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/polyphase.py
--rw-r--r--   0 runner    (1001) docker     (127)    24144 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/polyphasegenetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17982 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cli/unphase.py
--rw-r--r--   0 runner    (1001) docker     (127)  1052198 2024-01-26 14:51:26.000000 whatshap-2.2/whatshap/core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/core.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21650 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/phred_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.250504 whatshap-2.2/whatshap/polyphase/
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/clusterarrangement.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/offspringscoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    39121 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    21008 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)   731425 2024-01-26 14:51:26.000000 whatshap-2.2/whatshap/polyphase/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/solver.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/solver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/solver.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/polyphase/variantselection.py
--rw-r--r--   0 runner    (1001) docker     (127)   272263 2024-01-26 14:51:26.000000 whatshap-2.2/whatshap/priorityqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/priorityqueue.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/priorityqueue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/priorityqueue.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   480586 2024-01-26 14:51:27.000000 whatshap-2.2/whatshap/readselect.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/readselect.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/readselect.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)    28408 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/variants.py
--rw-r--r--   0 runner    (1001) docker     (127)    53377 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/vcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-01-26 14:45:49.000000 whatshap-2.2/whatshap/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 14:51:28.250504 whatshap-2.2/whatshap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-26 14:51:28.000000 whatshap-2.2/whatshap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.275828 whatshap-2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 12:06:13.000000 whatshap-2.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.187828 whatshap-2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 12:06:13.000000 whatshap-2.3/.github/issue_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.187828 whatshap-2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-05 12:06:13.000000 whatshap-2.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-05 12:06:13.000000 whatshap-2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-05 12:06:13.000000 whatshap-2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-05 12:06:13.000000 whatshap-2.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17345 2024-05-05 12:06:13.000000 whatshap-2.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-05 12:06:13.000000 whatshap-2.3/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-05 12:06:13.000000 whatshap-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-05 12:06:13.000000 whatshap-2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 12:11:50.275828 whatshap-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-05 12:06:13.000000 whatshap-2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.191828 whatshap-2.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-05 12:06:13.000000 whatshap-2.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-05 12:06:13.000000 whatshap-2.3/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.191828 whatshap-2.3/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26197 2024-05-05 12:06:13.000000 whatshap-2.3/doc/_static/gtf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29982 2024-05-05 12:06:13.000000 whatshap-2.3/doc/_static/haplotagged-HP.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66512 2024-05-05 12:06:13.000000 whatshap-2.3/doc/_static/haplotagged-PS.png
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-05 12:06:13.000000 whatshap-2.3/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-05 12:06:13.000000 whatshap-2.3/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-05 12:06:13.000000 whatshap-2.3/doc/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-05 12:06:13.000000 whatshap-2.3/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    51611 2024-05-05 12:06:13.000000 whatshap-2.3/doc/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 12:06:13.000000 whatshap-2.3/doc/howtocite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-05 12:06:13.000000 whatshap-2.3/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-05 12:06:13.000000 whatshap-2.3/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-05 12:06:13.000000 whatshap-2.3/doc/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-05 12:06:13.000000 whatshap-2.3/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.191828 whatshap-2.3/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-05 12:06:13.000000 whatshap-2.3/logo/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-05 12:06:13.000000 whatshap-2.3/logo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo_notext.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9472 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo_notext.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11310 2024-05-05 12:06:13.000000 whatshap-2.3/logo/whatshap_logo_text.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.191828 whatshap-2.3/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-05 12:06:13.000000 whatshap-2.3/misc/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-05 12:06:13.000000 whatshap-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:11:50.275828 whatshap-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-05 12:06:13.000000 whatshap-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.199828 whatshap-2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-05 12:06:13.000000 whatshap-2.3/src/backwardcolumniterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-05 12:06:13.000000 whatshap-2.3/src/backwardcolumniterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-05 12:06:13.000000 whatshap-2.3/src/binomial.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-05 12:06:13.000000 whatshap-2.3/src/binomial.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-05 12:06:13.000000 whatshap-2.3/src/caller.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-05 12:06:13.000000 whatshap-2.3/src/caller.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-05 12:06:13.000000 whatshap-2.3/src/columnindexingiterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-05 12:06:13.000000 whatshap-2.3/src/columnindexingiterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-05 12:06:13.000000 whatshap-2.3/src/columnindexingscheme.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 12:06:13.000000 whatshap-2.3/src/columnindexingscheme.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-05-05 12:06:13.000000 whatshap-2.3/src/columniterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-05 12:06:13.000000 whatshap-2.3/src/columniterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-05 12:06:13.000000 whatshap-2.3/src/entry.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-05 12:06:13.000000 whatshap-2.3/src/entry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotype.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotype.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypecolumncostcomputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypecolumncostcomputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypedistribution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypedistribution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypedptable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotypedptable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotyper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-05 12:06:13.000000 whatshap-2.3/src/genotyper.h
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-05 12:06:13.000000 whatshap-2.3/src/graycodes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-05 12:06:13.000000 whatshap-2.3/src/graycodes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.203828 whatshap-2.3/src/hapchat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/balancedcombinations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/balancedcombinations.h
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/basictypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/basictypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/binomialcoefficient.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/binomialcoefficient.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/combinations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/hapchatcolumniterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    51459 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/hapchatcore.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-05 12:06:13.000000 whatshap-2.3/src/hapchat/log.h
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-05 12:06:13.000000 whatshap-2.3/src/indexset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-05 12:06:13.000000 whatshap-2.3/src/indexset.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)      876 2024-05-05 12:06:13.000000 whatshap-2.3/src/mecheader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-05 12:06:13.000000 whatshap-2.3/src/multinomial.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-05 12:06:13.000000 whatshap-2.3/src/multinomial.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigree.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreecolumncostcomputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreecolumncostcomputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreedptable.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreedptable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreepartitions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedigreepartitions.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26689 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedmecheuristic.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8957 2024-05-05 12:06:13.000000 whatshap-2.3/src/pedmecheuristic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-05 12:06:13.000000 whatshap-2.3/src/phredgenotypelikelihoods.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-05 12:06:13.000000 whatshap-2.3/src/phredgenotypelikelihoods.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.207828 whatshap-2.3/src/polyphase/
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/allelematrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/allelematrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/clustereditingsolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/clustereditingsolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/clustereditingsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/clustereditingsolver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/edgeheap.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/edgeheap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17768 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/haplothreader.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/haplothreader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/inducedcostheuristic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/inducedcostheuristic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/progenygenotypelikelihoods.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/progenygenotypelikelihoods.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/readscoring.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/readscoring.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/staticsparsegraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/staticsparsegraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/switchflipcalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/switchflipcalculator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/trianglesparsematrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/trianglesparsematrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/tuple.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/tupleconverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-05 12:06:13.000000 whatshap-2.3/src/polyphase/tupleconverter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-05 12:06:13.000000 whatshap-2.3/src/read.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-05 12:06:13.000000 whatshap-2.3/src/read.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-05 12:06:13.000000 whatshap-2.3/src/readset.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-05 12:06:13.000000 whatshap-2.3/src/readset.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.211828 whatshap-2.3/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-05 12:06:13.000000 whatshap-2.3/src/testing/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   384567 2024-05-05 12:06:13.000000 whatshap-2.3/src/testing/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19136 2024-05-05 12:06:13.000000 whatshap-2.3/src/testing/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-05 12:06:13.000000 whatshap-2.3/src/transitionprobabilitycomputer.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-05 12:06:13.000000 whatshap-2.3/src/transitionprobabilitycomputer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-05 12:06:13.000000 whatshap-2.3/src/vector2d.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.215828 whatshap-2.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.251828 whatshap-2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.01.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.01.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.02.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.02.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.03.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.03.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.04.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.04.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.05.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.05.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.biallelic.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.multiallelic.01.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.multiallelic.01.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/alleledetection.multiallelic.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/chr-lengths.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/duplicate-positions.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/empty_format.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/expected-calls.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/genetic-haplotyping.ped
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/genetic-haplotyping.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/genotype-likelihoods.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    71353 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X.bam
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X_2.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X_2.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X_3.bam
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.10X_3.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)   415843 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.2.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.2.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)   602971 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.bam
+-rw-r--r--   0 runner    (1001) docker     (127)   120912 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.large.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.missing_chr.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.missing_chr.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)   327193 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.supplementary.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.supplementary.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.supplementary.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.supplementary.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.without_chr2.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag.without_chr2.vcf.gz.csi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_1.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_1.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_2.bcf
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_2.bcf.csi
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_2.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_2.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)   417657 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noRG.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noRG.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noRG.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noRG.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)   396326 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noSM.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_noSM.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)    84048 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_poly.bam
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_poly.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_poly.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_poly.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_sample.bam
+-rw-r--r--   0 runner    (1001) docker     (127)   120608 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_sample.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_sample.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_sample.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)    59894 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_triploid.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_triploid.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_triploid.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_triploid.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_with_csi_index.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/haplotag_with_csi_index.vcf.gz.csi
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/hexadecaploid.chr22.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/indels.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/indels.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/missing-headers.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/multiallelic.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/multisample.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/no-readgroup.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/no-readgroup.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/not-indexed.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/not-indexed.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread-readgroup-without-sample.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread-readgroup-without-sample.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread-ref.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread-ref.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread.crai
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/oneread.cram
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/onevariant.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/onevariant.vcf.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.255828 whatshap-2.3/tests/data/pacbio/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/hapcut.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100161 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/haplotagged.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/haplotagged.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/haplotags.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    90590 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/pacbio.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/pacbio.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/pacbio.crai
+-rw-r--r--   0 runner    (1001) docker     (127)    38094 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/pacbio.cram
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/phased.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/phased.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/phased.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/phased_hapchat.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    26521 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/reference.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/reference.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pacbio/variants.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/paired_end.sorted.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/paired_end.sorted.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    43180 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/ped_samples.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    30504 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/ped_samples.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/ped_samples.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/pedigree.ped
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-blocks.blocks.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    99666 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-blocks.reads.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-blocks.reads.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-blocks.variants.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-via-HP-polyploid.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-via-HP.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-via-PS-polyploid.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-via-PS.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased-via-mixed-HP-PS.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased.poly1.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased.poly2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased.poly3.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased1.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased3.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased_overlapping.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased_single_sample1.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phased_single_sample2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/phasedinput.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyphasegenetic.ped1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyphasegenetic.ped2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyphasegenetic.test.parents.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyphasegenetic.test.progeny.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyphasegenetic.test.progeny.vcf.gz.csi
+-rw-r--r--   0 runner    (1001) docker     (127)   370565 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.42M.12k.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.42M.12k.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.42M.12k.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.inconsistent.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.phased.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.chr22.unphased.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.cuts.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.cuts.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.cuts.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)   369929 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.human1.chr22.42M.5k.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    20616 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.human1.chr22.42M.5k.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)   426086 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.human2.chr22.42M.5k.bam
+-rw-r--r--   0 runner    (1001) docker     (127)    20672 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.human2.chr22.42M.5k.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.indels.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.indels.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.indels.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/polyploid.multisample.chr22.42M.5k.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/quartet.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/quartet.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/quartet2.ped
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/quartet2.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/quartet2.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/random0.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/random0.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/reads-no-sequence.bam
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/reads-no-sequence.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/reads-no-sequence.haplotags.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/recombination_breaks.map
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/recombination_breaks.ped
+-rw-r--r--   0 runner    (1001) docker     (127)   315878 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/recombination_breaks.sorted.sam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.255828 whatshap-2.3/tests/data/short-genome/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.259828 whatshap-2.3/tests/data/short-genome/learn-data/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/expected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/short-reads.bam
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/short-reads.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/short-reads.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/short_ref.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/short_ref.fasta.fai
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/learn-data/variant.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short-hap1.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short-hap2.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short-one-read-duplicate.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short-reads.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short-ref.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/short.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/short-genome/wrongchromosome.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/string_typed_ps_tag.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)    45367 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/test_dist_geno.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/test_dist_geno.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-mendelian-conflict.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)   732306 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-merged-blocks.sam
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-merged-blocks.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-missing-genotypes.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-symbolic-alt.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio-two-chromosomes.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio.map
+-rw-r--r--   0 runner    (1001) docker     (127)    95067 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio.pacbio.sam
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio.ped
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio_genotype_likelihoods.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio_genotype_log_likelihoods.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/trio_paired_end.ped
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/unknown-genotype.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/unmapped.bam
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/unmapped.bam.bai
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/unphased.vcf
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-05 12:06:13.000000 whatshap-2.3/tests/data/zero-genetic-distance.map
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test.matrix
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_allelematrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_bam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_clusterediting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_geneticmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12991 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_genotyping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_kmeralign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_merge_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_offspringscoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28062 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_pedigreegenotyping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_pedigreephasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_pedreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_phasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_polyphasegenetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_priorityqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_read_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_readscoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_readselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_readsetreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_find_snv_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16174 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_hapcut2vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_haplotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_haplotagphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35776 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_polyphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_run_unphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_variantselection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21185 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-05 12:06:13.000000 whatshap-2.3/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-05 12:06:13.000000 whatshap-2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.267828 whatshap-2.3/whatshap/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   472288 2024-05-05 12:11:46.000000 whatshap-2.3/whatshap/_variants.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/_variants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12514 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/_variants.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   955627 2024-05-05 12:11:47.000000 whatshap-2.3/whatshap/align.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/align.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/align.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/bam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.271828 whatshap-2.3/whatshap/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40498 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/find_snv_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/hapcut2vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27058 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/haplotag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15050 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/haplotagphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52281 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20352 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/polyphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24145 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/polyphasegenetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cli/unphase.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1068350 2024-05-05 12:11:47.000000 whatshap-2.3/whatshap/core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/phred_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.275828 whatshap-2.3/whatshap/polyphase/
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/clusterarrangement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/offspringscoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39161 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21006 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)   731425 2024-05-05 12:11:48.000000 whatshap-2.3/whatshap/polyphase/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/solver.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/solver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/solver.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/polyphase/variantselection.py
+-rw-r--r--   0 runner    (1001) docker     (127)   272263 2024-05-05 12:11:48.000000 whatshap-2.3/whatshap/priorityqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/priorityqueue.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/priorityqueue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/priorityqueue.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   480586 2024-05-05 12:11:48.000000 whatshap-2.3/whatshap/readselect.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/readselect.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11276 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/readselect.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33241 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53162 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/vcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-05 12:06:13.000000 whatshap-2.3/whatshap/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:11:50.275828 whatshap-2.3/whatshap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13096 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 12:11:50.000000 whatshap-2.3/whatshap.egg-info/top_level.txt
```

### Comparing `whatshap-2.2/.github/workflows/ci.yml` & `whatshap-2.3/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -11,71 +11,75 @@
     timeout-minutes: 10
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.10"]
         toxenv: [flake8, docs, twinecheck, black]
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: python -m pip install tox
     - name: Run tox ${{ matrix.toxenv }}
       run: tox -e ${{ matrix.toxenv }}
 
   build:
     if: >-
       github.event_name != 'pull_request' ||
       github.event.pull_request.head.repo.full_name != github.event.pull_request.base.repo.full_name
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
     - name: Install dependencies
       run: python -m pip install build
     - name: Build temporary sdist and wheel
       run: python -m build
 
   test:
     if: >-
       github.event_name != 'pull_request' ||
       github.event.pull_request.head.repo.full_name != github.event.pull_request.base.repo.full_name
     timeout-minutes: 15
-    runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        os: [ubuntu-latest]
+        include:
+        - os: macos-13
+          python-version: "3.10"
+    runs-on: ${{ matrix.os }}
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: python -m pip install tox
     - name: Test with tox
       run: tox -e py
 
   deploy:
     timeout-minutes: 30
     runs-on: ubuntu-latest
     needs: [lint, build, test]
     if: startsWith(github.ref, 'refs/tags')
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0  # required for setuptools_scm
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
     - name: Build wheels
       uses: pypa/cibuildwheel@v2.16.2
       with:
         output-dir: dist/
       env:
```

### Comparing `whatshap-2.2/CHANGES.rst` & `whatshap-2.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =======
 Changes
 =======
 
+v2.3 (2024-05-05)
+-----------------
+
+* :pr:`521`: Added ``haplotagphase`` command. The command adds phase information to variants
+  based on haplotagged reads.
+  Contributed by Nikolai Karpov (@nkkarpov) and Mitchell Robert Vollger (@mrvollger).
+* :issue:`516`: Added ``--use-supplementary`` option to ``phase``. Use this to use supplementary
+  alignments for phasing (previously, supplementary alignments would be ignored).
+  Contributed by Nikolai Karpov (@nkkarpov).
+
 v2.2 (2024-01-26)
 -----------------
 
 * :issue:`496`: Fixed a segmentation fault in ``polyphase``.
 * :issue:`498`: Fixed a numeric overflow in the scoring phase of ``polyphase``.
   It could occur for variants with extremely high coverages (i.e. >200X).
 * :issue:`472`: Fixed various warnings and assertion violations when running
```

### Comparing `whatshap-2.2/CITATION.rst` & `whatshap-2.3/CITATION.rst`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/LICENSE` & `whatshap-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/PKG-INFO` & `whatshap-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatshap
-Version: 2.2
+Version: 2.3
 Summary: phase genomic variants using DNA sequencing reads
 Author: WhatsHap authors
 License: MIT
 Project-URL: Homepage, https://github.com/whatshap/whatshap
 Project-URL: Changelog, https://whatshap.readthedocs.io/en/latest/changes.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatshap-2.2/README.md` & `whatshap-2.3/README.md`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/Makefile` & `whatshap-2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/README.rst` & `whatshap-2.3/doc/README.rst`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/_static/gtf.png` & `whatshap-2.3/doc/_static/gtf.png`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/_static/haplotagged-HP.png` & `whatshap-2.3/doc/_static/haplotagged-HP.png`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/_static/haplotagged-PS.png` & `whatshap-2.3/doc/_static/haplotagged-PS.png`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/conf.py` & `whatshap-2.3/doc/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Sphinx configuration
 
 import os
 import sys
-import time
 
 from setuptools_scm import get_version
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath(os.pardir))
```

### Comparing `whatshap-2.2/doc/develop.rst` & `whatshap-2.3/doc/develop.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,22 @@
 For development, make sure that you install Cython and tox. We also recommend
 using a virtualenv. This sequence of commands should work (use
 ``https://github.com/whatshap/whatshap.git`` as URL if you do not have a
 GitHub account)::
 
     git clone git@github.com:whatshap/whatshap.git
     cd whatshap
-    python3 -m venv venv
-    source venv/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip install -e .[dev]
 
 The last command installs also all the development dependencies.
 Omit the ``[dev]`` to leave them out.
 
-Next, you can run WhatsHap like this::
-
-    whatshap --help
+Install also `pre-commit <https://pre-commit.com/>`_ and run ``pre-commit install``.
 
 
 Development installation when using Conda
 -----------------------------------------
 
 If you are familiar with `Conda <https://docs.conda.io/en/latest/>`_, you can
 also use a Conda environment for developing WhatsHap. We recommend that you
@@ -55,25 +53,28 @@
 `tox <https://tox.readthedocs.io/>`_. It creates separate virtual environments for each Python
 version, installs WhatsHap into it and then runs the tests. It also tests documentation generation
 with ``sphinx``. Run it like this::
 
     tox
 
 If ``tox`` is installed on the system, you do not need to be inside a virtual environment for this.
-However, you need to have all tested Python versions installed on the system! See the instructions
-below for how to do this on Ubuntu.
+Run ``tox --skip-missing-interpreters`` if you do not have all tested Python versions installed.
+See one way below for how to install them on Ubuntu.
 
 
 Code style
 ----------
 
 Python code needs to be formatted with `Black <https://github.com/psf/black>`_.
-Either run `black whatshap tests` manually before you commit or use the
+Either run ``black whatshap tests`` manually before you commit or use the
 `pre-commit <https://pre-commit.com/>`_ framework to automate this.
 
+To check other style issues, run ::
+
+    tox -e flake8
 
 Installing other Python versions in Ubuntu
 ------------------------------------------
 
 Ubuntu comes with one default Python 3 version, and in order to test WhatsHap
 with older or newer Python versions, follow the instructions for enabling the
 `“deadsnakes” repository <https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa>`_.
@@ -179,27 +180,28 @@
 
 #. Run ``tox``.
 
 #. Tag the current commit with the version number (there must be a ``v`` prefix)::
 
        git tag -a -m "Version 0.1" v0.1
 
-   To release a development version, use a ``dev`` version number such as
-   ``v0.17.dev1``.
+   To release a development version, use an ``rc`` version number such as
+   ``v0.17rc1``.
    Users will only get these when they use ``pip install --pre``.
 
 #. Push the tag::
 
        git push --tags
 
 #. Wait for the GitHub Action to finish. It will deploy the sdist and wheels to
    PyPI if everything worked correctly.
 
-#. Update the `Bioconda recipe <https://github.com/bioconda/bioconda-recipes/blob/master/recipes/whatshap/meta.yaml>`_. It is easiest to wait for the Bioconda bot to open a PR. Ensure
-   that the list of dependencies (the ``requirements:``
+#. To update the `Bioconda recipe <https://github.com/bioconda/bioconda-recipes/blob/master/recipes/whatshap/meta.yaml>`_,
+   wait for the Bioconda bot to open a PR (in the ``bioconda-recipes`` repository).
+   Ensure that the list of dependencies (the ``requirements:``
    section in the recipe) is in sync with the ``setup.py`` file. If changes are
    necessary to the bot-generated PR, just add your own commits to that PR.
 
 If something went wrong, fix the problem and follow the above instructions again,
 but with an incremented revision in the version number. That is, go from version
 x.y to x.y.1. PyPI will not allow you to change a version that has already been
 uploaded.
```

### Comparing `whatshap-2.2/doc/faq.rst` & `whatshap-2.3/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/guide.rst` & `whatshap-2.3/doc/guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 :ref:`compare <whatshap-compare>`             Compare two or more phasings
 hapcut2vcf                                    Convert hapCUT output format to VCF
 unphase                                       Remove phasing information from a VCF file
 :ref:`haplotag <whatshap-haplotag>`           Tag reads by haplotype
 :ref:`genotype <whatshap-genotype>`           Genotype variants
 :ref:`split <whatshap-split>`                 Split reads by haplotype
 :ref:`learn <whatshap-learn>`                 Generate sequencing technology specific error profiles
+:ref:`haplotagphase <whatshap-haplotagphase>`  Phase VCF file using haplotagged BAM file
 ============================================= ======================================================
 
 Not all are fully documented in this manual, yet. To get help for a
 subcommand named ``SUBCOMMAND``, run ::
 
     whatshap SUBCOMMAND --help
 
@@ -529,16 +530,16 @@
 
 file_name
     The VCF file name to which the numbers in this row refer to.
 
 The numbers in these following columns are computed on the variant level.
 
 variants
-    Number of biallelic variants in the input VCF, but excluding any non-SNV variants if
-    ``--only-snvs`` was used.
+    Number of biallelic variants in the input VCF excluding duplicate positions
+    and, if ``--only-snvs`` was used, also excluding any non-SNV variants.
 
 heterozygous_variants
     The number of biallelic, heterozygous variants in the input VCF.
     This is a subset of *variants* as defined above.
 
 heterozygous_snvs
     The number of biallelic, heterozygous SNVs in the input VCF.
@@ -1182,7 +1183,28 @@
     python3 -m whatshap.phred_scores -i kmer_pair_counts_dir -o phred_scores.txt -k kmer_size -e pseudocount_value_for_unobserved_kmer_pairs
 
   Note that ``kmer_pair_counts_dir`` is the path to the directory containing the output from single whole genome or multiple chromosome specific iterations of ``whatshap learn``.
 
 2. Use ``whatshap genotype`` with additional arguments for *k*-merald based genotyping::
 
     whatshap genotype [options] --use-kmerald --reference ref.fasta variants.vcf reads.bam --kmeralign-costs phred_scores.txt --kmer-size kmer_size --kmerald-gappenalty gap_cost --kmerald-window window_size -o genotyped_variants.vcf
+
+.. _whatshap-haplotagphase:
+
+whatshap haplotagphase: Phase VCF file using haplotagged BAM file
+=================================================================
+Given a haplotagged BAM file, a file with variants, and a reference, this command sequence outputs a phased VCF file::
+
+    tabix input.vcf.gz
+    samtools index haplotagged.bam
+    whatshap haplotagphase [options] -r reference.fasta input.vcf.gz haplotagged.bam -o output.vcf.gz
+
+It assigns phase information to a variant if the majority of reads containing this variant support the assignment. Additionally, it does not assign phase information to variants located within long homopolymers. The command supports the following options:
+
+``-g x``
+    Assigns information to the variant only if at least x percent of reads support the assignment (default value is 70).
+
+``-c x``
+    Ignores variants that lie inside homopolymers of length at least x (default value is 10).
+
+``--only-indels``
+    Assigns information only to indel events.
```

### Comparing `whatshap-2.2/doc/installation.rst` & `whatshap-2.3/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/doc/notes.rst` & `whatshap-2.3/doc/notes.rst`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo.pdf` & `whatshap-2.3/logo/whatshap_logo.pdf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo.png` & `whatshap-2.3/logo/whatshap_logo.png`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo.svg` & `whatshap-2.3/logo/whatshap_logo.svg`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo_notext.png` & `whatshap-2.3/logo/whatshap_logo_notext.png`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo_notext.svg` & `whatshap-2.3/logo/whatshap_logo_notext.svg`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/logo/whatshap_logo_text.svg` & `whatshap-2.3/logo/whatshap_logo_text.svg`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/misc/example.py` & `whatshap-2.3/misc/example.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/pyproject.toml` & `whatshap-2.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -80,8 +80,11 @@
 # Disable tests for the moment because pip attempts to install pysam
 # from source for some reason although wheels exist.
 # test-requires = "pytest"
 # test-command = ["cd {project} ; pytest tests/test_run_phase.py"]
 
 [tool.ruff]
 line-length = 100
-ignore = ["E501"]  # line too long
+lint.ignore = [
+    "E501",  # line too long
+    "E741",  # Ambiguous variable name
+]
```

### Comparing `whatshap-2.2/setup.py` & `whatshap-2.3/setup.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/backwardcolumniterator.cpp` & `whatshap-2.3/src/backwardcolumniterator.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/backwardcolumniterator.h` & `whatshap-2.3/src/backwardcolumniterator.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/binomial.cpp` & `whatshap-2.3/src/binomial.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/caller.cpp` & `whatshap-2.3/src/caller.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/caller.h` & `whatshap-2.3/src/caller.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columnindexingiterator.cpp` & `whatshap-2.3/src/columnindexingiterator.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columnindexingiterator.h` & `whatshap-2.3/src/columnindexingiterator.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columnindexingscheme.cpp` & `whatshap-2.3/src/columnindexingscheme.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columnindexingscheme.h` & `whatshap-2.3/src/columnindexingscheme.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columniterator.cpp` & `whatshap-2.3/src/columniterator.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/columniterator.h` & `whatshap-2.3/src/columniterator.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/entry.cpp` & `whatshap-2.3/src/entry.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/entry.h` & `whatshap-2.3/src/entry.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotype.cpp` & `whatshap-2.3/src/genotype.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotype.h` & `whatshap-2.3/src/genotype.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypecolumncostcomputer.cpp` & `whatshap-2.3/src/genotypecolumncostcomputer.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypecolumncostcomputer.h` & `whatshap-2.3/src/genotypecolumncostcomputer.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypedistribution.cpp` & `whatshap-2.3/src/genotypedistribution.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypedistribution.h` & `whatshap-2.3/src/genotypedistribution.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypedptable.cpp` & `whatshap-2.3/src/genotypedptable.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotypedptable.h` & `whatshap-2.3/src/genotypedptable.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotyper.cpp` & `whatshap-2.3/src/genotyper.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/genotyper.h` & `whatshap-2.3/src/genotyper.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/graycodes.cpp` & `whatshap-2.3/src/graycodes.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/graycodes.h` & `whatshap-2.3/src/graycodes.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/balancedcombinations.cpp` & `whatshap-2.3/src/hapchat/balancedcombinations.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/balancedcombinations.h` & `whatshap-2.3/src/hapchat/balancedcombinations.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/basictypes.cpp` & `whatshap-2.3/src/hapchat/basictypes.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/basictypes.h` & `whatshap-2.3/src/hapchat/basictypes.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/binomialcoefficient.cpp` & `whatshap-2.3/src/hapchat/binomialcoefficient.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/binomialcoefficient.h` & `whatshap-2.3/src/hapchat/binomialcoefficient.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/combinations.h` & `whatshap-2.3/src/hapchat/combinations.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/hapchatcolumniterator.cpp` & `whatshap-2.3/src/hapchat/hapchatcolumniterator.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/hapchatcore.cpp` & `whatshap-2.3/src/hapchat/hapchatcore.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/hapchat/log.h` & `whatshap-2.3/src/hapchat/log.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/indexset.cpp` & `whatshap-2.3/src/indexset.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/indexset.h` & `whatshap-2.3/src/indexset.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/mecheader.h` & `whatshap-2.3/src/mecheader.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/multinomial.cpp` & `whatshap-2.3/src/multinomial.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/multinomial.h` & `whatshap-2.3/src/multinomial.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigree.cpp` & `whatshap-2.3/src/pedigree.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigree.h` & `whatshap-2.3/src/pedigree.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreecolumncostcomputer.cpp` & `whatshap-2.3/src/pedigreecolumncostcomputer.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreecolumncostcomputer.h` & `whatshap-2.3/src/pedigreecolumncostcomputer.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreedptable.cpp` & `whatshap-2.3/src/pedigreedptable.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreedptable.h` & `whatshap-2.3/src/pedigreedptable.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreepartitions.cpp` & `whatshap-2.3/src/pedigreepartitions.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedigreepartitions.h` & `whatshap-2.3/src/pedigreepartitions.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedmecheuristic.cpp` & `whatshap-2.3/src/pedmecheuristic.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/pedmecheuristic.h` & `whatshap-2.3/src/pedmecheuristic.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/phredgenotypelikelihoods.cpp` & `whatshap-2.3/src/phredgenotypelikelihoods.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/phredgenotypelikelihoods.h` & `whatshap-2.3/src/phredgenotypelikelihoods.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/allelematrix.cpp` & `whatshap-2.3/src/polyphase/allelematrix.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/allelematrix.h` & `whatshap-2.3/src/polyphase/allelematrix.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/clustereditingsolution.cpp` & `whatshap-2.3/src/polyphase/clustereditingsolution.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/clustereditingsolution.h` & `whatshap-2.3/src/polyphase/clustereditingsolution.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/clustereditingsolver.h` & `whatshap-2.3/src/polyphase/clustereditingsolver.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/edgeheap.cpp` & `whatshap-2.3/src/polyphase/edgeheap.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/edgeheap.h` & `whatshap-2.3/src/polyphase/edgeheap.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/haplothreader.cpp` & `whatshap-2.3/src/polyphase/haplothreader.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/haplothreader.h` & `whatshap-2.3/src/polyphase/haplothreader.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/inducedcostheuristic.cpp` & `whatshap-2.3/src/polyphase/inducedcostheuristic.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/inducedcostheuristic.h` & `whatshap-2.3/src/polyphase/inducedcostheuristic.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/progenygenotypelikelihoods.cpp` & `whatshap-2.3/src/polyphase/progenygenotypelikelihoods.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/progenygenotypelikelihoods.h` & `whatshap-2.3/src/polyphase/progenygenotypelikelihoods.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/readscoring.cpp` & `whatshap-2.3/src/polyphase/readscoring.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/readscoring.h` & `whatshap-2.3/src/polyphase/readscoring.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/staticsparsegraph.cpp` & `whatshap-2.3/src/polyphase/staticsparsegraph.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/staticsparsegraph.h` & `whatshap-2.3/src/polyphase/staticsparsegraph.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/switchflipcalculator.cpp` & `whatshap-2.3/src/polyphase/switchflipcalculator.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/switchflipcalculator.h` & `whatshap-2.3/src/polyphase/switchflipcalculator.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/trianglesparsematrix.cpp` & `whatshap-2.3/src/polyphase/trianglesparsematrix.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/trianglesparsematrix.h` & `whatshap-2.3/src/polyphase/trianglesparsematrix.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/tuple.h` & `whatshap-2.3/src/polyphase/tuple.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/tupleconverter.cpp` & `whatshap-2.3/src/polyphase/tupleconverter.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/polyphase/tupleconverter.h` & `whatshap-2.3/src/polyphase/tupleconverter.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/read.cpp` & `whatshap-2.3/src/read.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #include <cassert>
 
 
 #include "read.h"
 
 using namespace std;
 
-Read::Read(const std::string& name, int mapq, int source_id, int sample_id, int reference_start, const std::string& BX_tag) : name(name), mapqs(1, mapq), source_id(source_id), sample_id(sample_id), reference_start(reference_start), BX_tag(BX_tag) {
+Read::Read(const std::string& name, int mapq, int source_id, int sample_id, int reference_start, const std::string& BX_tag, int HP_tag, int PS_tag) : name(name), mapqs(1, mapq), source_id(source_id), sample_id(sample_id), reference_start(reference_start), BX_tag(BX_tag), HP_tag(HP_tag), PS_tag(PS_tag) {
 	this->id = -1;
 }
 
 
 string Read::toString() {
 	ostringstream oss;
 	oss << name << " mapq:(";
@@ -167,7 +167,23 @@
 	}
 	return true;
 }
 
 bool Read::hasBXTag() const {
 	return (BX_tag != "");
 }
+
+int Read::getHPTag() const {
+	return HP_tag; 
+}
+
+bool Read::hasHPTag() const {
+	return (HP_tag > 0);
+}
+
+int Read::getPSTag() const {
+	return PS_tag; 
+}
+
+bool Read::hasPSTag() const {
+	return (PS_tag > 0);
+}
```

### Comparing `whatshap-2.2/src/read.h` & `whatshap-2.3/src/read.h`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include <vector>
 #include <unordered_set>
 
 #include "entry.h"
 
 class Read {
 public:
-	Read(const std::string& name, int mapq, int source_id, int sample_id, int reference_start = -1, const std::string& BX_tag = "");
+	Read(const std::string& name, int mapq, int source_id, int sample_id, int reference_start = -1, const std::string& BX_tag = "", int HP_tag = -1, int PS_tag = -1);
 	virtual ~Read() {}
 	std::string toString();
 	void addVariant(int position, int allele, int quality);
 	void sortVariants();
 	/** Returns the position of the first variant. **/
 	int firstPosition() const;
 	/** Returns the position of the last variant. **/
@@ -35,14 +35,18 @@
 	void addMapq(int mapq);
 	int getSourceID() const;
 	int getSampleID() const;
 	int getReferenceStart() const;
 	const std::string& getBXTag() const;
 	bool isSorted() const;
 	bool hasBXTag() const;
+	int getHPTag() const;
+	bool hasHPTag() const;
+	int getPSTag() const;
+	bool hasPSTag() const;
 private:
 	typedef struct enriched_entry_t {
 		Entry entry;
 		int position;
 		enriched_entry_t(int position, int allele, int quality) :
 			entry(0,Entry::allele_t(allele),quality), position(position) {}
 	} enriched_entry_t;
@@ -57,11 +61,13 @@
 	std::string name;
 	std::vector<int> mapqs;
 	int source_id;
 	int sample_id;
 	int id;
 	int reference_start;
 	std::string BX_tag;
+	int HP_tag;
+	int PS_tag;
 	std::vector<enriched_entry_t> variants;
 };
 
 #endif
```

### Comparing `whatshap-2.2/src/readset.cpp` & `whatshap-2.3/src/readset.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/readset.h` & `whatshap-2.3/src/readset.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/testing/CMakeLists.txt` & `whatshap-2.3/src/testing/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/testing/catch.hpp` & `whatshap-2.3/src/testing/catch.hpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/testing/test.cpp` & `whatshap-2.3/src/testing/test.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/transitionprobabilitycomputer.cpp` & `whatshap-2.3/src/transitionprobabilitycomputer.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/transitionprobabilitycomputer.h` & `whatshap-2.3/src/transitionprobabilitycomputer.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/src/vector2d.h` & `whatshap-2.3/src/vector2d.h`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/alleledetection.biallelic.vcf` & `whatshap-2.3/tests/data/alleledetection.biallelic.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/alleledetection.fasta` & `whatshap-2.3/tests/data/alleledetection.fasta`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/alleledetection.multiallelic.vcf` & `whatshap-2.3/tests/data/alleledetection.multiallelic.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/empty_format.vcf` & `whatshap-2.3/tests/data/empty_format.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/expected-calls.vcf` & `whatshap-2.3/tests/data/expected-calls.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/genotype-likelihoods.vcf` & `whatshap-2.3/tests/data/genotype-likelihoods.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.10X.bam` & `whatshap-2.3/tests/data/haplotag.10X.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.10X.bam.bai` & `whatshap-2.3/tests/data/haplotag.10X.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.10X_3.bam` & `whatshap-2.3/tests/data/haplotag.10X_3.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.10X_3.bam.bai` & `whatshap-2.3/tests/data/haplotag.10X_3.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.bam` & `whatshap-2.3/tests/data/haplotag.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.bam.bai` & `whatshap-2.3/tests/data/haplotag.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.large.bam` & `whatshap-2.3/tests/data/haplotag.large.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.large.bam.bai` & `whatshap-2.3/tests/data/haplotag.large.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.supplementary.bam` & `whatshap-2.3/tests/data/haplotag.supplementary.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.supplementary.bam.bai` & `whatshap-2.3/tests/data/haplotag.supplementary.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag.supplementary.vcf.gz` & `whatshap-2.3/tests/data/haplotag.supplementary.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_1.vcf.gz` & `whatshap-2.3/tests/data/haplotag_1.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_2.bcf` & `whatshap-2.3/tests/data/haplotag_2.bcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_2.vcf.gz` & `whatshap-2.3/tests/data/haplotag_2.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_noRG.bam` & `whatshap-2.3/tests/data/haplotag_noRG.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_noRG.bam.bai` & `whatshap-2.3/tests/data/haplotag_noRG.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_noRG.vcf.gz` & `whatshap-2.3/tests/data/haplotag_noRG.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_noSM.bam` & `whatshap-2.3/tests/data/haplotag_noSM.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_noSM.bam.bai` & `whatshap-2.3/tests/data/haplotag_noSM.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_poly.bam` & `whatshap-2.3/tests/data/haplotag_poly.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_poly.bam.bai` & `whatshap-2.3/tests/data/haplotag_poly.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_poly.vcf.gz` & `whatshap-2.3/tests/data/haplotag_poly.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_sample.bam` & `whatshap-2.3/tests/data/haplotag_sample.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_sample.bam.bai` & `whatshap-2.3/tests/data/haplotag_sample.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_triploid.bam` & `whatshap-2.3/tests/data/haplotag_triploid.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_triploid.bam.bai` & `whatshap-2.3/tests/data/haplotag_triploid.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_triploid.vcf.gz` & `whatshap-2.3/tests/data/haplotag_triploid.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/haplotag_with_csi_index.vcf.gz` & `whatshap-2.3/tests/data/haplotag_with_csi_index.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/hexadecaploid.chr22.vcf` & `whatshap-2.3/tests/data/hexadecaploid.chr22.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/indels.sam` & `whatshap-2.3/tests/data/indels.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/multiallelic.vcf` & `whatshap-2.3/tests/data/multiallelic.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/oneread.cram` & `whatshap-2.3/tests/data/oneread.cram`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/Makefile` & `whatshap-2.3/tests/data/pacbio/Makefile`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/hapcut.txt` & `whatshap-2.3/tests/data/pacbio/hapcut.txt`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/haplotags.txt` & `whatshap-2.3/tests/data/pacbio/haplotags.txt`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/pacbio.bam` & `whatshap-2.3/tests/data/pacbio/pacbio.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/pacbio.cram` & `whatshap-2.3/tests/data/pacbio/pacbio.cram`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/phased.vcf` & `whatshap-2.3/tests/data/pacbio/phased.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/phased.vcf.gz` & `whatshap-2.3/tests/data/pacbio/phased.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/phased_hapchat.vcf` & `whatshap-2.3/tests/data/pacbio/phased_hapchat.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/reference.fasta` & `whatshap-2.3/tests/data/pacbio/reference.fasta`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/pacbio/variants.vcf` & `whatshap-2.3/tests/data/pacbio/variants.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/paired_end.sorted.sam` & `whatshap-2.3/tests/data/paired_end.sorted.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/ped_samples.bam` & `whatshap-2.3/tests/data/ped_samples.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/ped_samples.bam.bai` & `whatshap-2.3/tests/data/ped_samples.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/ped_samples.vcf` & `whatshap-2.3/tests/data/ped_samples.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-blocks.blocks.vcf` & `whatshap-2.3/tests/data/phased-blocks.blocks.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-blocks.reads.bam` & `whatshap-2.3/tests/data/phased-blocks.reads.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-blocks.variants.vcf` & `whatshap-2.3/tests/data/phased-blocks.variants.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-via-HP-polyploid.vcf` & `whatshap-2.3/tests/data/phased-via-HP-polyploid.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-via-HP.vcf` & `whatshap-2.3/tests/data/phased-via-HP.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-via-PS-polyploid.vcf` & `whatshap-2.3/tests/data/phased-via-PS-polyploid.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-via-PS.vcf` & `whatshap-2.3/tests/data/phased-via-PS.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased-via-mixed-HP-PS.vcf` & `whatshap-2.3/tests/data/phased-via-mixed-HP-PS.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased.poly1.vcf` & `whatshap-2.3/tests/data/phased.poly1.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased.poly2.vcf` & `whatshap-2.3/tests/data/phased.poly2.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased.poly3.vcf` & `whatshap-2.3/tests/data/phased.poly3.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased1.vcf` & `whatshap-2.3/tests/data/phased1.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased2.vcf` & `whatshap-2.3/tests/data/phased2.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased3.vcf` & `whatshap-2.3/tests/data/phased3.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/phased_overlapping.vcf` & `whatshap-2.3/tests/data/phased_overlapping.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyphasegenetic.test.parents.vcf` & `whatshap-2.3/tests/data/polyphasegenetic.test.parents.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyphasegenetic.test.progeny.vcf.gz` & `whatshap-2.3/tests/data/polyphasegenetic.test.progeny.vcf.gz`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.42M.12k.bam` & `whatshap-2.3/tests/data/polyploid.chr22.42M.12k.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.42M.12k.bam.bai` & `whatshap-2.3/tests/data/polyploid.chr22.42M.12k.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.42M.12k.vcf` & `whatshap-2.3/tests/data/polyploid.chr22.42M.12k.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.inconsistent.vcf` & `whatshap-2.3/tests/data/polyploid.chr22.inconsistent.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.phased.vcf` & `whatshap-2.3/tests/data/polyploid.chr22.phased.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.chr22.unphased.vcf` & `whatshap-2.3/tests/data/polyploid.chr22.unphased.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.cuts.bam` & `whatshap-2.3/tests/data/polyploid.cuts.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.cuts.vcf` & `whatshap-2.3/tests/data/polyploid.cuts.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.human1.chr22.42M.5k.bam` & `whatshap-2.3/tests/data/polyploid.human1.chr22.42M.5k.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.human1.chr22.42M.5k.bam.bai` & `whatshap-2.3/tests/data/polyploid.human1.chr22.42M.5k.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.human2.chr22.42M.5k.bam` & `whatshap-2.3/tests/data/polyploid.human2.chr22.42M.5k.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.human2.chr22.42M.5k.bam.bai` & `whatshap-2.3/tests/data/polyploid.human2.chr22.42M.5k.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.indels.vcf` & `whatshap-2.3/tests/data/polyploid.indels.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/polyploid.multisample.chr22.42M.5k.vcf` & `whatshap-2.3/tests/data/polyploid.multisample.chr22.42M.5k.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/quartet2.sam` & `whatshap-2.3/tests/data/quartet2.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/quartet2.vcf` & `whatshap-2.3/tests/data/quartet2.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/random0.fasta` & `whatshap-2.3/tests/data/random0.fasta`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/reads-no-sequence.bam` & `whatshap-2.3/tests/data/reads-no-sequence.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/recombination_breaks.sorted.sam` & `whatshap-2.3/tests/data/recombination_breaks.sorted.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/short-genome/short-one-read-duplicate.sam` & `whatshap-2.3/tests/data/short-genome/short-one-read-duplicate.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/short-genome/short.sam` & `whatshap-2.3/tests/data/short-genome/short.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/test_dist_geno.sam` & `whatshap-2.3/tests/data/test_dist_geno.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-mendelian-conflict.vcf` & `whatshap-2.3/tests/data/trio-mendelian-conflict.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-merged-blocks.sam` & `whatshap-2.3/tests/data/trio-merged-blocks.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-merged-blocks.vcf` & `whatshap-2.3/tests/data/trio-merged-blocks.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-missing-genotypes.vcf` & `whatshap-2.3/tests/data/trio-missing-genotypes.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-symbolic-alt.vcf` & `whatshap-2.3/tests/data/trio-symbolic-alt.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio-two-chromosomes.vcf` & `whatshap-2.3/tests/data/trio-two-chromosomes.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio.pacbio.sam` & `whatshap-2.3/tests/data/trio.pacbio.sam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio.vcf` & `whatshap-2.3/tests/data/trio.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio_genotype_likelihoods.vcf` & `whatshap-2.3/tests/data/trio_genotype_likelihoods.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/trio_genotype_log_likelihoods.vcf` & `whatshap-2.3/tests/data/trio_genotype_log_likelihoods.vcf`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/unmapped.bam` & `whatshap-2.3/tests/data/unmapped.bam`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/data/unmapped.bam.bai` & `whatshap-2.3/tests/data/unmapped.bam.bai`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_align.py` & `whatshap-2.3/tests/test_align.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Edit distance tests
 
 The initial version was copied from https://bitbucket.org/marcelm/sqt/src/af255d54a21815cb9a3e0b279b431a320d4626bd/tests/testalign.py
 """
+
 from whatshap.align import edit_distance as ed
 from whatshap.align import edit_distance_affine_gap as ed_aff
 from random import choice, seed, randint
 
 
 STRING_PAIRS = [
     ("", ""),
```

### Comparing `whatshap-2.2/tests/test_allelematrix.py` & `whatshap-2.3/tests/test_allelematrix.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_bam.py` & `whatshap-2.3/tests/test_bam.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_clusterediting.py` & `whatshap-2.3/tests/test_clusterediting.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_geneticmap.py` & `whatshap-2.3/tests/test_geneticmap.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_genotyping.py` & `whatshap-2.3/tests/test_genotyping.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_graph.py` & `whatshap-2.3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_merge_reads.py` & `whatshap-2.3/tests/test_merge_reads.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_offspringscoring.py` & `whatshap-2.3/tests/test_offspringscoring.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_pedigree.py` & `whatshap-2.3/tests/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_pedigreegenotyping.py` & `whatshap-2.3/tests/test_pedigreegenotyping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test genotyping of pedigrees
 """
+
 import math
 
 from whatshap.core import (
     GenotypeDPTable,
     ReadSet,
     Pedigree,
     NumericSampleIds,
```

### Comparing `whatshap-2.2/tests/test_pedigreephasing.py` & `whatshap-2.3/tests/test_pedigreephasing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test phasing of pedigrees (PedMEC algorithm)
 """
+
 from collections import defaultdict
 from pytest import raises
 from whatshap.core import (
     PedigreeDPTable,
     ReadSet,
     Pedigree,
     NumericSampleIds,
```

### Comparing `whatshap-2.2/tests/test_pedreader.py` & `whatshap-2.3/tests/test_pedreader.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_phasing.py` & `whatshap-2.3/tests/test_phasing.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_polyphasegenetic.py` & `whatshap-2.3/tests/test_polyphasegenetic.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_priorityqueue.py` & `whatshap-2.3/tests/test_priorityqueue.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_reads.py` & `whatshap-2.3/tests/test_reads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test Read and ReadSet classes
 """
+
 from pytest import raises
 from whatshap.core import Read, ReadSet, Variant
 
 
 def test_read():
     r = Read("name", 15)
     assert r.name == "name"
```

### Comparing `whatshap-2.2/tests/test_readscoring.py` & `whatshap-2.3/tests/test_readscoring.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_readselect.py` & `whatshap-2.3/tests/test_readselect.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_readsetreader.py` & `whatshap-2.3/tests/test_readsetreader.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_reorder.py` & `whatshap-2.3/tests/test_reorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     assert breakpoints[1].position == 6
     assert breakpoints[2].position == 9
     assert breakpoints[0].haplotypes == breakpoints[1].haplotypes == [0, 1, 2]
     assert breakpoints[2].haplotypes == [0, 2]
     assert haplotypes == haplotypes_old
 
 
-def test_integrate_subresults3():
+def test_integrate_subresults3() -> None:
     am, clustering, threads, haplotypes = get_instance3()
     sub = find_subinstances(am, clustering, threads, haplotypes)
     sub_results = []
     sub_results.append(
         PolyphaseBlockResult(0, [[0, 1, 2], [3, 4]], [[0, 1], [0, 1]], [[0, 0], [1, 1]], [])
     )
     breakpoints = integrate_sub_results(am, sub, sub_results, threads, haplotypes)
```

### Comparing `whatshap-2.2/tests/test_run_compare.py` & `whatshap-2.3/tests/test_run_compare.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_find_snv_candidates.py` & `whatshap-2.3/tests/test_run_find_snv_candidates.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_genotype.py` & `whatshap-2.3/tests/test_run_genotype.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_haplotag.py` & `whatshap-2.3/tests/test_run_haplotag.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_learn.py` & `whatshap-2.3/tests/test_run_learn.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_phase.py` & `whatshap-2.3/tests/test_run_phase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Integration tests that use the command-line entry points run_whatshap, run_haplotag etc.
 """
+
 import os
 from collections import namedtuple
 
 from pytest import raises, fixture, mark
 import pysam
 from whatshap.cli.phase import run_whatshap
 from whatshap.cli import CommandLineError
```

### Comparing `whatshap-2.2/tests/test_run_polyphase.py` & `whatshap-2.3/tests/test_run_polyphase.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Integration tests that use the command-line entry point run_polyphase.
 """
+
 import os
 
 from pytest import raises
 from whatshap.cli.polyphase import run_polyphase, CommandLineError
 from whatshap.vcf import VcfReader
```

### Comparing `whatshap-2.2/tests/test_run_split.py` & `whatshap-2.3/tests/test_run_split.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_run_stats.py` & `whatshap-2.3/tests/test_run_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests for 'whatshap stats'
 """
+
 from collections import namedtuple
 from whatshap.cli.stats import run_stats, unpack_chromosomes
 
 
 def test_stats1(tmp_path):
     outtsv = tmp_path / "output.tsv"
     run_stats(
```

### Comparing `whatshap-2.2/tests/test_run_unphase.py` & `whatshap-2.3/tests/test_run_unphase.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_threading.py` & `whatshap-2.3/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_utils.py` & `whatshap-2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_variantselection.py` & `whatshap-2.3/tests/test_variantselection.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_vcf.py` & `whatshap-2.3/tests/test_vcf.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tests/test_verification.py` & `whatshap-2.3/tests/test_verification.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/tox.ini` & `whatshap-2.3/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     build
 commands =
     python -m build --sdist --outdir {envtmpdir}/dist
     twine check {envtmpdir}/dist/*
 
 [testenv:black]
 basepython = python3.10
-deps = black==22.3.0
+deps = black==24.3.0
 skip_install = true
 commands = black --check whatshap/ tests/ setup.py
 
 [testenv:flake8]
 basepython = python3.10
 deps = flake8
 skip_install = true
```

### Comparing `whatshap-2.2/whatshap/__main__.py` & `whatshap-2.3/whatshap/__main__.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/_variants.cpp` & `whatshap-2.3/whatshap/_variants.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/_variants.pyi` & `whatshap-2.3/whatshap/_variants.pyi`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/_variants.pyx` & `whatshap-2.3/whatshap/_variants.pyx`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/align.cpp` & `whatshap-2.3/whatshap/align.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/align.pyx` & `whatshap-2.3/whatshap/align.pyx`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/args.py` & `whatshap-2.3/whatshap/args.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/bam.py` & `whatshap-2.3/whatshap/bam.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/cli/__init__.py` & `whatshap-2.3/whatshap/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/cli/compare.py` & `whatshap-2.3/whatshap/cli/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Compare two or more phased variant files
 """
+
 import logging
 import math
 from collections import defaultdict
 from contextlib import ExitStack
 import dataclasses
 from itertools import chain, permutations
 from typing import Set, List, Optional, DefaultDict, Dict
```

### Comparing `whatshap-2.2/whatshap/cli/find_snv_candidates.py` & `whatshap-2.3/whatshap/cli/find_snv_candidates.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/cli/genotype.py` & `whatshap-2.3/whatshap/cli/genotype.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Genotype variants
 
 Runs only the genotyping algorithm. Genotype Likelihoods are computed using the
 forward backward algorithm.
 """
+
 import logging
 import sys
 import platform
 from argparse import SUPPRESS
 from typing import Sequence, Optional
 
 from contextlib import ExitStack
```

### Comparing `whatshap-2.2/whatshap/cli/hapcut2vcf.py` & `whatshap-2.3/whatshap/cli/hapcut2vcf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 HapCUT’s output file format is explained at
 <https://github.com/vibansal/hapcut#format-of-input-and-output-files>
 
 HapCUT2’s output format is documented at
 <https://github.com/pjedge/hapcut2#output-format>
 """
+
 import logging
 import re
 import sys
 from collections import namedtuple
 import itertools
 from contextlib import ExitStack
```

### Comparing `whatshap-2.2/whatshap/cli/haplotag.py` & `whatshap-2.3/whatshap/cli/haplotag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Tag reads by haplotype
 
 Sequencing reads are read from file ALIGNMENTS (in BAM or CRAM format) and tagged reads
 are written to stdout.
 """
+
 import logging
 import sys
 import pysam
 import hashlib
 from collections import defaultdict
 from typing import List, Optional, Union, Dict, Tuple, FrozenSet, Sequence, TextIO
```

### Comparing `whatshap-2.2/whatshap/cli/learn.py` & `whatshap-2.3/whatshap/cli/learn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Generate sequencing technology specific error profiles
 """
+
 import logging
 import pysam
 import pyfaidx
 from whatshap.core import Caller
 from pysam import VariantFile
```

### Comparing `whatshap-2.2/whatshap/cli/phase.py` & `whatshap-2.3/whatshap/cli/phase.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     RecombinationCostComputer,
     Trio,
 )
 from whatshap.timer import StageTimer
 from whatshap.utils import plural_s, warn_once
 from whatshap.cli import CommandLineError, log_memory_usage, PhasedInputReader
 from whatshap.merge import ReadMerger, DoNothingReadMerger, ReadMergerBase
+from whatshap.types import PhasingAlgorithm
 
 __author__ = "Murray Patterson, Alexander Schönhuth, Tobias Marschall, Marcel Martin"
 
 logger = logging.getLogger(__name__)
 
 
 def find_components(
@@ -306,14 +307,16 @@
     tag: str = "PS",
     read_list_filename: Optional[str] = None,
     gl_regularizer: Optional[float] = None,
     gtchange_list_filename: Optional[str] = None,
     default_gq: int = 30,
     write_command_line_header: bool = True,
     use_ped_samples: bool = False,
+    use_supplementary: bool = False,
+    supplementary_distance_threshold: int = 100_000,
     algorithm: str = "whatshap",
 ) -> None:
     """
     Run WhatsHap.
 
     phase_input_files -- list of paths to BAM/CRAM/VCF files
     variant_file -- path to input VCF
@@ -324,14 +327,17 @@
     ignore_read_groups
     mapping_quality -- discard reads below this mapping quality
     read_merging -- whether or not to merge reads
     read_merging_error_rate -- probability that a nucleotide is wrong
     read_merging_max_error_rate -- max error rate on edge of merge graph considered
     read_merging_positive_threshold -- threshold on the ratio of the two probabilities
     read_merging_negative_threshold -- threshold on the opposite ratio of positive threshold
+    use_supplementary -- use supplementary alignments with primary
+    supplementary_distance_threshold -- distance threshold for filtering supplementary alignments
+
     max_coverage
     distrust_genotypes
     include_homozygous
     genetic_haplotyping -- in ped mode, merge disconnected blocks based on genotype status
     recombination_list_filename -- filename to write putative recombination events to
     tag -- How to store phasing info in the VCF, can be 'PS' or 'HP'
     read_list_filename -- name of file to write list of used reads to
@@ -342,15 +348,14 @@
     write_command_line_header -- whether to add a ##commandline header to the output VCF
     """
 
     if algorithm == "hapchat" and ped is not None:
         raise CommandLineError("The hapchat algorithm cannot do pedigree phasing")
     if samples is None:
         samples = []
-
     timers = StageTimer()
     logger.info(f"This is WhatsHap {__version__} running under Python {platform.python_version()}")
     numeric_sample_ids = NumericSampleIds()
     command_line: Optional[str]
     if write_command_line_header:
         command_line = "(whatshap {}) {}".format(__version__, " ".join(sys.argv[1:]))
     else:
@@ -373,14 +378,16 @@
             PhasedInputReader(
                 phase_input_files,
                 None if reference is False else reference,
                 numeric_sample_ids,
                 ignore_read_groups,
                 mapq_threshold=mapping_quality,
                 only_snvs=only_snvs,
+                use_supplementary=use_supplementary,
+                supplementary_distance_threshold=supplementary_distance_threshold,
             )
         )
         show_phase_vcfs = phased_input_reader.has_vcfs
 
         if phased_input_reader.has_alignments and reference is None:
             raise CommandLineError(
                 "A reference FASTA needs to be provided with -r/--reference; "
@@ -565,15 +572,15 @@
                     logger.info(
                         "Phasing %d sample%s by solving the %s problem ...",
                         len(family),
                         plural_s(len(family)),
                         problem_name,
                     )
 
-                    dp_table: Union[HapChatCore, PedigreeDPTable]
+                    dp_table: PhasingAlgorithm
                     if algorithm == "hapchat":
                         dp_table = HapChatCore(all_reads)
                     elif algorithm == "heuristic":
                         all_reads.sort()
                         dp_table = PedMecHeuristic(
                             all_reads,
                             recombination_costs,
@@ -605,14 +612,15 @@
                         homozygous_positions,
                         numeric_sample_ids,
                         superreads_list,
                     )
                     log_component_stats(overall_components, len(accessible_positions))
 
                 if recombination_list_filename:
+                    assert transmission_vector is not None
                     n_recombinations = write_recombination_list(
                         recombination_list_filename,
                         chromosome,
                         accessible_positions,
                         overall_components,
                         recombination_costs,
                         transmission_vector,
@@ -1134,14 +1142,20 @@
         action="store_false", default=True,
         help="Do not merge blocks that are not connected by reads (i.e. solely based on genotype "
         "status). Default: when in --ped mode, merge all blocks that contain at least one "
         "homozygous genotype in at least one individual into one block.")
     arg("--use-ped-samples", dest="use_ped_samples",
         action="store_true", default=False,
         help="Only work on samples mentioned in the provided PED file.")
+    arg("--use-supplementary", dest="use_supplementary", action="store_true", default=False,
+        help="Use also supplementary alignments (default: ignore supplementary_ alignments)")
+    arg("--supplementary-distance", metavar="DIST", dest="supplementary_distance_threshold", default=100_000,
+        help="Skip supplementary alignments further than DIST bp away from the primary alignment (default: %(default)s)")
+
+
 # fmt: on
 
 
 def validate(args, parser):
     if args.reference is not None and args.no_reference:
         parser.error("Options --reference and --no-reference cannot be used together")
     if args.ignore_read_groups and args.ped:
```

### Comparing `whatshap-2.2/whatshap/cli/polyphase.py` & `whatshap-2.3/whatshap/cli/polyphase.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Read a VCF and one or more files with phase information (BAM/CRAM or VCF phased
 blocks) and phase the variants. The phased VCF is written to standard output.
 Requires to specify a ploidy for the phasable input. Allows to specify a block
 cut sensitivity to balance out length and accuracy of phased blocks.
 
 """
+
 import sys
 import logging
 import platform
 import argparse
 
 from copy import deepcopy
```

### Comparing `whatshap-2.2/whatshap/cli/polyphasegenetic.py` & `whatshap-2.3/whatshap/cli/polyphasegenetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Read a VCF and one or more files with phase information (BAM/CRAM or VCF phased
 blocks) and phase the variants. The phased VCF is written to standard output.
 Requires to specify a ploidy for the phasable input. Allows to specify a block
 cut sensitivity to balance out length and accuracy of phased blocks.
 
 """
+
 import sys
 import logging
 import platform
 import argparse
 
 from collections import defaultdict
 from dataclasses import dataclass
```

### Comparing `whatshap-2.2/whatshap/cli/split.py` & `whatshap-2.3/whatshap/cli/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     whatshap split --output-h1 h1.fastq.gz --output-h2 h2.fastq.gz reads.fastq.gz haplotypes.txt
     whatshap split --output-h1 h1.bam --output-h2 h2.bam reads.bam haplotypes.txt
 
 Tetraploid:
 
     whatshap split -o h1.bam -o h2.bam -o h3.bam -o h4.bam reads.bam haplotypes.txt
 """
+
 import logging
 import os
 import pysam
 from collections import defaultdict, Counter
 import itertools
 
 from xopen import xopen
```

### Comparing `whatshap-2.2/whatshap/cli/stats.py` & `whatshap-2.3/whatshap/cli/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Print phasing statistics of a single VCF file
 """
+
 import logging
 from collections import defaultdict
 from contextlib import ExitStack
 import dataclasses
 from statistics import median
 from typing import List, Tuple, Optional, Dict, Sequence, Iterator
 from math import isnan
@@ -297,39 +298,43 @@
             return DetailedStats(
                 variants=self.variants,
                 phased=sum(block_sizes),
                 unphased=self.unphased,
                 singletons=n_singletons,
                 blocks=len(block_sizes),
                 variant_per_block_median=median(block_sizes),
-                variant_per_block_avg=sum(block_sizes) / len(block_sizes)
-                if len(block_sizes)
-                else float("nan"),
+                variant_per_block_avg=(
+                    sum(block_sizes) / len(block_sizes) if len(block_sizes) else float("nan")
+                ),
                 variant_per_block_min=block_sizes[0],
                 variant_per_block_max=block_sizes[-1],
                 variant_per_block_sum=sum(block_sizes),
                 bp_per_block_median=median(block_lengths),
-                bp_per_block_avg=sum(block_lengths) / len(block_lengths)
-                if len(block_lengths)
-                else float("nan"),
+                bp_per_block_avg=(
+                    sum(block_lengths) / len(block_lengths) if len(block_lengths) else float("nan")
+                ),
                 bp_per_block_min=block_lengths[0],
                 bp_per_block_max=block_lengths[-1],
                 bp_per_block_sum=sum(block_lengths),
                 heterozygous_variants=self.heterozygous_variants,
                 heterozygous_snvs=self.heterozygous_snvs,
                 phased_snvs=phased_snvs,
-                phased_fraction=sum(block_sizes) / self.heterozygous_variants
-                if self.heterozygous_variants
-                else float("nan"),
-                phased_snvs_fraction=phased_snvs / self.heterozygous_snvs
-                if self.heterozygous_snvs
-                else float("nan"),
-                block_n50=compute_ng50(self.split_blocks, chr_lengths)
-                if chr_lengths is not None
-                else float("nan"),
+                phased_fraction=(
+                    sum(block_sizes) / self.heterozygous_variants
+                    if self.heterozygous_variants
+                    else float("nan")
+                ),
+                phased_snvs_fraction=(
+                    phased_snvs / self.heterozygous_snvs if self.heterozygous_snvs else float("nan")
+                ),
+                block_n50=(
+                    compute_ng50(self.split_blocks, chr_lengths)
+                    if chr_lengths is not None
+                    else float("nan")
+                ),
             )
         else:
             return DetailedStats(
                 variants=self.variants,
                 unphased=self.unphased,
                 singletons=n_singletons,
                 heterozygous_variants=self.heterozygous_variants,
```

### Comparing `whatshap-2.2/whatshap/cli/unphase.py` & `whatshap-2.3/whatshap/cli/unphase.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 - The HP, PS and PQ tags are removed
 - Phasing in the GT tag (using pipe notation) is removed. The genotypes are
   sorted in ascending order. For example, a GT value of '1|0' is converted
   to '0/1'.
 
 It is not an error if no phasing information was found.
 """
+
 import sys
 import logging
 from pysam import VariantFile
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `whatshap-2.2/whatshap/core.cpp` & `whatshap-2.3/whatshap/core.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1235,16 +1235,16 @@
 struct __pyx_obj_8whatshap_4core_PedMecHeuristic {
   PyObject_HEAD
   PedMecHeuristic *thisptr;
   struct __pyx_obj_8whatshap_4core_Pedigree *pedigree;
 };
 
 
-/* "whatshap/core.pyx":117
- * 			return self.thisptr.getBXTag().decode('utf-8')
+/* "whatshap/core.pyx":128
+ * 			return self.thisptr.getPSTag()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		"""Iterate over all variants in this read"""
  * 		assert self.thisptr != NULL
  */
 struct __pyx_obj_8whatshap_4core___pyx_scope_struct____iter__ {
   PyObject_HEAD
@@ -1252,15 +1252,15 @@
   struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self;
   Py_ssize_t __pyx_t_0;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
 };
 
 
-/* "whatshap/core.pyx":234
+/* "whatshap/core.pyx":253
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for i in range(self.thisptr.size()):
  * 			yield self[i]
  */
 struct __pyx_obj_8whatshap_4core___pyx_scope_struct_1___iter__ {
@@ -1269,15 +1269,15 @@
   struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self;
   int __pyx_t_0;
   int __pyx_t_1;
   int __pyx_t_2;
 };
 
 
-/* "whatshap/core.pyx":429
+/* "whatshap/core.pyx":448
  * 		return self.thisptr.size()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for genotype in self.genotypes():
  * 			yield self[genotype]
  */
 struct __pyx_obj_8whatshap_4core___pyx_scope_struct_2___iter__ {
@@ -2079,14 +2079,16 @@
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_mapqs[] = "mapqs";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_BX_tag[] = "BX_tag";
 static const char __pyx_k_Caller[] = "Caller";
+static const char __pyx_k_HP_tag[] = "HP_tag";
+static const char __pyx_k_PS_tag[] = "PS_tag";
 static const char __pyx_k_allele[] = "allele";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_ploidy[] = "ploidy";
 static const char __pyx_k_reduce[] = "__reduce__";
@@ -2162,28 +2164,30 @@
 static const char __pyx_k_bam_alignment_cigartuples[] = "bam_alignment_cigartuples";
 static const char __pyx_k_Wrappers_for_core_C_classes[] = "\nWrappers for core C++ classes.\n";
 static const char __pyx_k_Read_does_not_support_slices[] = "Read does not support slices";
 static const char __pyx_k_PhredGenotypeLikelihoods___iter[] = "PhredGenotypeLikelihoods.__iter__";
 static const char __pyx_k_Querying_a_ReadSet_by_read_name[] = "Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead";
 static const char __pyx_k_ReadSet_does_not_support_slices[] = "ReadSet does not support slices";
 static const char __pyx_k_Expected_instance_of_Variant_but[] = "Expected instance of Variant, but found {}";
-static const char __pyx_k_Read_name_r_mapq_source_id_sampl[] = "Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})";
+static const char __pyx_k_Read_name_r_mapq_source_id_sampl[] = "Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static PyObject *__pyx_n_s_BX_tag;
 static PyObject *__pyx_n_s_Caller;
 static PyObject *__pyx_kp_u_Expected_instance_of_Variant_but;
 static PyObject *__pyx_n_s_Genotype;
 static PyObject *__pyx_n_s_GenotypeDPTable;
+static PyObject *__pyx_n_s_HP_tag;
 static PyObject *__pyx_n_s_HapChatCore;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_u_Index_out_of_bounds;
 static PyObject *__pyx_kp_u_Invalid_key;
 static PyObject *__pyx_n_s_KeyError;
 static PyObject *__pyx_n_s_NotImplementedError;
 static PyObject *__pyx_n_s_NumericSampleIds;
+static PyObject *__pyx_n_s_PS_tag;
 static PyObject *__pyx_n_s_PedMecHeuristic;
 static PyObject *__pyx_n_s_Pedigree;
 static PyObject *__pyx_n_s_PedigreeDPTable;
 static PyObject *__pyx_n_s_PhredGenotypeLikelihoods;
 static PyObject *__pyx_n_s_PhredGenotypeLikelihoods___iter;
 static PyObject *__pyx_kp_u_Querying_a_ReadSet_by_read_name;
 static PyObject *__pyx_n_s_Read;
@@ -2285,37 +2289,41 @@
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_6__str__(struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_8freeze(struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_10inverse_mapping(struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_12__getstate__(struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_14__setstate__(struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self, PyObject *__pyx_v_state); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_16NumericSampleIds_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_NumericSampleIds *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_8whatshap_4core_4Read___cinit__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_mapq, int __pyx_v_source_id, int __pyx_v_sample_id, int __pyx_v_reference_start, PyObject *__pyx_v_BX_tag); /* proto */
+static int __pyx_pf_8whatshap_4core_4Read___cinit__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_mapq, int __pyx_v_source_id, int __pyx_v_sample_id, int __pyx_v_reference_start, PyObject *__pyx_v_BX_tag, int __pyx_v_HP_tag, int __pyx_v_PS_tag); /* proto */
 static void __pyx_pf_8whatshap_4core_4Read_2__dealloc__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_4__repr__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_5mapqs___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_4name___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_9source_id___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_9sample_id___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_15reference_start___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_6BX_tag___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_6HP_tag___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_6PS_tag___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_6__iter__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_pf_8whatshap_4core_4Read_9__len__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_11__getitem__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
 static int __pyx_pf_8whatshap_4core_4Read_13__setitem__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_variant); /* proto */
 static int __pyx_pf_8whatshap_4core_4Read_15__contains__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_position); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_17__getstate__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_19__setstate__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_state); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_21add_variant(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, int __pyx_v_position, int __pyx_v_allele, int __pyx_v_quality); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_23add_mapq(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, int __pyx_v_mapq); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_25sort(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_27is_sorted(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_4Read_29has_BX_tag(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8whatshap_4core_4Read_31__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_8whatshap_4core_4Read_33__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_31has_HP_tag(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_33has_PS_tag(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_35__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_8whatshap_4core_4Read_37__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_pf_8whatshap_4core_7ReadSet___cinit__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self); /* proto */
 static void __pyx_pf_8whatshap_4core_7ReadSet_2__dealloc__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_7ReadSet_4add(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self, struct __pyx_obj_8whatshap_4core_Read *__pyx_v_read); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_7ReadSet_6__str__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_7ReadSet_8__iter__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_pf_8whatshap_4core_7ReadSet_11__len__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8whatshap_4core_7ReadSet_13__getitem__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
@@ -3280,43 +3288,49 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "whatshap/core.pyx":63
  * 
  * cdef class Read:
- * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None):             # <<<<<<<<<<<<<<
+ * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None, int HP_tag = -1, int PS_tag = -1):             # <<<<<<<<<<<<<<
  * 		cdef string _name = b''
  * 		cdef string _BX_tag = b''
  */
 
 /* Python wrapper */
 static int __pyx_pw_8whatshap_4core_4Read_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8whatshap_4core_4Read_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   int __pyx_v_mapq;
   int __pyx_v_source_id;
   int __pyx_v_sample_id;
   int __pyx_v_reference_start;
   PyObject *__pyx_v_BX_tag = 0;
+  int __pyx_v_HP_tag;
+  int __pyx_v_PS_tag;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_mapq,&__pyx_n_s_source_id,&__pyx_n_s_sample_id,&__pyx_n_s_reference_start,&__pyx_n_s_BX_tag,0};
-    PyObject* values[6] = {0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,&__pyx_n_s_mapq,&__pyx_n_s_source_id,&__pyx_n_s_sample_id,&__pyx_n_s_reference_start,&__pyx_n_s_BX_tag,&__pyx_n_s_HP_tag,&__pyx_n_s_PS_tag,0};
+    PyObject* values[8] = {0,0,0,0,0,0,0,0};
     values[0] = ((PyObject*)Py_None);
     values[5] = ((PyObject*)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -3361,20 +3375,36 @@
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_BX_tag);
           if (value) { values[5] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_HP_tag);
+          if (value) { values[6] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_PS_tag);
+          if (value) { values[7] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 63, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
         case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
         CYTHON_FALLTHROUGH;
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -3405,37 +3435,47 @@
     }
     if (values[4]) {
       __pyx_v_reference_start = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_reference_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 63, __pyx_L3_error)
     } else {
       __pyx_v_reference_start = ((int)-1);
     }
     __pyx_v_BX_tag = ((PyObject*)values[5]);
+    if (values[6]) {
+      __pyx_v_HP_tag = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_HP_tag == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 63, __pyx_L3_error)
+    } else {
+      __pyx_v_HP_tag = ((int)-1);
+    }
+    if (values[7]) {
+      __pyx_v_PS_tag = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_PS_tag == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 63, __pyx_L3_error)
+    } else {
+      __pyx_v_PS_tag = ((int)-1);
+    }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 63, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 63, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Read.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_name), (&PyUnicode_Type), 1, "name", 1))) __PYX_ERR(1, 63, __pyx_L1_error)
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_BX_tag), (&PyUnicode_Type), 1, "BX_tag", 1))) __PYX_ERR(1, 63, __pyx_L1_error)
-  __pyx_r = __pyx_pf_8whatshap_4core_4Read___cinit__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self), __pyx_v_name, __pyx_v_mapq, __pyx_v_source_id, __pyx_v_sample_id, __pyx_v_reference_start, __pyx_v_BX_tag);
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read___cinit__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self), __pyx_v_name, __pyx_v_mapq, __pyx_v_source_id, __pyx_v_sample_id, __pyx_v_reference_start, __pyx_v_BX_tag, __pyx_v_HP_tag, __pyx_v_PS_tag);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_8whatshap_4core_4Read___cinit__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_mapq, int __pyx_v_source_id, int __pyx_v_sample_id, int __pyx_v_reference_start, PyObject *__pyx_v_BX_tag) {
+static int __pyx_pf_8whatshap_4core_4Read___cinit__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_name, int __pyx_v_mapq, int __pyx_v_source_id, int __pyx_v_sample_id, int __pyx_v_reference_start, PyObject *__pyx_v_BX_tag, int __pyx_v_HP_tag, int __pyx_v_PS_tag) {
   std::string __pyx_v__name;
   std::string __pyx_v__BX_tag;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   std::string __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
@@ -3445,165 +3485,165 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "whatshap/core.pyx":64
  * cdef class Read:
- * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None):
+ * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None, int HP_tag = -1, int PS_tag = -1):
  * 		cdef string _name = b''             # <<<<<<<<<<<<<<
  * 		cdef string _BX_tag = b''
- * 		if name is None:
+ * 
  */
   __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 64, __pyx_L1_error)
   __pyx_v__name = __pyx_t_1;
 
   /* "whatshap/core.pyx":65
- * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None):
+ * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None, int HP_tag = -1, int PS_tag = -1):
  * 		cdef string _name = b''
  * 		cdef string _BX_tag = b''             # <<<<<<<<<<<<<<
+ * 
  * 		if name is None:
- * 			self.thisptr = NULL
  */
   __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 65, __pyx_L1_error)
   __pyx_v__BX_tag = __pyx_t_1;
 
-  /* "whatshap/core.pyx":66
- * 		cdef string _name = b''
+  /* "whatshap/core.pyx":67
  * 		cdef string _BX_tag = b''
+ * 
  * 		if name is None:             # <<<<<<<<<<<<<<
  * 			self.thisptr = NULL
  * 			self.ownsptr = False
  */
   __pyx_t_2 = (__pyx_v_name == ((PyObject*)Py_None));
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "whatshap/core.pyx":67
- * 		cdef string _BX_tag = b''
+    /* "whatshap/core.pyx":68
+ * 
  * 		if name is None:
  * 			self.thisptr = NULL             # <<<<<<<<<<<<<<
  * 			self.ownsptr = False
  * 		else:
  */
     __pyx_v_self->thisptr = NULL;
 
-    /* "whatshap/core.pyx":68
+    /* "whatshap/core.pyx":69
  * 		if name is None:
  * 			self.thisptr = NULL
  * 			self.ownsptr = False             # <<<<<<<<<<<<<<
  * 		else:
  * 			# TODO: Is this the best way to handle string arguments?
  */
     __pyx_v_self->ownsptr = 0;
 
-    /* "whatshap/core.pyx":66
- * 		cdef string _name = b''
+    /* "whatshap/core.pyx":67
  * 		cdef string _BX_tag = b''
+ * 
  * 		if name is None:             # <<<<<<<<<<<<<<
  * 			self.thisptr = NULL
  * 			self.ownsptr = False
  */
     goto __pyx_L3;
   }
 
-  /* "whatshap/core.pyx":71
+  /* "whatshap/core.pyx":72
  * 		else:
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')             # <<<<<<<<<<<<<<
  * 			if BX_tag is not '' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')
  */
   /*else*/ {
     if (unlikely(__pyx_v_name == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-      __PYX_ERR(1, 71, __pyx_L1_error)
+      __PYX_ERR(1, 72, __pyx_L1_error)
     }
-    __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 71, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_name); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 72, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 71, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 72, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v__name = __pyx_t_1;
 
-    /* "whatshap/core.pyx":72
+    /* "whatshap/core.pyx":73
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not '' and BX_tag is not None:             # <<<<<<<<<<<<<<
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  */
     __pyx_t_2 = (__pyx_v_BX_tag != __pyx_kp_u__3);
     __pyx_t_5 = (__pyx_t_2 != 0);
     if (__pyx_t_5) {
     } else {
       __pyx_t_3 = __pyx_t_5;
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_5 = (__pyx_v_BX_tag != ((PyObject*)Py_None));
     __pyx_t_2 = (__pyx_t_5 != 0);
     __pyx_t_3 = __pyx_t_2;
     __pyx_L5_bool_binop_done:;
     if (__pyx_t_3) {
 
-      /* "whatshap/core.pyx":73
+      /* "whatshap/core.pyx":74
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not '' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')             # <<<<<<<<<<<<<<
- * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  * 			self.ownsptr = True
  */
       if (unlikely(__pyx_v_BX_tag == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-        __PYX_ERR(1, 73, __pyx_L1_error)
+        __PYX_ERR(1, 74, __pyx_L1_error)
       }
-      __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_BX_tag); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 73, __pyx_L1_error)
+      __pyx_t_4 = PyUnicode_AsUTF8String(__pyx_v_BX_tag); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 73, __pyx_L1_error)
+      __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 74, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_v__BX_tag = __pyx_t_1;
 
-      /* "whatshap/core.pyx":72
+      /* "whatshap/core.pyx":73
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not '' and BX_tag is not None:             # <<<<<<<<<<<<<<
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  */
     }
 
-    /* "whatshap/core.pyx":74
+    /* "whatshap/core.pyx":75
  * 			if BX_tag is not '' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)             # <<<<<<<<<<<<<<
+ * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)             # <<<<<<<<<<<<<<
  * 			self.ownsptr = True
  * 
  */
     try {
-      __pyx_t_6 = new Read(__pyx_v__name, __pyx_v_mapq, __pyx_v_source_id, __pyx_v_sample_id, __pyx_v_reference_start, __pyx_v__BX_tag);
+      __pyx_t_6 = new Read(__pyx_v__name, __pyx_v_mapq, __pyx_v_source_id, __pyx_v_sample_id, __pyx_v_reference_start, __pyx_v__BX_tag, __pyx_v_HP_tag, __pyx_v_PS_tag);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 74, __pyx_L1_error)
+      __PYX_ERR(1, 75, __pyx_L1_error)
     }
     __pyx_v_self->thisptr = __pyx_t_6;
 
-    /* "whatshap/core.pyx":75
+    /* "whatshap/core.pyx":76
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  * 			self.ownsptr = True             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
     __pyx_v_self->ownsptr = 1;
   }
   __pyx_L3:;
 
   /* "whatshap/core.pyx":63
  * 
  * cdef class Read:
- * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None):             # <<<<<<<<<<<<<<
+ * 	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None, int HP_tag = -1, int PS_tag = -1):             # <<<<<<<<<<<<<<
  * 		cdef string _name = b''
  * 		cdef string _BX_tag = b''
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
@@ -3612,15 +3652,15 @@
   __Pyx_AddTraceback("whatshap.core.Read.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":77
+/* "whatshap/core.pyx":78
  * 			self.ownsptr = True
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		if self.ownsptr:
  * 			assert self.thisptr != NULL
  */
 
@@ -3639,59 +3679,59 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":78
+  /* "whatshap/core.pyx":79
  * 
  * 	def __dealloc__(self):
  * 		if self.ownsptr:             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			del self.thisptr
  */
   __pyx_t_1 = (__pyx_v_self->ownsptr != 0);
   if (__pyx_t_1) {
 
-    /* "whatshap/core.pyx":79
+    /* "whatshap/core.pyx":80
  * 	def __dealloc__(self):
  * 		if self.ownsptr:
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			del self.thisptr
  * 
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
-        __PYX_ERR(1, 79, __pyx_L1_error)
+        __PYX_ERR(1, 80, __pyx_L1_error)
       }
     }
     #endif
 
-    /* "whatshap/core.pyx":80
+    /* "whatshap/core.pyx":81
  * 		if self.ownsptr:
  * 			assert self.thisptr != NULL
  * 			del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def __repr__(self):
  */
     delete __pyx_v_self->thisptr;
 
-    /* "whatshap/core.pyx":78
+    /* "whatshap/core.pyx":79
  * 
  * 	def __dealloc__(self):
  * 		if self.ownsptr:             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			del self.thisptr
  */
   }
 
-  /* "whatshap/core.pyx":77
+  /* "whatshap/core.pyx":78
  * 			self.ownsptr = True
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		if self.ownsptr:
  * 			assert self.thisptr != NULL
  */
 
@@ -3699,20 +3739,20 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("whatshap.core.Read.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":82
+/* "whatshap/core.pyx":83
  * 			del self.thisptr
  * 
  * 	def __repr__(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
- * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(
+ * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8whatshap_4core_4Read_5__repr__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_8whatshap_4core_4Read_5__repr__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -3733,177 +3773,195 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
-  int __pyx_t_11;
+  PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
+  int __pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "whatshap/core.pyx":83
+  /* "whatshap/core.pyx":84
  * 
  * 	def __repr__(self):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
- * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(
- * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, list(self))
+ * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(
+ * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, list(self))
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 83, __pyx_L1_error)
+      __PYX_ERR(1, 84, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":84
+  /* "whatshap/core.pyx":85
  * 	def __repr__(self):
  * 		assert self.thisptr != NULL
- * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(             # <<<<<<<<<<<<<<
- * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, list(self))
+ * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(             # <<<<<<<<<<<<<<
+ * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, list(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Read_name_r_mapq_source_id_sampl, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 84, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Read_name_r_mapq_source_id_sampl, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "whatshap/core.pyx":85
+  /* "whatshap/core.pyx":86
  * 		assert self.thisptr != NULL
- * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(
- * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, list(self))             # <<<<<<<<<<<<<<
+ * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(
+ * 			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, list(self))             # <<<<<<<<<<<<<<
  * 
  * 	property mapqs:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mapqs); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mapqs); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_id); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_id); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reference_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reference_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BX_tag); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BX_tag); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = PySequence_List(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_HP_tag); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
-  __pyx_t_10 = NULL;
-  __pyx_t_11 = 0;
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_PS_tag); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_t_11 = PySequence_List(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 86, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __pyx_t_12 = NULL;
+  __pyx_t_13 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_10)) {
+    __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_12)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_10);
+      __Pyx_INCREF(__pyx_t_12);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
-      __pyx_t_11 = 1;
+      __pyx_t_13 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[8] = {__pyx_t_10, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 7+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 84, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    PyObject *__pyx_temp[10] = {__pyx_t_12, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 9+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 85, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
-    PyObject *__pyx_temp[8] = {__pyx_t_10, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_11, 7+__pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 84, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    PyObject *__pyx_temp[10] = {__pyx_t_12, __pyx_t_3, __pyx_t_4, __pyx_t_5, __pyx_t_6, __pyx_t_7, __pyx_t_8, __pyx_t_9, __pyx_t_10, __pyx_t_11};
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_13, 9+__pyx_t_13); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 85, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   } else
   #endif
   {
-    __pyx_t_12 = PyTuple_New(7+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 84, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    if (__pyx_t_10) {
-      __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
+    __pyx_t_14 = PyTuple_New(9+__pyx_t_13); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 85, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_14);
+    if (__pyx_t_12) {
+      __Pyx_GIVEREF(__pyx_t_12); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_12); __pyx_t_12 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_t_3);
+    PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_13, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_13, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_11, __pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_14, 2+__pyx_t_13, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_6);
-    PyTuple_SET_ITEM(__pyx_t_12, 3+__pyx_t_11, __pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_14, 3+__pyx_t_13, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
-    PyTuple_SET_ITEM(__pyx_t_12, 4+__pyx_t_11, __pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_14, 4+__pyx_t_13, __pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_8);
-    PyTuple_SET_ITEM(__pyx_t_12, 5+__pyx_t_11, __pyx_t_8);
+    PyTuple_SET_ITEM(__pyx_t_14, 5+__pyx_t_13, __pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_9);
-    PyTuple_SET_ITEM(__pyx_t_12, 6+__pyx_t_11, __pyx_t_9);
+    PyTuple_SET_ITEM(__pyx_t_14, 6+__pyx_t_13, __pyx_t_9);
+    __Pyx_GIVEREF(__pyx_t_10);
+    PyTuple_SET_ITEM(__pyx_t_14, 7+__pyx_t_13, __pyx_t_10);
+    __Pyx_GIVEREF(__pyx_t_11);
+    PyTuple_SET_ITEM(__pyx_t_14, 8+__pyx_t_13, __pyx_t_11);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
     __pyx_t_8 = 0;
     __pyx_t_9 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 84, __pyx_L1_error)
+    __pyx_t_10 = 0;
+    __pyx_t_11 = 0;
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_14, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 85, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":82
+  /* "whatshap/core.pyx":83
  * 			del self.thisptr
  * 
  * 	def __repr__(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
- * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(
+ * 		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_XDECREF(__pyx_t_14);
   __Pyx_AddTraceback("whatshap.core.Read.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":88
+/* "whatshap/core.pyx":89
  * 
  * 	property mapqs:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return tuple(self.thisptr.getMapqs())
  */
 
@@ -3927,54 +3985,54 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":89
+  /* "whatshap/core.pyx":90
  * 	property mapqs:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return tuple(self.thisptr.getMapqs())
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 89, __pyx_L1_error)
+      __PYX_ERR(1, 90, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":90
+  /* "whatshap/core.pyx":91
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return tuple(self.thisptr.getMapqs())             # <<<<<<<<<<<<<<
  * 
  * 	property name:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getMapqs();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 90, __pyx_L1_error)
+    __PYX_ERR(1, 91, __pyx_L1_error)
   }
-  __pyx_t_2 = __pyx_convert_vector_to_py_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_to_py_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 90, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":88
+  /* "whatshap/core.pyx":89
  * 
  * 	property mapqs:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return tuple(self.thisptr.getMapqs())
  */
 
@@ -3986,15 +4044,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":93
+/* "whatshap/core.pyx":94
  * 
  * 	property name:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getName().decode('utf-8')
  */
 
@@ -4017,51 +4075,51 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":94
+  /* "whatshap/core.pyx":95
  * 	property name:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return self.thisptr.getName().decode('utf-8')
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 94, __pyx_L1_error)
+      __PYX_ERR(1, 95, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":95
+  /* "whatshap/core.pyx":96
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getName().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 	property source_id:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getName();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 95, __pyx_L1_error)
+    __PYX_ERR(1, 96, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":93
+  /* "whatshap/core.pyx":94
  * 
  * 	property name:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getName().decode('utf-8')
  */
 
@@ -4072,15 +4130,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":98
+/* "whatshap/core.pyx":99
  * 
  * 	property source_id:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSourceID()
  */
 
@@ -4103,51 +4161,51 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":99
+  /* "whatshap/core.pyx":100
  * 	property source_id:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return self.thisptr.getSourceID()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 99, __pyx_L1_error)
+      __PYX_ERR(1, 100, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":100
+  /* "whatshap/core.pyx":101
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSourceID()             # <<<<<<<<<<<<<<
  * 
  * 	property sample_id:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getSourceID();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 100, __pyx_L1_error)
+    __PYX_ERR(1, 101, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 100, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":98
+  /* "whatshap/core.pyx":99
  * 
  * 	property source_id:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSourceID()
  */
 
@@ -4158,15 +4216,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":103
+/* "whatshap/core.pyx":104
  * 
  * 	property sample_id:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSampleID()
  */
 
@@ -4189,51 +4247,51 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":104
+  /* "whatshap/core.pyx":105
  * 	property sample_id:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return self.thisptr.getSampleID()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 104, __pyx_L1_error)
+      __PYX_ERR(1, 105, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":105
+  /* "whatshap/core.pyx":106
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSampleID()             # <<<<<<<<<<<<<<
  * 
  * 	property reference_start:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getSampleID();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 105, __pyx_L1_error)
+    __PYX_ERR(1, 106, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":103
+  /* "whatshap/core.pyx":104
  * 
  * 	property sample_id:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getSampleID()
  */
 
@@ -4244,15 +4302,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":108
+/* "whatshap/core.pyx":109
  * 
  * 	property reference_start:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getReferenceStart()
  */
 
@@ -4275,51 +4333,51 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":109
+  /* "whatshap/core.pyx":110
  * 	property reference_start:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return self.thisptr.getReferenceStart()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 109, __pyx_L1_error)
+      __PYX_ERR(1, 110, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":110
+  /* "whatshap/core.pyx":111
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getReferenceStart()             # <<<<<<<<<<<<<<
  * 
  * 	property BX_tag:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getReferenceStart();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 110, __pyx_L1_error)
+    __PYX_ERR(1, 111, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":108
+  /* "whatshap/core.pyx":109
  * 
  * 	property reference_start:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getReferenceStart()
  */
 
@@ -4330,15 +4388,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":113
+/* "whatshap/core.pyx":114
  * 
  * 	property BX_tag:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getBXTag().decode('utf-8')
  */
 
@@ -4361,51 +4419,51 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":114
+  /* "whatshap/core.pyx":115
  * 	property BX_tag:
  * 		def __get__(self):
  * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 			return self.thisptr.getBXTag().decode('utf-8')
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 114, __pyx_L1_error)
+      __PYX_ERR(1, 115, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":115
+  /* "whatshap/core.pyx":116
  * 		def __get__(self):
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getBXTag().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
- * 	def __iter__(self):
+ * 	property HP_tag:
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getBXTag();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 115, __pyx_L1_error)
+    __PYX_ERR(1, 116, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 115, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 116, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":113
+  /* "whatshap/core.pyx":114
  * 
  * 	property BX_tag:
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			assert self.thisptr != NULL
  * 			return self.thisptr.getBXTag().decode('utf-8')
  */
 
@@ -4415,18 +4473,190 @@
   __Pyx_AddTraceback("whatshap.core.Read.BX_tag.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+
+/* "whatshap/core.pyx":119
+ * 
+ * 	property HP_tag:
+ * 		def __get__(self):             # <<<<<<<<<<<<<<
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getHPTag()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8whatshap_4core_4Read_6HP_tag_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_6HP_tag_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_6HP_tag___get__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8whatshap_4core_4Read_6HP_tag___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "whatshap/core.pyx":120
+ * 	property HP_tag:
+ * 		def __get__(self):
+ * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
+ * 			return self.thisptr.getHPTag()
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
+      PyErr_SetNone(PyExc_AssertionError);
+      __PYX_ERR(1, 120, __pyx_L1_error)
+    }
+  }
+  #endif
+
+  /* "whatshap/core.pyx":121
+ * 		def __get__(self):
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getHPTag()             # <<<<<<<<<<<<<<
+ * 
+ * 	property PS_tag:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  try {
+    __pyx_t_1 = __pyx_v_self->thisptr->getHPTag();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 121, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 121, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "whatshap/core.pyx":119
+ * 
+ * 	property HP_tag:
+ * 		def __get__(self):             # <<<<<<<<<<<<<<
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getHPTag()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("whatshap.core.Read.HP_tag.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "whatshap/core.pyx":124
+ * 
+ * 	property PS_tag:
+ * 		def __get__(self):             # <<<<<<<<<<<<<<
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getPSTag()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8whatshap_4core_4Read_6PS_tag_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_6PS_tag_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_6PS_tag___get__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8whatshap_4core_4Read_6PS_tag___get__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__get__", 0);
+
+  /* "whatshap/core.pyx":125
+ * 	property PS_tag:
+ * 		def __get__(self):
+ * 			assert self.thisptr != NULL             # <<<<<<<<<<<<<<
+ * 			return self.thisptr.getPSTag()
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
+      PyErr_SetNone(PyExc_AssertionError);
+      __PYX_ERR(1, 125, __pyx_L1_error)
+    }
+  }
+  #endif
+
+  /* "whatshap/core.pyx":126
+ * 		def __get__(self):
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getPSTag()             # <<<<<<<<<<<<<<
+ * 
+ * 	def __iter__(self):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  try {
+    __pyx_t_1 = __pyx_v_self->thisptr->getPSTag();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 126, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 126, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "whatshap/core.pyx":124
+ * 
+ * 	property PS_tag:
+ * 		def __get__(self):             # <<<<<<<<<<<<<<
+ * 			assert self.thisptr != NULL
+ * 			return self.thisptr.getPSTag()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("whatshap.core.Read.PS_tag.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
 static PyObject *__pyx_gb_8whatshap_4core_4Read_8generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "whatshap/core.pyx":117
- * 			return self.thisptr.getBXTag().decode('utf-8')
+/* "whatshap/core.pyx":128
+ * 			return self.thisptr.getPSTag()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		"""Iterate over all variants in this read"""
  * 		assert self.thisptr != NULL
  */
 
 /* Python wrapper */
@@ -4454,23 +4684,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_8whatshap_4core___pyx_scope_struct____iter__ *)__pyx_tp_new_8whatshap_4core___pyx_scope_struct____iter__(__pyx_ptype_8whatshap_4core___pyx_scope_struct____iter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8whatshap_4core___pyx_scope_struct____iter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(1, 117, __pyx_L1_error)
+    __PYX_ERR(1, 128, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_4Read_8generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Read___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 117, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_4Read_8generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Read___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 128, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4499,52 +4729,52 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 117, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 128, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":119
+  /* "whatshap/core.pyx":130
  * 	def __iter__(self):
  * 		"""Iterate over all variants in this read"""
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		for i in range(len(self)):
  * 			yield self[i]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_cur_scope->__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 119, __pyx_L1_error)
+      __PYX_ERR(1, 130, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":120
+  /* "whatshap/core.pyx":131
  * 		"""Iterate over all variants in this read"""
  * 		assert self.thisptr != NULL
  * 		for i in range(len(self)):             # <<<<<<<<<<<<<<
  * 			yield self[i]
  * 
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_cur_scope->__pyx_v_self)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 120, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_cur_scope->__pyx_v_self)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 131, __pyx_L1_error)
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_cur_scope->__pyx_v_i = __pyx_t_3;
 
-    /* "whatshap/core.pyx":121
+    /* "whatshap/core.pyx":132
  * 		assert self.thisptr != NULL
  * 		for i in range(len(self)):
  * 			yield self[i]             # <<<<<<<<<<<<<<
  * 
  * 	def __len__(self):
  */
-    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 121, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
     __Pyx_XGIVEREF(__pyx_r);
@@ -4553,20 +4783,20 @@
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 121, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 132, __pyx_L1_error)
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "whatshap/core.pyx":117
- * 			return self.thisptr.getBXTag().decode('utf-8')
+  /* "whatshap/core.pyx":128
+ * 			return self.thisptr.getPSTag()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		"""Iterate over all variants in this read"""
  * 		assert self.thisptr != NULL
  */
 
   /* function exit code */
@@ -4582,15 +4812,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":123
+/* "whatshap/core.pyx":134
  * 			yield self[i]
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		"""Return number of variants in this read"""
  * 		assert self.thisptr != NULL
  */
 
@@ -4616,47 +4846,47 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "whatshap/core.pyx":125
+  /* "whatshap/core.pyx":136
  * 	def __len__(self):
  * 		"""Return number of variants in this read"""
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		return self.thisptr.getVariantCount()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 125, __pyx_L1_error)
+      __PYX_ERR(1, 136, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":126
+  /* "whatshap/core.pyx":137
  * 		"""Return number of variants in this read"""
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.getVariantCount()             # <<<<<<<<<<<<<<
  * 
  * 	def __getitem__(self, key):
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getVariantCount();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 126, __pyx_L1_error)
+    __PYX_ERR(1, 137, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":123
+  /* "whatshap/core.pyx":134
  * 			yield self[i]
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		"""Return number of variants in this read"""
  * 		assert self.thisptr != NULL
  */
 
@@ -4665,15 +4895,15 @@
   __Pyx_AddTraceback("whatshap.core.Read.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":128
+/* "whatshap/core.pyx":139
  * 		return self.thisptr.getVariantCount()
  * 
  * 	def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 		"""Return Variant object at the given integer index"""
  * 		assert self.thisptr != NULL
  */
 
@@ -4707,280 +4937,280 @@
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
   __Pyx_INCREF(__pyx_v_key);
 
-  /* "whatshap/core.pyx":130
+  /* "whatshap/core.pyx":141
  * 	def __getitem__(self, key):
  * 		"""Return Variant object at the given integer index"""
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError("Read does not support slices")
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 130, __pyx_L1_error)
+      __PYX_ERR(1, 141, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":131
+  /* "whatshap/core.pyx":142
  * 		"""Return Variant object at the given integer index"""
  * 		assert self.thisptr != NULL
  * 		if isinstance(key, slice):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError("Read does not support slices")
  * 		assert isinstance(key, int)
  */
   __pyx_t_1 = PySlice_Check(__pyx_v_key); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "whatshap/core.pyx":132
+    /* "whatshap/core.pyx":143
  * 		assert self.thisptr != NULL
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError("Read does not support slices")             # <<<<<<<<<<<<<<
  * 		assert isinstance(key, int)
  * 		cdef int n = self.thisptr.getVariantCount()
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 132, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 143, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 132, __pyx_L1_error)
+    __PYX_ERR(1, 143, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":131
+    /* "whatshap/core.pyx":142
  * 		"""Return Variant object at the given integer index"""
  * 		assert self.thisptr != NULL
  * 		if isinstance(key, slice):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError("Read does not support slices")
  * 		assert isinstance(key, int)
  */
   }
 
-  /* "whatshap/core.pyx":133
+  /* "whatshap/core.pyx":144
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError("Read does not support slices")
  * 		assert isinstance(key, int)             # <<<<<<<<<<<<<<
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= key < n):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = PyInt_Check(__pyx_v_key); 
     if (unlikely(!(__pyx_t_2 != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 133, __pyx_L1_error)
+      __PYX_ERR(1, 144, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":134
+  /* "whatshap/core.pyx":145
  * 			raise NotImplementedError("Read does not support slices")
  * 		assert isinstance(key, int)
  * 		cdef int n = self.thisptr.getVariantCount()             # <<<<<<<<<<<<<<
  * 		if not (-n <= key < n):
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  */
   try {
     __pyx_t_4 = __pyx_v_self->thisptr->getVariantCount();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 134, __pyx_L1_error)
+    __PYX_ERR(1, 145, __pyx_L1_error)
   }
   __pyx_v_n = __pyx_t_4;
 
-  /* "whatshap/core.pyx":135
+  /* "whatshap/core.pyx":146
  * 		assert isinstance(key, int)
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= key < n):             # <<<<<<<<<<<<<<
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  * 		if key < 0:
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int((-__pyx_v_n)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 135, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int((-__pyx_v_n)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_v_key, Py_LE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 135, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_3, __pyx_v_key, Py_LE); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 146, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_5)) {
     __Pyx_DECREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 135, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 146, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = PyObject_RichCompare(__pyx_v_key, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 135, __pyx_L1_error)
+    __pyx_t_5 = PyObject_RichCompare(__pyx_v_key, __pyx_t_6, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 146, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 135, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 146, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_1 = ((!__pyx_t_2) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "whatshap/core.pyx":136
+    /* "whatshap/core.pyx":147
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= key < n):
  * 			raise IndexError('Index out of bounds: {}'.format(key))             # <<<<<<<<<<<<<<
  * 		if key < 0:
  * 			key = n + key
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_out_of_bounds, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_out_of_bounds, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_key);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 136, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 136, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 136, __pyx_L1_error)
+    __PYX_ERR(1, 147, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":135
+    /* "whatshap/core.pyx":146
  * 		assert isinstance(key, int)
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= key < n):             # <<<<<<<<<<<<<<
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  * 		if key < 0:
  */
   }
 
-  /* "whatshap/core.pyx":137
+  /* "whatshap/core.pyx":148
  * 		if not (-n <= key < n):
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  * 		if key < 0:             # <<<<<<<<<<<<<<
  * 			key = n + key
  * 		return Variant(
  */
-  __pyx_t_3 = PyObject_RichCompare(__pyx_v_key, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_v_key, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 148, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_1) {
 
-    /* "whatshap/core.pyx":138
+    /* "whatshap/core.pyx":149
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  * 		if key < 0:
  * 			key = n + key             # <<<<<<<<<<<<<<
  * 		return Variant(
  * 			position=self.thisptr.getPosition(key),
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 138, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 138, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_Add(__pyx_t_3, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_key, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "whatshap/core.pyx":137
+    /* "whatshap/core.pyx":148
  * 		if not (-n <= key < n):
  * 			raise IndexError('Index out of bounds: {}'.format(key))
  * 		if key < 0:             # <<<<<<<<<<<<<<
  * 			key = n + key
  * 		return Variant(
  */
   }
 
-  /* "whatshap/core.pyx":139
+  /* "whatshap/core.pyx":150
  * 		if key < 0:
  * 			key = n + key
  * 		return Variant(             # <<<<<<<<<<<<<<
  * 			position=self.thisptr.getPosition(key),
  * 			allele=self.thisptr.getAllele(key),
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Variant); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 139, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_Variant); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "whatshap/core.pyx":140
+  /* "whatshap/core.pyx":151
  * 			key = n + key
  * 		return Variant(
  * 			position=self.thisptr.getPosition(key),             # <<<<<<<<<<<<<<
  * 			allele=self.thisptr.getAllele(key),
  * 			quality=self.thisptr.getVariantQuality(key)
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 151, __pyx_L1_error)
   try {
     __pyx_t_7 = __pyx_v_self->thisptr->getPosition(__pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 140, __pyx_L1_error)
+    __PYX_ERR(1, 151, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 140, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_position, __pyx_t_6) < 0) __PYX_ERR(1, 140, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_position, __pyx_t_6) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":141
+  /* "whatshap/core.pyx":152
  * 		return Variant(
  * 			position=self.thisptr.getPosition(key),
  * 			allele=self.thisptr.getAllele(key),             # <<<<<<<<<<<<<<
  * 			quality=self.thisptr.getVariantQuality(key)
  * 		)
  */
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 141, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 152, __pyx_L1_error)
   try {
     __pyx_t_4 = __pyx_v_self->thisptr->getAllele(__pyx_t_7);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 141, __pyx_L1_error)
+    __PYX_ERR(1, 152, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 141, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 152, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allele, __pyx_t_6) < 0) __PYX_ERR(1, 140, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allele, __pyx_t_6) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":142
+  /* "whatshap/core.pyx":153
  * 			position=self.thisptr.getPosition(key),
  * 			allele=self.thisptr.getAllele(key),
  * 			quality=self.thisptr.getVariantQuality(key)             # <<<<<<<<<<<<<<
  * 		)
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 142, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 153, __pyx_L1_error)
   try {
     __pyx_t_7 = __pyx_v_self->thisptr->getVariantQuality(__pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 142, __pyx_L1_error)
+    __PYX_ERR(1, 153, __pyx_L1_error)
   }
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 142, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_quality, __pyx_t_6) < 0) __PYX_ERR(1, 140, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_quality, __pyx_t_6) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":139
+  /* "whatshap/core.pyx":150
  * 		if key < 0:
  * 			key = n + key
  * 		return Variant(             # <<<<<<<<<<<<<<
  * 			position=self.thisptr.getPosition(key),
  * 			allele=self.thisptr.getAllele(key),
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 139, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":128
+  /* "whatshap/core.pyx":139
  * 		return self.thisptr.getVariantCount()
  * 
  * 	def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 		"""Return Variant object at the given integer index"""
  * 		assert self.thisptr != NULL
  */
 
@@ -4994,15 +5224,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":145
+/* "whatshap/core.pyx":156
  * 		)
  * 
  * 	def __setitem__(self, index, variant):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		cdef int n = self.thisptr.getVariantCount()
  */
 
@@ -5032,256 +5262,256 @@
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "whatshap/core.pyx":146
+  /* "whatshap/core.pyx":157
  * 
  * 	def __setitem__(self, index, variant):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= index < n):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 146, __pyx_L1_error)
+      __PYX_ERR(1, 157, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":147
+  /* "whatshap/core.pyx":158
  * 	def __setitem__(self, index, variant):
  * 		assert self.thisptr != NULL
  * 		cdef int n = self.thisptr.getVariantCount()             # <<<<<<<<<<<<<<
  * 		if not (-n <= index < n):
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getVariantCount();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 147, __pyx_L1_error)
+    __PYX_ERR(1, 158, __pyx_L1_error)
   }
   __pyx_v_n = __pyx_t_1;
 
-  /* "whatshap/core.pyx":148
+  /* "whatshap/core.pyx":159
  * 		assert self.thisptr != NULL
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= index < n):             # <<<<<<<<<<<<<<
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  * 		if index < 0:
  */
-  __pyx_t_2 = __Pyx_PyInt_From_int((-__pyx_v_n)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int((-__pyx_v_n)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 159, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_index, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_2, __pyx_v_index, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 159, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_3)) {
     __Pyx_DECREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 148, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_v_index, __pyx_t_4, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 148, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_v_index, __pyx_t_4, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 148, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 159, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_6 = ((!__pyx_t_5) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "whatshap/core.pyx":149
+    /* "whatshap/core.pyx":160
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= index < n):
  * 			raise IndexError('Index out of bounds: {}'.format(index))             # <<<<<<<<<<<<<<
  * 		if index < 0:
  * 			index = n + index
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_out_of_bounds, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Index_out_of_bounds, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 160, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_index) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_index);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 160, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 160, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 149, __pyx_L1_error)
+    __PYX_ERR(1, 160, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":148
+    /* "whatshap/core.pyx":159
  * 		assert self.thisptr != NULL
  * 		cdef int n = self.thisptr.getVariantCount()
  * 		if not (-n <= index < n):             # <<<<<<<<<<<<<<
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  * 		if index < 0:
  */
   }
 
-  /* "whatshap/core.pyx":150
+  /* "whatshap/core.pyx":161
  * 		if not (-n <= index < n):
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  * 		if index < 0:             # <<<<<<<<<<<<<<
  * 			index = n + index
  * 		if not isinstance(variant, Variant):
  */
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_index, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 150, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 150, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_index, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 161, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 161, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_6) {
 
-    /* "whatshap/core.pyx":151
+    /* "whatshap/core.pyx":162
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  * 		if index < 0:
  * 			index = n + index             # <<<<<<<<<<<<<<
  * 		if not isinstance(variant, Variant):
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 151, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 162, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "whatshap/core.pyx":150
+    /* "whatshap/core.pyx":161
  * 		if not (-n <= index < n):
  * 			raise IndexError('Index out of bounds: {}'.format(index))
  * 		if index < 0:             # <<<<<<<<<<<<<<
  * 			index = n + index
  * 		if not isinstance(variant, Variant):
  */
   }
 
-  /* "whatshap/core.pyx":152
+  /* "whatshap/core.pyx":163
  * 		if index < 0:
  * 			index = n + index
  * 		if not isinstance(variant, Variant):             # <<<<<<<<<<<<<<
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))
  * 		self.thisptr.setPosition(index, variant.position)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Variant); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 152, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Variant); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyObject_IsInstance(__pyx_v_variant, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 152, __pyx_L1_error)
+  __pyx_t_6 = PyObject_IsInstance(__pyx_v_variant, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = ((!(__pyx_t_6 != 0)) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "whatshap/core.pyx":153
+    /* "whatshap/core.pyx":164
  * 			index = n + index
  * 		if not isinstance(variant, Variant):
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))             # <<<<<<<<<<<<<<
  * 		self.thisptr.setPosition(index, variant.position)
  * 		self.thisptr.setAllele(index, variant.allele)
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Expected_instance_of_Variant_but, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 153, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Expected_instance_of_Variant_but, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, ((PyObject *)Py_TYPE(__pyx_v_variant))) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)Py_TYPE(__pyx_v_variant)));
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 153, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 153, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 153, __pyx_L1_error)
+    __PYX_ERR(1, 164, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":152
+    /* "whatshap/core.pyx":163
  * 		if index < 0:
  * 			index = n + index
  * 		if not isinstance(variant, Variant):             # <<<<<<<<<<<<<<
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))
  * 		self.thisptr.setPosition(index, variant.position)
  */
   }
 
-  /* "whatshap/core.pyx":154
+  /* "whatshap/core.pyx":165
  * 		if not isinstance(variant, Variant):
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))
  * 		self.thisptr.setPosition(index, variant.position)             # <<<<<<<<<<<<<<
  * 		self.thisptr.setAllele(index, variant.allele)
  * 		self.thisptr.setVariantQuality(index, variant.quality)
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 154, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_position); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_position); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 165, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 165, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   try {
     __pyx_v_self->thisptr->setPosition(__pyx_t_1, __pyx_t_7);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 154, __pyx_L1_error)
+    __PYX_ERR(1, 165, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":155
+  /* "whatshap/core.pyx":166
  * 			raise ValueError('Expected instance of Variant, but found {}'.format(type(variant)))
  * 		self.thisptr.setPosition(index, variant.position)
  * 		self.thisptr.setAllele(index, variant.allele)             # <<<<<<<<<<<<<<
  * 		self.thisptr.setVariantQuality(index, variant.quality)
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 155, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_allele); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 166, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_allele); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 166, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   try {
     __pyx_v_self->thisptr->setAllele(__pyx_t_7, __pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 155, __pyx_L1_error)
+    __PYX_ERR(1, 166, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":156
+  /* "whatshap/core.pyx":167
  * 		self.thisptr.setPosition(index, variant.position)
  * 		self.thisptr.setAllele(index, variant.allele)
  * 		self.thisptr.setVariantQuality(index, variant.quality)             # <<<<<<<<<<<<<<
  * 
  * 	def __contains__(self, position):
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 156, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_quality); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 156, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_index); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 167, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_quality); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 167, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 156, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 167, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   try {
     __pyx_v_self->thisptr->setVariantQuality(__pyx_t_1, __pyx_t_7);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 156, __pyx_L1_error)
+    __PYX_ERR(1, 167, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":145
+  /* "whatshap/core.pyx":156
  * 		)
  * 
  * 	def __setitem__(self, index, variant):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		cdef int n = self.thisptr.getVariantCount()
  */
 
@@ -5296,15 +5526,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":158
+/* "whatshap/core.pyx":169
  * 		self.thisptr.setVariantQuality(index, variant.quality)
  * 
  * 	def __contains__(self, position):             # <<<<<<<<<<<<<<
  * 		"""Return whether this read contains a variant at the given position.
  * 		A linear search is used.
  */
 
@@ -5336,152 +5566,152 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__contains__", 0);
 
-  /* "whatshap/core.pyx":162
+  /* "whatshap/core.pyx":173
  * 		A linear search is used.
  * 		"""
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		assert isinstance(position, int)
  * 		for variant in self:
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 162, __pyx_L1_error)
+      __PYX_ERR(1, 173, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":163
+  /* "whatshap/core.pyx":174
  * 		"""
  * 		assert self.thisptr != NULL
  * 		assert isinstance(position, int)             # <<<<<<<<<<<<<<
  * 		for variant in self:
  * 			if variant.position == position:
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = PyInt_Check(__pyx_v_position); 
     if (unlikely(!(__pyx_t_1 != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 163, __pyx_L1_error)
+      __PYX_ERR(1, 174, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":164
+  /* "whatshap/core.pyx":175
  * 		assert self.thisptr != NULL
  * 		assert isinstance(position, int)
  * 		for variant in self:             # <<<<<<<<<<<<<<
  * 			if variant.position == position:
  * 				return True
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
     __pyx_t_2 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 164, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 164, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 175, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 164, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 175, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 164, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 175, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 164, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 175, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 164, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 175, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 164, __pyx_L1_error)
+          else __PYX_ERR(1, 175, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_variant, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "whatshap/core.pyx":165
+    /* "whatshap/core.pyx":176
  * 		assert isinstance(position, int)
  * 		for variant in self:
  * 			if variant.position == position:             # <<<<<<<<<<<<<<
  * 				return True
  * 		return False
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_position); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 165, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_variant, __pyx_n_s_position); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 176, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = PyObject_RichCompare(__pyx_t_5, __pyx_v_position, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 165, __pyx_L1_error)
+    __pyx_t_6 = PyObject_RichCompare(__pyx_t_5, __pyx_v_position, Py_EQ); __Pyx_XGOTREF(__pyx_t_6); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 176, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 165, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(1, 176, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (__pyx_t_1) {
 
-      /* "whatshap/core.pyx":166
+      /* "whatshap/core.pyx":177
  * 		for variant in self:
  * 			if variant.position == position:
  * 				return True             # <<<<<<<<<<<<<<
  * 		return False
  * 
  */
       __pyx_r = 1;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "whatshap/core.pyx":165
+      /* "whatshap/core.pyx":176
  * 		assert isinstance(position, int)
  * 		for variant in self:
  * 			if variant.position == position:             # <<<<<<<<<<<<<<
  * 				return True
  * 		return False
  */
     }
 
-    /* "whatshap/core.pyx":164
+    /* "whatshap/core.pyx":175
  * 		assert self.thisptr != NULL
  * 		assert isinstance(position, int)
  * 		for variant in self:             # <<<<<<<<<<<<<<
  * 			if variant.position == position:
  * 				return True
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":167
+  /* "whatshap/core.pyx":178
  * 			if variant.position == position:
  * 				return True
  * 		return False             # <<<<<<<<<<<<<<
  * 
  * 	def __getstate__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":158
+  /* "whatshap/core.pyx":169
  * 		self.thisptr.setVariantQuality(index, variant.quality)
  * 
  * 	def __contains__(self, position):             # <<<<<<<<<<<<<<
  * 		"""Return whether this read contains a variant at the given position.
  * 		A linear search is used.
  */
 
@@ -5494,15 +5724,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_variant);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":169
+/* "whatshap/core.pyx":180
  * 		return False
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		mapqs = [mapq for mapq in self.mapqs]
  * 		variants = [(var.position, var.allele, var.quality) for var in self]
  */
 
@@ -5530,214 +5760,226 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getstate__", 0);
 
-  /* "whatshap/core.pyx":170
+  /* "whatshap/core.pyx":181
  * 
  * 	def __getstate__(self):
  * 		mapqs = [mapq for mapq in self.mapqs]             # <<<<<<<<<<<<<<
  * 		variants = [(var.position, var.allele, var.quality) for var in self]
- * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)
+ * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 181, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mapqs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mapqs); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 181, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 181, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 170, __pyx_L5_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 181, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 170, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 181, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 181, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 170, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 181, __pyx_L5_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L5_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 181, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 170, __pyx_L5_error)
+            else __PYX_ERR(1, 181, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_mapq, __pyx_t_2);
       __pyx_t_2 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr1__pyx_v_mapq))) __PYX_ERR(1, 170, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr1__pyx_v_mapq))) __PYX_ERR(1, 181, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_mapq); __pyx_8genexpr1__pyx_v_mapq = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_mapq); __pyx_8genexpr1__pyx_v_mapq = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_mapqs = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":171
+  /* "whatshap/core.pyx":182
  * 	def __getstate__(self):
  * 		mapqs = [mapq for mapq in self.mapqs]
  * 		variants = [(var.position, var.allele, var.quality) for var in self]             # <<<<<<<<<<<<<<
- * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)
+ * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)
  * 
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 171, __pyx_L11_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 182, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
       __pyx_t_3 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_3); __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_5 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 182, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 171, __pyx_L11_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 182, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 171, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 171, __pyx_L11_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 182, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 171, __pyx_L11_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 171, __pyx_L11_error)
+            else __PYX_ERR(1, 182, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_var, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_position); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_position); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_allele); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_allele); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_quality); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr2__pyx_v_var, __pyx_n_s_quality); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 171, __pyx_L11_error)
+      __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_7);
       PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
       __pyx_t_2 = 0;
       __pyx_t_6 = 0;
       __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(1, 171, __pyx_L11_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(1, 182, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_var); __pyx_8genexpr2__pyx_v_var = 0;
     goto __pyx_L14_exit_scope;
     __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_var); __pyx_8genexpr2__pyx_v_var = 0;
     goto __pyx_L1_error;
     __pyx_L14_exit_scope:;
   } /* exit inner scope */
   __pyx_v_variants = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":172
+  /* "whatshap/core.pyx":183
  * 		mapqs = [mapq for mapq in self.mapqs]
  * 		variants = [(var.position, var.allele, var.quality) for var in self]
- * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)             # <<<<<<<<<<<<<<
+ * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)             # <<<<<<<<<<<<<<
  * 
  * 	def __setstate__(self, state):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_source_id); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_id); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sample_id); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reference_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_reference_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BX_tag); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_BX_tag); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = PyTuple_New(7); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 172, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_HP_tag); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 183, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_PS_tag); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  __pyx_t_10 = PyTuple_New(9); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 183, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_v_mapqs);
   __Pyx_GIVEREF(__pyx_v_mapqs);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_mapqs);
+  PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_v_mapqs);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_10, 3, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_10, 4, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_10, 5, __pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_10, 6, __pyx_t_2);
+  __Pyx_GIVEREF(__pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_10, 7, __pyx_t_9);
   __Pyx_INCREF(__pyx_v_variants);
   __Pyx_GIVEREF(__pyx_v_variants);
-  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_v_variants);
+  PyTuple_SET_ITEM(__pyx_t_10, 8, __pyx_v_variants);
   __pyx_t_1 = 0;
   __pyx_t_3 = 0;
   __pyx_t_8 = 0;
   __pyx_t_7 = 0;
   __pyx_t_6 = 0;
-  __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
+  __pyx_t_9 = 0;
+  __pyx_r = __pyx_t_10;
+  __pyx_t_10 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":169
+  /* "whatshap/core.pyx":180
  * 		return False
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		mapqs = [mapq for mapq in self.mapqs]
  * 		variants = [(var.position, var.allele, var.quality) for var in self]
  */
 
@@ -5745,31 +5987,33 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("whatshap.core.Read.__getstate__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mapqs);
   __Pyx_XDECREF(__pyx_v_variants);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_mapq);
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_var);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":174
- * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)
+/* "whatshap/core.pyx":185
+ * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
- * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, variants = state
+ * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, HP_tag, PS_tag, variants = state
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_8whatshap_4core_4Read_20__setstate__(PyObject *__pyx_v_self, PyObject *__pyx_v_state); /*proto*/
 static PyObject *__pyx_pw_8whatshap_4core_4Read_20__setstate__(PyObject *__pyx_v_self, PyObject *__pyx_v_state) {
   PyObject *__pyx_r = 0;
@@ -5785,14 +6029,16 @@
 static PyObject *__pyx_pf_8whatshap_4core_4Read_19__setstate__(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, PyObject *__pyx_v_state) {
   PyObject *__pyx_v_mapqs = NULL;
   PyObject *__pyx_v_name = NULL;
   PyObject *__pyx_v_source_id = NULL;
   PyObject *__pyx_v_sample_id = NULL;
   PyObject *__pyx_v_reference_start = NULL;
   PyObject *__pyx_v_BX_tag = NULL;
+  PyObject *__pyx_v_HP_tag = NULL;
+  PyObject *__pyx_v_PS_tag = NULL;
   PyObject *__pyx_v_variants = NULL;
   std::string __pyx_v__name;
   std::string __pyx_v__BX_tag;
   PyObject *__pyx_v_mapq = NULL;
   PyObject *__pyx_v_pos = NULL;
   PyObject *__pyx_v_allele = NULL;
   PyObject *__pyx_v_quality = NULL;
@@ -5802,571 +6048,587 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  PyObject *(*__pyx_t_9)(PyObject *);
-  std::string __pyx_t_10;
-  int __pyx_t_11;
-  int __pyx_t_12;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *(*__pyx_t_11)(PyObject *);
+  std::string __pyx_t_12;
   int __pyx_t_13;
   int __pyx_t_14;
-  Py_ssize_t __pyx_t_15;
+  int __pyx_t_15;
   int __pyx_t_16;
-  int __pyx_t_17;
+  Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
-  Read *__pyx_t_19;
-  PyObject *(*__pyx_t_20)(PyObject *);
+  int __pyx_t_19;
+  int __pyx_t_20;
+  int __pyx_t_21;
+  int __pyx_t_22;
+  Read *__pyx_t_23;
+  PyObject *(*__pyx_t_24)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate__", 0);
 
-  /* "whatshap/core.pyx":175
+  /* "whatshap/core.pyx":186
  * 
  * 	def __setstate__(self, state):
- * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, variants = state             # <<<<<<<<<<<<<<
+ * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, HP_tag, PS_tag, variants = state             # <<<<<<<<<<<<<<
  * 
  * 		# TODO: Duplicated code from __cinit__ is ugly, but cinit cannot be used here directly
  */
   if ((likely(PyTuple_CheckExact(__pyx_v_state))) || (PyList_CheckExact(__pyx_v_state))) {
     PyObject* sequence = __pyx_v_state;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
-    if (unlikely(size != 7)) {
-      if (size > 7) __Pyx_RaiseTooManyValuesError(7);
+    if (unlikely(size != 9)) {
+      if (size > 9) __Pyx_RaiseTooManyValuesError(9);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 175, __pyx_L1_error)
+      __PYX_ERR(1, 186, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 3); 
       __pyx_t_5 = PyTuple_GET_ITEM(sequence, 4); 
       __pyx_t_6 = PyTuple_GET_ITEM(sequence, 5); 
       __pyx_t_7 = PyTuple_GET_ITEM(sequence, 6); 
+      __pyx_t_8 = PyTuple_GET_ITEM(sequence, 7); 
+      __pyx_t_9 = PyTuple_GET_ITEM(sequence, 8); 
     } else {
       __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 2); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 3); 
       __pyx_t_5 = PyList_GET_ITEM(sequence, 4); 
       __pyx_t_6 = PyList_GET_ITEM(sequence, 5); 
       __pyx_t_7 = PyList_GET_ITEM(sequence, 6); 
+      __pyx_t_8 = PyList_GET_ITEM(sequence, 7); 
+      __pyx_t_9 = PyList_GET_ITEM(sequence, 8); 
     }
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_t_7);
+    __Pyx_INCREF(__pyx_t_8);
+    __Pyx_INCREF(__pyx_t_9);
     #else
     {
       Py_ssize_t i;
-      PyObject** temps[7] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5,&__pyx_t_6,&__pyx_t_7};
-      for (i=0; i < 7; i++) {
-        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(1, 175, __pyx_L1_error)
+      PyObject** temps[9] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5,&__pyx_t_6,&__pyx_t_7,&__pyx_t_8,&__pyx_t_9};
+      for (i=0; i < 9; i++) {
+        PyObject* item = PySequence_ITEM(sequence, i); if (unlikely(!item)) __PYX_ERR(1, 186, __pyx_L1_error)
         __Pyx_GOTREF(item);
         *(temps[i]) = item;
       }
     }
     #endif
   } else {
     Py_ssize_t index = -1;
-    PyObject** temps[7] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5,&__pyx_t_6,&__pyx_t_7};
-    __pyx_t_8 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 175, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = Py_TYPE(__pyx_t_8)->tp_iternext;
-    for (index=0; index < 7; index++) {
-      PyObject* item = __pyx_t_9(__pyx_t_8); if (unlikely(!item)) goto __pyx_L3_unpacking_failed;
+    PyObject** temps[9] = {&__pyx_t_1,&__pyx_t_2,&__pyx_t_3,&__pyx_t_4,&__pyx_t_5,&__pyx_t_6,&__pyx_t_7,&__pyx_t_8,&__pyx_t_9};
+    __pyx_t_10 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 186, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
+    for (index=0; index < 9; index++) {
+      PyObject* item = __pyx_t_11(__pyx_t_10); if (unlikely(!item)) goto __pyx_L3_unpacking_failed;
       __Pyx_GOTREF(item);
       *(temps[index]) = item;
     }
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 7) < 0) __PYX_ERR(1, 175, __pyx_L1_error)
-    __pyx_t_9 = NULL;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 9) < 0) __PYX_ERR(1, 186, __pyx_L1_error)
+    __pyx_t_11 = NULL;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_9 = NULL;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __pyx_t_11 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(1, 175, __pyx_L1_error)
+    __PYX_ERR(1, 186, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_mapqs = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_name = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_source_id = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_sample_id = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_reference_start = __pyx_t_5;
   __pyx_t_5 = 0;
   __pyx_v_BX_tag = __pyx_t_6;
   __pyx_t_6 = 0;
-  __pyx_v_variants = __pyx_t_7;
+  __pyx_v_HP_tag = __pyx_t_7;
   __pyx_t_7 = 0;
+  __pyx_v_PS_tag = __pyx_t_8;
+  __pyx_t_8 = 0;
+  __pyx_v_variants = __pyx_t_9;
+  __pyx_t_9 = 0;
 
-  /* "whatshap/core.pyx":178
+  /* "whatshap/core.pyx":189
  * 
  * 		# TODO: Duplicated code from __cinit__ is ugly, but cinit cannot be used here directly
  * 		cdef string _name = b''             # <<<<<<<<<<<<<<
  * 		cdef string _BX_tag = b''
- * 		if name is None:
+ * 
  */
-  __pyx_t_10 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 178, __pyx_L1_error)
-  __pyx_v__name = __pyx_t_10;
+  __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 189, __pyx_L1_error)
+  __pyx_v__name = __pyx_t_12;
 
-  /* "whatshap/core.pyx":179
+  /* "whatshap/core.pyx":190
  * 		# TODO: Duplicated code from __cinit__ is ugly, but cinit cannot be used here directly
  * 		cdef string _name = b''
  * 		cdef string _BX_tag = b''             # <<<<<<<<<<<<<<
+ * 
  * 		if name is None:
- * 			self.thisptr = NULL
  */
-  __pyx_t_10 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 179, __pyx_L1_error)
-  __pyx_v__BX_tag = __pyx_t_10;
+  __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 190, __pyx_L1_error)
+  __pyx_v__BX_tag = __pyx_t_12;
 
-  /* "whatshap/core.pyx":180
- * 		cdef string _name = b''
+  /* "whatshap/core.pyx":192
  * 		cdef string _BX_tag = b''
+ * 
  * 		if name is None:             # <<<<<<<<<<<<<<
  * 			self.thisptr = NULL
  * 			self.ownsptr = False
  */
-  __pyx_t_11 = (__pyx_v_name == Py_None);
-  __pyx_t_12 = (__pyx_t_11 != 0);
-  if (__pyx_t_12) {
+  __pyx_t_13 = (__pyx_v_name == Py_None);
+  __pyx_t_14 = (__pyx_t_13 != 0);
+  if (__pyx_t_14) {
 
-    /* "whatshap/core.pyx":181
- * 		cdef string _BX_tag = b''
+    /* "whatshap/core.pyx":193
+ * 
  * 		if name is None:
  * 			self.thisptr = NULL             # <<<<<<<<<<<<<<
  * 			self.ownsptr = False
  * 		else:
  */
     __pyx_v_self->thisptr = NULL;
 
-    /* "whatshap/core.pyx":182
+    /* "whatshap/core.pyx":194
  * 		if name is None:
  * 			self.thisptr = NULL
  * 			self.ownsptr = False             # <<<<<<<<<<<<<<
  * 		else:
  * 			# TODO: Is this the best way to handle string arguments?
  */
     __pyx_v_self->ownsptr = 0;
 
-    /* "whatshap/core.pyx":180
- * 		cdef string _name = b''
+    /* "whatshap/core.pyx":192
  * 		cdef string _BX_tag = b''
+ * 
  * 		if name is None:             # <<<<<<<<<<<<<<
  * 			self.thisptr = NULL
  * 			self.ownsptr = False
  */
     goto __pyx_L5;
   }
 
-  /* "whatshap/core.pyx":185
+  /* "whatshap/core.pyx":197
  * 		else:
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')             # <<<<<<<<<<<<<<
  * 			if BX_tag is not b'' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_7 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_7)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_6, function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
-    __pyx_t_7 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_u_UTF_8);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 185, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __pyx_t_10 = __pyx_convert_string_from_py_std__in_string(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 185, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_v__name = __pyx_t_10;
+    __pyx_t_9 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_UTF_8);
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 197, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __pyx_v__name = __pyx_t_12;
 
-    /* "whatshap/core.pyx":186
+    /* "whatshap/core.pyx":198
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not b'' and BX_tag is not None:             # <<<<<<<<<<<<<<
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  */
-    __pyx_t_11 = (__pyx_v_BX_tag != __pyx_kp_b__3);
-    __pyx_t_13 = (__pyx_t_11 != 0);
-    if (__pyx_t_13) {
+    __pyx_t_13 = (__pyx_v_BX_tag != __pyx_kp_b__3);
+    __pyx_t_15 = (__pyx_t_13 != 0);
+    if (__pyx_t_15) {
     } else {
-      __pyx_t_12 = __pyx_t_13;
+      __pyx_t_14 = __pyx_t_15;
       goto __pyx_L7_bool_binop_done;
     }
-    __pyx_t_13 = (__pyx_v_BX_tag != Py_None);
-    __pyx_t_11 = (__pyx_t_13 != 0);
-    __pyx_t_12 = __pyx_t_11;
+    __pyx_t_15 = (__pyx_v_BX_tag != Py_None);
+    __pyx_t_13 = (__pyx_t_15 != 0);
+    __pyx_t_14 = __pyx_t_13;
     __pyx_L7_bool_binop_done:;
-    if (__pyx_t_12) {
+    if (__pyx_t_14) {
 
-      /* "whatshap/core.pyx":187
+      /* "whatshap/core.pyx":199
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not b'' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')             # <<<<<<<<<<<<<<
- * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  * 			self.ownsptr = True
  */
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_BX_tag, __pyx_n_s_encode); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 187, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_5 = NULL;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
-        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
-        if (likely(__pyx_t_5)) {
-          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
-          __Pyx_INCREF(__pyx_t_5);
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_BX_tag, __pyx_n_s_encode); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 199, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_7 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+        __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_8);
+        if (likely(__pyx_t_7)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
-          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __Pyx_DECREF_SET(__pyx_t_8, function);
         }
       }
-      __pyx_t_7 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_5, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_kp_u_UTF_8);
-      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 187, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_10 = __pyx_convert_string_from_py_std__in_string(__pyx_t_7); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 187, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_v__BX_tag = __pyx_t_10;
+      __pyx_t_9 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_7, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_kp_u_UTF_8);
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 199, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_12 = __pyx_convert_string_from_py_std__in_string(__pyx_t_9); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 199, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_v__BX_tag = __pyx_t_12;
 
-      /* "whatshap/core.pyx":186
+      /* "whatshap/core.pyx":198
  * 			# TODO: Is this the best way to handle string arguments?
  * 			_name = name.encode('UTF-8')
  * 			if BX_tag is not b'' and BX_tag is not None:             # <<<<<<<<<<<<<<
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  */
     }
 
-    /* "whatshap/core.pyx":188
+    /* "whatshap/core.pyx":200
  * 			if BX_tag is not b'' and BX_tag is not None:
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)             # <<<<<<<<<<<<<<
+ * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)             # <<<<<<<<<<<<<<
  * 			self.ownsptr = True
  * 
  */
-    __pyx_t_15 = PyObject_Length(__pyx_v_mapqs); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(1, 188, __pyx_L1_error)
-    if (((__pyx_t_15 > 0) != 0)) {
-      __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_mapqs, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 188, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_16 = __Pyx_PyInt_As_int(__pyx_t_7); if (unlikely((__pyx_t_16 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L1_error)
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_14 = __pyx_t_16;
+    __pyx_t_17 = PyObject_Length(__pyx_v_mapqs); if (unlikely(__pyx_t_17 == ((Py_ssize_t)-1))) __PYX_ERR(1, 200, __pyx_L1_error)
+    if (((__pyx_t_17 > 0) != 0)) {
+      __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_mapqs, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 200, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __pyx_t_18 = __Pyx_PyInt_As_int(__pyx_t_9); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_16 = __pyx_t_18;
     } else {
-      __pyx_t_14 = 0;
+      __pyx_t_16 = 0;
     }
-    __pyx_t_16 = __Pyx_PyInt_As_int(__pyx_v_source_id); if (unlikely((__pyx_t_16 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L1_error)
-    __pyx_t_17 = __Pyx_PyInt_As_int(__pyx_v_sample_id); if (unlikely((__pyx_t_17 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L1_error)
-    __pyx_t_18 = __Pyx_PyInt_As_int(__pyx_v_reference_start); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyInt_As_int(__pyx_v_source_id); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
+    __pyx_t_19 = __Pyx_PyInt_As_int(__pyx_v_sample_id); if (unlikely((__pyx_t_19 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
+    __pyx_t_20 = __Pyx_PyInt_As_int(__pyx_v_reference_start); if (unlikely((__pyx_t_20 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
+    __pyx_t_21 = __Pyx_PyInt_As_int(__pyx_v_HP_tag); if (unlikely((__pyx_t_21 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
+    __pyx_t_22 = __Pyx_PyInt_As_int(__pyx_v_PS_tag); if (unlikely((__pyx_t_22 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L1_error)
     try {
-      __pyx_t_19 = new Read(__pyx_v__name, __pyx_t_14, __pyx_t_16, __pyx_t_17, __pyx_t_18, __pyx_v__BX_tag);
+      __pyx_t_23 = new Read(__pyx_v__name, __pyx_t_16, __pyx_t_18, __pyx_t_19, __pyx_t_20, __pyx_v__BX_tag, __pyx_t_21, __pyx_t_22);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 188, __pyx_L1_error)
+      __PYX_ERR(1, 200, __pyx_L1_error)
     }
-    __pyx_v_self->thisptr = __pyx_t_19;
+    __pyx_v_self->thisptr = __pyx_t_23;
 
-    /* "whatshap/core.pyx":189
+    /* "whatshap/core.pyx":201
  * 				_BX_tag = BX_tag.encode('UTF-8')
- * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)
+ * 			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
  * 			self.ownsptr = True             # <<<<<<<<<<<<<<
  * 
  * 		for mapq in mapqs[1:]:
  */
     __pyx_v_self->ownsptr = 1;
   }
   __pyx_L5:;
 
-  /* "whatshap/core.pyx":191
+  /* "whatshap/core.pyx":203
  * 			self.ownsptr = True
  * 
  * 		for mapq in mapqs[1:]:             # <<<<<<<<<<<<<<
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:
  */
-  __pyx_t_7 = __Pyx_PyObject_GetSlice(__pyx_v_mapqs, 1, 0, NULL, NULL, &__pyx_slice__5, 1, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_7);
-  if (likely(PyList_CheckExact(__pyx_t_7)) || PyTuple_CheckExact(__pyx_t_7)) {
-    __pyx_t_6 = __pyx_t_7; __Pyx_INCREF(__pyx_t_6); __pyx_t_15 = 0;
-    __pyx_t_20 = NULL;
+  __pyx_t_9 = __Pyx_PyObject_GetSlice(__pyx_v_mapqs, 1, 0, NULL, NULL, &__pyx_slice__5, 1, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 203, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+  if (likely(PyList_CheckExact(__pyx_t_9)) || PyTuple_CheckExact(__pyx_t_9)) {
+    __pyx_t_8 = __pyx_t_9; __Pyx_INCREF(__pyx_t_8); __pyx_t_17 = 0;
+    __pyx_t_24 = NULL;
   } else {
-    __pyx_t_15 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 191, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_20 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 191, __pyx_L1_error)
+    __pyx_t_17 = -1; __pyx_t_8 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 203, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_24 = Py_TYPE(__pyx_t_8)->tp_iternext; if (unlikely(!__pyx_t_24)) __PYX_ERR(1, 203, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
   for (;;) {
-    if (likely(!__pyx_t_20)) {
-      if (likely(PyList_CheckExact(__pyx_t_6))) {
-        if (__pyx_t_15 >= PyList_GET_SIZE(__pyx_t_6)) break;
+    if (likely(!__pyx_t_24)) {
+      if (likely(PyList_CheckExact(__pyx_t_8))) {
+        if (__pyx_t_17 >= PyList_GET_SIZE(__pyx_t_8)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_15); __Pyx_INCREF(__pyx_t_7); __pyx_t_15++; if (unlikely(0 < 0)) __PYX_ERR(1, 191, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(1, 203, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_6, __pyx_t_15); __pyx_t_15++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 191, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 203, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
-        if (__pyx_t_15 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+        if (__pyx_t_17 >= PyTuple_GET_SIZE(__pyx_t_8)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_15); __Pyx_INCREF(__pyx_t_7); __pyx_t_15++; if (unlikely(0 < 0)) __PYX_ERR(1, 191, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_8, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(1, 203, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_6, __pyx_t_15); __pyx_t_15++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 191, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 203, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
-      __pyx_t_7 = __pyx_t_20(__pyx_t_6);
-      if (unlikely(!__pyx_t_7)) {
+      __pyx_t_9 = __pyx_t_24(__pyx_t_8);
+      if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 191, __pyx_L1_error)
+          else __PYX_ERR(1, 203, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_9);
     }
-    __Pyx_XDECREF_SET(__pyx_v_mapq, __pyx_t_7);
-    __pyx_t_7 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_mapq, __pyx_t_9);
+    __pyx_t_9 = 0;
 
-    /* "whatshap/core.pyx":192
+    /* "whatshap/core.pyx":204
  * 
  * 		for mapq in mapqs[1:]:
  * 			self.add_mapq(mapq)             # <<<<<<<<<<<<<<
  * 		for (pos, allele, quality) in variants:
  * 			self.add_variant(pos, allele, quality)
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_mapq); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 192, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = NULL;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
-        __Pyx_INCREF(__pyx_t_4);
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_mapq); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_7);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __Pyx_DECREF_SET(__pyx_t_7, function);
       }
     }
-    __pyx_t_7 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_mapq) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_mapq);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 192, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_9 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_6, __pyx_v_mapq) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_mapq);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "whatshap/core.pyx":191
+    /* "whatshap/core.pyx":203
  * 			self.ownsptr = True
  * 
  * 		for mapq in mapqs[1:]:             # <<<<<<<<<<<<<<
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:
  */
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "whatshap/core.pyx":193
+  /* "whatshap/core.pyx":205
  * 		for mapq in mapqs[1:]:
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:             # <<<<<<<<<<<<<<
  * 			self.add_variant(pos, allele, quality)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_variants)) || PyTuple_CheckExact(__pyx_v_variants)) {
-    __pyx_t_6 = __pyx_v_variants; __Pyx_INCREF(__pyx_t_6); __pyx_t_15 = 0;
-    __pyx_t_20 = NULL;
+    __pyx_t_8 = __pyx_v_variants; __Pyx_INCREF(__pyx_t_8); __pyx_t_17 = 0;
+    __pyx_t_24 = NULL;
   } else {
-    __pyx_t_15 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_variants); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 193, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_20 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_17 = -1; __pyx_t_8 = PyObject_GetIter(__pyx_v_variants); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 205, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_24 = Py_TYPE(__pyx_t_8)->tp_iternext; if (unlikely(!__pyx_t_24)) __PYX_ERR(1, 205, __pyx_L1_error)
   }
   for (;;) {
-    if (likely(!__pyx_t_20)) {
-      if (likely(PyList_CheckExact(__pyx_t_6))) {
-        if (__pyx_t_15 >= PyList_GET_SIZE(__pyx_t_6)) break;
+    if (likely(!__pyx_t_24)) {
+      if (likely(PyList_CheckExact(__pyx_t_8))) {
+        if (__pyx_t_17 >= PyList_GET_SIZE(__pyx_t_8)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_15); __Pyx_INCREF(__pyx_t_7); __pyx_t_15++; if (unlikely(0 < 0)) __PYX_ERR(1, 193, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(1, 205, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_6, __pyx_t_15); __pyx_t_15++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 193, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 205, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
-        if (__pyx_t_15 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
+        if (__pyx_t_17 >= PyTuple_GET_SIZE(__pyx_t_8)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_15); __Pyx_INCREF(__pyx_t_7); __pyx_t_15++; if (unlikely(0 < 0)) __PYX_ERR(1, 193, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_8, __pyx_t_17); __Pyx_INCREF(__pyx_t_9); __pyx_t_17++; if (unlikely(0 < 0)) __PYX_ERR(1, 205, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_6, __pyx_t_15); __pyx_t_15++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 193, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_7);
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_17); __pyx_t_17++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 205, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
-      __pyx_t_7 = __pyx_t_20(__pyx_t_6);
-      if (unlikely(!__pyx_t_7)) {
+      __pyx_t_9 = __pyx_t_24(__pyx_t_8);
+      if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 193, __pyx_L1_error)
+          else __PYX_ERR(1, 205, __pyx_L1_error)
         }
         break;
       }
-      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_9);
     }
-    if ((likely(PyTuple_CheckExact(__pyx_t_7))) || (PyList_CheckExact(__pyx_t_7))) {
-      PyObject* sequence = __pyx_t_7;
+    if ((likely(PyTuple_CheckExact(__pyx_t_9))) || (PyList_CheckExact(__pyx_t_9))) {
+      PyObject* sequence = __pyx_t_9;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 3)) {
         if (size > 3) __Pyx_RaiseTooManyValuesError(3);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(1, 193, __pyx_L1_error)
+        __PYX_ERR(1, 205, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
-        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
-        __pyx_t_3 = PyTuple_GET_ITEM(sequence, 2); 
+        __pyx_t_7 = PyTuple_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyTuple_GET_ITEM(sequence, 1); 
+        __pyx_t_5 = PyTuple_GET_ITEM(sequence, 2); 
       } else {
-        __pyx_t_5 = PyList_GET_ITEM(sequence, 0); 
-        __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
-        __pyx_t_3 = PyList_GET_ITEM(sequence, 2); 
+        __pyx_t_7 = PyList_GET_ITEM(sequence, 0); 
+        __pyx_t_6 = PyList_GET_ITEM(sequence, 1); 
+        __pyx_t_5 = PyList_GET_ITEM(sequence, 2); 
       }
+      __Pyx_INCREF(__pyx_t_7);
+      __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
-      __Pyx_INCREF(__pyx_t_4);
-      __Pyx_INCREF(__pyx_t_3);
       #else
-      __pyx_t_5 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 193, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 205, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __pyx_t_6 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 205, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_5 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 205, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 193, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_3 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
       #endif
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_2 = PyObject_GetIter(__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 193, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_9 = Py_TYPE(__pyx_t_2)->tp_iternext;
-      index = 0; __pyx_t_5 = __pyx_t_9(__pyx_t_2); if (unlikely(!__pyx_t_5)) goto __pyx_L13_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_5);
-      index = 1; __pyx_t_4 = __pyx_t_9(__pyx_t_2); if (unlikely(!__pyx_t_4)) goto __pyx_L13_unpacking_failed;
+      __pyx_t_4 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 205, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      index = 2; __pyx_t_3 = __pyx_t_9(__pyx_t_2); if (unlikely(!__pyx_t_3)) goto __pyx_L13_unpacking_failed;
-      __Pyx_GOTREF(__pyx_t_3);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_2), 3) < 0) __PYX_ERR(1, 193, __pyx_L1_error)
-      __pyx_t_9 = NULL;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_t_11 = Py_TYPE(__pyx_t_4)->tp_iternext;
+      index = 0; __pyx_t_7 = __pyx_t_11(__pyx_t_4); if (unlikely(!__pyx_t_7)) goto __pyx_L13_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_7);
+      index = 1; __pyx_t_6 = __pyx_t_11(__pyx_t_4); if (unlikely(!__pyx_t_6)) goto __pyx_L13_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_6);
+      index = 2; __pyx_t_5 = __pyx_t_11(__pyx_t_4); if (unlikely(!__pyx_t_5)) goto __pyx_L13_unpacking_failed;
+      __Pyx_GOTREF(__pyx_t_5);
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_4), 3) < 0) __PYX_ERR(1, 205, __pyx_L1_error)
+      __pyx_t_11 = NULL;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       goto __pyx_L14_unpacking_done;
       __pyx_L13_unpacking_failed:;
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_9 = NULL;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_11 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(1, 193, __pyx_L1_error)
+      __PYX_ERR(1, 205, __pyx_L1_error)
       __pyx_L14_unpacking_done:;
     }
-    __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_5);
+    __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_allele, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_XDECREF_SET(__pyx_v_quality, __pyx_t_5);
     __pyx_t_5 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_allele, __pyx_t_4);
-    __pyx_t_4 = 0;
-    __Pyx_XDECREF_SET(__pyx_v_quality, __pyx_t_3);
-    __pyx_t_3 = 0;
 
-    /* "whatshap/core.pyx":194
+    /* "whatshap/core.pyx":206
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:
  * 			self.add_variant(pos, allele, quality)             # <<<<<<<<<<<<<<
  * 
  * 	def add_variant(self, int position, int allele, int quality):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_variant); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 194, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = NULL;
-    __pyx_t_18 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-      if (likely(__pyx_t_4)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-        __Pyx_INCREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add_variant); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    __pyx_t_22 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_18 = 1;
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_22 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_pos, __pyx_v_allele, __pyx_v_quality};
-      __pyx_t_7 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 3+__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 194, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_7);
+    if (PyFunction_Check(__pyx_t_5)) {
+      PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_pos, __pyx_v_allele, __pyx_v_quality};
+      __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 206, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
-    if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-      PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_pos, __pyx_v_allele, __pyx_v_quality};
-      __pyx_t_7 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_18, 3+__pyx_t_18); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 194, __pyx_L1_error)
-      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __Pyx_GOTREF(__pyx_t_7);
+    if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
+      PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_pos, __pyx_v_allele, __pyx_v_quality};
+      __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_22, 3+__pyx_t_22); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 206, __pyx_L1_error)
+      __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GOTREF(__pyx_t_9);
     } else
     #endif
     {
-      __pyx_t_5 = PyTuple_New(3+__pyx_t_18); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 194, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      if (__pyx_t_4) {
-        __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4); __pyx_t_4 = NULL;
+      __pyx_t_7 = PyTuple_New(3+__pyx_t_22); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      if (__pyx_t_6) {
+        __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_INCREF(__pyx_v_pos);
       __Pyx_GIVEREF(__pyx_v_pos);
-      PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_18, __pyx_v_pos);
+      PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_22, __pyx_v_pos);
       __Pyx_INCREF(__pyx_v_allele);
       __Pyx_GIVEREF(__pyx_v_allele);
-      PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_18, __pyx_v_allele);
+      PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_22, __pyx_v_allele);
       __Pyx_INCREF(__pyx_v_quality);
       __Pyx_GIVEREF(__pyx_v_quality);
-      PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_18, __pyx_v_quality);
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_5, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 194, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_7);
-      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_22, __pyx_v_quality);
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "whatshap/core.pyx":193
+    /* "whatshap/core.pyx":205
  * 		for mapq in mapqs[1:]:
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:             # <<<<<<<<<<<<<<
  * 			self.add_variant(pos, allele, quality)
  * 
  */
   }
-  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "whatshap/core.pyx":174
- * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)
+  /* "whatshap/core.pyx":185
+ * 		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
- * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, variants = state
+ * 		mapqs, name, source_id, sample_id, reference_start, BX_tag, HP_tag, PS_tag, variants = state
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -6374,34 +6636,38 @@
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("whatshap.core.Read.__setstate__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mapqs);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XDECREF(__pyx_v_source_id);
   __Pyx_XDECREF(__pyx_v_sample_id);
   __Pyx_XDECREF(__pyx_v_reference_start);
   __Pyx_XDECREF(__pyx_v_BX_tag);
+  __Pyx_XDECREF(__pyx_v_HP_tag);
+  __Pyx_XDECREF(__pyx_v_PS_tag);
   __Pyx_XDECREF(__pyx_v_variants);
   __Pyx_XDECREF(__pyx_v_mapq);
   __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_XDECREF(__pyx_v_allele);
   __Pyx_XDECREF(__pyx_v_quality);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":196
+/* "whatshap/core.pyx":208
  * 			self.add_variant(pos, allele, quality)
  * 
  * 	def add_variant(self, int position, int allele, int quality):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addVariant(position, allele, quality)
  */
 
@@ -6438,40 +6704,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_position)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allele)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, 1); __PYX_ERR(1, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, 1); __PYX_ERR(1, 208, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_quality)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, 2); __PYX_ERR(1, 196, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, 2); __PYX_ERR(1, 208, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_variant") < 0)) __PYX_ERR(1, 196, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_variant") < 0)) __PYX_ERR(1, 208, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_position = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_position == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L3_error)
-    __pyx_v_allele = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_allele == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L3_error)
-    __pyx_v_quality = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_quality == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 196, __pyx_L3_error)
+    __pyx_v_position = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_position == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 208, __pyx_L3_error)
+    __pyx_v_allele = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_allele == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 208, __pyx_L3_error)
+    __pyx_v_quality = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_quality == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 208, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 196, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_variant", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 208, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Read.add_variant", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_4Read_21add_variant(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self), __pyx_v_position, __pyx_v_allele, __pyx_v_quality);
 
@@ -6484,45 +6750,45 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_variant", 0);
 
-  /* "whatshap/core.pyx":197
+  /* "whatshap/core.pyx":209
  * 
  * 	def add_variant(self, int position, int allele, int quality):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		self.thisptr.addVariant(position, allele, quality)
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 197, __pyx_L1_error)
+      __PYX_ERR(1, 209, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":198
+  /* "whatshap/core.pyx":210
  * 	def add_variant(self, int position, int allele, int quality):
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addVariant(position, allele, quality)             # <<<<<<<<<<<<<<
  * 
  * 	def add_mapq(self, int mapq):
  */
   try {
     __pyx_v_self->thisptr->addVariant(__pyx_v_position, __pyx_v_allele, __pyx_v_quality);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 198, __pyx_L1_error)
+    __PYX_ERR(1, 210, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":196
+  /* "whatshap/core.pyx":208
  * 			self.add_variant(pos, allele, quality)
  * 
  * 	def add_variant(self, int position, int allele, int quality):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addVariant(position, allele, quality)
  */
 
@@ -6534,15 +6800,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":200
+/* "whatshap/core.pyx":212
  * 		self.thisptr.addVariant(position, allele, quality)
  * 
  * 	def add_mapq(self, int mapq):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addMapq(mapq)
  */
 
@@ -6553,15 +6819,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add_mapq (wrapper)", 0);
   assert(__pyx_arg_mapq); {
-    __pyx_v_mapq = __Pyx_PyInt_As_int(__pyx_arg_mapq); if (unlikely((__pyx_v_mapq == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 200, __pyx_L3_error)
+    __pyx_v_mapq = __Pyx_PyInt_As_int(__pyx_arg_mapq); if (unlikely((__pyx_v_mapq == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 212, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Read.add_mapq", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -6576,45 +6842,45 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_mapq", 0);
 
-  /* "whatshap/core.pyx":201
+  /* "whatshap/core.pyx":213
  * 
  * 	def add_mapq(self, int mapq):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		self.thisptr.addMapq(mapq)
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 201, __pyx_L1_error)
+      __PYX_ERR(1, 213, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":202
+  /* "whatshap/core.pyx":214
  * 	def add_mapq(self, int mapq):
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addMapq(mapq)             # <<<<<<<<<<<<<<
  * 
  * 	def sort(self):
  */
   try {
     __pyx_v_self->thisptr->addMapq(__pyx_v_mapq);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 202, __pyx_L1_error)
+    __PYX_ERR(1, 214, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":200
+  /* "whatshap/core.pyx":212
  * 		self.thisptr.addVariant(position, allele, quality)
  * 
  * 	def add_mapq(self, int mapq):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.addMapq(mapq)
  */
 
@@ -6626,15 +6892,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":204
+/* "whatshap/core.pyx":216
  * 		self.thisptr.addMapq(mapq)
  * 
  * 	def sort(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.sortVariants()
  */
 
@@ -6655,45 +6921,45 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sort", 0);
 
-  /* "whatshap/core.pyx":205
+  /* "whatshap/core.pyx":217
  * 
  * 	def sort(self):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		self.thisptr.sortVariants()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 205, __pyx_L1_error)
+      __PYX_ERR(1, 217, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":206
+  /* "whatshap/core.pyx":218
  * 	def sort(self):
  * 		assert self.thisptr != NULL
  * 		self.thisptr.sortVariants()             # <<<<<<<<<<<<<<
  * 
  * 	def is_sorted(self):
  */
   try {
     __pyx_v_self->thisptr->sortVariants();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 206, __pyx_L1_error)
+    __PYX_ERR(1, 218, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":204
+  /* "whatshap/core.pyx":216
  * 		self.thisptr.addMapq(mapq)
  * 
  * 	def sort(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		self.thisptr.sortVariants()
  */
 
@@ -6705,15 +6971,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":208
+/* "whatshap/core.pyx":220
  * 		self.thisptr.sortVariants()
  * 
  * 	def is_sorted(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.isSorted()
  */
 
@@ -6736,51 +7002,51 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_sorted", 0);
 
-  /* "whatshap/core.pyx":209
+  /* "whatshap/core.pyx":221
  * 
  * 	def is_sorted(self):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		return self.thisptr.isSorted()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 209, __pyx_L1_error)
+      __PYX_ERR(1, 221, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":210
+  /* "whatshap/core.pyx":222
  * 	def is_sorted(self):
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.isSorted()             # <<<<<<<<<<<<<<
  * 
  * 	def has_BX_tag(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->isSorted();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 210, __pyx_L1_error)
+    __PYX_ERR(1, 222, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 210, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":208
+  /* "whatshap/core.pyx":220
  * 		self.thisptr.sortVariants()
  * 
  * 	def is_sorted(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.isSorted()
  */
 
@@ -6791,15 +7057,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":212
+/* "whatshap/core.pyx":224
  * 		return self.thisptr.isSorted()
  * 
  * 	def has_BX_tag(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.hasBXTag()
  */
 
@@ -6822,51 +7088,51 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("has_BX_tag", 0);
 
-  /* "whatshap/core.pyx":213
+  /* "whatshap/core.pyx":225
  * 
  * 	def has_BX_tag(self):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		return self.thisptr.hasBXTag()
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 213, __pyx_L1_error)
+      __PYX_ERR(1, 225, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":214
+  /* "whatshap/core.pyx":226
  * 	def has_BX_tag(self):
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.hasBXTag()             # <<<<<<<<<<<<<<
  * 
- * 
+ * 	def has_HP_tag(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->hasBXTag();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 214, __pyx_L1_error)
+    __PYX_ERR(1, 226, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 214, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":212
+  /* "whatshap/core.pyx":224
  * 		return self.thisptr.isSorted()
  * 
  * 	def has_BX_tag(self):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		return self.thisptr.hasBXTag()
  */
 
@@ -6877,34 +7143,206 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "whatshap/core.pyx":228
+ * 		return self.thisptr.hasBXTag()
+ * 
+ * 	def has_HP_tag(self):             # <<<<<<<<<<<<<<
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8whatshap_4core_4Read_32has_HP_tag(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_32has_HP_tag(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("has_HP_tag (wrapper)", 0);
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_31has_HP_tag(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8whatshap_4core_4Read_31has_HP_tag(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  bool __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("has_HP_tag", 0);
+
+  /* "whatshap/core.pyx":229
+ * 
+ * 	def has_HP_tag(self):
+ * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
+ * 		return self.thisptr.hasBXTag()
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
+      PyErr_SetNone(PyExc_AssertionError);
+      __PYX_ERR(1, 229, __pyx_L1_error)
+    }
+  }
+  #endif
+
+  /* "whatshap/core.pyx":230
+ * 	def has_HP_tag(self):
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()             # <<<<<<<<<<<<<<
+ * 
+ * 	def has_PS_tag(self):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  try {
+    __pyx_t_1 = __pyx_v_self->thisptr->hasBXTag();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 230, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "whatshap/core.pyx":228
+ * 		return self.thisptr.hasBXTag()
+ * 
+ * 	def has_HP_tag(self):             # <<<<<<<<<<<<<<
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("whatshap.core.Read.has_HP_tag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "whatshap/core.pyx":232
+ * 		return self.thisptr.hasBXTag()
+ * 
+ * 	def has_PS_tag(self):             # <<<<<<<<<<<<<<
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8whatshap_4core_4Read_34has_PS_tag(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_34has_PS_tag(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("has_PS_tag (wrapper)", 0);
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_33has_PS_tag(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8whatshap_4core_4Read_33has_PS_tag(struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  bool __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("has_PS_tag", 0);
+
+  /* "whatshap/core.pyx":233
+ * 
+ * 	def has_PS_tag(self):
+ * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
+ * 		return self.thisptr.hasBXTag()
+ * 
+ */
+  #ifndef CYTHON_WITHOUT_ASSERTIONS
+  if (unlikely(__pyx_assertions_enabled())) {
+    if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
+      PyErr_SetNone(PyExc_AssertionError);
+      __PYX_ERR(1, 233, __pyx_L1_error)
+    }
+  }
+  #endif
+
+  /* "whatshap/core.pyx":234
+ * 	def has_PS_tag(self):
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()             # <<<<<<<<<<<<<<
+ * 
+ * cdef class ReadSet:
+ */
+  __Pyx_XDECREF(__pyx_r);
+  try {
+    __pyx_t_1 = __pyx_v_self->thisptr->hasBXTag();
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 234, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "whatshap/core.pyx":232
+ * 		return self.thisptr.hasBXTag()
+ * 
+ * 	def has_PS_tag(self):             # <<<<<<<<<<<<<<
+ * 		assert self.thisptr != NULL
+ * 		return self.thisptr.hasBXTag()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("whatshap.core.Read.has_PS_tag", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8whatshap_4core_4Read_32__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_8whatshap_4core_4Read_32__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_8whatshap_4core_4Read_36__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_36__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8whatshap_4core_4Read_31__reduce_cython__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_35__reduce_cython__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8whatshap_4core_4Read_31__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
+static PyObject *__pyx_pf_8whatshap_4core_4Read_35__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -6941,27 +7379,27 @@
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_8whatshap_4core_4Read_34__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_8whatshap_4core_4Read_34__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_8whatshap_4core_4Read_38__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_8whatshap_4core_4Read_38__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_8whatshap_4core_4Read_33__setstate_cython__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_8whatshap_4core_4Read_37__setstate_cython__(((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8whatshap_4core_4Read_33__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_8whatshap_4core_4Read_37__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_8whatshap_4core_Read *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -6990,15 +7428,15 @@
   __Pyx_AddTraceback("whatshap.core.Read.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":218
+/* "whatshap/core.pyx":237
  * 
  * cdef class ReadSet:
  * 	def __cinit__(self):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.ReadSet()
  * 
  */
 
@@ -7023,30 +7461,30 @@
   __Pyx_RefNannyDeclarations
   ReadSet *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":219
+  /* "whatshap/core.pyx":238
  * cdef class ReadSet:
  * 	def __cinit__(self):
  * 		self.thisptr = new cpp.ReadSet()             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   try {
     __pyx_t_1 = new ReadSet();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 219, __pyx_L1_error)
+    __PYX_ERR(1, 238, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":218
+  /* "whatshap/core.pyx":237
  * 
  * cdef class ReadSet:
  * 	def __cinit__(self):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.ReadSet()
  * 
  */
 
@@ -7057,15 +7495,15 @@
   __Pyx_AddTraceback("whatshap.core.ReadSet.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":221
+/* "whatshap/core.pyx":240
  * 		self.thisptr = new cpp.ReadSet()
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -7080,36 +7518,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_7ReadSet_2__dealloc__(struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":222
+  /* "whatshap/core.pyx":241
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def add(self, Read read):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":221
+  /* "whatshap/core.pyx":240
  * 		self.thisptr = new cpp.ReadSet()
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":224
+/* "whatshap/core.pyx":243
  * 		del self.thisptr
  * 
  * 	def add(self, Read read):             # <<<<<<<<<<<<<<
  * 		"""Adds a read to the set.
  * 		WARNING: this will internally create a copy of the wrapped C++ Read object,
  */
 
@@ -7119,15 +7557,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_7ReadSet_5add(PyObject *__pyx_v_self, PyObject *__pyx_v_read) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("add (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read), __pyx_ptype_8whatshap_4core_Read, 1, "read", 0))) __PYX_ERR(1, 224, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_read), __pyx_ptype_8whatshap_4core_Read, 1, "read", 0))) __PYX_ERR(1, 243, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_7ReadSet_4add(((struct __pyx_obj_8whatshap_4core_ReadSet *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_Read *)__pyx_v_read));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -7140,35 +7578,35 @@
   __Pyx_RefNannyDeclarations
   Read *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add", 0);
 
-  /* "whatshap/core.pyx":229
+  /* "whatshap/core.pyx":248
  * 		so that subsequent changes to the Read don't affect the
  * 		newly created copy that is added to the ReadSet."""
  * 		self.thisptr.add(new cpp.Read(read.thisptr[0]))             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
   try {
     __pyx_t_1 = new Read((__pyx_v_read->thisptr[0]));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 229, __pyx_L1_error)
+    __PYX_ERR(1, 248, __pyx_L1_error)
   }
   try {
     __pyx_v_self->thisptr->add(__pyx_t_1);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 229, __pyx_L1_error)
+    __PYX_ERR(1, 248, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":224
+  /* "whatshap/core.pyx":243
  * 		del self.thisptr
  * 
  * 	def add(self, Read read):             # <<<<<<<<<<<<<<
  * 		"""Adds a read to the set.
  * 		WARNING: this will internally create a copy of the wrapped C++ Read object,
  */
 
@@ -7180,15 +7618,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":231
+/* "whatshap/core.pyx":250
  * 		self.thisptr.add(new cpp.Read(read.thisptr[0]))
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -7211,35 +7649,35 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "whatshap/core.pyx":232
+  /* "whatshap/core.pyx":251
  * 
  * 	def __str__(self):
  * 		return self.thisptr.toString().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 	def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->toString();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 232, __pyx_L1_error)
+    __PYX_ERR(1, 251, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 232, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":231
+  /* "whatshap/core.pyx":250
  * 		self.thisptr.add(new cpp.Read(read.thisptr[0]))
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -7251,15 +7689,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8whatshap_4core_7ReadSet_10generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "whatshap/core.pyx":234
+/* "whatshap/core.pyx":253
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for i in range(self.thisptr.size()):
  * 			yield self[i]
  */
 
@@ -7284,23 +7722,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_8whatshap_4core___pyx_scope_struct_1___iter__ *)__pyx_tp_new_8whatshap_4core___pyx_scope_struct_1___iter__(__pyx_ptype_8whatshap_4core___pyx_scope_struct_1___iter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8whatshap_4core___pyx_scope_struct_1___iter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(1, 234, __pyx_L1_error)
+    __PYX_ERR(1, 253, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_7ReadSet_10generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_ReadSet___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 234, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_7ReadSet_10generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_ReadSet___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7329,41 +7767,41 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 234, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 253, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":235
+  /* "whatshap/core.pyx":254
  * 
  * 	def __iter__(self):
  * 		for i in range(self.thisptr.size()):             # <<<<<<<<<<<<<<
  * 			yield self[i]
  * 
  */
   try {
     __pyx_t_1 = __pyx_cur_scope->__pyx_v_self->thisptr->size();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 235, __pyx_L1_error)
+    __PYX_ERR(1, 254, __pyx_L1_error)
   }
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_cur_scope->__pyx_v_i = __pyx_t_3;
 
-    /* "whatshap/core.pyx":236
+    /* "whatshap/core.pyx":255
  * 	def __iter__(self):
  * 		for i in range(self.thisptr.size()):
  * 			yield self[i]             # <<<<<<<<<<<<<<
  * 
  * 	def __len__(self):
  */
-    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 236, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 255, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
     __Pyx_XGIVEREF(__pyx_r);
@@ -7372,19 +7810,19 @@
     /* return from generator, yielding value */
     __pyx_generator->resume_label = 1;
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 236, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 255, __pyx_L1_error)
   }
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "whatshap/core.pyx":234
+  /* "whatshap/core.pyx":253
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for i in range(self.thisptr.size()):
  * 			yield self[i]
  */
 
@@ -7401,15 +7839,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":238
+/* "whatshap/core.pyx":257
  * 			yield self[i]
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
@@ -7431,31 +7869,31 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "whatshap/core.pyx":239
+  /* "whatshap/core.pyx":258
  * 
  * 	def __len__(self):
  * 		return self.thisptr.size()             # <<<<<<<<<<<<<<
  * 
  * 	def __getitem__(self, key):
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->size();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 239, __pyx_L1_error)
+    __PYX_ERR(1, 258, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":238
+  /* "whatshap/core.pyx":257
  * 			yield self[i]
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
@@ -7464,15 +7902,15 @@
   __Pyx_AddTraceback("whatshap.core.ReadSet.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":241
+/* "whatshap/core.pyx":260
  * 		return self.thisptr.size()
  * 
  * 	def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError('ReadSet does not support slices')
  */
 
@@ -7507,353 +7945,353 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "whatshap/core.pyx":242
+  /* "whatshap/core.pyx":261
  * 
  * 	def __getitem__(self, key):
  * 		if isinstance(key, slice):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError('ReadSet does not support slices')
  * 		cdef string name = b''
  */
   __pyx_t_1 = PySlice_Check(__pyx_v_key); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "whatshap/core.pyx":243
+    /* "whatshap/core.pyx":262
  * 	def __getitem__(self, key):
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError('ReadSet does not support slices')             # <<<<<<<<<<<<<<
  * 		cdef string name = b''
  * 		cdef cpp.Read* cread = NULL
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 243, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 243, __pyx_L1_error)
+    __PYX_ERR(1, 262, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":242
+    /* "whatshap/core.pyx":261
  * 
  * 	def __getitem__(self, key):
  * 		if isinstance(key, slice):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError('ReadSet does not support slices')
  * 		cdef string name = b''
  */
   }
 
-  /* "whatshap/core.pyx":244
+  /* "whatshap/core.pyx":263
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError('ReadSet does not support slices')
  * 		cdef string name = b''             # <<<<<<<<<<<<<<
  * 		cdef cpp.Read* cread = NULL
  * 		cdef Read read = Read()
  */
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_kp_b__3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 263, __pyx_L1_error)
   __pyx_v_name = __pyx_t_4;
 
-  /* "whatshap/core.pyx":245
+  /* "whatshap/core.pyx":264
  * 			raise NotImplementedError('ReadSet does not support slices')
  * 		cdef string name = b''
  * 		cdef cpp.Read* cread = NULL             # <<<<<<<<<<<<<<
  * 		cdef Read read = Read()
  * 		if isinstance(key, int):
  */
   __pyx_v_cread = NULL;
 
-  /* "whatshap/core.pyx":246
+  /* "whatshap/core.pyx":265
  * 		cdef string name = b''
  * 		cdef cpp.Read* cread = NULL
  * 		cdef Read read = Read()             # <<<<<<<<<<<<<<
  * 		if isinstance(key, int):
  * 			read.thisptr = self.thisptr.get(key)
  */
-  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_Read)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 246, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_Read)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_read = ((struct __pyx_obj_8whatshap_4core_Read *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "whatshap/core.pyx":247
+  /* "whatshap/core.pyx":266
  * 		cdef cpp.Read* cread = NULL
  * 		cdef Read read = Read()
  * 		if isinstance(key, int):             # <<<<<<<<<<<<<<
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):
  */
   __pyx_t_2 = PyInt_Check(__pyx_v_key); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "whatshap/core.pyx":248
+    /* "whatshap/core.pyx":267
  * 		cdef Read read = Read()
  * 		if isinstance(key, int):
  * 			read.thisptr = self.thisptr.get(key)             # <<<<<<<<<<<<<<
  * 		elif isinstance(key, str):
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  */
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 248, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_key); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 267, __pyx_L1_error)
     try {
       __pyx_t_6 = __pyx_v_self->thisptr->get(__pyx_t_5);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 248, __pyx_L1_error)
+      __PYX_ERR(1, 267, __pyx_L1_error)
     }
     __pyx_v_read->thisptr = __pyx_t_6;
 
-    /* "whatshap/core.pyx":247
+    /* "whatshap/core.pyx":266
  * 		cdef cpp.Read* cread = NULL
  * 		cdef Read read = Read()
  * 		if isinstance(key, int):             # <<<<<<<<<<<<<<
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):
  */
     goto __pyx_L4;
   }
 
-  /* "whatshap/core.pyx":249
+  /* "whatshap/core.pyx":268
  * 		if isinstance(key, int):
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_key); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "whatshap/core.pyx":250
+    /* "whatshap/core.pyx":269
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')             # <<<<<<<<<<<<<<
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  * 			source_id = key[0]
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 250, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 269, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(1, 250, __pyx_L1_error)
+    __PYX_ERR(1, 269, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":249
+    /* "whatshap/core.pyx":268
  * 		if isinstance(key, int):
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):             # <<<<<<<<<<<<<<
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  */
   }
 
-  /* "whatshap/core.pyx":251
+  /* "whatshap/core.pyx":270
  * 		elif isinstance(key, str):
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):             # <<<<<<<<<<<<<<
  * 			source_id = key[0]
  * 			name = key[1].encode('UTF-8')
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_key); 
   __pyx_t_7 = (__pyx_t_1 != 0);
   if (__pyx_t_7) {
   } else {
     __pyx_t_2 = __pyx_t_7;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_8 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 251, __pyx_L1_error)
+  __pyx_t_8 = PyObject_Length(__pyx_v_key); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 270, __pyx_L1_error)
   __pyx_t_7 = ((__pyx_t_8 == 2) != 0);
   if (__pyx_t_7) {
   } else {
     __pyx_t_2 = __pyx_t_7;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 251, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_7 = PyInt_Check(__pyx_t_3); 
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_1 = (__pyx_t_7 != 0);
   if (__pyx_t_1) {
   } else {
     __pyx_t_2 = __pyx_t_1;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 251, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 270, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = PyUnicode_Check(__pyx_t_3); 
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_7 = (__pyx_t_1 != 0);
   __pyx_t_2 = __pyx_t_7;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_2) {
 
-    /* "whatshap/core.pyx":252
+    /* "whatshap/core.pyx":271
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  * 			source_id = key[0]             # <<<<<<<<<<<<<<
  * 			name = key[1].encode('UTF-8')
  * 			cread = self.thisptr.getByName(name, source_id)
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 252, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_key, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_source_id = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "whatshap/core.pyx":253
+    /* "whatshap/core.pyx":272
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  * 			source_id = key[0]
  * 			name = key[1].encode('UTF-8')             # <<<<<<<<<<<<<<
  * 			cread = self.thisptr.getByName(name, source_id)
  * 			if cread == NULL:
  */
-    __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_key, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 253, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_GetItemInt(__pyx_v_key, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 253, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_9, __pyx_n_s_encode); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_t_9 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
         __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_10, function);
       }
     }
     __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_kp_u_UTF_8);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 253, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 272, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 253, __pyx_L1_error)
+    __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 272, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_name = __pyx_t_4;
 
-    /* "whatshap/core.pyx":254
+    /* "whatshap/core.pyx":273
  * 			source_id = key[0]
  * 			name = key[1].encode('UTF-8')
  * 			cread = self.thisptr.getByName(name, source_id)             # <<<<<<<<<<<<<<
  * 			if cread == NULL:
  * 				raise KeyError(key)
  */
-    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_source_id); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 254, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_v_source_id); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L1_error)
     try {
       __pyx_t_6 = __pyx_v_self->thisptr->getByName(__pyx_v_name, __pyx_t_5);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 254, __pyx_L1_error)
+      __PYX_ERR(1, 273, __pyx_L1_error)
     }
     __pyx_v_cread = __pyx_t_6;
 
-    /* "whatshap/core.pyx":255
+    /* "whatshap/core.pyx":274
  * 			name = key[1].encode('UTF-8')
  * 			cread = self.thisptr.getByName(name, source_id)
  * 			if cread == NULL:             # <<<<<<<<<<<<<<
  * 				raise KeyError(key)
  * 			else:
  */
     __pyx_t_2 = ((__pyx_v_cread == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "whatshap/core.pyx":256
+      /* "whatshap/core.pyx":275
  * 			cread = self.thisptr.getByName(name, source_id)
  * 			if cread == NULL:
  * 				raise KeyError(key)             # <<<<<<<<<<<<<<
  * 			else:
  * 				read.thisptr = cread
  */
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 256, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_KeyError, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 275, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(1, 256, __pyx_L1_error)
+      __PYX_ERR(1, 275, __pyx_L1_error)
 
-      /* "whatshap/core.pyx":255
+      /* "whatshap/core.pyx":274
  * 			name = key[1].encode('UTF-8')
  * 			cread = self.thisptr.getByName(name, source_id)
  * 			if cread == NULL:             # <<<<<<<<<<<<<<
  * 				raise KeyError(key)
  * 			else:
  */
     }
 
-    /* "whatshap/core.pyx":258
+    /* "whatshap/core.pyx":277
  * 				raise KeyError(key)
  * 			else:
  * 				read.thisptr = cread             # <<<<<<<<<<<<<<
  * 		else:
  * 			assert False, 'Invalid key: {}'.format(key)
  */
     /*else*/ {
       __pyx_v_read->thisptr = __pyx_v_cread;
     }
 
-    /* "whatshap/core.pyx":251
+    /* "whatshap/core.pyx":270
  * 		elif isinstance(key, str):
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):             # <<<<<<<<<<<<<<
  * 			source_id = key[0]
  * 			name = key[1].encode('UTF-8')
  */
     goto __pyx_L4;
   }
 
-  /* "whatshap/core.pyx":260
+  /* "whatshap/core.pyx":279
  * 				read.thisptr = cread
  * 		else:
  * 			assert False, 'Invalid key: {}'.format(key)             # <<<<<<<<<<<<<<
  * 		return read
  * 
  */
   /*else*/ {
     #ifndef CYTHON_WITHOUT_ASSERTIONS
     if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!0)) {
-        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_key, __pyx_n_s_format); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 260, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Invalid_key, __pyx_n_s_format); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __pyx_t_9 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_10))) {
           __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_10);
           if (likely(__pyx_t_9)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
             __Pyx_INCREF(__pyx_t_9);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_10, function);
           }
         }
         __pyx_t_3 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_9, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_v_key);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 260, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __pyx_t_10 = PyTuple_Pack(1, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 260, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_Pack(1, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 279, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         PyErr_SetObject(PyExc_AssertionError, __pyx_t_10);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        __PYX_ERR(1, 260, __pyx_L1_error)
+        __PYX_ERR(1, 279, __pyx_L1_error)
       }
     }
     #endif
   }
   __pyx_L4:;
 
-  /* "whatshap/core.pyx":261
+  /* "whatshap/core.pyx":280
  * 		else:
  * 			assert False, 'Invalid key: {}'.format(key)
  * 		return read             # <<<<<<<<<<<<<<
  * 
  * 	def __getstate__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_read));
   __pyx_r = ((PyObject *)__pyx_v_read);
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":241
+  /* "whatshap/core.pyx":260
  * 		return self.thisptr.size()
  * 
  * 	def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError('ReadSet does not support slices')
  */
 
@@ -7868,15 +8306,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_read);
   __Pyx_XDECREF(__pyx_v_source_id);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":263
+/* "whatshap/core.pyx":282
  * 		return read
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		return ([read for read in self])
  * 
  */
 
@@ -7903,81 +8341,81 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getstate__", 0);
 
-  /* "whatshap/core.pyx":264
+  /* "whatshap/core.pyx":283
  * 
  * 	def __getstate__(self):
  * 		return ([read for read in self])             # <<<<<<<<<<<<<<
  * 
  * 	def __setstate__(self, state):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 264, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 283, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self))) {
       __pyx_t_2 = ((PyObject *)__pyx_v_self); __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 264, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 283, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 264, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 283, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 264, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 283, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 264, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 283, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 264, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 283, __pyx_L5_error)
           #else
-          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 264, __pyx_L5_error)
+          __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 283, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 264, __pyx_L5_error)
+            else __PYX_ERR(1, 283, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_read, __pyx_t_5);
       __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr3__pyx_v_read))) __PYX_ERR(1, 264, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr3__pyx_v_read))) __PYX_ERR(1, 283, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_read); __pyx_8genexpr3__pyx_v_read = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_read); __pyx_8genexpr3__pyx_v_read = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":263
+  /* "whatshap/core.pyx":282
  * 		return read
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		return ([read for read in self])
  * 
  */
 
@@ -7991,15 +8429,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_read);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":266
+/* "whatshap/core.pyx":285
  * 		return ([read for read in self])
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.ReadSet()
  * 		for read in state:
  */
 
@@ -8028,115 +8466,115 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate__", 0);
 
-  /* "whatshap/core.pyx":267
+  /* "whatshap/core.pyx":286
  * 
  * 	def __setstate__(self, state):
  * 		self.thisptr = new cpp.ReadSet()             # <<<<<<<<<<<<<<
  * 		for read in state:
  * 			self.add(read)
  */
   try {
     __pyx_t_1 = new ReadSet();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 267, __pyx_L1_error)
+    __PYX_ERR(1, 286, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":268
+  /* "whatshap/core.pyx":287
  * 	def __setstate__(self, state):
  * 		self.thisptr = new cpp.ReadSet()
  * 		for read in state:             # <<<<<<<<<<<<<<
  * 			self.add(read)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_state)) || PyTuple_CheckExact(__pyx_v_state)) {
     __pyx_t_2 = __pyx_v_state; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 268, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 287, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 268, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 268, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 287, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 268, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 287, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 268, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 287, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 268, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 287, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 268, __pyx_L1_error)
+          else __PYX_ERR(1, 287, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_read, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "whatshap/core.pyx":269
+    /* "whatshap/core.pyx":288
  * 		self.thisptr = new cpp.ReadSet()
  * 		for read in state:
  * 			self.add(read)             # <<<<<<<<<<<<<<
  * 
  * 	#def get_by_name(self, name):
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 269, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_v_read) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_v_read);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 269, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 288, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "whatshap/core.pyx":268
+    /* "whatshap/core.pyx":287
  * 	def __setstate__(self, state):
  * 		self.thisptr = new cpp.ReadSet()
  * 		for read in state:             # <<<<<<<<<<<<<<
  * 			self.add(read)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":266
+  /* "whatshap/core.pyx":285
  * 		return ([read for read in self])
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.ReadSet()
  * 		for read in state:
  */
 
@@ -8153,15 +8591,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_read);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":281
+/* "whatshap/core.pyx":300
  * 			#return read
  * 
  * 	def sort(self):             # <<<<<<<<<<<<<<
  * 		"""Sort contained reads by the position of the first variant they contain. Note that
  * 		this is not necessarily the variant with the lowest position, unless sort() has been
  */
 
@@ -8183,29 +8621,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("sort", 0);
 
-  /* "whatshap/core.pyx":285
+  /* "whatshap/core.pyx":304
  * 		this is not necessarily the variant with the lowest position, unless sort() has been
  * 		called on all contained reads. Ties are resolved by comparing the read name."""
  * 		self.thisptr.sort()             # <<<<<<<<<<<<<<
  * 
  * 	def subset(self, reads_to_select):
  */
   try {
     __pyx_v_self->thisptr->sort();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 285, __pyx_L1_error)
+    __PYX_ERR(1, 304, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":281
+  /* "whatshap/core.pyx":300
  * 			#return read
  * 
  * 	def sort(self):             # <<<<<<<<<<<<<<
  * 		"""Sort contained reads by the position of the first variant they contain. Note that
  * 		this is not necessarily the variant with the lowest position, unless sort() has been
  */
 
@@ -8217,15 +8655,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":287
+/* "whatshap/core.pyx":306
  * 		self.thisptr.sort()
  * 
  * 	def subset(self, reads_to_select):             # <<<<<<<<<<<<<<
  * 		# TODO: is there a way of avoiding to unecessarily creating/destroying a ReadSet object?
  * 		cdef cpp.IndexSet* index_set = new cpp.IndexSet()
  */
 
@@ -8256,161 +8694,161 @@
   int __pyx_t_6;
   ReadSet *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("subset", 0);
 
-  /* "whatshap/core.pyx":289
+  /* "whatshap/core.pyx":308
  * 	def subset(self, reads_to_select):
  * 		# TODO: is there a way of avoiding to unecessarily creating/destroying a ReadSet object?
  * 		cdef cpp.IndexSet* index_set = new cpp.IndexSet()             # <<<<<<<<<<<<<<
  * 		cdef int i
  * 		for i in reads_to_select:
  */
   try {
     __pyx_t_1 = new IndexSet();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 289, __pyx_L1_error)
+    __PYX_ERR(1, 308, __pyx_L1_error)
   }
   __pyx_v_index_set = __pyx_t_1;
 
-  /* "whatshap/core.pyx":291
+  /* "whatshap/core.pyx":310
  * 		cdef cpp.IndexSet* index_set = new cpp.IndexSet()
  * 		cdef int i
  * 		for i in reads_to_select:             # <<<<<<<<<<<<<<
  * 			index_set.add(i)
  * 		result = ReadSet()
  */
   if (likely(PyList_CheckExact(__pyx_v_reads_to_select)) || PyTuple_CheckExact(__pyx_v_reads_to_select)) {
     __pyx_t_2 = __pyx_v_reads_to_select; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_reads_to_select); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 291, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_reads_to_select); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 310, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 291, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 310, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 291, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 310, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 291, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 310, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 291, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(1, 310, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 291, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 310, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 291, __pyx_L1_error)
+          else __PYX_ERR(1, 310, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 291, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_5); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 310, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_i = __pyx_t_6;
 
-    /* "whatshap/core.pyx":292
+    /* "whatshap/core.pyx":311
  * 		cdef int i
  * 		for i in reads_to_select:
  * 			index_set.add(i)             # <<<<<<<<<<<<<<
  * 		result = ReadSet()
  * 		del result.thisptr
  */
     try {
       __pyx_v_index_set->add(__pyx_v_i);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 292, __pyx_L1_error)
+      __PYX_ERR(1, 311, __pyx_L1_error)
     }
 
-    /* "whatshap/core.pyx":291
+    /* "whatshap/core.pyx":310
  * 		cdef cpp.IndexSet* index_set = new cpp.IndexSet()
  * 		cdef int i
  * 		for i in reads_to_select:             # <<<<<<<<<<<<<<
  * 			index_set.add(i)
  * 		result = ReadSet()
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":293
+  /* "whatshap/core.pyx":312
  * 		for i in reads_to_select:
  * 			index_set.add(i)
  * 		result = ReadSet()             # <<<<<<<<<<<<<<
  * 		del result.thisptr
  * 		result.thisptr = self.thisptr.subset(index_set)
  */
-  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 312, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_result = ((struct __pyx_obj_8whatshap_4core_ReadSet *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":294
+  /* "whatshap/core.pyx":313
  * 			index_set.add(i)
  * 		result = ReadSet()
  * 		del result.thisptr             # <<<<<<<<<<<<<<
  * 		result.thisptr = self.thisptr.subset(index_set)
  * 		del index_set
  */
   delete __pyx_v_result->thisptr;
 
-  /* "whatshap/core.pyx":295
+  /* "whatshap/core.pyx":314
  * 		result = ReadSet()
  * 		del result.thisptr
  * 		result.thisptr = self.thisptr.subset(index_set)             # <<<<<<<<<<<<<<
  * 		del index_set
  * 		return result
  */
   try {
     __pyx_t_7 = __pyx_v_self->thisptr->subset(__pyx_v_index_set);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 295, __pyx_L1_error)
+    __PYX_ERR(1, 314, __pyx_L1_error)
   }
   __pyx_v_result->thisptr = __pyx_t_7;
 
-  /* "whatshap/core.pyx":296
+  /* "whatshap/core.pyx":315
  * 		del result.thisptr
  * 		result.thisptr = self.thisptr.subset(index_set)
  * 		del index_set             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_index_set;
 
-  /* "whatshap/core.pyx":297
+  /* "whatshap/core.pyx":316
  * 		result.thisptr = self.thisptr.subset(index_set)
  * 		del index_set
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * 	def get_positions(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":287
+  /* "whatshap/core.pyx":306
  * 		self.thisptr.sort()
  * 
  * 	def subset(self, reads_to_select):             # <<<<<<<<<<<<<<
  * 		# TODO: is there a way of avoiding to unecessarily creating/destroying a ReadSet object?
  * 		cdef cpp.IndexSet* index_set = new cpp.IndexSet()
  */
 
@@ -8423,15 +8861,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":299
+/* "whatshap/core.pyx":318
  * 		return result
  * 
  * 	def get_positions(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[unsigned int]* v = self.thisptr.get_positions()
  * 		result = list(v[0])
  */
 
@@ -8456,60 +8894,60 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_positions", 0);
 
-  /* "whatshap/core.pyx":300
+  /* "whatshap/core.pyx":319
  * 
  * 	def get_positions(self):
  * 		cdef vector[unsigned int]* v = self.thisptr.get_positions()             # <<<<<<<<<<<<<<
  * 		result = list(v[0])
  * 		del v
  */
   __pyx_v_v = __pyx_v_self->thisptr->get_positions();
 
-  /* "whatshap/core.pyx":301
+  /* "whatshap/core.pyx":320
  * 	def get_positions(self):
  * 		cdef vector[unsigned int]* v = self.thisptr.get_positions()
  * 		result = list(v[0])             # <<<<<<<<<<<<<<
  * 		del v
  * 		return result
  */
-  __pyx_t_1 = __pyx_convert_vector_to_py_unsigned_int((__pyx_v_v[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_unsigned_int((__pyx_v_v[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 301, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":302
+  /* "whatshap/core.pyx":321
  * 		cdef vector[unsigned int]* v = self.thisptr.get_positions()
  * 		result = list(v[0])
  * 		del v             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_v;
 
-  /* "whatshap/core.pyx":303
+  /* "whatshap/core.pyx":322
  * 		result = list(v[0])
  * 		del v
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":299
+  /* "whatshap/core.pyx":318
  * 		return result
  * 
  * 	def get_positions(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[unsigned int]* v = self.thisptr.get_positions()
  * 		result = list(v[0])
  */
 
@@ -8635,15 +9073,15 @@
   __Pyx_AddTraceback("whatshap.core.ReadSet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":307
+/* "whatshap/core.pyx":326
  * 
  * cdef class PedigreeDPTable:
  * 	def __cinit__(self, ReadSet readset, recombcost, Pedigree pedigree, bool distrust_genotypes = False, positions = None):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -8687,21 +9125,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_readset)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_recombcost)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(1, 307, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(1, 326, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pedigree)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(1, 307, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(1, 326, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_distrust_genotypes);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -8709,15 +9147,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_positions);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 307, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 326, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -8728,30 +9166,30 @@
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_readset = ((struct __pyx_obj_8whatshap_4core_ReadSet *)values[0]);
     __pyx_v_recombcost = values[1];
     __pyx_v_pedigree = ((struct __pyx_obj_8whatshap_4core_Pedigree *)values[2]);
     if (values[3]) {
-      __pyx_v_distrust_genotypes = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_distrust_genotypes == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 307, __pyx_L3_error)
+      __pyx_v_distrust_genotypes = __Pyx_PyObject_IsTrue(values[3]); if (unlikely((__pyx_v_distrust_genotypes == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 326, __pyx_L3_error)
     } else {
       __pyx_v_distrust_genotypes = ((bool)0);
     }
     __pyx_v_positions = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 307, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 326, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.PedigreeDPTable.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 307, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 307, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 326, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 326, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_15PedigreeDPTable___cinit__(((struct __pyx_obj_8whatshap_4core_PedigreeDPTable *)__pyx_v_self), __pyx_v_readset, __pyx_v_recombcost, __pyx_v_pedigree, __pyx_v_distrust_genotypes, __pyx_v_positions);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -8775,162 +9213,162 @@
   std::vector<unsigned int>  __pyx_t_9;
   PedigreeDPTable *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":312
+  /* "whatshap/core.pyx":331
  * 		in the read set must also be sorted (by position of their left-most variant).
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL             # <<<<<<<<<<<<<<
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  */
   __pyx_v_c_positions = NULL;
 
-  /* "whatshap/core.pyx":313
+  /* "whatshap/core.pyx":332
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   __pyx_t_1 = (__pyx_v_positions != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "whatshap/core.pyx":314
+    /* "whatshap/core.pyx":333
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()             # <<<<<<<<<<<<<<
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  */
     try {
       __pyx_t_3 = new std::vector<unsigned int> ();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 314, __pyx_L1_error)
+      __PYX_ERR(1, 333, __pyx_L1_error)
     }
     __pyx_v_c_positions = __pyx_t_3;
 
-    /* "whatshap/core.pyx":315
+    /* "whatshap/core.pyx":334
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedigreeDPTable(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions)
  */
     if (likely(PyList_CheckExact(__pyx_v_positions)) || PyTuple_CheckExact(__pyx_v_positions)) {
       __pyx_t_4 = __pyx_v_positions; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 315, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 334, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 315, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 334, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 315, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 334, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 315, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 334, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 315, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 334, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 315, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 334, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 315, __pyx_L1_error)
+            else __PYX_ERR(1, 334, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "whatshap/core.pyx":316
+      /* "whatshap/core.pyx":335
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  * 				c_positions.push_back(pos)             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.PedigreeDPTable(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions)
  * 		self.pedigree = pedigree
  */
-      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 316, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 335, __pyx_L1_error)
       try {
         __pyx_v_c_positions->push_back(__pyx_t_8);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 316, __pyx_L1_error)
+        __PYX_ERR(1, 335, __pyx_L1_error)
       }
 
-      /* "whatshap/core.pyx":315
+      /* "whatshap/core.pyx":334
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedigreeDPTable(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions)
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "whatshap/core.pyx":313
+    /* "whatshap/core.pyx":332
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   }
 
-  /* "whatshap/core.pyx":317
+  /* "whatshap/core.pyx":336
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedigreeDPTable(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions)             # <<<<<<<<<<<<<<
  * 		self.pedigree = pedigree
  * 
  */
-  __pyx_t_9 = __pyx_convert_vector_from_py_unsigned_int(__pyx_v_recombcost); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 317, __pyx_L1_error)
+  __pyx_t_9 = __pyx_convert_vector_from_py_unsigned_int(__pyx_v_recombcost); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 336, __pyx_L1_error)
   try {
     __pyx_t_10 = new PedigreeDPTable(__pyx_v_readset->thisptr, __pyx_t_9, __pyx_v_pedigree->thisptr, __pyx_v_distrust_genotypes, __pyx_v_c_positions);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 317, __pyx_L1_error)
+    __PYX_ERR(1, 336, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_10;
 
-  /* "whatshap/core.pyx":318
+  /* "whatshap/core.pyx":337
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedigreeDPTable(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions)
  * 		self.pedigree = pedigree             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GOTREF(__pyx_v_self->pedigree);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->pedigree));
   __pyx_v_self->pedigree = __pyx_v_pedigree;
 
-  /* "whatshap/core.pyx":307
+  /* "whatshap/core.pyx":326
  * 
  * cdef class PedigreeDPTable:
  * 	def __cinit__(self, ReadSet readset, recombcost, Pedigree pedigree, bool distrust_genotypes = False, positions = None):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -8944,15 +9382,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":320
+/* "whatshap/core.pyx":339
  * 		self.pedigree = pedigree
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -8967,36 +9405,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_15PedigreeDPTable_2__dealloc__(struct __pyx_obj_8whatshap_4core_PedigreeDPTable *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":321
+  /* "whatshap/core.pyx":340
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def get_super_reads(self):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":320
+  /* "whatshap/core.pyx":339
  * 		self.pedigree = pedigree
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":323
+/* "whatshap/core.pyx":342
  * 		del self.thisptr
  * 
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		"""Obtain optimal-score haplotypes. Returns a triple (mother, father, child)
  * 		IMPORTANT: The ReadSet given at construction time must not have been altered.
  */
 
@@ -9035,203 +9473,203 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_super_reads", 0);
 
-  /* "whatshap/core.pyx":330
+  /* "whatshap/core.pyx":349
  * 		TODO: Change that.
  * 		"""
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()             # <<<<<<<<<<<<<<
  * 
  * 		for i in range(len(self.pedigree)):
  */
   try {
     __pyx_t_1 = new std::vector<ReadSet *> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 330, __pyx_L1_error)
+    __PYX_ERR(1, 349, __pyx_L1_error)
   }
   __pyx_v_read_sets = __pyx_t_1;
 
-  /* "whatshap/core.pyx":332
+  /* "whatshap/core.pyx":351
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  * 
  * 		for i in range(len(self.pedigree)):             # <<<<<<<<<<<<<<
  * 			read_sets.push_back(new cpp.ReadSet())
  * 		transmission_vector_ptr = new vector[unsigned int]()
  */
   __pyx_t_2 = ((PyObject *)__pyx_v_self->pedigree);
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 332, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 351, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "whatshap/core.pyx":333
+    /* "whatshap/core.pyx":352
  * 
  * 		for i in range(len(self.pedigree)):
  * 			read_sets.push_back(new cpp.ReadSet())             # <<<<<<<<<<<<<<
  * 		transmission_vector_ptr = new vector[unsigned int]()
  * 		self.thisptr.get_super_reads(read_sets, transmission_vector_ptr)
  */
     try {
       __pyx_t_6 = new ReadSet();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 333, __pyx_L1_error)
+      __PYX_ERR(1, 352, __pyx_L1_error)
     }
     try {
       __pyx_v_read_sets->push_back(__pyx_t_6);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 333, __pyx_L1_error)
+      __PYX_ERR(1, 352, __pyx_L1_error)
     }
   }
 
-  /* "whatshap/core.pyx":334
+  /* "whatshap/core.pyx":353
  * 		for i in range(len(self.pedigree)):
  * 			read_sets.push_back(new cpp.ReadSet())
  * 		transmission_vector_ptr = new vector[unsigned int]()             # <<<<<<<<<<<<<<
  * 		self.thisptr.get_super_reads(read_sets, transmission_vector_ptr)
  * 
  */
   try {
     __pyx_t_7 = new std::vector<unsigned int> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 334, __pyx_L1_error)
+    __PYX_ERR(1, 353, __pyx_L1_error)
   }
   __pyx_v_transmission_vector_ptr = __pyx_t_7;
 
-  /* "whatshap/core.pyx":335
+  /* "whatshap/core.pyx":354
  * 			read_sets.push_back(new cpp.ReadSet())
  * 		transmission_vector_ptr = new vector[unsigned int]()
  * 		self.thisptr.get_super_reads(read_sets, transmission_vector_ptr)             # <<<<<<<<<<<<<<
  * 
  * 		results = []
  */
   try {
     __pyx_v_self->thisptr->get_super_reads(__pyx_v_read_sets, __pyx_v_transmission_vector_ptr);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 335, __pyx_L1_error)
+    __PYX_ERR(1, 354, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":337
+  /* "whatshap/core.pyx":356
  * 		self.thisptr.get_super_reads(read_sets, transmission_vector_ptr)
  * 
  * 		results = []             # <<<<<<<<<<<<<<
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 337, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 356, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_results = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":338
+  /* "whatshap/core.pyx":357
  * 
  * 		results = []
  * 		for i in range(read_sets.size()):             # <<<<<<<<<<<<<<
  * 			rs = ReadSet()
  * 			del rs.thisptr
  */
   __pyx_t_5 = __pyx_v_read_sets->size();
   __pyx_t_8 = __pyx_t_5;
   for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
     __pyx_v_i = __pyx_t_9;
 
-    /* "whatshap/core.pyx":339
+    /* "whatshap/core.pyx":358
  * 		results = []
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()             # <<<<<<<<<<<<<<
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]
  */
-    __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 339, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 358, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_rs, ((struct __pyx_obj_8whatshap_4core_ReadSet *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "whatshap/core.pyx":340
+    /* "whatshap/core.pyx":359
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()
  * 			del rs.thisptr             # <<<<<<<<<<<<<<
  * 			rs.thisptr = deref(read_sets)[i]
  * 			results.append(rs)
  */
     delete __pyx_v_rs->thisptr;
 
-    /* "whatshap/core.pyx":341
+    /* "whatshap/core.pyx":360
  * 			rs = ReadSet()
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]             # <<<<<<<<<<<<<<
  * 			results.append(rs)
  * 
  */
     __pyx_v_rs->thisptr = ((*__pyx_v_read_sets)[__pyx_v_i]);
 
-    /* "whatshap/core.pyx":342
+    /* "whatshap/core.pyx":361
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]
  * 			results.append(rs)             # <<<<<<<<<<<<<<
  * 
  * 		python_transmission_vector = list(transmission_vector_ptr[0])
  */
-    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(1, 342, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(1, 361, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":344
+  /* "whatshap/core.pyx":363
  * 			results.append(rs)
  * 
  * 		python_transmission_vector = list(transmission_vector_ptr[0])             # <<<<<<<<<<<<<<
  * 		del transmission_vector_ptr
  * 		return results, python_transmission_vector
  */
-  __pyx_t_2 = __pyx_convert_vector_to_py_unsigned_int((__pyx_v_transmission_vector_ptr[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 344, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_to_py_unsigned_int((__pyx_v_transmission_vector_ptr[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_11 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 344, __pyx_L1_error)
+  __pyx_t_11 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_python_transmission_vector = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "whatshap/core.pyx":345
+  /* "whatshap/core.pyx":364
  * 
  * 		python_transmission_vector = list(transmission_vector_ptr[0])
  * 		del transmission_vector_ptr             # <<<<<<<<<<<<<<
  * 		return results, python_transmission_vector
  * 
  */
   delete __pyx_v_transmission_vector_ptr;
 
-  /* "whatshap/core.pyx":346
+  /* "whatshap/core.pyx":365
  * 		python_transmission_vector = list(transmission_vector_ptr[0])
  * 		del transmission_vector_ptr
  * 		return results, python_transmission_vector             # <<<<<<<<<<<<<<
  * 
  * 	def get_optimal_cost(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 346, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(1, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_INCREF(__pyx_v_results);
   __Pyx_GIVEREF(__pyx_v_results);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_results);
   __Pyx_INCREF(__pyx_v_python_transmission_vector);
   __Pyx_GIVEREF(__pyx_v_python_transmission_vector);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_v_python_transmission_vector);
   __pyx_r = __pyx_t_11;
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":323
+  /* "whatshap/core.pyx":342
  * 		del self.thisptr
  * 
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		"""Obtain optimal-score haplotypes. Returns a triple (mother, father, child)
  * 		IMPORTANT: The ReadSet given at construction time must not have been altered.
  */
 
@@ -9246,15 +9684,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_rs);
   __Pyx_XDECREF(__pyx_v_python_transmission_vector);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":348
+/* "whatshap/core.pyx":367
  * 		return results, python_transmission_vector
  * 
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.get_optimal_score()
  */
 
@@ -9278,35 +9716,35 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_cost", 0);
 
-  /* "whatshap/core.pyx":350
+  /* "whatshap/core.pyx":369
  * 	def get_optimal_cost(self):
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.get_optimal_score()             # <<<<<<<<<<<<<<
  * 
  * 	def get_optimal_partitioning(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_optimal_score();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 350, __pyx_L1_error)
+    __PYX_ERR(1, 369, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 350, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":348
+  /* "whatshap/core.pyx":367
  * 		return results, python_transmission_vector
  * 
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.get_optimal_score()
  */
 
@@ -9317,15 +9755,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":352
+/* "whatshap/core.pyx":371
  * 		return self.thisptr.get_optimal_score()
  * 
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  */
 
@@ -9355,32 +9793,32 @@
   bool __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_partitioning", 0);
 
-  /* "whatshap/core.pyx":355
+  /* "whatshap/core.pyx":374
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()             # <<<<<<<<<<<<<<
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p
  */
   __pyx_v_p = __pyx_v_self->thisptr->get_optimal_partitioning();
 
-  /* "whatshap/core.pyx":356
+  /* "whatshap/core.pyx":375
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = [0 if x else 1 for x in p[0]]             # <<<<<<<<<<<<<<
  * 		del p
  * 		return result
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 356, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 375, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = &(__pyx_v_p[0]);
     __pyx_t_2 = __pyx_t_3->begin();
     for (;;) {
       if (!(__pyx_t_2 != __pyx_t_3->end())) break;
       __pyx_t_4 = *__pyx_t_2;
       ++__pyx_t_2;
@@ -9388,43 +9826,43 @@
       if ((__pyx_8genexpr4__pyx_v_x != 0)) {
         __Pyx_INCREF(__pyx_int_0);
         __pyx_t_5 = __pyx_int_0;
       } else {
         __Pyx_INCREF(__pyx_int_1);
         __pyx_t_5 = __pyx_int_1;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 356, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 375, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":357
+  /* "whatshap/core.pyx":376
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_p;
 
-  /* "whatshap/core.pyx":358
+  /* "whatshap/core.pyx":377
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":352
+  /* "whatshap/core.pyx":371
  * 		return self.thisptr.get_optimal_score()
  * 
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  */
 
@@ -9550,15 +9988,15 @@
   __Pyx_AddTraceback("whatshap.core.PedigreeDPTable.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":362
+/* "whatshap/core.pyx":381
  * 
  * cdef class Pedigree:
  * 	def __cinit__(self, numeric_sample_ids):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Pedigree()
  * 		self.numeric_sample_ids = numeric_sample_ids
  */
 
@@ -9587,26 +10025,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_numeric_sample_ids)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 362, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 381, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_numeric_sample_ids = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 362, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 381, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Pedigree.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Pedigree___cinit__(((struct __pyx_obj_8whatshap_4core_Pedigree *)__pyx_v_self), __pyx_v_numeric_sample_ids);
 
@@ -9621,46 +10059,46 @@
   Pedigree *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":363
+  /* "whatshap/core.pyx":382
  * cdef class Pedigree:
  * 	def __cinit__(self, numeric_sample_ids):
  * 		self.thisptr = new cpp.Pedigree()             # <<<<<<<<<<<<<<
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  */
   try {
     __pyx_t_1 = new Pedigree();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 363, __pyx_L1_error)
+    __PYX_ERR(1, 382, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":364
+  /* "whatshap/core.pyx":383
  * 	def __cinit__(self, numeric_sample_ids):
  * 		self.thisptr = new cpp.Pedigree()
  * 		self.numeric_sample_ids = numeric_sample_ids             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
-  if (!(likely(((__pyx_v_numeric_sample_ids) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_numeric_sample_ids, __pyx_ptype_8whatshap_4core_NumericSampleIds))))) __PYX_ERR(1, 364, __pyx_L1_error)
+  if (!(likely(((__pyx_v_numeric_sample_ids) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_numeric_sample_ids, __pyx_ptype_8whatshap_4core_NumericSampleIds))))) __PYX_ERR(1, 383, __pyx_L1_error)
   __pyx_t_2 = __pyx_v_numeric_sample_ids;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->numeric_sample_ids);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->numeric_sample_ids));
   __pyx_v_self->numeric_sample_ids = ((struct __pyx_obj_8whatshap_4core_NumericSampleIds *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":362
+  /* "whatshap/core.pyx":381
  * 
  * cdef class Pedigree:
  * 	def __cinit__(self, numeric_sample_ids):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Pedigree()
  * 		self.numeric_sample_ids = numeric_sample_ids
  */
 
@@ -9672,15 +10110,15 @@
   __Pyx_AddTraceback("whatshap.core.Pedigree.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":366
+/* "whatshap/core.pyx":385
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -9695,36 +10133,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_8Pedigree_2__dealloc__(struct __pyx_obj_8whatshap_4core_Pedigree *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":367
+  /* "whatshap/core.pyx":386
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def add_individual(self, id, genotypes, genotype_likelihoods=None):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":366
+  /* "whatshap/core.pyx":385
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":369
+/* "whatshap/core.pyx":388
  * 		del self.thisptr
  * 
  * 	def add_individual(self, id, genotypes, genotype_likelihoods=None):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.Genotype*] gt_vector
  * 		for gt in genotypes:
  */
 
@@ -9762,25 +10200,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_genotypes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_individual", 0, 2, 3, 1); __PYX_ERR(1, 369, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_individual", 0, 2, 3, 1); __PYX_ERR(1, 388, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_genotype_likelihoods);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_individual") < 0)) __PYX_ERR(1, 369, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_individual") < 0)) __PYX_ERR(1, 388, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -9790,15 +10228,15 @@
     }
     __pyx_v_id = values[0];
     __pyx_v_genotypes = values[1];
     __pyx_v_genotype_likelihoods = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_individual", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 369, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_individual", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 388, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Pedigree.add_individual", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Pedigree_4add_individual(((struct __pyx_obj_8whatshap_4core_Pedigree *)__pyx_v_self), __pyx_v_id, __pyx_v_genotypes, __pyx_v_genotype_likelihoods);
 
@@ -9825,327 +10263,327 @@
   PhredGenotypeLikelihoods *__pyx_t_8;
   unsigned int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_individual", 0);
 
-  /* "whatshap/core.pyx":371
+  /* "whatshap/core.pyx":390
  * 	def add_individual(self, id, genotypes, genotype_likelihoods=None):
  * 		cdef vector[cpp.Genotype*] gt_vector
  * 		for gt in genotypes:             # <<<<<<<<<<<<<<
  * 			gt_vector.push_back(new cpp.Genotype((<Genotype?>gt).thisptr[0]))
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  */
   if (likely(PyList_CheckExact(__pyx_v_genotypes)) || PyTuple_CheckExact(__pyx_v_genotypes)) {
     __pyx_t_1 = __pyx_v_genotypes; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 371, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 390, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 371, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 390, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 371, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 390, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 371, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 390, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 371, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 390, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 371, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 390, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 371, __pyx_L1_error)
+          else __PYX_ERR(1, 390, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_gt, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "whatshap/core.pyx":372
+    /* "whatshap/core.pyx":391
  * 		cdef vector[cpp.Genotype*] gt_vector
  * 		for gt in genotypes:
  * 			gt_vector.push_back(new cpp.Genotype((<Genotype?>gt).thisptr[0]))             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  * 		if genotype_likelihoods:
  */
-    if (!(likely(__Pyx_TypeTest(__pyx_v_gt, __pyx_ptype_8whatshap_4core_Genotype)))) __PYX_ERR(1, 372, __pyx_L1_error)
+    if (!(likely(__Pyx_TypeTest(__pyx_v_gt, __pyx_ptype_8whatshap_4core_Genotype)))) __PYX_ERR(1, 391, __pyx_L1_error)
     try {
       __pyx_t_5 = new Genotype((((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_gt)->thisptr[0]));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 372, __pyx_L1_error)
+      __PYX_ERR(1, 391, __pyx_L1_error)
     }
     try {
       __pyx_v_gt_vector.push_back(__pyx_t_5);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 372, __pyx_L1_error)
+      __PYX_ERR(1, 391, __pyx_L1_error)
     }
 
-    /* "whatshap/core.pyx":371
+    /* "whatshap/core.pyx":390
  * 	def add_individual(self, id, genotypes, genotype_likelihoods=None):
  * 		cdef vector[cpp.Genotype*] gt_vector
  * 		for gt in genotypes:             # <<<<<<<<<<<<<<
  * 			gt_vector.push_back(new cpp.Genotype((<Genotype?>gt).thisptr[0]))
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":374
+  /* "whatshap/core.pyx":393
  * 			gt_vector.push_back(new cpp.Genotype((<Genotype?>gt).thisptr[0]))
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  * 		if genotype_likelihoods:             # <<<<<<<<<<<<<<
  * 			for gl in genotype_likelihoods:
  * 				if gl is None:
  */
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_genotype_likelihoods); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 374, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_genotype_likelihoods); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(1, 393, __pyx_L1_error)
   if (__pyx_t_6) {
 
-    /* "whatshap/core.pyx":375
+    /* "whatshap/core.pyx":394
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  * 		if genotype_likelihoods:
  * 			for gl in genotype_likelihoods:             # <<<<<<<<<<<<<<
  * 				if gl is None:
  * 					gl_vector.push_back(NULL)
  */
     if (likely(PyList_CheckExact(__pyx_v_genotype_likelihoods)) || PyTuple_CheckExact(__pyx_v_genotype_likelihoods)) {
       __pyx_t_1 = __pyx_v_genotype_likelihoods; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
       __pyx_t_3 = NULL;
     } else {
-      __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotype_likelihoods); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 375, __pyx_L1_error)
+      __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotype_likelihoods); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 394, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 375, __pyx_L1_error)
+      __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 394, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_3)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 375, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 394, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 375, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 394, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 375, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 394, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 375, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 394, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_3(__pyx_t_1);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 375, __pyx_L1_error)
+            else __PYX_ERR(1, 394, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_gl, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "whatshap/core.pyx":376
+      /* "whatshap/core.pyx":395
  * 		if genotype_likelihoods:
  * 			for gl in genotype_likelihoods:
  * 				if gl is None:             # <<<<<<<<<<<<<<
  * 					gl_vector.push_back(NULL)
  * 				else:
  */
       __pyx_t_6 = (__pyx_v_gl == Py_None);
       __pyx_t_7 = (__pyx_t_6 != 0);
       if (__pyx_t_7) {
 
-        /* "whatshap/core.pyx":377
+        /* "whatshap/core.pyx":396
  * 			for gl in genotype_likelihoods:
  * 				if gl is None:
  * 					gl_vector.push_back(NULL)             # <<<<<<<<<<<<<<
  * 				else:
  * 					gl_vector.push_back(new cpp.PhredGenotypeLikelihoods((<PhredGenotypeLikelihoods?>gl).thisptr[0]) )
  */
         try {
           __pyx_v_gl_vector.push_back(NULL);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(1, 377, __pyx_L1_error)
+          __PYX_ERR(1, 396, __pyx_L1_error)
         }
 
-        /* "whatshap/core.pyx":376
+        /* "whatshap/core.pyx":395
  * 		if genotype_likelihoods:
  * 			for gl in genotype_likelihoods:
  * 				if gl is None:             # <<<<<<<<<<<<<<
  * 					gl_vector.push_back(NULL)
  * 				else:
  */
         goto __pyx_L8;
       }
 
-      /* "whatshap/core.pyx":379
+      /* "whatshap/core.pyx":398
  * 					gl_vector.push_back(NULL)
  * 				else:
  * 					gl_vector.push_back(new cpp.PhredGenotypeLikelihoods((<PhredGenotypeLikelihoods?>gl).thisptr[0]) )             # <<<<<<<<<<<<<<
  * 		else:
  * 			for _ in genotypes:
  */
       /*else*/ {
-        if (!(likely(__Pyx_TypeTest(__pyx_v_gl, __pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods)))) __PYX_ERR(1, 379, __pyx_L1_error)
+        if (!(likely(__Pyx_TypeTest(__pyx_v_gl, __pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods)))) __PYX_ERR(1, 398, __pyx_L1_error)
         try {
           __pyx_t_8 = new PhredGenotypeLikelihoods((((struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *)__pyx_v_gl)->thisptr[0]));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(1, 379, __pyx_L1_error)
+          __PYX_ERR(1, 398, __pyx_L1_error)
         }
         try {
           __pyx_v_gl_vector.push_back(__pyx_t_8);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(1, 379, __pyx_L1_error)
+          __PYX_ERR(1, 398, __pyx_L1_error)
         }
       }
       __pyx_L8:;
 
-      /* "whatshap/core.pyx":375
+      /* "whatshap/core.pyx":394
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  * 		if genotype_likelihoods:
  * 			for gl in genotype_likelihoods:             # <<<<<<<<<<<<<<
  * 				if gl is None:
  * 					gl_vector.push_back(NULL)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "whatshap/core.pyx":374
+    /* "whatshap/core.pyx":393
  * 			gt_vector.push_back(new cpp.Genotype((<Genotype?>gt).thisptr[0]))
  * 		cdef vector[cpp.PhredGenotypeLikelihoods*] gl_vector
  * 		if genotype_likelihoods:             # <<<<<<<<<<<<<<
  * 			for gl in genotype_likelihoods:
  * 				if gl is None:
  */
     goto __pyx_L5;
   }
 
-  /* "whatshap/core.pyx":381
+  /* "whatshap/core.pyx":400
  * 					gl_vector.push_back(new cpp.PhredGenotypeLikelihoods((<PhredGenotypeLikelihoods?>gl).thisptr[0]) )
  * 		else:
  * 			for _ in genotypes:             # <<<<<<<<<<<<<<
  * 				gl_vector.push_back(NULL)
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)
  */
   /*else*/ {
     if (likely(PyList_CheckExact(__pyx_v_genotypes)) || PyTuple_CheckExact(__pyx_v_genotypes)) {
       __pyx_t_1 = __pyx_v_genotypes; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
       __pyx_t_3 = NULL;
     } else {
-      __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 381, __pyx_L1_error)
+      __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_genotypes); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 400, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 381, __pyx_L1_error)
+      __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 400, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_3)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 381, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 400, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 381, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 381, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 400, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 381, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 400, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_3(__pyx_t_1);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 381, __pyx_L1_error)
+            else __PYX_ERR(1, 400, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v__, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "whatshap/core.pyx":382
+      /* "whatshap/core.pyx":401
  * 		else:
  * 			for _ in genotypes:
  * 				gl_vector.push_back(NULL)             # <<<<<<<<<<<<<<
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)
  * 
  */
       try {
         __pyx_v_gl_vector.push_back(NULL);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 382, __pyx_L1_error)
+        __PYX_ERR(1, 401, __pyx_L1_error)
       }
 
-      /* "whatshap/core.pyx":381
+      /* "whatshap/core.pyx":400
  * 					gl_vector.push_back(new cpp.PhredGenotypeLikelihoods((<PhredGenotypeLikelihoods?>gl).thisptr[0]) )
  * 		else:
  * 			for _ in genotypes:             # <<<<<<<<<<<<<<
  * 				gl_vector.push_back(NULL)
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L5:;
 
-  /* "whatshap/core.pyx":383
+  /* "whatshap/core.pyx":402
  * 			for _ in genotypes:
  * 				gl_vector.push_back(NULL)
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)             # <<<<<<<<<<<<<<
  * 
  * 	def add_relationship(self, father_id, mother_id, child_id):
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 383, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 383, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_9 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_v_self->thisptr->addIndividual(__pyx_t_9, __pyx_v_gt_vector, __pyx_v_gl_vector);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 383, __pyx_L1_error)
+    __PYX_ERR(1, 402, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":369
+  /* "whatshap/core.pyx":388
  * 		del self.thisptr
  * 
  * 	def add_individual(self, id, genotypes, genotype_likelihoods=None):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.Genotype*] gt_vector
  * 		for gt in genotypes:
  */
 
@@ -10162,15 +10600,15 @@
   __Pyx_XDECREF(__pyx_v_gl);
   __Pyx_XDECREF(__pyx_v__);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":385
+/* "whatshap/core.pyx":404
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)
  * 
  * 	def add_relationship(self, father_id, mother_id, child_id):             # <<<<<<<<<<<<<<
  * 		self.thisptr.addRelationship(self.numeric_sample_ids[father_id], self.numeric_sample_ids[mother_id], self.numeric_sample_ids[child_id])
  * 
  */
 
@@ -10207,40 +10645,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_father_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mother_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, 1); __PYX_ERR(1, 385, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, 1); __PYX_ERR(1, 404, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_child_id)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, 2); __PYX_ERR(1, 385, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, 2); __PYX_ERR(1, 404, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_relationship") < 0)) __PYX_ERR(1, 385, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_relationship") < 0)) __PYX_ERR(1, 404, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_father_id = values[0];
     __pyx_v_mother_id = values[1];
     __pyx_v_child_id = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 385, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_relationship", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 404, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Pedigree.add_relationship", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Pedigree_6add_relationship(((struct __pyx_obj_8whatshap_4core_Pedigree *)__pyx_v_self), __pyx_v_father_id, __pyx_v_mother_id, __pyx_v_child_id);
 
@@ -10257,41 +10695,41 @@
   unsigned int __pyx_t_3;
   unsigned int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_relationship", 0);
 
-  /* "whatshap/core.pyx":386
+  /* "whatshap/core.pyx":405
  * 
  * 	def add_relationship(self, father_id, mother_id, child_id):
  * 		self.thisptr.addRelationship(self.numeric_sample_ids[father_id], self.numeric_sample_ids[mother_id], self.numeric_sample_ids[child_id])             # <<<<<<<<<<<<<<
  * 
  * 	property variant_count:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_father_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_father_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_mother_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_mother_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_child_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_child_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 386, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_4 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_v_self->thisptr->addRelationship(__pyx_t_2, __pyx_t_3, __pyx_t_4);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 386, __pyx_L1_error)
+    __PYX_ERR(1, 405, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":385
+  /* "whatshap/core.pyx":404
  * 		self.thisptr.addIndividual(self.numeric_sample_ids[id], gt_vector, gl_vector)
  * 
  * 	def add_relationship(self, father_id, mother_id, child_id):             # <<<<<<<<<<<<<<
  * 		self.thisptr.addRelationship(self.numeric_sample_ids[father_id], self.numeric_sample_ids[mother_id], self.numeric_sample_ids[child_id])
  * 
  */
 
@@ -10304,15 +10742,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":390
+/* "whatshap/core.pyx":409
  * 	property variant_count:
  * 		"""Number of variants stored for each individual."""
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			return self.thisptr.get_variant_count()
  * 
  */
 
@@ -10335,35 +10773,35 @@
   unsigned int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "whatshap/core.pyx":391
+  /* "whatshap/core.pyx":410
  * 		"""Number of variants stored for each individual."""
  * 		def __get__(self):
  * 			return self.thisptr.get_variant_count()             # <<<<<<<<<<<<<<
  * 
  * 	def genotype(self, sample_id, unsigned int variant_index):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_variant_count();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 391, __pyx_L1_error)
+    __PYX_ERR(1, 410, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 391, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":390
+  /* "whatshap/core.pyx":409
  * 	property variant_count:
  * 		"""Number of variants stored for each individual."""
  * 		def __get__(self):             # <<<<<<<<<<<<<<
  * 			return self.thisptr.get_variant_count()
  * 
  */
 
@@ -10374,15 +10812,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":393
+/* "whatshap/core.pyx":412
  * 			return self.thisptr.get_variant_count()
  * 
  * 	def genotype(self, sample_id, unsigned int variant_index):             # <<<<<<<<<<<<<<
  * 		cdef const cpp.Genotype* gt = self.thisptr.get_genotype_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		return Genotype(gt[0].as_vector())
  */
 
@@ -10416,32 +10854,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_variant_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("genotype", 1, 2, 2, 1); __PYX_ERR(1, 393, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("genotype", 1, 2, 2, 1); __PYX_ERR(1, 412, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "genotype") < 0)) __PYX_ERR(1, 393, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "genotype") < 0)) __PYX_ERR(1, 412, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_sample_id = values[0];
-    __pyx_v_variant_index = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_variant_index == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
+    __pyx_v_variant_index = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_variant_index == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 412, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("genotype", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 393, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("genotype", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 412, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Pedigree.genotype", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Pedigree_8genotype(((struct __pyx_obj_8whatshap_4core_Pedigree *)__pyx_v_self), __pyx_v_sample_id, __pyx_v_variant_index);
 
@@ -10460,57 +10898,57 @@
   std::vector<uint32_t>  __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genotype", 0);
 
-  /* "whatshap/core.pyx":394
+  /* "whatshap/core.pyx":413
  * 
  * 	def genotype(self, sample_id, unsigned int variant_index):
  * 		cdef const cpp.Genotype* gt = self.thisptr.get_genotype_by_id(self.numeric_sample_ids[sample_id], variant_index)             # <<<<<<<<<<<<<<
  * 		return Genotype(gt[0].as_vector())
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 394, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 413, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 413, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_genotype_by_id(__pyx_t_2, __pyx_v_variant_index);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 394, __pyx_L1_error)
+    __PYX_ERR(1, 413, __pyx_L1_error)
   }
   __pyx_v_gt = __pyx_t_3;
 
-  /* "whatshap/core.pyx":395
+  /* "whatshap/core.pyx":414
  * 	def genotype(self, sample_id, unsigned int variant_index):
  * 		cdef const cpp.Genotype* gt = self.thisptr.get_genotype_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		return Genotype(gt[0].as_vector())             # <<<<<<<<<<<<<<
  * 
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_4 = (__pyx_v_gt[0]).as_vector();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 395, __pyx_L1_error)
+    __PYX_ERR(1, 414, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 395, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 395, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":393
+  /* "whatshap/core.pyx":412
  * 			return self.thisptr.get_variant_count()
  * 
  * 	def genotype(self, sample_id, unsigned int variant_index):             # <<<<<<<<<<<<<<
  * 		cdef const cpp.Genotype* gt = self.thisptr.get_genotype_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		return Genotype(gt[0].as_vector())
  */
 
@@ -10522,15 +10960,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":397
+/* "whatshap/core.pyx":416
  * 		return Genotype(gt[0].as_vector())
  * 
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):             # <<<<<<<<<<<<<<
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		if gl == NULL:
  */
 
@@ -10564,32 +11002,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_variant_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("genotype_likelihoods", 1, 2, 2, 1); __PYX_ERR(1, 397, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("genotype_likelihoods", 1, 2, 2, 1); __PYX_ERR(1, 416, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "genotype_likelihoods") < 0)) __PYX_ERR(1, 397, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "genotype_likelihoods") < 0)) __PYX_ERR(1, 416, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_sample_id = values[0];
-    __pyx_v_variant_index = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_variant_index == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 397, __pyx_L3_error)
+    __pyx_v_variant_index = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_variant_index == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 416, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("genotype_likelihoods", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 397, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("genotype_likelihoods", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 416, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Pedigree.genotype_likelihoods", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Pedigree_10genotype_likelihoods(((struct __pyx_obj_8whatshap_4core_Pedigree *)__pyx_v_self), __pyx_v_sample_id, __pyx_v_variant_index);
 
@@ -10611,116 +11049,116 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genotype_likelihoods", 0);
 
-  /* "whatshap/core.pyx":398
+  /* "whatshap/core.pyx":417
  * 
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)             # <<<<<<<<<<<<<<
  * 		if gl == NULL:
  * 			return None
  */
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 398, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 417, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 398, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 417, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_genotype_likelihoods_by_id(__pyx_t_2, __pyx_v_variant_index);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 398, __pyx_L1_error)
+    __PYX_ERR(1, 417, __pyx_L1_error)
   }
   __pyx_v_gl = __pyx_t_3;
 
-  /* "whatshap/core.pyx":399
+  /* "whatshap/core.pyx":418
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		if gl == NULL:             # <<<<<<<<<<<<<<
  * 			return None
  * 		else:
  */
   __pyx_t_4 = ((__pyx_v_gl == NULL) != 0);
   if (__pyx_t_4) {
 
-    /* "whatshap/core.pyx":400
+    /* "whatshap/core.pyx":419
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		if gl == NULL:
  * 			return None             # <<<<<<<<<<<<<<
  * 		else:
  * 			return PhredGenotypeLikelihoods(gl[0].as_vector(), gl[0].get_ploidy(), gl[0].get_nr_alleles())
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "whatshap/core.pyx":399
+    /* "whatshap/core.pyx":418
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		if gl == NULL:             # <<<<<<<<<<<<<<
  * 			return None
  * 		else:
  */
   }
 
-  /* "whatshap/core.pyx":402
+  /* "whatshap/core.pyx":421
  * 			return None
  * 		else:
  * 			return PhredGenotypeLikelihoods(gl[0].as_vector(), gl[0].get_ploidy(), gl[0].get_nr_alleles())             # <<<<<<<<<<<<<<
  * 
  * 	def __len__(self):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     try {
       __pyx_t_5 = (__pyx_v_gl[0]).as_vector();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 402, __pyx_L1_error)
+      __PYX_ERR(1, 421, __pyx_L1_error)
     }
-    __pyx_t_1 = __pyx_convert_vector_to_py_double(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 402, __pyx_L1_error)
+    __pyx_t_1 = __pyx_convert_vector_to_py_double(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     try {
       __pyx_t_2 = (__pyx_v_gl[0]).get_ploidy();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 402, __pyx_L1_error)
+      __PYX_ERR(1, 421, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 402, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_unsigned_int(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     try {
       __pyx_t_2 = (__pyx_v_gl[0]).get_nr_alleles();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 402, __pyx_L1_error)
+      __PYX_ERR(1, 421, __pyx_L1_error)
     }
-    __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 402, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_unsigned_int(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 402, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
     __pyx_t_1 = 0;
     __pyx_t_6 = 0;
     __pyx_t_7 = 0;
-    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 402, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_r = __pyx_t_7;
     __pyx_t_7 = 0;
     goto __pyx_L0;
   }
 
-  /* "whatshap/core.pyx":397
+  /* "whatshap/core.pyx":416
  * 		return Genotype(gt[0].as_vector())
  * 
  * 	def genotype_likelihoods(self, sample_id, unsigned int variant_index):             # <<<<<<<<<<<<<<
  * 		cdef const cpp.PhredGenotypeLikelihoods* gl = self.thisptr.get_genotype_likelihoods_by_id(self.numeric_sample_ids[sample_id], variant_index)
  * 		if gl == NULL:
  */
 
@@ -10734,15 +11172,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":404
+/* "whatshap/core.pyx":423
  * 			return PhredGenotypeLikelihoods(gl[0].as_vector(), gl[0].get_ploidy(), gl[0].get_nr_alleles())
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
@@ -10760,39 +11198,39 @@
 }
 
 static Py_ssize_t __pyx_pf_8whatshap_4core_8Pedigree_12__len__(struct __pyx_obj_8whatshap_4core_Pedigree *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "whatshap/core.pyx":405
+  /* "whatshap/core.pyx":424
  * 
  * 	def __len__(self):
  * 		return self.thisptr.size()             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
   __pyx_r = __pyx_v_self->thisptr->size();
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":404
+  /* "whatshap/core.pyx":423
  * 			return PhredGenotypeLikelihoods(gl[0].as_vector(), gl[0].get_ploidy(), gl[0].get_nr_alleles())
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":407
+/* "whatshap/core.pyx":426
  * 		return self.thisptr.size()
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -10815,35 +11253,35 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "whatshap/core.pyx":408
+  /* "whatshap/core.pyx":427
  * 
  * 	def __str__(self):
  * 		return self.thisptr.toString().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->toString();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 408, __pyx_L1_error)
+    __PYX_ERR(1, 427, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 408, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":407
+  /* "whatshap/core.pyx":426
  * 		return self.thisptr.size()
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -10967,15 +11405,15 @@
   __Pyx_AddTraceback("whatshap.core.Pedigree.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":412
+/* "whatshap/core.pyx":431
  * 
  * cdef class PhredGenotypeLikelihoods:
  * 	def __cinit__(self, vector[double] gl, unsigned int ploidy=2, unsigned int nr_alleles=2):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.PhredGenotypeLikelihoods(gl, ploidy, nr_alleles)
  * 
  */
 
@@ -11022,42 +11460,42 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nr_alleles);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 412, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 431, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_gl = __pyx_convert_vector_from_py_double(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 412, __pyx_L3_error)
+    __pyx_v_gl = __pyx_convert_vector_from_py_double(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 431, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_ploidy = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_ploidy == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 412, __pyx_L3_error)
+      __pyx_v_ploidy = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_ploidy == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 431, __pyx_L3_error)
     } else {
       __pyx_v_ploidy = ((unsigned int)2);
     }
     if (values[2]) {
-      __pyx_v_nr_alleles = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_nr_alleles == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 412, __pyx_L3_error)
+      __pyx_v_nr_alleles = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_nr_alleles == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 431, __pyx_L3_error)
     } else {
       __pyx_v_nr_alleles = ((unsigned int)2);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 412, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 431, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.PhredGenotypeLikelihoods.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_24PhredGenotypeLikelihoods___cinit__(((struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *)__pyx_v_self), __pyx_v_gl, __pyx_v_ploidy, __pyx_v_nr_alleles);
 
@@ -11071,30 +11509,30 @@
   __Pyx_RefNannyDeclarations
   PhredGenotypeLikelihoods *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":413
+  /* "whatshap/core.pyx":432
  * cdef class PhredGenotypeLikelihoods:
  * 	def __cinit__(self, vector[double] gl, unsigned int ploidy=2, unsigned int nr_alleles=2):
  * 		self.thisptr = new cpp.PhredGenotypeLikelihoods(gl, ploidy, nr_alleles)             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   try {
     __pyx_t_1 = new PhredGenotypeLikelihoods(__pyx_v_gl, __pyx_v_ploidy, __pyx_v_nr_alleles);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 413, __pyx_L1_error)
+    __PYX_ERR(1, 432, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":412
+  /* "whatshap/core.pyx":431
  * 
  * cdef class PhredGenotypeLikelihoods:
  * 	def __cinit__(self, vector[double] gl, unsigned int ploidy=2, unsigned int nr_alleles=2):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.PhredGenotypeLikelihoods(gl, ploidy, nr_alleles)
  * 
  */
 
@@ -11105,15 +11543,15 @@
   __Pyx_AddTraceback("whatshap.core.PhredGenotypeLikelihoods.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":415
+/* "whatshap/core.pyx":434
  * 		self.thisptr = new cpp.PhredGenotypeLikelihoods(gl, ploidy, nr_alleles)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -11128,36 +11566,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_24PhredGenotypeLikelihoods_2__dealloc__(struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":416
+  /* "whatshap/core.pyx":435
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":415
+  /* "whatshap/core.pyx":434
  * 		self.thisptr = new cpp.PhredGenotypeLikelihoods(gl, ploidy, nr_alleles)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":418
+/* "whatshap/core.pyx":437
  * 		del self.thisptr
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -11180,35 +11618,35 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "whatshap/core.pyx":419
+  /* "whatshap/core.pyx":438
  * 
  * 	def __str__(self):
  * 		return self.thisptr.toString().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 	def __getitem__(self, Genotype genotype):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->toString();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 419, __pyx_L1_error)
+    __PYX_ERR(1, 438, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 419, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":418
+  /* "whatshap/core.pyx":437
  * 		del self.thisptr
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -11219,15 +11657,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":421
+/* "whatshap/core.pyx":440
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __getitem__(self, Genotype genotype):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		assert genotype.is_diploid_and_biallelic()
  */
 
@@ -11236,15 +11674,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_24PhredGenotypeLikelihoods_7__getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_genotype) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_genotype), __pyx_ptype_8whatshap_4core_Genotype, 1, "genotype", 0))) __PYX_ERR(1, 421, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_genotype), __pyx_ptype_8whatshap_4core_Genotype, 1, "genotype", 0))) __PYX_ERR(1, 440, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_24PhredGenotypeLikelihoods_6__getitem__(((struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_genotype));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -11261,86 +11699,86 @@
   int __pyx_t_4;
   double __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "whatshap/core.pyx":422
+  /* "whatshap/core.pyx":441
  * 
  * 	def __getitem__(self, Genotype genotype):
  * 		assert self.thisptr != NULL             # <<<<<<<<<<<<<<
  * 		assert genotype.is_diploid_and_biallelic()
  * 		return self.thisptr.get(genotype.thisptr[0])
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_self->thisptr != NULL) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 422, __pyx_L1_error)
+      __PYX_ERR(1, 441, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":423
+  /* "whatshap/core.pyx":442
  * 	def __getitem__(self, Genotype genotype):
  * 		assert self.thisptr != NULL
  * 		assert genotype.is_diploid_and_biallelic()             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get(genotype.thisptr[0])
  * 
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_genotype), __pyx_n_s_is_diploid_and_biallelic); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_genotype), __pyx_n_s_is_diploid_and_biallelic); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 423, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 442, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 423, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(1, 442, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(!__pyx_t_4)) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(1, 423, __pyx_L1_error)
+      __PYX_ERR(1, 442, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "whatshap/core.pyx":424
+  /* "whatshap/core.pyx":443
  * 		assert self.thisptr != NULL
  * 		assert genotype.is_diploid_and_biallelic()
  * 		return self.thisptr.get(genotype.thisptr[0])             # <<<<<<<<<<<<<<
  * 
  * 	def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_5 = __pyx_v_self->thisptr->get((__pyx_v_genotype->thisptr[0]));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 424, __pyx_L1_error)
+    __PYX_ERR(1, 443, __pyx_L1_error)
   }
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 424, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":421
+  /* "whatshap/core.pyx":440
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __getitem__(self, Genotype genotype):             # <<<<<<<<<<<<<<
  * 		assert self.thisptr != NULL
  * 		assert genotype.is_diploid_and_biallelic()
  */
 
@@ -11353,15 +11791,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":426
+/* "whatshap/core.pyx":445
  * 		return self.thisptr.get(genotype.thisptr[0])
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
@@ -11383,31 +11821,31 @@
   __Pyx_RefNannyDeclarations
   unsigned int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "whatshap/core.pyx":427
+  /* "whatshap/core.pyx":446
  * 
  * 	def __len__(self):
  * 		return self.thisptr.size()             # <<<<<<<<<<<<<<
  * 
  * 	def __iter__(self):
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->size();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 427, __pyx_L1_error)
+    __PYX_ERR(1, 446, __pyx_L1_error)
   }
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":426
+  /* "whatshap/core.pyx":445
  * 		return self.thisptr.get(genotype.thisptr[0])
  * 
  * 	def __len__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.size()
  * 
  */
 
@@ -11417,15 +11855,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_8whatshap_4core_24PhredGenotypeLikelihoods_12generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "whatshap/core.pyx":429
+/* "whatshap/core.pyx":448
  * 		return self.thisptr.size()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for genotype in self.genotypes():
  * 			yield self[genotype]
  */
 
@@ -11450,23 +11888,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_8whatshap_4core___pyx_scope_struct_2___iter__ *)__pyx_tp_new_8whatshap_4core___pyx_scope_struct_2___iter__(__pyx_ptype_8whatshap_4core___pyx_scope_struct_2___iter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_8whatshap_4core___pyx_scope_struct_2___iter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(1, 429, __pyx_L1_error)
+    __PYX_ERR(1, 448, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_24PhredGenotypeLikelihoods_12generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_PhredGenotypeLikelihoods___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 429, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_8whatshap_4core_24PhredGenotypeLikelihoods_12generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_PhredGenotypeLikelihoods___iter, __pyx_n_s_whatshap_core); if (unlikely(!gen)) __PYX_ERR(1, 448, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -11496,93 +11934,93 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 429, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 448, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":430
+  /* "whatshap/core.pyx":449
  * 
  * 	def __iter__(self):
  * 		for genotype in self.genotypes():             # <<<<<<<<<<<<<<
  * 			yield self[genotype]
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 430, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 430, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 449, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 430, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 430, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 449, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 430, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 449, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 430, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 449, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 430, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(1, 449, __pyx_L1_error)
         #else
-        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 430, __pyx_L1_error)
+        __pyx_t_1 = PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 449, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_5(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 430, __pyx_L1_error)
+          else __PYX_ERR(1, 449, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_genotype);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_genotype, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "whatshap/core.pyx":431
+    /* "whatshap/core.pyx":450
  * 	def __iter__(self):
  * 		for genotype in self.genotypes():
  * 			yield self[genotype]             # <<<<<<<<<<<<<<
  * 
  * 	def __eq__(self, PhredGenotypeLikelihoods other):
  */
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_genotype); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 431, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_cur_scope->__pyx_v_self), __pyx_cur_scope->__pyx_v_genotype); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 450, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     __Pyx_XGIVEREF(__pyx_t_2);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_4;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_5;
@@ -11594,28 +12032,28 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_2);
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_5 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 431, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(1, 450, __pyx_L1_error)
 
-    /* "whatshap/core.pyx":430
+    /* "whatshap/core.pyx":449
  * 
  * 	def __iter__(self):
  * 		for genotype in self.genotypes():             # <<<<<<<<<<<<<<
  * 			yield self[genotype]
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "whatshap/core.pyx":429
+  /* "whatshap/core.pyx":448
  * 		return self.thisptr.size()
  * 
  * 	def __iter__(self):             # <<<<<<<<<<<<<<
  * 		for genotype in self.genotypes():
  * 			yield self[genotype]
  */
 
@@ -11634,15 +12072,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":433
+/* "whatshap/core.pyx":452
  * 			yield self[genotype]
  * 
  * 	def __eq__(self, PhredGenotypeLikelihoods other):             # <<<<<<<<<<<<<<
  * 		if self.genotypes() != other.genotypes():
  * 			return False
  */
 
@@ -11651,15 +12089,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_24PhredGenotypeLikelihoods_14__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_other) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods, 1, "other", 0))) __PYX_ERR(1, 433, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_other), __pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods, 1, "other", 0))) __PYX_ERR(1, 452, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_24PhredGenotypeLikelihoods_13__eq__(((struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_PhredGenotypeLikelihoods *)__pyx_v_other));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -11679,213 +12117,213 @@
   Py_ssize_t __pyx_t_6;
   PyObject *(*__pyx_t_7)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
 
-  /* "whatshap/core.pyx":434
+  /* "whatshap/core.pyx":453
  * 
  * 	def __eq__(self, PhredGenotypeLikelihoods other):
  * 		if self.genotypes() != other.genotypes():             # <<<<<<<<<<<<<<
  * 			return False
  * 		for genotype in self.genotypes():
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 434, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 434, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 434, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_other), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 434, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 434, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 434, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 453, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_5) {
 
-    /* "whatshap/core.pyx":435
+    /* "whatshap/core.pyx":454
  * 	def __eq__(self, PhredGenotypeLikelihoods other):
  * 		if self.genotypes() != other.genotypes():
  * 			return False             # <<<<<<<<<<<<<<
  * 		for genotype in self.genotypes():
  * 			if self[genotype] != other[genotype]:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     goto __pyx_L0;
 
-    /* "whatshap/core.pyx":434
+    /* "whatshap/core.pyx":453
  * 
  * 	def __eq__(self, PhredGenotypeLikelihoods other):
  * 		if self.genotypes() != other.genotypes():             # <<<<<<<<<<<<<<
  * 			return False
  * 		for genotype in self.genotypes():
  */
   }
 
-  /* "whatshap/core.pyx":436
+  /* "whatshap/core.pyx":455
  * 		if self.genotypes() != other.genotypes():
  * 			return False
  * 		for genotype in self.genotypes():             # <<<<<<<<<<<<<<
  * 			if self[genotype] != other[genotype]:
  * 				return False
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 436, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_genotypes); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 436, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 455, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 436, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 455, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 436, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 455, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(1, 436, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(1, 455, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 436, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 455, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(1, 436, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(1, 455, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 436, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 455, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 436, __pyx_L1_error)
+          else __PYX_ERR(1, 455, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_genotype, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "whatshap/core.pyx":437
+    /* "whatshap/core.pyx":456
  * 			return False
  * 		for genotype in self.genotypes():
  * 			if self[genotype] != other[genotype]:             # <<<<<<<<<<<<<<
  * 				return False
  * 		return True
  */
-    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_genotype); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 437, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_genotype); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 456, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_other), __pyx_v_genotype); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 437, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_other), __pyx_v_genotype); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 456, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 437, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_t_1, Py_NE); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 456, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 437, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(1, 456, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
 
-      /* "whatshap/core.pyx":438
+      /* "whatshap/core.pyx":457
  * 		for genotype in self.genotypes():
  * 			if self[genotype] != other[genotype]:
  * 				return False             # <<<<<<<<<<<<<<
  * 		return True
  * 
  */
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_False);
       __pyx_r = Py_False;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       goto __pyx_L0;
 
-      /* "whatshap/core.pyx":437
+      /* "whatshap/core.pyx":456
  * 			return False
  * 		for genotype in self.genotypes():
  * 			if self[genotype] != other[genotype]:             # <<<<<<<<<<<<<<
  * 				return False
  * 		return True
  */
     }
 
-    /* "whatshap/core.pyx":436
+    /* "whatshap/core.pyx":455
  * 		if self.genotypes() != other.genotypes():
  * 			return False
  * 		for genotype in self.genotypes():             # <<<<<<<<<<<<<<
  * 			if self[genotype] != other[genotype]:
  * 				return False
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":439
+  /* "whatshap/core.pyx":458
  * 			if self[genotype] != other[genotype]:
  * 				return False
  * 		return True             # <<<<<<<<<<<<<<
  * 
  * 	def genotypes(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(Py_True);
   __pyx_r = Py_True;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":433
+  /* "whatshap/core.pyx":452
  * 			yield self[genotype]
  * 
  * 	def __eq__(self, PhredGenotypeLikelihoods other):             # <<<<<<<<<<<<<<
  * 		if self.genotypes() != other.genotypes():
  * 			return False
  */
 
@@ -11900,15 +12338,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_genotype);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":441
+/* "whatshap/core.pyx":460
  * 		return True
  * 
  * 	def genotypes(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.Genotype]* genotypes = new vector[cpp.Genotype]()
  * 		self.thisptr.get_genotypes(deref(genotypes))
  */
 
@@ -11939,100 +12377,100 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genotypes", 0);
 
-  /* "whatshap/core.pyx":442
+  /* "whatshap/core.pyx":461
  * 
  * 	def genotypes(self):
  * 		cdef vector[cpp.Genotype]* genotypes = new vector[cpp.Genotype]()             # <<<<<<<<<<<<<<
  * 		self.thisptr.get_genotypes(deref(genotypes))
  * 		result = [Genotype(genotype.as_vector()) for genotype in genotypes[0]]
  */
   try {
     __pyx_t_1 = new std::vector<Genotype> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 442, __pyx_L1_error)
+    __PYX_ERR(1, 461, __pyx_L1_error)
   }
   __pyx_v_genotypes = __pyx_t_1;
 
-  /* "whatshap/core.pyx":443
+  /* "whatshap/core.pyx":462
  * 	def genotypes(self):
  * 		cdef vector[cpp.Genotype]* genotypes = new vector[cpp.Genotype]()
  * 		self.thisptr.get_genotypes(deref(genotypes))             # <<<<<<<<<<<<<<
  * 		result = [Genotype(genotype.as_vector()) for genotype in genotypes[0]]
  * 		del genotypes
  */
   try {
     __pyx_v_self->thisptr->get_genotypes((*__pyx_v_genotypes));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 443, __pyx_L1_error)
+    __PYX_ERR(1, 462, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":444
+  /* "whatshap/core.pyx":463
  * 		cdef vector[cpp.Genotype]* genotypes = new vector[cpp.Genotype]()
  * 		self.thisptr.get_genotypes(deref(genotypes))
  * 		result = [Genotype(genotype.as_vector()) for genotype in genotypes[0]]             # <<<<<<<<<<<<<<
  * 		del genotypes
  * 		return result
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 444, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = &(__pyx_v_genotypes[0]);
     __pyx_t_3 = __pyx_t_1->begin();
     for (;;) {
       if (!(__pyx_t_3 != __pyx_t_1->end())) break;
       __pyx_t_4 = *__pyx_t_3;
       ++__pyx_t_3;
       __pyx_8genexpr5__pyx_v_genotype = __pyx_t_4;
       try {
         __pyx_t_5 = __pyx_8genexpr5__pyx_v_genotype.as_vector();
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 444, __pyx_L1_error)
+        __PYX_ERR(1, 463, __pyx_L1_error)
       }
-      __pyx_t_6 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 444, __pyx_L1_error)
+      __pyx_t_6 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 463, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 444, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 463, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(1, 444, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_7))) __PYX_ERR(1, 463, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
   } /* exit inner scope */
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":445
+  /* "whatshap/core.pyx":464
  * 		self.thisptr.get_genotypes(deref(genotypes))
  * 		result = [Genotype(genotype.as_vector()) for genotype in genotypes[0]]
  * 		del genotypes             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_genotypes;
 
-  /* "whatshap/core.pyx":446
+  /* "whatshap/core.pyx":465
  * 		result = [Genotype(genotype.as_vector()) for genotype in genotypes[0]]
  * 		del genotypes
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":441
+  /* "whatshap/core.pyx":460
  * 		return True
  * 
  * 	def genotypes(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.Genotype]* genotypes = new vector[cpp.Genotype]()
  * 		self.thisptr.get_genotypes(deref(genotypes))
  */
 
@@ -12159,15 +12597,15 @@
   __Pyx_AddTraceback("whatshap.core.PhredGenotypeLikelihoods.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":449
+/* "whatshap/core.pyx":468
  * 
  * 
  * def binomial_coefficient(int n, int k):             # <<<<<<<<<<<<<<
  * 	return cpp.binomial_coefficient(n, k)
  * 
  */
 
@@ -12202,32 +12640,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_k)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("binomial_coefficient", 1, 2, 2, 1); __PYX_ERR(1, 449, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("binomial_coefficient", 1, 2, 2, 1); __PYX_ERR(1, 468, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "binomial_coefficient") < 0)) __PYX_ERR(1, 449, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "binomial_coefficient") < 0)) __PYX_ERR(1, 468, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_n = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 449, __pyx_L3_error)
-    __pyx_v_k = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 449, __pyx_L3_error)
+    __pyx_v_n = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 468, __pyx_L3_error)
+    __pyx_v_k = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 468, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("binomial_coefficient", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 449, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("binomial_coefficient", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 468, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.binomial_coefficient", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_binomial_coefficient(__pyx_self, __pyx_v_n, __pyx_v_k);
 
@@ -12242,35 +12680,35 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("binomial_coefficient", 0);
 
-  /* "whatshap/core.pyx":450
+  /* "whatshap/core.pyx":469
  * 
  * def binomial_coefficient(int n, int k):
  * 	return cpp.binomial_coefficient(n, k)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = binomial_coefficient(__pyx_v_n, __pyx_v_k);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 450, __pyx_L1_error)
+    __PYX_ERR(1, 469, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 450, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 469, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":449
+  /* "whatshap/core.pyx":468
  * 
  * 
  * def binomial_coefficient(int n, int k):             # <<<<<<<<<<<<<<
  * 	return cpp.binomial_coefficient(n, k)
  * 
  */
 
@@ -12281,15 +12719,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":455
+/* "whatshap/core.pyx":474
  * cdef class Genotype:
  * 
  * 	def __cinit__(self, vector[uint32_t] alleles):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  */
 
@@ -12318,26 +12756,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_alleles)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 455, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 474, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
-    __pyx_v_alleles = __pyx_convert_vector_from_py_uint32_t(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 455, __pyx_L3_error)
+    __pyx_v_alleles = __pyx_convert_vector_from_py_uint32_t(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 474, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 455, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 474, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Genotype.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_8Genotype___cinit__(((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_self), __pyx_v_alleles);
 
@@ -12351,30 +12789,30 @@
   __Pyx_RefNannyDeclarations
   Genotype *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":456
+  /* "whatshap/core.pyx":475
  * 
  * 	def __cinit__(self, vector[uint32_t] alleles):
  * 		self.thisptr = new cpp.Genotype(alleles)             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   try {
     __pyx_t_1 = new Genotype(__pyx_v_alleles);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 456, __pyx_L1_error)
+    __PYX_ERR(1, 475, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":455
+  /* "whatshap/core.pyx":474
  * cdef class Genotype:
  * 
  * 	def __cinit__(self, vector[uint32_t] alleles):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  */
 
@@ -12385,15 +12823,15 @@
   __Pyx_AddTraceback("whatshap.core.Genotype.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":458
+/* "whatshap/core.pyx":477
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -12408,36 +12846,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_8Genotype_2__dealloc__(struct __pyx_obj_8whatshap_4core_Genotype *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":459
+  /* "whatshap/core.pyx":478
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def __str__(self):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":458
+  /* "whatshap/core.pyx":477
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":461
+/* "whatshap/core.pyx":480
  * 		del self.thisptr
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -12460,35 +12898,35 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "whatshap/core.pyx":462
+  /* "whatshap/core.pyx":481
  * 
  * 	def __str__(self):
  * 		return self.thisptr.toString().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 	def __repr__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->toString();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 462, __pyx_L1_error)
+    __PYX_ERR(1, 481, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 462, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 481, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":461
+  /* "whatshap/core.pyx":480
  * 		del self.thisptr
  * 
  * 	def __str__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -12499,15 +12937,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":464
+/* "whatshap/core.pyx":483
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __repr__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -12530,35 +12968,35 @@
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "whatshap/core.pyx":465
+  /* "whatshap/core.pyx":484
  * 
  * 	def __repr__(self):
  * 		return self.thisptr.toString().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 	def is_none(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->toString();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 465, __pyx_L1_error)
+    __PYX_ERR(1, 484, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 465, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_t_1, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 484, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":464
+  /* "whatshap/core.pyx":483
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def __repr__(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  */
 
@@ -12569,15 +13007,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":467
+/* "whatshap/core.pyx":486
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def is_none(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_none()
  * 
  */
 
@@ -12600,35 +13038,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_none", 0);
 
-  /* "whatshap/core.pyx":468
+  /* "whatshap/core.pyx":487
  * 
  * 	def is_none(self):
  * 		return self.thisptr.is_none()             # <<<<<<<<<<<<<<
  * 
  * 	def get_index(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->is_none();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 468, __pyx_L1_error)
+    __PYX_ERR(1, 487, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 468, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":467
+  /* "whatshap/core.pyx":486
  * 		return self.thisptr.toString().decode('utf-8')
  * 
  * 	def is_none(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_none()
  * 
  */
 
@@ -12639,15 +13077,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":470
+/* "whatshap/core.pyx":489
  * 		return self.thisptr.is_none()
  * 
  * 	def get_index(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_index()
  * 
  */
 
@@ -12670,35 +13108,35 @@
   uint64_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_index", 0);
 
-  /* "whatshap/core.pyx":471
+  /* "whatshap/core.pyx":490
  * 
  * 	def get_index(self):
  * 		return self.thisptr.get_index()             # <<<<<<<<<<<<<<
  * 
  * 	def as_vector(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_index();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 471, __pyx_L1_error)
+    __PYX_ERR(1, 490, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 471, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":470
+  /* "whatshap/core.pyx":489
  * 		return self.thisptr.is_none()
  * 
  * 	def get_index(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_index()
  * 
  */
 
@@ -12709,15 +13147,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":473
+/* "whatshap/core.pyx":492
  * 		return self.thisptr.get_index()
  * 
  * 	def as_vector(self):             # <<<<<<<<<<<<<<
  * 		result = []
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  */
 
@@ -12746,91 +13184,91 @@
   uint32_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("as_vector", 0);
 
-  /* "whatshap/core.pyx":474
+  /* "whatshap/core.pyx":493
  * 
  * 	def as_vector(self):
  * 		result = []             # <<<<<<<<<<<<<<
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  * 		for allele in alleles:
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 474, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 493, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":475
+  /* "whatshap/core.pyx":494
  * 	def as_vector(self):
  * 		result = []
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()             # <<<<<<<<<<<<<<
  * 		for allele in alleles:
  * 			result.append(allele)
  */
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->as_vector();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 475, __pyx_L1_error)
+    __PYX_ERR(1, 494, __pyx_L1_error)
   }
   __pyx_v_alleles = __pyx_t_2;
 
-  /* "whatshap/core.pyx":476
+  /* "whatshap/core.pyx":495
  * 		result = []
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  * 		for allele in alleles:             # <<<<<<<<<<<<<<
  * 			result.append(allele)
  * 		return alleles
  */
   __pyx_t_3 = __pyx_v_alleles.begin();
   for (;;) {
     if (!(__pyx_t_3 != __pyx_v_alleles.end())) break;
     __pyx_t_4 = *__pyx_t_3;
     ++__pyx_t_3;
     __pyx_v_allele = __pyx_t_4;
 
-    /* "whatshap/core.pyx":477
+    /* "whatshap/core.pyx":496
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  * 		for allele in alleles:
  * 			result.append(allele)             # <<<<<<<<<<<<<<
  * 		return alleles
  * 
  */
-    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_allele); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 477, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_uint32_t(__pyx_v_allele); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 477, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_result, __pyx_t_1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "whatshap/core.pyx":476
+    /* "whatshap/core.pyx":495
  * 		result = []
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  * 		for allele in alleles:             # <<<<<<<<<<<<<<
  * 			result.append(allele)
  * 		return alleles
  */
   }
 
-  /* "whatshap/core.pyx":478
+  /* "whatshap/core.pyx":497
  * 		for allele in alleles:
  * 			result.append(allele)
  * 		return alleles             # <<<<<<<<<<<<<<
  * 
  * 	def is_homozygous(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_uint32_t(__pyx_v_alleles); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 478, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_uint32_t(__pyx_v_alleles); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":473
+  /* "whatshap/core.pyx":492
  * 		return self.thisptr.get_index()
  * 
  * 	def as_vector(self):             # <<<<<<<<<<<<<<
  * 		result = []
  * 		cdef vector[uint32_t] alleles = self.thisptr.as_vector()
  */
 
@@ -12842,15 +13280,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":480
+/* "whatshap/core.pyx":499
  * 		return alleles
  * 
  * 	def is_homozygous(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_homozygous()
  * 
  */
 
@@ -12873,35 +13311,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_homozygous", 0);
 
-  /* "whatshap/core.pyx":481
+  /* "whatshap/core.pyx":500
  * 
  * 	def is_homozygous(self):
  * 		return self.thisptr.is_homozygous()             # <<<<<<<<<<<<<<
  * 
  * 	def is_diploid_and_biallelic(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->is_homozygous();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 481, __pyx_L1_error)
+    __PYX_ERR(1, 500, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 481, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 500, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":480
+  /* "whatshap/core.pyx":499
  * 		return alleles
  * 
  * 	def is_homozygous(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_homozygous()
  * 
  */
 
@@ -12912,15 +13350,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":483
+/* "whatshap/core.pyx":502
  * 		return self.thisptr.is_homozygous()
  * 
  * 	def is_diploid_and_biallelic(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_diploid_and_biallelic()
  * 
  */
 
@@ -12943,35 +13381,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_diploid_and_biallelic", 0);
 
-  /* "whatshap/core.pyx":484
+  /* "whatshap/core.pyx":503
  * 
  * 	def is_diploid_and_biallelic(self):
  * 		return self.thisptr.is_diploid_and_biallelic()             # <<<<<<<<<<<<<<
  * 
  * 	def get_ploidy(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->is_diploid_and_biallelic();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 484, __pyx_L1_error)
+    __PYX_ERR(1, 503, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 484, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 503, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":483
+  /* "whatshap/core.pyx":502
  * 		return self.thisptr.is_homozygous()
  * 
  * 	def is_diploid_and_biallelic(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.is_diploid_and_biallelic()
  * 
  */
 
@@ -12982,15 +13420,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":486
+/* "whatshap/core.pyx":505
  * 		return self.thisptr.is_diploid_and_biallelic()
  * 
  * 	def get_ploidy(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_ploidy()
  * 
  */
 
@@ -13013,35 +13451,35 @@
   uint32_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_ploidy", 0);
 
-  /* "whatshap/core.pyx":487
+  /* "whatshap/core.pyx":506
  * 
  * 	def get_ploidy(self):
  * 		return self.thisptr.get_ploidy()             # <<<<<<<<<<<<<<
  * 
  * 	def __eq__(self, Genotype g):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_ploidy();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 487, __pyx_L1_error)
+    __PYX_ERR(1, 506, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 487, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":486
+  /* "whatshap/core.pyx":505
  * 		return self.thisptr.is_diploid_and_biallelic()
  * 
  * 	def get_ploidy(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_ploidy()
  * 
  */
 
@@ -13052,15 +13490,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":489
+/* "whatshap/core.pyx":508
  * 		return self.thisptr.get_ploidy()
  * 
  * 	def __eq__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] == g.thisptr[0]
  * 
  */
 
@@ -13069,15 +13507,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_8Genotype_21__eq__(PyObject *__pyx_v_self, PyObject *__pyx_v_g) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__eq__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 489, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 508, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_8Genotype_20__eq__(((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_g));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13091,35 +13529,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
 
-  /* "whatshap/core.pyx":490
+  /* "whatshap/core.pyx":509
  * 
  * 	def __eq__(self, Genotype g):
  * 		return self.thisptr[0] == g.thisptr[0]             # <<<<<<<<<<<<<<
  * 
  * 	def __ne__(self, Genotype g):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = ((__pyx_v_self->thisptr[0]) == (__pyx_v_g->thisptr[0]));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 490, __pyx_L1_error)
+    __PYX_ERR(1, 509, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 490, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":489
+  /* "whatshap/core.pyx":508
  * 		return self.thisptr.get_ploidy()
  * 
  * 	def __eq__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] == g.thisptr[0]
  * 
  */
 
@@ -13130,15 +13568,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":492
+/* "whatshap/core.pyx":511
  * 		return self.thisptr[0] == g.thisptr[0]
  * 
  * 	def __ne__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] != g.thisptr[0]
  * 
  */
 
@@ -13147,15 +13585,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_8Genotype_23__ne__(PyObject *__pyx_v_self, PyObject *__pyx_v_g) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__ne__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 492, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 511, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_8Genotype_22__ne__(((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_g));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13169,35 +13607,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__ne__", 0);
 
-  /* "whatshap/core.pyx":493
+  /* "whatshap/core.pyx":512
  * 
  * 	def __ne__(self, Genotype g):
  * 		return self.thisptr[0] != g.thisptr[0]             # <<<<<<<<<<<<<<
  * 
  * 	def __lt__(self, Genotype g):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = ((__pyx_v_self->thisptr[0]) != (__pyx_v_g->thisptr[0]));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 493, __pyx_L1_error)
+    __PYX_ERR(1, 512, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 493, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":492
+  /* "whatshap/core.pyx":511
  * 		return self.thisptr[0] == g.thisptr[0]
  * 
  * 	def __ne__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] != g.thisptr[0]
  * 
  */
 
@@ -13208,15 +13646,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":495
+/* "whatshap/core.pyx":514
  * 		return self.thisptr[0] != g.thisptr[0]
  * 
  * 	def __lt__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] < g.thisptr[0]
  * 
  */
 
@@ -13225,15 +13663,15 @@
 static PyObject *__pyx_pw_8whatshap_4core_8Genotype_25__lt__(PyObject *__pyx_v_self, PyObject *__pyx_v_g) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__lt__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 495, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_8whatshap_4core_Genotype, 1, "g", 0))) __PYX_ERR(1, 514, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_8Genotype_24__lt__(((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_self), ((struct __pyx_obj_8whatshap_4core_Genotype *)__pyx_v_g));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -13247,35 +13685,35 @@
   bool __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__lt__", 0);
 
-  /* "whatshap/core.pyx":496
+  /* "whatshap/core.pyx":515
  * 
  * 	def __lt__(self, Genotype g):
  * 		return self.thisptr[0] < g.thisptr[0]             # <<<<<<<<<<<<<<
  * 
  * 	def __getstate__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = ((__pyx_v_self->thisptr[0]) < (__pyx_v_g->thisptr[0]));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 496, __pyx_L1_error)
+    __PYX_ERR(1, 515, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 496, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":495
+  /* "whatshap/core.pyx":514
  * 		return self.thisptr[0] != g.thisptr[0]
  * 
  * 	def __lt__(self, Genotype g):             # <<<<<<<<<<<<<<
  * 		return self.thisptr[0] < g.thisptr[0]
  * 
  */
 
@@ -13286,15 +13724,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":498
+/* "whatshap/core.pyx":517
  * 		return self.thisptr[0] < g.thisptr[0]
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		return (self.thisptr.get_index(), self.thisptr.get_ploidy())
  * 
  */
 
@@ -13320,51 +13758,51 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getstate__", 0);
 
-  /* "whatshap/core.pyx":499
+  /* "whatshap/core.pyx":518
  * 
  * 	def __getstate__(self):
  * 		return (self.thisptr.get_index(), self.thisptr.get_ploidy())             # <<<<<<<<<<<<<<
  * 
  * 	def __setstate__(self, state):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_index();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 499, __pyx_L1_error)
+    __PYX_ERR(1, 518, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 499, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_ploidy();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 499, __pyx_L1_error)
+    __PYX_ERR(1, 518, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 499, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_uint32_t(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 499, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":498
+  /* "whatshap/core.pyx":517
  * 		return self.thisptr[0] < g.thisptr[0]
  * 
  * 	def __getstate__(self):             # <<<<<<<<<<<<<<
  * 		return (self.thisptr.get_index(), self.thisptr.get_ploidy())
  * 
  */
 
@@ -13377,15 +13815,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":501
+/* "whatshap/core.pyx":520
  * 		return (self.thisptr.get_index(), self.thisptr.get_ploidy())
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
  * 		index, ploidy = state
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  */
 
@@ -13418,131 +13856,131 @@
   int __pyx_t_8;
   Genotype *__pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate__", 0);
 
-  /* "whatshap/core.pyx":502
+  /* "whatshap/core.pyx":521
  * 
  * 	def __setstate__(self, state):
  * 		index, ploidy = state             # <<<<<<<<<<<<<<
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  * 		if self.thisptr != NULL:
  */
   if ((likely(PyTuple_CheckExact(__pyx_v_state))) || (PyList_CheckExact(__pyx_v_state))) {
     PyObject* sequence = __pyx_v_state;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(1, 502, __pyx_L1_error)
+      __PYX_ERR(1, 521, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_1 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_1 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_2 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_2);
     #else
-    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __pyx_t_1 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     #endif
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_3 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 502, __pyx_L1_error)
+    __pyx_t_3 = PyObject_GetIter(__pyx_v_state); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 521, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext;
     index = 0; __pyx_t_1 = __pyx_t_4(__pyx_t_3); if (unlikely(!__pyx_t_1)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_1);
     index = 1; __pyx_t_2 = __pyx_t_4(__pyx_t_3); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_4(__pyx_t_3), 2) < 0) __PYX_ERR(1, 502, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_4(__pyx_t_3), 2) < 0) __PYX_ERR(1, 521, __pyx_L1_error)
     __pyx_t_4 = NULL;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(1, 502, __pyx_L1_error)
+    __PYX_ERR(1, 521, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_index = __pyx_t_1;
   __pyx_t_1 = 0;
   __pyx_v_ploidy = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":503
+  /* "whatshap/core.pyx":522
  * 	def __setstate__(self, state):
  * 		index, ploidy = state
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)             # <<<<<<<<<<<<<<
  * 		if self.thisptr != NULL:
  * 			del self.thisptr
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint64_t(__pyx_v_index); if (unlikely((__pyx_t_5 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 503, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_ploidy); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 503, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint64_t(__pyx_v_index); if (unlikely((__pyx_t_5 == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 522, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint32_t(__pyx_v_ploidy); if (unlikely((__pyx_t_6 == ((uint32_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 522, __pyx_L1_error)
   try {
     __pyx_t_7 = convert_index_to_alleles(__pyx_t_5, __pyx_t_6);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 503, __pyx_L1_error)
+    __PYX_ERR(1, 522, __pyx_L1_error)
   }
   __pyx_v_alleles = __pyx_t_7;
 
-  /* "whatshap/core.pyx":504
+  /* "whatshap/core.pyx":523
  * 		index, ploidy = state
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  * 		if self.thisptr != NULL:             # <<<<<<<<<<<<<<
  * 			del self.thisptr
  * 		self.thisptr = new cpp.Genotype(alleles)
  */
   __pyx_t_8 = ((__pyx_v_self->thisptr != NULL) != 0);
   if (__pyx_t_8) {
 
-    /* "whatshap/core.pyx":505
+    /* "whatshap/core.pyx":524
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  * 		if self.thisptr != NULL:
  * 			del self.thisptr             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  */
     delete __pyx_v_self->thisptr;
 
-    /* "whatshap/core.pyx":504
+    /* "whatshap/core.pyx":523
  * 		index, ploidy = state
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  * 		if self.thisptr != NULL:             # <<<<<<<<<<<<<<
  * 			del self.thisptr
  * 		self.thisptr = new cpp.Genotype(alleles)
  */
   }
 
-  /* "whatshap/core.pyx":506
+  /* "whatshap/core.pyx":525
  * 		if self.thisptr != NULL:
  * 			del self.thisptr
  * 		self.thisptr = new cpp.Genotype(alleles)             # <<<<<<<<<<<<<<
  * 
  * 	def __deepcopy__(self, memo):
  */
   try {
     __pyx_t_9 = new Genotype(__pyx_v_alleles);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 506, __pyx_L1_error)
+    __PYX_ERR(1, 525, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_9;
 
-  /* "whatshap/core.pyx":501
+  /* "whatshap/core.pyx":520
  * 		return (self.thisptr.get_index(), self.thisptr.get_ploidy())
  * 
  * 	def __setstate__(self, state):             # <<<<<<<<<<<<<<
  * 		index, ploidy = state
  * 		cdef vector[uint32_t] alleles = cpp.convert_index_to_alleles(index, ploidy)
  */
 
@@ -13559,15 +13997,15 @@
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XDECREF(__pyx_v_ploidy);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":508
+/* "whatshap/core.pyx":527
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  * 	def __deepcopy__(self, memo):             # <<<<<<<<<<<<<<
  * 		return Genotype.__new__(Genotype, self.as_vector())
  * 
  */
 
@@ -13591,52 +14029,52 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__deepcopy__", 0);
 
-  /* "whatshap/core.pyx":509
+  /* "whatshap/core.pyx":528
  * 
  * 	def __deepcopy__(self, memo):
  * 		return Genotype.__new__(Genotype, self.as_vector())             # <<<<<<<<<<<<<<
  * 
  * 	def __hash__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_as_vector); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 509, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_as_vector); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 509, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 509, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 528, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8whatshap_4core_Genotype(((PyTypeObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_2, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 509, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8whatshap_4core_Genotype(((PyTypeObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_2, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 528, __pyx_L1_error)
   __Pyx_GOTREF(((PyObject *)__pyx_t_1));
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = ((PyObject *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":508
+  /* "whatshap/core.pyx":527
  * 		self.thisptr = new cpp.Genotype(alleles)
  * 
  * 	def __deepcopy__(self, memo):             # <<<<<<<<<<<<<<
  * 		return Genotype.__new__(Genotype, self.as_vector())
  * 
  */
 
@@ -13649,15 +14087,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":511
+/* "whatshap/core.pyx":530
  * 		return Genotype.__new__(Genotype, self.as_vector())
  * 
  * 	def __hash__(self):             # <<<<<<<<<<<<<<
  * 		return hash(self.thisptr.get_index())
  * 
  */
 
@@ -13681,35 +14119,35 @@
   PyObject *__pyx_t_2 = NULL;
   Py_hash_t __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__hash__", 0);
 
-  /* "whatshap/core.pyx":512
+  /* "whatshap/core.pyx":531
  * 
  * 	def __hash__(self):
  * 		return hash(self.thisptr.get_index())             # <<<<<<<<<<<<<<
  * 
  * 
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->get_index();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 512, __pyx_L1_error)
+    __PYX_ERR(1, 531, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 512, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint64_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Hash(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_hash_t)-1))) __PYX_ERR(1, 512, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Hash(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_hash_t)-1))) __PYX_ERR(1, 531, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":511
+  /* "whatshap/core.pyx":530
  * 		return Genotype.__new__(Genotype, self.as_vector())
  * 
  * 	def __hash__(self):             # <<<<<<<<<<<<<<
  * 		return hash(self.thisptr.get_index())
  * 
  */
 
@@ -13833,15 +14271,15 @@
   __Pyx_AddTraceback("whatshap.core.Genotype.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":515
+/* "whatshap/core.pyx":534
  * 
  * 
  * def get_max_genotype_ploidy():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_ploidy()
  * 
  */
 
@@ -13865,35 +14303,35 @@
   uint32_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_genotype_ploidy", 0);
 
-  /* "whatshap/core.pyx":516
+  /* "whatshap/core.pyx":535
  * 
  * def get_max_genotype_ploidy():
  * 	return cpp.get_max_genotype_ploidy()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = get_max_genotype_ploidy();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 516, __pyx_L1_error)
+    __PYX_ERR(1, 535, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 516, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":515
+  /* "whatshap/core.pyx":534
  * 
  * 
  * def get_max_genotype_ploidy():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_ploidy()
  * 
  */
 
@@ -13904,15 +14342,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":519
+/* "whatshap/core.pyx":538
  * 
  * 
  * def get_max_genotype_alleles():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_alleles()
  * 
  */
 
@@ -13936,35 +14374,35 @@
   uint32_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_max_genotype_alleles", 0);
 
-  /* "whatshap/core.pyx":520
+  /* "whatshap/core.pyx":539
  * 
  * def get_max_genotype_alleles():
  * 	return cpp.get_max_genotype_alleles()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = get_max_genotype_alleles();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 520, __pyx_L1_error)
+    __PYX_ERR(1, 539, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 520, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_uint32_t(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 539, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":519
+  /* "whatshap/core.pyx":538
  * 
  * 
  * def get_max_genotype_alleles():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_alleles()
  * 
  */
 
@@ -13975,15 +14413,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":524
+/* "whatshap/core.pyx":543
  * 
  * cdef class GenotypeDPTable:
  * 	def __cinit__(self, numeric_sample_ids, ReadSet readset, recombcost, Pedigree pedigree, positions = None):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -14027,37 +14465,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_numeric_sample_ids)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_readset)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 1); __PYX_ERR(1, 524, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 1); __PYX_ERR(1, 543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_recombcost)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 2); __PYX_ERR(1, 524, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 2); __PYX_ERR(1, 543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pedigree)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 3); __PYX_ERR(1, 524, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 3); __PYX_ERR(1, 543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_positions);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 524, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 543, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -14071,22 +14509,22 @@
     __pyx_v_readset = ((struct __pyx_obj_8whatshap_4core_ReadSet *)values[1]);
     __pyx_v_recombcost = values[2];
     __pyx_v_pedigree = ((struct __pyx_obj_8whatshap_4core_Pedigree *)values[3]);
     __pyx_v_positions = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 524, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 543, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.GenotypeDPTable.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 524, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 524, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 543, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 543, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_15GenotypeDPTable___cinit__(((struct __pyx_obj_8whatshap_4core_GenotypeDPTable *)__pyx_v_self), __pyx_v_numeric_sample_ids, __pyx_v_readset, __pyx_v_recombcost, __pyx_v_pedigree, __pyx_v_positions);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -14110,178 +14548,178 @@
   std::vector<unsigned int>  __pyx_t_9;
   GenotypeDPTable *__pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":529
+  /* "whatshap/core.pyx":548
  * 		in the read set must also be sorted (by position of their left-most variant).
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL             # <<<<<<<<<<<<<<
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  */
   __pyx_v_c_positions = NULL;
 
-  /* "whatshap/core.pyx":530
+  /* "whatshap/core.pyx":549
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   __pyx_t_1 = (__pyx_v_positions != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "whatshap/core.pyx":531
+    /* "whatshap/core.pyx":550
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()             # <<<<<<<<<<<<<<
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  */
     try {
       __pyx_t_3 = new std::vector<unsigned int> ();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 531, __pyx_L1_error)
+      __PYX_ERR(1, 550, __pyx_L1_error)
     }
     __pyx_v_c_positions = __pyx_t_3;
 
-    /* "whatshap/core.pyx":532
+    /* "whatshap/core.pyx":551
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)
  */
     if (likely(PyList_CheckExact(__pyx_v_positions)) || PyTuple_CheckExact(__pyx_v_positions)) {
       __pyx_t_4 = __pyx_v_positions; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 532, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 551, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 532, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 551, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 532, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 551, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 532, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 551, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 532, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 551, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 532, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 551, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 532, __pyx_L1_error)
+            else __PYX_ERR(1, 551, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "whatshap/core.pyx":533
+      /* "whatshap/core.pyx":552
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  * 				c_positions.push_back(pos)             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)
  * 		self.pedigree = pedigree
  */
-      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 533, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 552, __pyx_L1_error)
       try {
         __pyx_v_c_positions->push_back(__pyx_t_8);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 533, __pyx_L1_error)
+        __PYX_ERR(1, 552, __pyx_L1_error)
       }
 
-      /* "whatshap/core.pyx":532
+      /* "whatshap/core.pyx":551
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "whatshap/core.pyx":530
+    /* "whatshap/core.pyx":549
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   }
 
-  /* "whatshap/core.pyx":534
+  /* "whatshap/core.pyx":553
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)             # <<<<<<<<<<<<<<
  * 		self.pedigree = pedigree
  * 		self.numeric_sample_ids = numeric_sample_ids
  */
-  __pyx_t_9 = __pyx_convert_vector_from_py_unsigned_int(__pyx_v_recombcost); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 534, __pyx_L1_error)
+  __pyx_t_9 = __pyx_convert_vector_from_py_unsigned_int(__pyx_v_recombcost); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 553, __pyx_L1_error)
   try {
     __pyx_t_10 = new GenotypeDPTable(__pyx_v_readset->thisptr, __pyx_t_9, __pyx_v_pedigree->thisptr, __pyx_v_c_positions);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 534, __pyx_L1_error)
+    __PYX_ERR(1, 553, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_10;
 
-  /* "whatshap/core.pyx":535
+  /* "whatshap/core.pyx":554
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)
  * 		self.pedigree = pedigree             # <<<<<<<<<<<<<<
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GOTREF(__pyx_v_self->pedigree);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->pedigree));
   __pyx_v_self->pedigree = __pyx_v_pedigree;
 
-  /* "whatshap/core.pyx":536
+  /* "whatshap/core.pyx":555
  * 		self.thisptr = new cpp.GenotypeDPTable(readset.thisptr, recombcost, pedigree.thisptr, c_positions)
  * 		self.pedigree = pedigree
  * 		self.numeric_sample_ids = numeric_sample_ids             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
-  if (!(likely(((__pyx_v_numeric_sample_ids) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_numeric_sample_ids, __pyx_ptype_8whatshap_4core_NumericSampleIds))))) __PYX_ERR(1, 536, __pyx_L1_error)
+  if (!(likely(((__pyx_v_numeric_sample_ids) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_numeric_sample_ids, __pyx_ptype_8whatshap_4core_NumericSampleIds))))) __PYX_ERR(1, 555, __pyx_L1_error)
   __pyx_t_4 = __pyx_v_numeric_sample_ids;
   __Pyx_INCREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->numeric_sample_ids);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->numeric_sample_ids));
   __pyx_v_self->numeric_sample_ids = ((struct __pyx_obj_8whatshap_4core_NumericSampleIds *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "whatshap/core.pyx":524
+  /* "whatshap/core.pyx":543
  * 
  * cdef class GenotypeDPTable:
  * 	def __cinit__(self, numeric_sample_ids, ReadSet readset, recombcost, Pedigree pedigree, positions = None):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -14295,15 +14733,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":538
+/* "whatshap/core.pyx":557
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -14318,36 +14756,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_15GenotypeDPTable_2__dealloc__(struct __pyx_obj_8whatshap_4core_GenotypeDPTable *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":539
+  /* "whatshap/core.pyx":558
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def get_genotype_likelihoods(self, sample_id, unsigned int pos):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":538
+  /* "whatshap/core.pyx":557
  * 		self.numeric_sample_ids = numeric_sample_ids
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":541
+/* "whatshap/core.pyx":560
  * 		del self.thisptr
  * 
  * 	def get_genotype_likelihoods(self, sample_id, unsigned int pos):             # <<<<<<<<<<<<<<
  * 		return PhredGenotypeLikelihoods(self.thisptr.get_genotype_likelihoods(self.numeric_sample_ids[sample_id],pos))
  * 
  */
 
@@ -14381,32 +14819,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sample_id)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("get_genotype_likelihoods", 1, 2, 2, 1); __PYX_ERR(1, 541, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_genotype_likelihoods", 1, 2, 2, 1); __PYX_ERR(1, 560, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_genotype_likelihoods") < 0)) __PYX_ERR(1, 541, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_genotype_likelihoods") < 0)) __PYX_ERR(1, 560, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_sample_id = values[0];
-    __pyx_v_pos = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_pos == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 541, __pyx_L3_error)
+    __pyx_v_pos = __Pyx_PyInt_As_unsigned_int(values[1]); if (unlikely((__pyx_v_pos == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 560, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_genotype_likelihoods", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 541, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_genotype_likelihoods", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 560, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.GenotypeDPTable.get_genotype_likelihoods", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_15GenotypeDPTable_4get_genotype_likelihoods(((struct __pyx_obj_8whatshap_4core_GenotypeDPTable *)__pyx_v_self), __pyx_v_sample_id, __pyx_v_pos);
 
@@ -14423,42 +14861,42 @@
   std::vector<long double>  __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_genotype_likelihoods", 0);
 
-  /* "whatshap/core.pyx":542
+  /* "whatshap/core.pyx":561
  * 
  * 	def get_genotype_likelihoods(self, sample_id, unsigned int pos):
  * 		return PhredGenotypeLikelihoods(self.thisptr.get_genotype_likelihoods(self.numeric_sample_ids[sample_id],pos))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 542, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self->numeric_sample_ids), __pyx_v_sample_id); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 542, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_unsigned_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 561, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   try {
     __pyx_t_3 = __pyx_v_self->thisptr->get_genotype_likelihoods(__pyx_t_2, __pyx_v_pos);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 542, __pyx_L1_error)
+    __PYX_ERR(1, 561, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_convert_vector_to_py_long__double(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 542, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_long__double(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 542, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods), __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":541
+  /* "whatshap/core.pyx":560
  * 		del self.thisptr
  * 
  * 	def get_genotype_likelihoods(self, sample_id, unsigned int pos):             # <<<<<<<<<<<<<<
  * 		return PhredGenotypeLikelihoods(self.thisptr.get_genotype_likelihoods(self.numeric_sample_ids[sample_id],pos))
  * 
  */
 
@@ -14583,15 +15021,15 @@
   __Pyx_AddTraceback("whatshap.core.GenotypeDPTable.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":545
+/* "whatshap/core.pyx":564
  * 
  * 
  * def compute_genotypes(ReadSet readset, positions = None):             # <<<<<<<<<<<<<<
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  */
 
@@ -14631,15 +15069,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_positions);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compute_genotypes") < 0)) __PYX_ERR(1, 545, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "compute_genotypes") < 0)) __PYX_ERR(1, 564, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -14647,21 +15085,21 @@
       }
     }
     __pyx_v_readset = ((struct __pyx_obj_8whatshap_4core_ReadSet *)values[0]);
     __pyx_v_positions = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("compute_genotypes", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 545, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("compute_genotypes", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 564, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.compute_genotypes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 545, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 564, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_6compute_genotypes(__pyx_self, __pyx_v_readset, __pyx_v_positions);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -14701,306 +15139,306 @@
   PyObject *__pyx_t_19 = NULL;
   PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("compute_genotypes", 0);
 
-  /* "whatshap/core.pyx":546
+  /* "whatshap/core.pyx":565
  * 
  * def compute_genotypes(ReadSet readset, positions = None):
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()             # <<<<<<<<<<<<<<
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  * 	cdef vector[unsigned int]* c_positions = NULL
  */
   try {
     __pyx_t_1 = new std::vector<Genotype> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 546, __pyx_L1_error)
+    __PYX_ERR(1, 565, __pyx_L1_error)
   }
   __pyx_v_genotypes_vector = __pyx_t_1;
 
-  /* "whatshap/core.pyx":547
+  /* "whatshap/core.pyx":566
  * def compute_genotypes(ReadSet readset, positions = None):
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()             # <<<<<<<<<<<<<<
  * 	cdef vector[unsigned int]* c_positions = NULL
  * 	if positions is not None:
  */
   try {
     __pyx_t_2 = new std::vector<GenotypeDistribution> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 547, __pyx_L1_error)
+    __PYX_ERR(1, 566, __pyx_L1_error)
   }
   __pyx_v_gl_vector = __pyx_t_2;
 
-  /* "whatshap/core.pyx":548
+  /* "whatshap/core.pyx":567
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  * 	cdef vector[unsigned int]* c_positions = NULL             # <<<<<<<<<<<<<<
  * 	if positions is not None:
  * 		c_positions = new vector[unsigned int]()
  */
   __pyx_v_c_positions = NULL;
 
-  /* "whatshap/core.pyx":549
+  /* "whatshap/core.pyx":568
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  * 	cdef vector[unsigned int]* c_positions = NULL
  * 	if positions is not None:             # <<<<<<<<<<<<<<
  * 		c_positions = new vector[unsigned int]()
  * 		for pos in positions:
  */
   __pyx_t_3 = (__pyx_v_positions != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "whatshap/core.pyx":550
+    /* "whatshap/core.pyx":569
  * 	cdef vector[unsigned int]* c_positions = NULL
  * 	if positions is not None:
  * 		c_positions = new vector[unsigned int]()             # <<<<<<<<<<<<<<
  * 		for pos in positions:
  * 			c_positions.push_back(pos)
  */
     try {
       __pyx_t_5 = new std::vector<unsigned int> ();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 550, __pyx_L1_error)
+      __PYX_ERR(1, 569, __pyx_L1_error)
     }
     __pyx_v_c_positions = __pyx_t_5;
 
-    /* "whatshap/core.pyx":551
+    /* "whatshap/core.pyx":570
  * 	if positions is not None:
  * 		c_positions = new vector[unsigned int]()
  * 		for pos in positions:             # <<<<<<<<<<<<<<
  * 			c_positions.push_back(pos)
  * 	cpp.compute_genotypes(readset.thisptr[0], genotypes_vector, gl_vector, c_positions)
  */
     if (likely(PyList_CheckExact(__pyx_v_positions)) || PyTuple_CheckExact(__pyx_v_positions)) {
       __pyx_t_6 = __pyx_v_positions; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
       __pyx_t_8 = NULL;
     } else {
-      __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 551, __pyx_L1_error)
+      __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 570, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 551, __pyx_L1_error)
+      __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 570, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_8)) {
         if (likely(PyList_CheckExact(__pyx_t_6))) {
           if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 551, __pyx_L1_error)
+          __pyx_t_9 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 570, __pyx_L1_error)
           #else
-          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 551, __pyx_L1_error)
+          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 570, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         } else {
           if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 551, __pyx_L1_error)
+          __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(1, 570, __pyx_L1_error)
           #else
-          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 551, __pyx_L1_error)
+          __pyx_t_9 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 570, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           #endif
         }
       } else {
         __pyx_t_9 = __pyx_t_8(__pyx_t_6);
         if (unlikely(!__pyx_t_9)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 551, __pyx_L1_error)
+            else __PYX_ERR(1, 570, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_9);
       }
       __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "whatshap/core.pyx":552
+      /* "whatshap/core.pyx":571
  * 		c_positions = new vector[unsigned int]()
  * 		for pos in positions:
  * 			c_positions.push_back(pos)             # <<<<<<<<<<<<<<
  * 	cpp.compute_genotypes(readset.thisptr[0], genotypes_vector, gl_vector, c_positions)
  * 	# TODO: Inefficient
  */
-      __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 552, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_10 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 571, __pyx_L1_error)
       try {
         __pyx_v_c_positions->push_back(__pyx_t_10);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 552, __pyx_L1_error)
+        __PYX_ERR(1, 571, __pyx_L1_error)
       }
 
-      /* "whatshap/core.pyx":551
+      /* "whatshap/core.pyx":570
  * 	if positions is not None:
  * 		c_positions = new vector[unsigned int]()
  * 		for pos in positions:             # <<<<<<<<<<<<<<
  * 			c_positions.push_back(pos)
  * 	cpp.compute_genotypes(readset.thisptr[0], genotypes_vector, gl_vector, c_positions)
  */
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "whatshap/core.pyx":549
+    /* "whatshap/core.pyx":568
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  * 	cdef vector[unsigned int]* c_positions = NULL
  * 	if positions is not None:             # <<<<<<<<<<<<<<
  * 		c_positions = new vector[unsigned int]()
  * 		for pos in positions:
  */
   }
 
-  /* "whatshap/core.pyx":553
+  /* "whatshap/core.pyx":572
  * 		for pos in positions:
  * 			c_positions.push_back(pos)
  * 	cpp.compute_genotypes(readset.thisptr[0], genotypes_vector, gl_vector, c_positions)             # <<<<<<<<<<<<<<
  * 	# TODO: Inefficient
  * 	genotypes = [Genotype(genotype.as_vector()) for genotype in genotypes_vector[0]]
  */
   try {
     compute_genotypes((__pyx_v_readset->thisptr[0]), __pyx_v_genotypes_vector, __pyx_v_gl_vector, __pyx_v_c_positions);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 553, __pyx_L1_error)
+    __PYX_ERR(1, 572, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":555
+  /* "whatshap/core.pyx":574
  * 	cpp.compute_genotypes(readset.thisptr[0], genotypes_vector, gl_vector, c_positions)
  * 	# TODO: Inefficient
  * 	genotypes = [Genotype(genotype.as_vector()) for genotype in genotypes_vector[0]]             # <<<<<<<<<<<<<<
  * 	#genotypes = list(genotypes_vector[0])
  * 	gls = [(gl_vector[0][i].probabilityOf(0), gl_vector[0][i].probabilityOf(1), gl_vector[0][i].probabilityOf(2)) for i in range(gl_vector[0].size())]
  */
   { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 555, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 574, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 = &(__pyx_v_genotypes_vector[0]);
     __pyx_t_11 = __pyx_t_1->begin();
     for (;;) {
       if (!(__pyx_t_11 != __pyx_t_1->end())) break;
       __pyx_t_12 = *__pyx_t_11;
       ++__pyx_t_11;
       __pyx_8genexpr6__pyx_v_genotype = __pyx_t_12;
       try {
         __pyx_t_13 = __pyx_8genexpr6__pyx_v_genotype.as_vector();
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 555, __pyx_L1_error)
+        __PYX_ERR(1, 574, __pyx_L1_error)
       }
-      __pyx_t_9 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 555, __pyx_L1_error)
+      __pyx_t_9 = __pyx_convert_vector_to_py_uint32_t(__pyx_t_13); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 574, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_14 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_9); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 555, __pyx_L1_error)
+      __pyx_t_14 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8whatshap_4core_Genotype), __pyx_t_9); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 574, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_14))) __PYX_ERR(1, 555, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_14))) __PYX_ERR(1, 574, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     }
   } /* exit inner scope */
   __pyx_v_genotypes = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":557
+  /* "whatshap/core.pyx":576
  * 	genotypes = [Genotype(genotype.as_vector()) for genotype in genotypes_vector[0]]
  * 	#genotypes = list(genotypes_vector[0])
  * 	gls = [(gl_vector[0][i].probabilityOf(0), gl_vector[0][i].probabilityOf(1), gl_vector[0][i].probabilityOf(2)) for i in range(gl_vector[0].size())]             # <<<<<<<<<<<<<<
  * 	del genotypes_vector
  * 	del gl_vector
  */
   { /* enter inner scope */
-    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 557, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 576, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_15 = (__pyx_v_gl_vector[0]).size();
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_8genexpr7__pyx_v_i = __pyx_t_17;
       try {
         __pyx_t_18 = ((__pyx_v_gl_vector[0])[__pyx_8genexpr7__pyx_v_i]).probabilityOf(0);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 557, __pyx_L1_error)
+        __PYX_ERR(1, 576, __pyx_L1_error)
       }
-      __pyx_t_14 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 557, __pyx_L1_error)
+      __pyx_t_14 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 576, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       try {
         __pyx_t_18 = ((__pyx_v_gl_vector[0])[__pyx_8genexpr7__pyx_v_i]).probabilityOf(1);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 557, __pyx_L1_error)
+        __PYX_ERR(1, 576, __pyx_L1_error)
       }
-      __pyx_t_9 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 557, __pyx_L1_error)
+      __pyx_t_9 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 576, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       try {
         __pyx_t_18 = ((__pyx_v_gl_vector[0])[__pyx_8genexpr7__pyx_v_i]).probabilityOf(2);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 557, __pyx_L1_error)
+        __PYX_ERR(1, 576, __pyx_L1_error)
       }
-      __pyx_t_19 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(1, 557, __pyx_L1_error)
+      __pyx_t_19 = PyFloat_FromDouble(__pyx_t_18); if (unlikely(!__pyx_t_19)) __PYX_ERR(1, 576, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_19);
-      __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 557, __pyx_L1_error)
+      __pyx_t_20 = PyTuple_New(3); if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 576, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_20);
       __Pyx_GIVEREF(__pyx_t_14);
       PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_t_14);
       __Pyx_GIVEREF(__pyx_t_9);
       PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_9);
       __Pyx_GIVEREF(__pyx_t_19);
       PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_t_19);
       __pyx_t_14 = 0;
       __pyx_t_9 = 0;
       __pyx_t_19 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_20))) __PYX_ERR(1, 557, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_t_20))) __PYX_ERR(1, 576, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
     }
   } /* exit inner scope */
   __pyx_v_gls = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":558
+  /* "whatshap/core.pyx":577
  * 	#genotypes = list(genotypes_vector[0])
  * 	gls = [(gl_vector[0][i].probabilityOf(0), gl_vector[0][i].probabilityOf(1), gl_vector[0][i].probabilityOf(2)) for i in range(gl_vector[0].size())]
  * 	del genotypes_vector             # <<<<<<<<<<<<<<
  * 	del gl_vector
  * 	return genotypes, gls
  */
   delete __pyx_v_genotypes_vector;
 
-  /* "whatshap/core.pyx":559
+  /* "whatshap/core.pyx":578
  * 	gls = [(gl_vector[0][i].probabilityOf(0), gl_vector[0][i].probabilityOf(1), gl_vector[0][i].probabilityOf(2)) for i in range(gl_vector[0].size())]
  * 	del genotypes_vector
  * 	del gl_vector             # <<<<<<<<<<<<<<
  * 	return genotypes, gls
  * 
  */
   delete __pyx_v_gl_vector;
 
-  /* "whatshap/core.pyx":560
+  /* "whatshap/core.pyx":579
  * 	del genotypes_vector
  * 	del gl_vector
  * 	return genotypes, gls             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 560, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_genotypes);
   __Pyx_GIVEREF(__pyx_v_genotypes);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_genotypes);
   __Pyx_INCREF(__pyx_v_gls);
   __Pyx_GIVEREF(__pyx_v_gls);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_v_gls);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":545
+  /* "whatshap/core.pyx":564
  * 
  * 
  * def compute_genotypes(ReadSet readset, positions = None):             # <<<<<<<<<<<<<<
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  */
 
@@ -15018,15 +15456,15 @@
   __Pyx_XDECREF(__pyx_v_genotypes);
   __Pyx_XDECREF(__pyx_v_gls);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":564
+/* "whatshap/core.pyx":583
  * 
  * cdef class HapChatCore:
  * 	def __cinit__(self, ReadSet readset):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)
  * 	def __dealloc__(self):
  */
 
@@ -15055,32 +15493,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_readset)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 564, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 583, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_readset = ((struct __pyx_obj_8whatshap_4core_ReadSet *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 564, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 583, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.HapChatCore.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 564, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 583, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_11HapChatCore___cinit__(((struct __pyx_obj_8whatshap_4core_HapChatCore *)__pyx_v_self), __pyx_v_readset);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -15089,38 +15527,38 @@
 }
 
 static int __pyx_pf_8whatshap_4core_11HapChatCore___cinit__(struct __pyx_obj_8whatshap_4core_HapChatCore *__pyx_v_self, struct __pyx_obj_8whatshap_4core_ReadSet *__pyx_v_readset) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":565
+  /* "whatshap/core.pyx":584
  * cdef class HapChatCore:
  * 	def __cinit__(self, ReadSet readset):
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)             # <<<<<<<<<<<<<<
  * 	def __dealloc__(self):
  * 		del self.thisptr
  */
   __pyx_v_self->thisptr = new HapChatCore(__pyx_v_readset->thisptr);
 
-  /* "whatshap/core.pyx":564
+  /* "whatshap/core.pyx":583
  * 
  * cdef class HapChatCore:
  * 	def __cinit__(self, ReadSet readset):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)
  * 	def __dealloc__(self):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":566
+/* "whatshap/core.pyx":585
  * 	def __cinit__(self, ReadSet readset):
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 	def get_length(self):
  */
 
@@ -15135,36 +15573,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_11HapChatCore_2__dealloc__(struct __pyx_obj_8whatshap_4core_HapChatCore *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":567
+  /* "whatshap/core.pyx":586
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 	def get_length(self):
  * 		return self.thisptr.get_length()
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":566
+  /* "whatshap/core.pyx":585
  * 	def __cinit__(self, ReadSet readset):
  * 		self.thisptr = new cpp.HapChatCore(readset.thisptr)
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 	def get_length(self):
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":568
+/* "whatshap/core.pyx":587
  * 	def __dealloc__(self):
  * 		del self.thisptr
  * 	def get_length(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_length()
  * 	def get_super_reads(self):
  */
 
@@ -15186,29 +15624,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_length", 0);
 
-  /* "whatshap/core.pyx":569
+  /* "whatshap/core.pyx":588
  * 		del self.thisptr
  * 	def get_length(self):
  * 		return self.thisptr.get_length()             # <<<<<<<<<<<<<<
  * 	def get_super_reads(self):
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_length()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 569, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_length()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 588, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":568
+  /* "whatshap/core.pyx":587
  * 	def __dealloc__(self):
  * 		del self.thisptr
  * 	def get_length(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_length()
  * 	def get_super_reads(self):
  */
 
@@ -15219,15 +15657,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":570
+/* "whatshap/core.pyx":589
  * 	def get_length(self):
  * 		return self.thisptr.get_length()
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  * 		leng=self.thisptr.get_length()
  */
 
@@ -15262,165 +15700,165 @@
   std::vector<ReadSet *> ::size_type __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_super_reads", 0);
 
-  /* "whatshap/core.pyx":571
+  /* "whatshap/core.pyx":590
  * 		return self.thisptr.get_length()
  * 	def get_super_reads(self):
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()             # <<<<<<<<<<<<<<
  * 		leng=self.thisptr.get_length()
  * 		for i in range(leng):
  */
   try {
     __pyx_t_1 = new std::vector<ReadSet *> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 571, __pyx_L1_error)
+    __PYX_ERR(1, 590, __pyx_L1_error)
   }
   __pyx_v_read_sets = __pyx_t_1;
 
-  /* "whatshap/core.pyx":572
+  /* "whatshap/core.pyx":591
  * 	def get_super_reads(self):
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  * 		leng=self.thisptr.get_length()             # <<<<<<<<<<<<<<
  * 		for i in range(leng):
  * 			read_sets.push_back(new cpp.ReadSet())
  */
   __pyx_v_leng = __pyx_v_self->thisptr->get_length();
 
-  /* "whatshap/core.pyx":573
+  /* "whatshap/core.pyx":592
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  * 		leng=self.thisptr.get_length()
  * 		for i in range(leng):             # <<<<<<<<<<<<<<
  * 			read_sets.push_back(new cpp.ReadSet())
  * 		self.thisptr.get_super_reads(read_sets)
  */
   __pyx_t_2 = __pyx_v_leng;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "whatshap/core.pyx":574
+    /* "whatshap/core.pyx":593
  * 		leng=self.thisptr.get_length()
  * 		for i in range(leng):
  * 			read_sets.push_back(new cpp.ReadSet())             # <<<<<<<<<<<<<<
  * 		self.thisptr.get_super_reads(read_sets)
  * 
  */
     try {
       __pyx_t_5 = new ReadSet();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 574, __pyx_L1_error)
+      __PYX_ERR(1, 593, __pyx_L1_error)
     }
     try {
       __pyx_v_read_sets->push_back(__pyx_t_5);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 574, __pyx_L1_error)
+      __PYX_ERR(1, 593, __pyx_L1_error)
     }
   }
 
-  /* "whatshap/core.pyx":575
+  /* "whatshap/core.pyx":594
  * 		for i in range(leng):
  * 			read_sets.push_back(new cpp.ReadSet())
  * 		self.thisptr.get_super_reads(read_sets)             # <<<<<<<<<<<<<<
  * 
  * 		results = []
  */
   __pyx_v_self->thisptr->get_super_reads(__pyx_v_read_sets);
 
-  /* "whatshap/core.pyx":577
+  /* "whatshap/core.pyx":596
  * 		self.thisptr.get_super_reads(read_sets)
  * 
  * 		results = []             # <<<<<<<<<<<<<<
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()
  */
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 596, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_results = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
 
-  /* "whatshap/core.pyx":578
+  /* "whatshap/core.pyx":597
  * 
  * 		results = []
  * 		for i in range(read_sets.size()):             # <<<<<<<<<<<<<<
  * 			rs = ReadSet()
  * 			del rs.thisptr
  */
   __pyx_t_4 = __pyx_v_read_sets->size();
   __pyx_t_7 = __pyx_t_4;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_i = __pyx_t_8;
 
-    /* "whatshap/core.pyx":579
+    /* "whatshap/core.pyx":598
  * 		results = []
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()             # <<<<<<<<<<<<<<
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]
  */
-    __pyx_t_6 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 598, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_rs, ((struct __pyx_obj_8whatshap_4core_ReadSet *)__pyx_t_6));
     __pyx_t_6 = 0;
 
-    /* "whatshap/core.pyx":580
+    /* "whatshap/core.pyx":599
  * 		for i in range(read_sets.size()):
  * 			rs = ReadSet()
  * 			del rs.thisptr             # <<<<<<<<<<<<<<
  * 			rs.thisptr = deref(read_sets)[i]
  * 			results.append(rs)
  */
     delete __pyx_v_rs->thisptr;
 
-    /* "whatshap/core.pyx":581
+    /* "whatshap/core.pyx":600
  * 			rs = ReadSet()
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]             # <<<<<<<<<<<<<<
  * 			results.append(rs)
  * 
  */
     __pyx_v_rs->thisptr = ((*__pyx_v_read_sets)[__pyx_v_i]);
 
-    /* "whatshap/core.pyx":582
+    /* "whatshap/core.pyx":601
  * 			del rs.thisptr
  * 			rs.thisptr = deref(read_sets)[i]
  * 			results.append(rs)             # <<<<<<<<<<<<<<
  * 
  * 		return results, None
  */
-    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 582, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 601, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":584
+  /* "whatshap/core.pyx":603
  * 			results.append(rs)
  * 
  * 		return results, None             # <<<<<<<<<<<<<<
  * 	def get_optimal_cost(self):
  * 		return self.thisptr.get_optimal_cost()
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 584, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_v_results);
   __Pyx_GIVEREF(__pyx_v_results);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_v_results);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_6, 1, Py_None);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":570
+  /* "whatshap/core.pyx":589
  * 	def get_length(self):
  * 		return self.thisptr.get_length()
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[cpp.ReadSet*]* read_sets = new vector[cpp.ReadSet*]()
  * 		leng=self.thisptr.get_length()
  */
 
@@ -15433,15 +15871,15 @@
   __Pyx_XDECREF(__pyx_v_results);
   __Pyx_XDECREF((PyObject *)__pyx_v_rs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":585
+/* "whatshap/core.pyx":604
  * 
  * 		return results, None
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_optimal_cost()
  * 	def get_optimal_partitioning(self):
  */
 
@@ -15463,29 +15901,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_cost", 0);
 
-  /* "whatshap/core.pyx":586
+  /* "whatshap/core.pyx":605
  * 		return results, None
  * 	def get_optimal_cost(self):
  * 		return self.thisptr.get_optimal_cost()             # <<<<<<<<<<<<<<
  * 	def get_optimal_partitioning(self):
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_optimal_cost()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 586, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->thisptr->get_optimal_cost()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":585
+  /* "whatshap/core.pyx":604
  * 
  * 		return results, None
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		return self.thisptr.get_optimal_cost()
  * 	def get_optimal_partitioning(self):
  */
 
@@ -15496,15 +15934,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":587
+/* "whatshap/core.pyx":606
  * 	def get_optimal_cost(self):
  * 		return self.thisptr.get_optimal_cost()
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = ['*' for x in p[0]]
  */
 
@@ -15532,68 +15970,68 @@
   std::vector<bool>  *__pyx_t_3;
   bool __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_partitioning", 0);
 
-  /* "whatshap/core.pyx":588
+  /* "whatshap/core.pyx":607
  * 		return self.thisptr.get_optimal_cost()
  * 	def get_optimal_partitioning(self):
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()             # <<<<<<<<<<<<<<
  * 		result = ['*' for x in p[0]]
  * 		del p
  */
   __pyx_v_p = __pyx_v_self->thisptr->get_optimal_partitioning();
 
-  /* "whatshap/core.pyx":589
+  /* "whatshap/core.pyx":608
  * 	def get_optimal_partitioning(self):
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = ['*' for x in p[0]]             # <<<<<<<<<<<<<<
  * 		del p
  * 		return result
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 589, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 608, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = &(__pyx_v_p[0]);
     __pyx_t_2 = __pyx_t_3->begin();
     for (;;) {
       if (!(__pyx_t_2 != __pyx_t_3->end())) break;
       __pyx_t_4 = *__pyx_t_2;
       ++__pyx_t_2;
       __pyx_8genexpr8__pyx_v_x = __pyx_t_4;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_kp_u__22))) __PYX_ERR(1, 589, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_kp_u__22))) __PYX_ERR(1, 608, __pyx_L1_error)
     }
   } /* exit inner scope */
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":590
+  /* "whatshap/core.pyx":609
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = ['*' for x in p[0]]
  * 		del p             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_p;
 
-  /* "whatshap/core.pyx":591
+  /* "whatshap/core.pyx":610
  * 		result = ['*' for x in p[0]]
  * 		del p
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * cdef class Caller:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":587
+  /* "whatshap/core.pyx":606
  * 	def get_optimal_cost(self):
  * 		return self.thisptr.get_optimal_cost()
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		cdef vector[bool]* p = self.thisptr.get_optimal_partitioning()
  * 		result = ['*' for x in p[0]]
  */
 
@@ -15718,15 +16156,15 @@
   __Pyx_AddTraceback("whatshap.core.HapChatCore.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":594
+/* "whatshap/core.pyx":613
  * 
  * cdef class Caller:
  * 	def __cinit__(self, string reference, int k, int window ):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Caller(reference, k, window)
  * 
  */
 
@@ -15763,40 +16201,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_reference)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_k)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(1, 594, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(1, 613, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_window)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(1, 594, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(1, 613, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 594, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 613, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
-    __pyx_v_reference = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 594, __pyx_L3_error)
-    __pyx_v_k = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 594, __pyx_L3_error)
-    __pyx_v_window = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_window == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 594, __pyx_L3_error)
+    __pyx_v_reference = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 613, __pyx_L3_error)
+    __pyx_v_k = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 613, __pyx_L3_error)
+    __pyx_v_window = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_window == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 613, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 594, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 613, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Caller.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_6Caller___cinit__(((struct __pyx_obj_8whatshap_4core_Caller *)__pyx_v_self), __pyx_v_reference, __pyx_v_k, __pyx_v_window);
 
@@ -15810,30 +16248,30 @@
   __Pyx_RefNannyDeclarations
   Caller *__pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":595
+  /* "whatshap/core.pyx":614
  * cdef class Caller:
  * 	def __cinit__(self, string reference, int k, int window ):
  * 		self.thisptr = new cpp.Caller(reference, k, window)             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   try {
     __pyx_t_1 = new Caller(__pyx_v_reference, __pyx_v_k, __pyx_v_window);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 595, __pyx_L1_error)
+    __PYX_ERR(1, 614, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_1;
 
-  /* "whatshap/core.pyx":594
+  /* "whatshap/core.pyx":613
  * 
  * cdef class Caller:
  * 	def __cinit__(self, string reference, int k, int window ):             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.Caller(reference, k, window)
  * 
  */
 
@@ -15844,15 +16282,15 @@
   __Pyx_AddTraceback("whatshap.core.Caller.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":597
+/* "whatshap/core.pyx":616
  * 		self.thisptr = new cpp.Caller(reference, k, window)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -15867,36 +16305,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_6Caller_2__dealloc__(struct __pyx_obj_8whatshap_4core_Caller *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":598
+  /* "whatshap/core.pyx":617
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def all_variants(self, vector[pair[int,int]] variants_list):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":597
+  /* "whatshap/core.pyx":616
  * 		self.thisptr = new cpp.Caller(reference, k, window)
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":600
+/* "whatshap/core.pyx":619
  * 		del self.thisptr
  * 
  * 	def all_variants(self, vector[pair[int,int]] variants_list):             # <<<<<<<<<<<<<<
  * 		cdef deque[pair[int,int]] v_list
  * 		for v in variants_list:
  */
 
@@ -15907,15 +16345,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("all_variants (wrapper)", 0);
   assert(__pyx_arg_variants_list); {
-    __pyx_v_variants_list = __pyx_convert_vector_from_py_std_3a__3a_pair_3c_int_2c_int_3e___(__pyx_arg_variants_list); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 600, __pyx_L3_error)
+    __pyx_v_variants_list = __pyx_convert_vector_from_py_std_3a__3a_pair_3c_int_2c_int_3e___(__pyx_arg_variants_list); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 619, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Caller.all_variants", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -15934,61 +16372,61 @@
   std::vector<std::pair<int,int> > ::iterator __pyx_t_1;
   std::pair<int,int>  __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("all_variants", 0);
 
-  /* "whatshap/core.pyx":602
+  /* "whatshap/core.pyx":621
  * 	def all_variants(self, vector[pair[int,int]] variants_list):
  * 		cdef deque[pair[int,int]] v_list
  * 		for v in variants_list:             # <<<<<<<<<<<<<<
  * 			v_list.push_back(v)
  * 		self.thisptr.all_variants(v_list)
  */
   __pyx_t_1 = __pyx_v_variants_list.begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_v_variants_list.end())) break;
     __pyx_t_2 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_v = __pyx_t_2;
 
-    /* "whatshap/core.pyx":603
+    /* "whatshap/core.pyx":622
  * 		cdef deque[pair[int,int]] v_list
  * 		for v in variants_list:
  * 			v_list.push_back(v)             # <<<<<<<<<<<<<<
  * 		self.thisptr.all_variants(v_list)
  * 
  */
     __pyx_v_v_list.push_back(__pyx_v_v);
 
-    /* "whatshap/core.pyx":602
+    /* "whatshap/core.pyx":621
  * 	def all_variants(self, vector[pair[int,int]] variants_list):
  * 		cdef deque[pair[int,int]] v_list
  * 		for v in variants_list:             # <<<<<<<<<<<<<<
  * 			v_list.push_back(v)
  * 		self.thisptr.all_variants(v_list)
  */
   }
 
-  /* "whatshap/core.pyx":604
+  /* "whatshap/core.pyx":623
  * 		for v in variants_list:
  * 			v_list.push_back(v)
  * 		self.thisptr.all_variants(v_list)             # <<<<<<<<<<<<<<
  * 
  * 	def add_read(self, int bam_alignment_pos, vector[vector[int]]  bam_alignment_cigartuples, string bam_alignment_query, string outfile):
  */
   try {
     __pyx_v_self->thisptr->all_variants(__pyx_v_v_list);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 604, __pyx_L1_error)
+    __PYX_ERR(1, 623, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":600
+  /* "whatshap/core.pyx":619
  * 		del self.thisptr
  * 
  * 	def all_variants(self, vector[pair[int,int]] variants_list):             # <<<<<<<<<<<<<<
  * 		cdef deque[pair[int,int]] v_list
  * 		for v in variants_list:
  */
 
@@ -16000,15 +16438,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":606
+/* "whatshap/core.pyx":625
  * 		self.thisptr.all_variants(v_list)
  * 
  * 	def add_read(self, int bam_alignment_pos, vector[vector[int]]  bam_alignment_cigartuples, string bam_alignment_query, string outfile):             # <<<<<<<<<<<<<<
  * 		self.thisptr.add_read(bam_alignment_pos, bam_alignment_cigartuples, bam_alignment_query, outfile)
  * 
  */
 
@@ -16048,48 +16486,48 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bam_alignment_pos)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bam_alignment_cigartuples)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 1); __PYX_ERR(1, 606, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 1); __PYX_ERR(1, 625, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bam_alignment_query)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 2); __PYX_ERR(1, 606, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 2); __PYX_ERR(1, 625, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_outfile)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 3); __PYX_ERR(1, 606, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, 3); __PYX_ERR(1, 625, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_read") < 0)) __PYX_ERR(1, 606, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "add_read") < 0)) __PYX_ERR(1, 625, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
-    __pyx_v_bam_alignment_pos = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_bam_alignment_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 606, __pyx_L3_error)
-    __pyx_v_bam_alignment_cigartuples = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 606, __pyx_L3_error)
-    __pyx_v_bam_alignment_query = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 606, __pyx_L3_error)
-    __pyx_v_outfile = __pyx_convert_string_from_py_std__in_string(values[3]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 606, __pyx_L3_error)
+    __pyx_v_bam_alignment_pos = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_bam_alignment_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 625, __pyx_L3_error)
+    __pyx_v_bam_alignment_cigartuples = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_int_3e___(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 625, __pyx_L3_error)
+    __pyx_v_bam_alignment_query = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 625, __pyx_L3_error)
+    __pyx_v_outfile = __pyx_convert_string_from_py_std__in_string(values[3]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 625, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 606, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_read", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 625, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Caller.add_read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8whatshap_4core_6Caller_6add_read(((struct __pyx_obj_8whatshap_4core_Caller *)__pyx_v_self), __pyx_v_bam_alignment_pos, __pyx_v_bam_alignment_cigartuples, __pyx_v_bam_alignment_query, __pyx_v_outfile);
 
@@ -16102,29 +16540,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_read", 0);
 
-  /* "whatshap/core.pyx":607
+  /* "whatshap/core.pyx":626
  * 
  * 	def add_read(self, int bam_alignment_pos, vector[vector[int]]  bam_alignment_cigartuples, string bam_alignment_query, string outfile):
  * 		self.thisptr.add_read(bam_alignment_pos, bam_alignment_cigartuples, bam_alignment_query, outfile)             # <<<<<<<<<<<<<<
  * 
  * 	def final_pop(self, string outfile):
  */
   try {
     __pyx_v_self->thisptr->add_read(__pyx_v_bam_alignment_pos, __pyx_v_bam_alignment_cigartuples, __pyx_v_bam_alignment_query, __pyx_v_outfile);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 607, __pyx_L1_error)
+    __PYX_ERR(1, 626, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":606
+  /* "whatshap/core.pyx":625
  * 		self.thisptr.all_variants(v_list)
  * 
  * 	def add_read(self, int bam_alignment_pos, vector[vector[int]]  bam_alignment_cigartuples, string bam_alignment_query, string outfile):             # <<<<<<<<<<<<<<
  * 		self.thisptr.add_read(bam_alignment_pos, bam_alignment_cigartuples, bam_alignment_query, outfile)
  * 
  */
 
@@ -16136,15 +16574,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":609
+/* "whatshap/core.pyx":628
  * 		self.thisptr.add_read(bam_alignment_pos, bam_alignment_cigartuples, bam_alignment_query, outfile)
  * 
  * 	def final_pop(self, string outfile):             # <<<<<<<<<<<<<<
  * 		self.thisptr.final_pop(outfile)
  * 
  */
 
@@ -16155,15 +16593,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("final_pop (wrapper)", 0);
   assert(__pyx_arg_outfile); {
-    __pyx_v_outfile = __pyx_convert_string_from_py_std__in_string(__pyx_arg_outfile); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 609, __pyx_L3_error)
+    __pyx_v_outfile = __pyx_convert_string_from_py_std__in_string(__pyx_arg_outfile); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 628, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.Caller.final_pop", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -16178,29 +16616,29 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("final_pop", 0);
 
-  /* "whatshap/core.pyx":610
+  /* "whatshap/core.pyx":629
  * 
  * 	def final_pop(self, string outfile):
  * 		self.thisptr.final_pop(outfile)             # <<<<<<<<<<<<<<
  * 
  * 	def finish(self):
  */
   try {
     __pyx_v_self->thisptr->final_pop(__pyx_v_outfile);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 610, __pyx_L1_error)
+    __PYX_ERR(1, 629, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":609
+  /* "whatshap/core.pyx":628
  * 		self.thisptr.add_read(bam_alignment_pos, bam_alignment_cigartuples, bam_alignment_query, outfile)
  * 
  * 	def final_pop(self, string outfile):             # <<<<<<<<<<<<<<
  * 		self.thisptr.final_pop(outfile)
  * 
  */
 
@@ -16212,15 +16650,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":612
+/* "whatshap/core.pyx":631
  * 		self.thisptr.final_pop(outfile)
  * 
  * 	def finish(self):             # <<<<<<<<<<<<<<
  * 		pass
  * 
  */
 
@@ -16358,15 +16796,15 @@
   __Pyx_AddTraceback("whatshap.core.Caller.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":617
+/* "whatshap/core.pyx":636
  * 
  * cdef class PedMecHeuristic:
  * 	def __cinit__(self, ReadSet readset, vector[unsigned int] recombcost, Pedigree pedigree, int row_limit = 256, bool distrust_genotypes = False, positions = None, bool allow_mutations = True, int verbosity = 0):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -16419,21 +16857,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_readset)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_recombcost)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, 1); __PYX_ERR(1, 617, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, 1); __PYX_ERR(1, 636, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pedigree)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, 2); __PYX_ERR(1, 617, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, 2); __PYX_ERR(1, 636, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_row_limit);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -16459,15 +16897,15 @@
         case  7:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_verbosity);
           if (value) { values[7] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 617, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(1, 636, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
         CYTHON_FALLTHROUGH;
@@ -16481,48 +16919,48 @@
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_readset = ((struct __pyx_obj_8whatshap_4core_ReadSet *)values[0]);
-    __pyx_v_recombcost = __pyx_convert_vector_from_py_unsigned_int(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 617, __pyx_L3_error)
+    __pyx_v_recombcost = __pyx_convert_vector_from_py_unsigned_int(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L3_error)
     __pyx_v_pedigree = ((struct __pyx_obj_8whatshap_4core_Pedigree *)values[2]);
     if (values[3]) {
-      __pyx_v_row_limit = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_row_limit == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 617, __pyx_L3_error)
+      __pyx_v_row_limit = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_row_limit == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L3_error)
     } else {
       __pyx_v_row_limit = ((int)0x100);
     }
     if (values[4]) {
-      __pyx_v_distrust_genotypes = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_distrust_genotypes == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 617, __pyx_L3_error)
+      __pyx_v_distrust_genotypes = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_distrust_genotypes == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L3_error)
     } else {
       __pyx_v_distrust_genotypes = ((bool)0);
     }
     __pyx_v_positions = values[5];
     if (values[6]) {
-      __pyx_v_allow_mutations = __Pyx_PyObject_IsTrue(values[6]); if (unlikely((__pyx_v_allow_mutations == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 617, __pyx_L3_error)
+      __pyx_v_allow_mutations = __Pyx_PyObject_IsTrue(values[6]); if (unlikely((__pyx_v_allow_mutations == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L3_error)
     } else {
       __pyx_v_allow_mutations = ((bool)1);
     }
     if (values[7]) {
-      __pyx_v_verbosity = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_verbosity == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 617, __pyx_L3_error)
+      __pyx_v_verbosity = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_verbosity == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 636, __pyx_L3_error)
     } else {
       __pyx_v_verbosity = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 617, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 8, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 636, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("whatshap.core.PedMecHeuristic.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 617, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 617, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_readset), __pyx_ptype_8whatshap_4core_ReadSet, 1, "readset", 0))) __PYX_ERR(1, 636, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pedigree), __pyx_ptype_8whatshap_4core_Pedigree, 1, "pedigree", 0))) __PYX_ERR(1, 636, __pyx_L1_error)
   __pyx_r = __pyx_pf_8whatshap_4core_15PedMecHeuristic___cinit__(((struct __pyx_obj_8whatshap_4core_PedMecHeuristic *)__pyx_v_self), __pyx_v_readset, __pyx_v_recombcost, __pyx_v_pedigree, __pyx_v_row_limit, __pyx_v_distrust_genotypes, __pyx_v_positions, __pyx_v_allow_mutations, __pyx_v_verbosity);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -16545,161 +16983,161 @@
   unsigned int __pyx_t_8;
   PedMecHeuristic *__pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "whatshap/core.pyx":622
+  /* "whatshap/core.pyx":641
  * 		in the read set must also be sorted (by position of their left-most variant).
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL             # <<<<<<<<<<<<<<
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  */
   __pyx_v_c_positions = NULL;
 
-  /* "whatshap/core.pyx":623
+  /* "whatshap/core.pyx":642
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   __pyx_t_1 = (__pyx_v_positions != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "whatshap/core.pyx":624
+    /* "whatshap/core.pyx":643
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()             # <<<<<<<<<<<<<<
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  */
     try {
       __pyx_t_3 = new std::vector<unsigned int> ();
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(1, 624, __pyx_L1_error)
+      __PYX_ERR(1, 643, __pyx_L1_error)
     }
     __pyx_v_c_positions = __pyx_t_3;
 
-    /* "whatshap/core.pyx":625
+    /* "whatshap/core.pyx":644
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedMecHeuristic(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions, row_limit, allow_mutations, verbosity)
  */
     if (likely(PyList_CheckExact(__pyx_v_positions)) || PyTuple_CheckExact(__pyx_v_positions)) {
       __pyx_t_4 = __pyx_v_positions; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 625, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_positions); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 644, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 625, __pyx_L1_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 644, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 625, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 644, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 625, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 644, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 625, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(1, 644, __pyx_L1_error)
           #else
-          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 625, __pyx_L1_error)
+          __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 644, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 625, __pyx_L1_error)
+            else __PYX_ERR(1, 644, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XDECREF_SET(__pyx_v_pos, __pyx_t_7);
       __pyx_t_7 = 0;
 
-      /* "whatshap/core.pyx":626
+      /* "whatshap/core.pyx":645
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  * 				c_positions.push_back(pos)             # <<<<<<<<<<<<<<
  * 		self.thisptr = new cpp.PedMecHeuristic(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions, row_limit, allow_mutations, verbosity)
  * 		self.pedigree = pedigree
  */
-      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 626, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_As_unsigned_int(__pyx_v_pos); if (unlikely((__pyx_t_8 == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(1, 645, __pyx_L1_error)
       try {
         __pyx_v_c_positions->push_back(__pyx_t_8);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(1, 626, __pyx_L1_error)
+        __PYX_ERR(1, 645, __pyx_L1_error)
       }
 
-      /* "whatshap/core.pyx":625
+      /* "whatshap/core.pyx":644
  * 		if positions is not None:
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:             # <<<<<<<<<<<<<<
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedMecHeuristic(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions, row_limit, allow_mutations, verbosity)
  */
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "whatshap/core.pyx":623
+    /* "whatshap/core.pyx":642
  * 		"""
  * 		cdef vector[unsigned int]* c_positions = NULL
  * 		if positions is not None:             # <<<<<<<<<<<<<<
  * 			c_positions = new vector[unsigned int]()
  * 			for pos in positions:
  */
   }
 
-  /* "whatshap/core.pyx":627
+  /* "whatshap/core.pyx":646
  * 			for pos in positions:
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedMecHeuristic(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions, row_limit, allow_mutations, verbosity)             # <<<<<<<<<<<<<<
  * 		self.pedigree = pedigree
  * 
  */
   try {
     __pyx_t_9 = new PedMecHeuristic(__pyx_v_readset->thisptr, __pyx_v_recombcost, __pyx_v_pedigree->thisptr, __pyx_v_distrust_genotypes, __pyx_v_c_positions, __pyx_v_row_limit, __pyx_v_allow_mutations, __pyx_v_verbosity);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 627, __pyx_L1_error)
+    __PYX_ERR(1, 646, __pyx_L1_error)
   }
   __pyx_v_self->thisptr = __pyx_t_9;
 
-  /* "whatshap/core.pyx":628
+  /* "whatshap/core.pyx":647
  * 				c_positions.push_back(pos)
  * 		self.thisptr = new cpp.PedMecHeuristic(readset.thisptr, recombcost, pedigree.thisptr, distrust_genotypes, c_positions, row_limit, allow_mutations, verbosity)
  * 		self.pedigree = pedigree             # <<<<<<<<<<<<<<
  * 
  * 	def __dealloc__(self):
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_pedigree));
   __Pyx_GOTREF(__pyx_v_self->pedigree);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->pedigree));
   __pyx_v_self->pedigree = __pyx_v_pedigree;
 
-  /* "whatshap/core.pyx":617
+  /* "whatshap/core.pyx":636
  * 
  * cdef class PedMecHeuristic:
  * 	def __cinit__(self, ReadSet readset, vector[unsigned int] recombcost, Pedigree pedigree, int row_limit = 256, bool distrust_genotypes = False, positions = None, bool allow_mutations = True, int verbosity = 0):             # <<<<<<<<<<<<<<
  * 		"""Build the DP table from the given read set which is assumed to be sorted;
  * 		that is, the variants in each read must be sorted by position and the reads
  */
 
@@ -16713,15 +17151,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pos);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":630
+/* "whatshap/core.pyx":649
  * 		self.pedigree = pedigree
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
@@ -16736,36 +17174,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8whatshap_4core_15PedMecHeuristic_2__dealloc__(struct __pyx_obj_8whatshap_4core_PedMecHeuristic *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "whatshap/core.pyx":631
+  /* "whatshap/core.pyx":650
  * 
  * 	def __dealloc__(self):
  * 		del self.thisptr             # <<<<<<<<<<<<<<
  * 
  * 	def get_super_reads(self):
  */
   delete __pyx_v_self->thisptr;
 
-  /* "whatshap/core.pyx":630
+  /* "whatshap/core.pyx":649
  * 		self.pedigree = pedigree
  * 
  * 	def __dealloc__(self):             # <<<<<<<<<<<<<<
  * 		del self.thisptr
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "whatshap/core.pyx":633
+/* "whatshap/core.pyx":652
  * 		del self.thisptr
  * 
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		#Interface is identical to PedigreeDPTable
  * 
  */
 
@@ -16800,181 +17238,181 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_super_reads", 0);
 
-  /* "whatshap/core.pyx":636
+  /* "whatshap/core.pyx":655
  * 		#Interface is identical to PedigreeDPTable
  * 
  * 		cdef vector[cpp.ReadSet*]* readSets = new vector[cpp.ReadSet*]()             # <<<<<<<<<<<<<<
  * 		cdef vector[uint32_t]* opt_trans_ptr
  * 		self.thisptr.solve()
  */
   try {
     __pyx_t_1 = new std::vector<ReadSet *> ();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 636, __pyx_L1_error)
+    __PYX_ERR(1, 655, __pyx_L1_error)
   }
   __pyx_v_readSets = __pyx_t_1;
 
-  /* "whatshap/core.pyx":638
+  /* "whatshap/core.pyx":657
  * 		cdef vector[cpp.ReadSet*]* readSets = new vector[cpp.ReadSet*]()
  * 		cdef vector[uint32_t]* opt_trans_ptr
  * 		self.thisptr.solve()             # <<<<<<<<<<<<<<
  * 
  * 		opt_trans_ptr = self.thisptr.getOptTransmission()
  */
   try {
     __pyx_v_self->thisptr->solve();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 638, __pyx_L1_error)
+    __PYX_ERR(1, 657, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":640
+  /* "whatshap/core.pyx":659
  * 		self.thisptr.solve()
  * 
  * 		opt_trans_ptr = self.thisptr.getOptTransmission()             # <<<<<<<<<<<<<<
  * 		self.thisptr.getSuperReads(readSets)
  * 
  */
   try {
     __pyx_t_2 = __pyx_v_self->thisptr->getOptTransmission();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 640, __pyx_L1_error)
+    __PYX_ERR(1, 659, __pyx_L1_error)
   }
   __pyx_v_opt_trans_ptr = __pyx_t_2;
 
-  /* "whatshap/core.pyx":641
+  /* "whatshap/core.pyx":660
  * 
  * 		opt_trans_ptr = self.thisptr.getOptTransmission()
  * 		self.thisptr.getSuperReads(readSets)             # <<<<<<<<<<<<<<
  * 
  * 		results = []
  */
   try {
     __pyx_v_self->thisptr->getSuperReads(__pyx_v_readSets);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 641, __pyx_L1_error)
+    __PYX_ERR(1, 660, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":643
+  /* "whatshap/core.pyx":662
  * 		self.thisptr.getSuperReads(readSets)
  * 
  * 		results = []             # <<<<<<<<<<<<<<
  * 		for i in range(readSets.size()):
  * 			rs = ReadSet()
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 643, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_results = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "whatshap/core.pyx":644
+  /* "whatshap/core.pyx":663
  * 
  * 		results = []
  * 		for i in range(readSets.size()):             # <<<<<<<<<<<<<<
  * 			rs = ReadSet()
  * 			del rs.thisptr
  */
   __pyx_t_4 = __pyx_v_readSets->size();
   __pyx_t_5 = __pyx_t_4;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "whatshap/core.pyx":645
+    /* "whatshap/core.pyx":664
  * 		results = []
  * 		for i in range(readSets.size()):
  * 			rs = ReadSet()             # <<<<<<<<<<<<<<
  * 			del rs.thisptr
  * 			rs.thisptr = deref(readSets)[i]
  */
-    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 645, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_8whatshap_4core_ReadSet)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 664, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_rs, ((struct __pyx_obj_8whatshap_4core_ReadSet *)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "whatshap/core.pyx":646
+    /* "whatshap/core.pyx":665
  * 		for i in range(readSets.size()):
  * 			rs = ReadSet()
  * 			del rs.thisptr             # <<<<<<<<<<<<<<
  * 			rs.thisptr = deref(readSets)[i]
  * 			results.append(rs)
  */
     delete __pyx_v_rs->thisptr;
 
-    /* "whatshap/core.pyx":647
+    /* "whatshap/core.pyx":666
  * 			rs = ReadSet()
  * 			del rs.thisptr
  * 			rs.thisptr = deref(readSets)[i]             # <<<<<<<<<<<<<<
  * 			results.append(rs)
  * 
  */
     __pyx_v_rs->thisptr = ((*__pyx_v_readSets)[__pyx_v_i]);
 
-    /* "whatshap/core.pyx":648
+    /* "whatshap/core.pyx":667
  * 			del rs.thisptr
  * 			rs.thisptr = deref(readSets)[i]
  * 			results.append(rs)             # <<<<<<<<<<<<<<
  * 
  * 		python_transmission_vector = list(opt_trans_ptr[0])
  */
-    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 648, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyList_Append(__pyx_v_results, ((PyObject *)__pyx_v_rs)); if (unlikely(__pyx_t_7 == ((int)-1))) __PYX_ERR(1, 667, __pyx_L1_error)
   }
 
-  /* "whatshap/core.pyx":650
+  /* "whatshap/core.pyx":669
  * 			results.append(rs)
  * 
  * 		python_transmission_vector = list(opt_trans_ptr[0])             # <<<<<<<<<<<<<<
  * 		del opt_trans_ptr
  * 		return results, python_transmission_vector
  */
-  __pyx_t_3 = __pyx_convert_vector_to_py_uint32_t((__pyx_v_opt_trans_ptr[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 650, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_vector_to_py_uint32_t((__pyx_v_opt_trans_ptr[0])); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 650, __pyx_L1_error)
+  __pyx_t_8 = PySequence_List(__pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_python_transmission_vector = ((PyObject*)__pyx_t_8);
   __pyx_t_8 = 0;
 
-  /* "whatshap/core.pyx":651
+  /* "whatshap/core.pyx":670
  * 
  * 		python_transmission_vector = list(opt_trans_ptr[0])
  * 		del opt_trans_ptr             # <<<<<<<<<<<<<<
  * 		return results, python_transmission_vector
  * 
  */
   delete __pyx_v_opt_trans_ptr;
 
-  /* "whatshap/core.pyx":652
+  /* "whatshap/core.pyx":671
  * 		python_transmission_vector = list(opt_trans_ptr[0])
  * 		del opt_trans_ptr
  * 		return results, python_transmission_vector             # <<<<<<<<<<<<<<
  * 
  * 	def get_optimal_cost(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 652, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 671, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_v_results);
   __Pyx_GIVEREF(__pyx_v_results);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_results);
   __Pyx_INCREF(__pyx_v_python_transmission_vector);
   __Pyx_GIVEREF(__pyx_v_python_transmission_vector);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_v_python_transmission_vector);
   __pyx_r = __pyx_t_8;
   __pyx_t_8 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":633
+  /* "whatshap/core.pyx":652
  * 		del self.thisptr
  * 
  * 	def get_super_reads(self):             # <<<<<<<<<<<<<<
  * 		#Interface is identical to PedigreeDPTable
  * 
  */
 
@@ -16989,15 +17427,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_rs);
   __Pyx_XDECREF(__pyx_v_python_transmission_vector);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":654
+/* "whatshap/core.pyx":673
  * 		return results, python_transmission_vector
  * 
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.getOptScore()
  */
 
@@ -17021,35 +17459,35 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_cost", 0);
 
-  /* "whatshap/core.pyx":656
+  /* "whatshap/core.pyx":675
  * 	def get_optimal_cost(self):
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.getOptScore()             # <<<<<<<<<<<<<<
  * 
  * 	def get_optimal_partitioning(self):
  */
   __Pyx_XDECREF(__pyx_r);
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getOptScore();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 656, __pyx_L1_error)
+    __PYX_ERR(1, 675, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 656, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":654
+  /* "whatshap/core.pyx":673
  * 		return results, python_transmission_vector
  * 
  * 	def get_optimal_cost(self):             # <<<<<<<<<<<<<<
  * 		"""Returns the cost resulting from solving the Minimum Error Correction (MEC) problem."""
  * 		return self.thisptr.getOptScore()
  */
 
@@ -17060,15 +17498,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":658
+/* "whatshap/core.pyx":677
  * 		return self.thisptr.getOptScore()
  * 
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  */
 
@@ -17098,38 +17536,38 @@
   bool __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_optimal_partitioning", 0);
 
-  /* "whatshap/core.pyx":661
+  /* "whatshap/core.pyx":680
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  * 		cdef vector[bool]* p = self.thisptr.getOptBipartition()             # <<<<<<<<<<<<<<
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getOptBipartition();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 661, __pyx_L1_error)
+    __PYX_ERR(1, 680, __pyx_L1_error)
   }
   __pyx_v_p = __pyx_t_1;
 
-  /* "whatshap/core.pyx":662
+  /* "whatshap/core.pyx":681
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  * 		cdef vector[bool]* p = self.thisptr.getOptBipartition()
  * 		result = [0 if x else 1 for x in p[0]]             # <<<<<<<<<<<<<<
  * 		del p
  * 		return result
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 662, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 681, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = &(__pyx_v_p[0]);
     __pyx_t_3 = __pyx_t_1->begin();
     for (;;) {
       if (!(__pyx_t_3 != __pyx_t_1->end())) break;
       __pyx_t_4 = *__pyx_t_3;
       ++__pyx_t_3;
@@ -17137,43 +17575,43 @@
       if ((__pyx_8genexpr9__pyx_v_x != 0)) {
         __Pyx_INCREF(__pyx_int_0);
         __pyx_t_5 = __pyx_int_0;
       } else {
         __Pyx_INCREF(__pyx_int_1);
         __pyx_t_5 = __pyx_int_1;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 662, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 681, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "whatshap/core.pyx":663
+  /* "whatshap/core.pyx":682
  * 		cdef vector[bool]* p = self.thisptr.getOptBipartition()
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p             # <<<<<<<<<<<<<<
  * 		return result
  * 
  */
   delete __pyx_v_p;
 
-  /* "whatshap/core.pyx":664
+  /* "whatshap/core.pyx":683
  * 		result = [0 if x else 1 for x in p[0]]
  * 		del p
  * 		return result             # <<<<<<<<<<<<<<
  * 
  * 	def get_mutations(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":658
+  /* "whatshap/core.pyx":677
  * 		return self.thisptr.getOptScore()
  * 
  * 	def get_optimal_partitioning(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a list of the same size as the read set, where each entry is either 0 or 1,
  * 		telling whether the corresponding read is in partition 0 or in partition 1,"""
  */
 
@@ -17186,15 +17624,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "whatshap/core.pyx":666
+/* "whatshap/core.pyx":685
  * 		return result
  * 
  * 	def get_mutations(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a 2D-list indicating which alleles contain a mutation. The outer list contains
  * 		one sub-list for each sample and the sub-list contains <hap_id, position> pairs of alleles
  */
 
@@ -17221,63 +17659,63 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_mutations", 0);
 
-  /* "whatshap/core.pyx":670
+  /* "whatshap/core.pyx":689
  * 		one sub-list for each sample and the sub-list contains <hap_id, position> pairs of alleles
  * 		not following their respective parent."""
  * 		cdef vector[vector[pair[uint32_t, uint32_t]]]* m = self.thisptr.getMutations()             # <<<<<<<<<<<<<<
  * 		result = list (m[0])
  * 		#result = [[] for _ in range(len(m))]
  */
   try {
     __pyx_t_1 = __pyx_v_self->thisptr->getMutations();
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(1, 670, __pyx_L1_error)
+    __PYX_ERR(1, 689, __pyx_L1_error)
   }
   __pyx_v_m = __pyx_t_1;
 
-  /* "whatshap/core.pyx":671
+  /* "whatshap/core.pyx":690
  * 		not following their respective parent."""
  * 		cdef vector[vector[pair[uint32_t, uint32_t]]]* m = self.thisptr.getMutations()
  * 		result = list (m[0])             # <<<<<<<<<<<<<<
  * 		#result = [[] for _ in range(len(m))]
  * 		#for i in range(len(m)):
  */
-  __pyx_t_2 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_uint32_t_2c_uint32_t_3e____3e___((__pyx_v_m[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 671, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_uint32_t_2c_uint32_t_3e____3e___((__pyx_v_m[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 671, __pyx_L1_error)
+  __pyx_t_3 = PySequence_List(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "whatshap/core.pyx":676
+  /* "whatshap/core.pyx":695
  * 		#	for pair in m[i]:
  * 		#		result[i].append(pair)
  * 		del m             # <<<<<<<<<<<<<<
  * 		return result
  */
   delete __pyx_v_m;
 
-  /* "whatshap/core.pyx":677
+  /* "whatshap/core.pyx":696
  * 		#		result[i].append(pair)
  * 		del m
  * 		return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "whatshap/core.pyx":666
+  /* "whatshap/core.pyx":685
  * 		return result
  * 
  * 	def get_mutations(self):             # <<<<<<<<<<<<<<
  * 		"""Returns a 2D-list indicating which alleles contain a mutation. The outer list contains
  * 		one sub-list for each sample and the sub-list contains <hap_id, position> pairs of alleles
  */
 
@@ -19248,34 +19686,46 @@
   return __pyx_pw_8whatshap_4core_4Read_15reference_start_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_8whatshap_4core_4Read_BX_tag(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_8whatshap_4core_4Read_6BX_tag_1__get__(o);
 }
 
+static PyObject *__pyx_getprop_8whatshap_4core_4Read_HP_tag(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_8whatshap_4core_4Read_6HP_tag_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_8whatshap_4core_4Read_PS_tag(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_8whatshap_4core_4Read_6PS_tag_1__get__(o);
+}
+
 static PyMethodDef __pyx_methods_8whatshap_4core_Read[] = {
   {"__getstate__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_18__getstate__, METH_NOARGS, 0},
   {"__setstate__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_20__setstate__, METH_O, 0},
   {"add_variant", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8whatshap_4core_4Read_22add_variant, METH_VARARGS|METH_KEYWORDS, 0},
   {"add_mapq", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_24add_mapq, METH_O, 0},
   {"sort", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_26sort, METH_NOARGS, 0},
   {"is_sorted", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_28is_sorted, METH_NOARGS, 0},
   {"has_BX_tag", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_30has_BX_tag, METH_NOARGS, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_32__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_34__setstate_cython__, METH_O, 0},
+  {"has_HP_tag", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_32has_HP_tag, METH_NOARGS, 0},
+  {"has_PS_tag", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_34has_PS_tag, METH_NOARGS, 0},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_36__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_8whatshap_4core_4Read_38__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_8whatshap_4core_Read[] = {
   {(char *)"mapqs", __pyx_getprop_8whatshap_4core_4Read_mapqs, 0, (char *)0, 0},
   {(char *)"name", __pyx_getprop_8whatshap_4core_4Read_name, 0, (char *)0, 0},
   {(char *)"source_id", __pyx_getprop_8whatshap_4core_4Read_source_id, 0, (char *)0, 0},
   {(char *)"sample_id", __pyx_getprop_8whatshap_4core_4Read_sample_id, 0, (char *)0, 0},
   {(char *)"reference_start", __pyx_getprop_8whatshap_4core_4Read_reference_start, 0, (char *)0, 0},
   {(char *)"BX_tag", __pyx_getprop_8whatshap_4core_4Read_BX_tag, 0, (char *)0, 0},
+  {(char *)"HP_tag", __pyx_getprop_8whatshap_4core_4Read_HP_tag, 0, (char *)0, 0},
+  {(char *)"PS_tag", __pyx_getprop_8whatshap_4core_4Read_PS_tag, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
 static PySequenceMethods __pyx_tp_as_sequence_Read = {
   __pyx_pw_8whatshap_4core_4Read_10__len__, /*sq_length*/
   0, /*sq_concat*/
   0, /*sq_repeat*/
@@ -20997,21 +21447,23 @@
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_BX_tag, __pyx_k_BX_tag, sizeof(__pyx_k_BX_tag), 0, 0, 1, 1},
   {&__pyx_n_s_Caller, __pyx_k_Caller, sizeof(__pyx_k_Caller), 0, 0, 1, 1},
   {&__pyx_kp_u_Expected_instance_of_Variant_but, __pyx_k_Expected_instance_of_Variant_but, sizeof(__pyx_k_Expected_instance_of_Variant_but), 0, 1, 0, 0},
   {&__pyx_n_s_Genotype, __pyx_k_Genotype, sizeof(__pyx_k_Genotype), 0, 0, 1, 1},
   {&__pyx_n_s_GenotypeDPTable, __pyx_k_GenotypeDPTable, sizeof(__pyx_k_GenotypeDPTable), 0, 0, 1, 1},
+  {&__pyx_n_s_HP_tag, __pyx_k_HP_tag, sizeof(__pyx_k_HP_tag), 0, 0, 1, 1},
   {&__pyx_n_s_HapChatCore, __pyx_k_HapChatCore, sizeof(__pyx_k_HapChatCore), 0, 0, 1, 1},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_u_Index_out_of_bounds, __pyx_k_Index_out_of_bounds, sizeof(__pyx_k_Index_out_of_bounds), 0, 1, 0, 0},
   {&__pyx_kp_u_Invalid_key, __pyx_k_Invalid_key, sizeof(__pyx_k_Invalid_key), 0, 1, 0, 0},
   {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
   {&__pyx_n_s_NotImplementedError, __pyx_k_NotImplementedError, sizeof(__pyx_k_NotImplementedError), 0, 0, 1, 1},
   {&__pyx_n_s_NumericSampleIds, __pyx_k_NumericSampleIds, sizeof(__pyx_k_NumericSampleIds), 0, 0, 1, 1},
+  {&__pyx_n_s_PS_tag, __pyx_k_PS_tag, sizeof(__pyx_k_PS_tag), 0, 0, 1, 1},
   {&__pyx_n_s_PedMecHeuristic, __pyx_k_PedMecHeuristic, sizeof(__pyx_k_PedMecHeuristic), 0, 0, 1, 1},
   {&__pyx_n_s_Pedigree, __pyx_k_Pedigree, sizeof(__pyx_k_Pedigree), 0, 0, 1, 1},
   {&__pyx_n_s_PedigreeDPTable, __pyx_k_PedigreeDPTable, sizeof(__pyx_k_PedigreeDPTable), 0, 0, 1, 1},
   {&__pyx_n_s_PhredGenotypeLikelihoods, __pyx_k_PhredGenotypeLikelihoods, sizeof(__pyx_k_PhredGenotypeLikelihoods), 0, 0, 1, 1},
   {&__pyx_n_s_PhredGenotypeLikelihoods___iter, __pyx_k_PhredGenotypeLikelihoods___iter, sizeof(__pyx_k_PhredGenotypeLikelihoods___iter), 0, 0, 1, 1},
   {&__pyx_kp_u_Querying_a_ReadSet_by_read_name, __pyx_k_Querying_a_ReadSet_by_read_name, sizeof(__pyx_k_Querying_a_ReadSet_by_read_name), 0, 1, 0, 0},
   {&__pyx_n_s_Read, __pyx_k_Read, sizeof(__pyx_k_Read), 0, 0, 1, 1},
@@ -21107,19 +21559,19 @@
   {&__pyx_n_s_whatshap_core, __pyx_k_whatshap_core, sizeof(__pyx_k_whatshap_core), 0, 0, 1, 1},
   {&__pyx_kp_s_whatshap_core_pyx, __pyx_k_whatshap_core_pyx, sizeof(__pyx_k_whatshap_core_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_window, __pyx_k_window, sizeof(__pyx_k_window), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 120, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(1, 132, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 136, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 153, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 256, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 131, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(1, 143, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 147, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 164, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(1, 275, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -21140,33 +21592,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "whatshap/core.pyx":132
+  /* "whatshap/core.pyx":143
  * 		assert self.thisptr != NULL
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError("Read does not support slices")             # <<<<<<<<<<<<<<
  * 		assert isinstance(key, int)
  * 		cdef int n = self.thisptr.getVariantCount()
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Read_does_not_support_slices); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 132, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_Read_does_not_support_slices); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "whatshap/core.pyx":191
+  /* "whatshap/core.pyx":203
  * 			self.ownsptr = True
  * 
  * 		for mapq in mapqs[1:]:             # <<<<<<<<<<<<<<
  * 			self.add_mapq(mapq)
  * 		for (pos, allele, quality) in variants:
  */
-  __pyx_slice__5 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(1, 191, __pyx_L1_error)
+  __pyx_slice__5 = PySlice_New(__pyx_int_1, Py_None, Py_None); if (unlikely(!__pyx_slice__5)) __PYX_ERR(1, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -21181,33 +21633,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "whatshap/core.pyx":243
+  /* "whatshap/core.pyx":262
  * 	def __getitem__(self, key):
  * 		if isinstance(key, slice):
  * 			raise NotImplementedError('ReadSet does not support slices')             # <<<<<<<<<<<<<<
  * 		cdef string name = b''
  * 		cdef cpp.Read* cread = NULL
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_ReadSet_does_not_support_slices); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_ReadSet_does_not_support_slices); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 262, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "whatshap/core.pyx":250
+  /* "whatshap/core.pyx":269
  * 			read.thisptr = self.thisptr.get(key)
  * 		elif isinstance(key, str):
  * 			raise NotImplementedError('Querying a ReadSet by read name is deprecated, please query by (source_id, name) instead')             # <<<<<<<<<<<<<<
  * 		elif isinstance(key, tuple) and (len(key) == 2) and (isinstance(key[0],int) and isinstance(key[1],str)):
  * 			source_id = key[0]
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Querying_a_ReadSet_by_read_name); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 250, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_Querying_a_ReadSet_by_read_name); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 269, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -21374,55 +21826,55 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
 
-  /* "whatshap/core.pyx":449
+  /* "whatshap/core.pyx":468
  * 
  * 
  * def binomial_coefficient(int n, int k):             # <<<<<<<<<<<<<<
  * 	return cpp.binomial_coefficient(n, k)
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_n, __pyx_n_s_k); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 449, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_n, __pyx_n_s_k); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_binomial_coefficient, 449, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 449, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_binomial_coefficient, 468, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 468, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":515
+  /* "whatshap/core.pyx":534
  * 
  * 
  * def get_max_genotype_ploidy():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_ploidy()
  * 
  */
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_get_max_genotype_ploidy, 515, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 515, __pyx_L1_error)
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_get_max_genotype_ploidy, 534, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 534, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":519
+  /* "whatshap/core.pyx":538
  * 
  * 
  * def get_max_genotype_alleles():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_alleles()
  * 
  */
-  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_get_max_genotype_alleles, 519, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 519, __pyx_L1_error)
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_get_max_genotype_alleles, 538, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 538, __pyx_L1_error)
 
-  /* "whatshap/core.pyx":545
+  /* "whatshap/core.pyx":564
  * 
  * 
  * def compute_genotypes(ReadSet readset, positions = None):             # <<<<<<<<<<<<<<
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  */
-  __pyx_tuple__33 = PyTuple_Pack(10, __pyx_n_s_readset, __pyx_n_s_positions, __pyx_n_s_genotypes_vector, __pyx_n_s_gl_vector, __pyx_n_s_c_positions, __pyx_n_s_pos, __pyx_n_s_genotypes, __pyx_n_s_gls, __pyx_n_s_genotype, __pyx_n_s_i); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 545, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(10, __pyx_n_s_readset, __pyx_n_s_positions, __pyx_n_s_genotypes_vector, __pyx_n_s_gl_vector, __pyx_n_s_c_positions, __pyx_n_s_pos, __pyx_n_s_genotypes, __pyx_n_s_gls, __pyx_n_s_genotype, __pyx_n_s_i); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_compute_genotypes, 545, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 545, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(2, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_whatshap_core_pyx, __pyx_n_s_compute_genotypes, 564, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 564, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -21535,121 +21987,121 @@
       ((PyWrapperDescrObject *)wrapper)->d_base = &__pyx_wrapperbase_8whatshap_4core_4Read_15__contains__;
     }
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Read, (PyObject *)&__pyx_type_8whatshap_4core_Read) < 0) __PYX_ERR(1, 62, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Read) < 0) __PYX_ERR(1, 62, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_Read = &__pyx_type_8whatshap_4core_Read;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 217, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 236, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_ReadSet.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_ReadSet.tp_dictoffset && __pyx_type_8whatshap_4core_ReadSet.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_ReadSet.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ReadSet, (PyObject *)&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 217, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 217, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ReadSet, (PyObject *)&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 236, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_ReadSet) < 0) __PYX_ERR(1, 236, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_ReadSet = &__pyx_type_8whatshap_4core_ReadSet;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 361, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 380, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_Pedigree.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_Pedigree.tp_dictoffset && __pyx_type_8whatshap_4core_Pedigree.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_Pedigree.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Pedigree, (PyObject *)&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 361, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 361, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Pedigree, (PyObject *)&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 380, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Pedigree) < 0) __PYX_ERR(1, 380, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_Pedigree = &__pyx_type_8whatshap_4core_Pedigree;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 306, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 325, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_PedigreeDPTable.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_PedigreeDPTable.tp_dictoffset && __pyx_type_8whatshap_4core_PedigreeDPTable.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_PedigreeDPTable.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PedigreeDPTable, (PyObject *)&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 306, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 306, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PedigreeDPTable, (PyObject *)&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 325, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PedigreeDPTable) < 0) __PYX_ERR(1, 325, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_PedigreeDPTable = &__pyx_type_8whatshap_4core_PedigreeDPTable;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 411, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 430, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_PhredGenotypeLikelihoods.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods.tp_dictoffset && __pyx_type_8whatshap_4core_PhredGenotypeLikelihoods.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_PhredGenotypeLikelihoods.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PhredGenotypeLikelihoods, (PyObject *)&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 411, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 411, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PhredGenotypeLikelihoods, (PyObject *)&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 430, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods) < 0) __PYX_ERR(1, 430, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_PhredGenotypeLikelihoods = &__pyx_type_8whatshap_4core_PhredGenotypeLikelihoods;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 453, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 472, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_Genotype.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_Genotype.tp_dictoffset && __pyx_type_8whatshap_4core_Genotype.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_Genotype.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Genotype, (PyObject *)&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 453, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 453, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Genotype, (PyObject *)&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 472, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Genotype) < 0) __PYX_ERR(1, 472, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_Genotype = &__pyx_type_8whatshap_4core_Genotype;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 523, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 542, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_GenotypeDPTable.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_GenotypeDPTable.tp_dictoffset && __pyx_type_8whatshap_4core_GenotypeDPTable.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_GenotypeDPTable.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GenotypeDPTable, (PyObject *)&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 523, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 523, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_GenotypeDPTable, (PyObject *)&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 542, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_GenotypeDPTable) < 0) __PYX_ERR(1, 542, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_GenotypeDPTable = &__pyx_type_8whatshap_4core_GenotypeDPTable;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_HapChatCore.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_HapChatCore.tp_dictoffset && __pyx_type_8whatshap_4core_HapChatCore.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_HapChatCore.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_HapChatCore, (PyObject *)&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 563, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_HapChatCore, (PyObject *)&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_HapChatCore) < 0) __PYX_ERR(1, 582, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_HapChatCore = &__pyx_type_8whatshap_4core_HapChatCore;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 593, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 612, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_Caller.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_Caller.tp_dictoffset && __pyx_type_8whatshap_4core_Caller.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_Caller.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Caller, (PyObject *)&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 593, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 593, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Caller, (PyObject *)&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 612, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_Caller) < 0) __PYX_ERR(1, 612, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_Caller = &__pyx_type_8whatshap_4core_Caller;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 616, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 635, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core_PedMecHeuristic.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core_PedMecHeuristic.tp_dictoffset && __pyx_type_8whatshap_4core_PedMecHeuristic.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core_PedMecHeuristic.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PedMecHeuristic, (PyObject *)&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 616, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 616, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_PedMecHeuristic, (PyObject *)&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 635, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8whatshap_4core_PedMecHeuristic) < 0) __PYX_ERR(1, 635, __pyx_L1_error)
   __pyx_ptype_8whatshap_4core_PedMecHeuristic = &__pyx_type_8whatshap_4core_PedMecHeuristic;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct____iter__) < 0) __PYX_ERR(1, 117, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct____iter__) < 0) __PYX_ERR(1, 128, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core___pyx_scope_struct____iter__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core___pyx_scope_struct____iter__.tp_dictoffset && __pyx_type_8whatshap_4core___pyx_scope_struct____iter__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core___pyx_scope_struct____iter__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8whatshap_4core___pyx_scope_struct____iter__ = &__pyx_type_8whatshap_4core___pyx_scope_struct____iter__;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__) < 0) __PYX_ERR(1, 234, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__) < 0) __PYX_ERR(1, 253, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__.tp_dictoffset && __pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8whatshap_4core___pyx_scope_struct_1___iter__ = &__pyx_type_8whatshap_4core___pyx_scope_struct_1___iter__;
-  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__) < 0) __PYX_ERR(1, 429, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__) < 0) __PYX_ERR(1, 448, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__.tp_dictoffset && __pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_8whatshap_4core___pyx_scope_struct_2___iter__ = &__pyx_type_8whatshap_4core___pyx_scope_struct_2___iter__;
@@ -21923,60 +22375,60 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_namedtuple); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_namedtuple, __pyx_t_2) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":449
+  /* "whatshap/core.pyx":468
  * 
  * 
  * def binomial_coefficient(int n, int k):             # <<<<<<<<<<<<<<
  * 	return cpp.binomial_coefficient(n, k)
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_1binomial_coefficient, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 449, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_1binomial_coefficient, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_binomial_coefficient, __pyx_t_1) < 0) __PYX_ERR(1, 449, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_binomial_coefficient, __pyx_t_1) < 0) __PYX_ERR(1, 468, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":515
+  /* "whatshap/core.pyx":534
  * 
  * 
  * def get_max_genotype_ploidy():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_ploidy()
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_3get_max_genotype_ploidy, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 515, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_3get_max_genotype_ploidy, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 534, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_max_genotype_ploidy, __pyx_t_1) < 0) __PYX_ERR(1, 515, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_max_genotype_ploidy, __pyx_t_1) < 0) __PYX_ERR(1, 534, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":519
+  /* "whatshap/core.pyx":538
  * 
  * 
  * def get_max_genotype_alleles():             # <<<<<<<<<<<<<<
  * 	return cpp.get_max_genotype_alleles()
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_5get_max_genotype_alleles, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 519, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_5get_max_genotype_alleles, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_max_genotype_alleles, __pyx_t_1) < 0) __PYX_ERR(1, 519, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_max_genotype_alleles, __pyx_t_1) < 0) __PYX_ERR(1, 538, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "whatshap/core.pyx":545
+  /* "whatshap/core.pyx":564
  * 
  * 
  * def compute_genotypes(ReadSet readset, positions = None):             # <<<<<<<<<<<<<<
  * 	cdef vector[cpp.Genotype]* genotypes_vector = new vector[cpp.Genotype]()
  * 	cdef vector[cpp.GenotypeDistribution]* gl_vector = new vector[cpp.GenotypeDistribution]()
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_7compute_genotypes, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 545, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_8whatshap_4core_7compute_genotypes, NULL, __pyx_n_s_whatshap_core); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_genotypes, __pyx_t_1) < 0) __PYX_ERR(1, 545, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_compute_genotypes, __pyx_t_1) < 0) __PYX_ERR(1, 564, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "whatshap/core.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * 
  * """
  */
```

### Comparing `whatshap-2.2/whatshap/core.pxd` & `whatshap-2.3/whatshap/core.pxd`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/core.pyi` & `whatshap-2.3/whatshap/core.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from collections import namedtuple
 from typing import Dict, Iterable, Optional, Tuple, List, Sequence, Iterator
 
+from whatshap.types import PhasingAlgorithm
+
 Variant = namedtuple("Variant", "position allele quality")
 
 class NumericSampleIds:
     def __getitem__(self, sample: str) -> int: ...
     def __len__(self) -> int: ...
     def __str__(self) -> str: ...
     def freeze(self) -> None: ...
@@ -15,48 +17,56 @@
         self,
         name: Optional[str] = ...,
         mapq: int = ...,
         source_id: int = ...,
         sample_id: int = ...,
         reference_start: int = ...,
         BX_tag: Optional[str] = ...,
+        HP_tag: Optional[int] = ...,
+        PS_tag: Optional[int] = ...,
     ): ...
     @property
     def mapqs(self) -> Tuple[int]: ...
     @property
     def name(self) -> str: ...
     @property
     def source_id(self) -> int: ...
     @property
     def sample_id(self) -> int: ...
     @property
     def reference_start(self) -> int: ...
     @property
     def BX_tag(self) -> str: ...
+    @property
+    def HP_tag(self) -> int: ...
+    @property
+    def PS_tag(self) -> int: ...
     def __iter__(self) -> Iterator[Variant]: ...
     def __len__(self) -> int: ...
     def __getitem__(self, key: int) -> Variant: ...
     def __setitem__(self, index: int, variant: Variant): ...
     def __contains__(self, position: int) -> bool: ...
     def add_variant(self, position: int, allele: int, quality: int) -> None: ...
     def add_mapq(self, mapq: int) -> None: ...
     def sort(self) -> None: ...
     def is_sorted(self) -> bool: ...
     def has_BX_tag(self) -> bool: ...
+    def has_HP_tag(self) -> bool: ...
+    def has_PS_tag(self) -> bool: ...
 
 class ReadSet:
     def add(self, read: Read) -> None: ...
     def __iter__(self) -> Iterator[Read]: ...
     def __len__(self) -> int: ...
     def __getitem__(self, key: int) -> Read: ...
     def sort(self) -> None: ...
     def subset(self, reads_to_select: Iterable[int]) -> ReadSet: ...
     def get_positions(self) -> List[int]: ...
 
-class PedigreeDPTable:
+class PedigreeDPTable(PhasingAlgorithm):
     def __init__(
         self,
         readset: ReadSet,
         recombcost: Sequence[int],
         pedigree: Pedigree,
         distrust_genotypes: bool = ...,
         positions: Optional[Iterable[int]] = ...,
@@ -118,18 +128,18 @@
     ): ...
     def get_genotype_likelihoods(self, sample_id: int, pos: int) -> PhredGenotypeLikelihoods: ...
 
 def compute_genotypes(
     readset: ReadSet, positions: Optional[Iterable[int]] = ...
 ) -> Tuple[List[Genotype], List[Tuple[float, float, float]]]: ...
 
-class HapChatCore:
+class HapChatCore(PhasingAlgorithm):
     def __init__(self, readset: ReadSet): ...
     def get_length(self) -> int: ...
-    def get_super_reads(self) -> Tuple[List[ReadSet], List[int]]: ...
+    def get_super_reads(self) -> Tuple[List[ReadSet], Optional[List[int]]]: ...
     def get_optimal_cost(self) -> int: ...
     def get_optimal_partitioning(self) -> List[int]: ...
 
 class Caller:
     def __init__(self, reference: str, k: int, window: int): ...
     def all_variants(self, variants_list: List[Tuple[int, int]]): ...
     def add_read(
@@ -138,25 +148,25 @@
         bam_alignment_cigartuples: List[List[int]],
         bam_alignment_query: str,
         outfile: str,
     ): ...
     def final_pop(self, outfile: str): ...
     def finish(self): ...
 
-class PedMecHeuristic:
+class PedMecHeuristic(PhasingAlgorithm):
     def __init__(
         self,
         readset: ReadSet,
         recombcost: Sequence[int],
         pedigree: Pedigree,
+        row_limit: Optional[int] = ...,
         distrust_genotypes: bool = ...,
         positions: Optional[Iterable[int]] = ...,
-        row_limit: Optional[int] = ...,
         allow_mutations: Optional[bool] = ...,
         verbosity: Optional[int] = ...,
     ): ...
-    def get_super_reads(self) -> List[ReadSet]: ...
+    def get_super_reads(self) -> Tuple[List[ReadSet], Optional[List[int]]]: ...
     def get_opt_transmission(self) -> List[int]: ...
     def get_optimal_cost(self) -> int: ...
     def get_optimal_partitioning(self) -> List[int]: ...
     def get_mutations(self) -> List[List[Tuple[int, int]]]: ...
     def solve(self): ...
```

### Comparing `whatshap-2.2/whatshap/core.pyx` & `whatshap-2.3/whatshap/core.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -56,37 +56,38 @@
 	def __setstate__(self, state):
 		mapping, frozen = state
 		self.mapping = mapping
 		self.frozen = frozen
 
 
 cdef class Read:
-	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None):
+	def __cinit__(self, str name = None, int mapq = 0, int source_id = 0, int sample_id = 0, int reference_start = -1, str BX_tag = None, int HP_tag = -1, int PS_tag = -1):
 		cdef string _name = b''
 		cdef string _BX_tag = b''
+
 		if name is None:
 			self.thisptr = NULL
 			self.ownsptr = False
 		else:
 			# TODO: Is this the best way to handle string arguments?
 			_name = name.encode('UTF-8')
 			if BX_tag is not '' and BX_tag is not None:
 				_BX_tag = BX_tag.encode('UTF-8')
-			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag)
+			self.thisptr = new cpp.Read(_name, mapq, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
 			self.ownsptr = True
 
 	def __dealloc__(self):
 		if self.ownsptr:
 			assert self.thisptr != NULL
 			del self.thisptr
 
 	def __repr__(self):
 		assert self.thisptr != NULL
-		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, variants={})'.format(
-			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, list(self))
+		return 'Read(name={!r}, mapq={}, source_id={}, sample_id={}, reference_start={},  BX_tag={}, HP_tag={}, PS_tag={}, variants={})'.format(
+			self.name, self.mapqs, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, list(self))
 
 	property mapqs:
 		def __get__(self):
 			assert self.thisptr != NULL
 			return tuple(self.thisptr.getMapqs())
 
 	property name:
@@ -110,14 +111,24 @@
 			return self.thisptr.getReferenceStart()
 
 	property BX_tag:
 		def __get__(self):
 			assert self.thisptr != NULL
 			return self.thisptr.getBXTag().decode('utf-8')
 
+	property HP_tag:
+		def __get__(self):
+			assert self.thisptr != NULL
+			return self.thisptr.getHPTag()
+
+	property PS_tag:
+		def __get__(self):
+			assert self.thisptr != NULL
+			return self.thisptr.getPSTag()
+
 	def __iter__(self):
 		"""Iterate over all variants in this read"""
 		assert self.thisptr != NULL
 		for i in range(len(self)):
 			yield self[i]
 
 	def __len__(self):
@@ -165,31 +176,32 @@
 			if variant.position == position:
 				return True
 		return False
 	
 	def __getstate__(self):
 		mapqs = [mapq for mapq in self.mapqs]
 		variants = [(var.position, var.allele, var.quality) for var in self]
-		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, variants)
+		return (mapqs, self.name, self.source_id, self.sample_id, self.reference_start, self.BX_tag, self.HP_tag, self.PS_tag, variants)
 	
 	def __setstate__(self, state):
-		mapqs, name, source_id, sample_id, reference_start, BX_tag, variants = state
+		mapqs, name, source_id, sample_id, reference_start, BX_tag, HP_tag, PS_tag, variants = state
 		
 		# TODO: Duplicated code from __cinit__ is ugly, but cinit cannot be used here directly
 		cdef string _name = b''
 		cdef string _BX_tag = b''
+
 		if name is None:
 			self.thisptr = NULL
 			self.ownsptr = False
 		else:
 			# TODO: Is this the best way to handle string arguments?
 			_name = name.encode('UTF-8')
 			if BX_tag is not b'' and BX_tag is not None:
 				_BX_tag = BX_tag.encode('UTF-8')
-			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag)
+			self.thisptr = new cpp.Read(_name, mapqs[0] if len(mapqs) > 0 else 0, source_id, sample_id, reference_start, _BX_tag, HP_tag, PS_tag)
 			self.ownsptr = True
 
 		for mapq in mapqs[1:]:
 			self.add_mapq(mapq)
 		for (pos, allele, quality) in variants:
 			self.add_variant(pos, allele, quality)
 
@@ -209,14 +221,21 @@
 		assert self.thisptr != NULL
 		return self.thisptr.isSorted()
 
 	def has_BX_tag(self):
 		assert self.thisptr != NULL
 		return self.thisptr.hasBXTag()
 
+	def has_HP_tag(self):
+		assert self.thisptr != NULL
+		return self.thisptr.hasBXTag()
+
+	def has_PS_tag(self):
+		assert self.thisptr != NULL
+		return self.thisptr.hasBXTag()
 
 cdef class ReadSet:
 	def __cinit__(self):
 		self.thisptr = new cpp.ReadSet()
 
 	def __dealloc__(self):
 		del self.thisptr
```

### Comparing `whatshap-2.2/whatshap/cpp.pxd` & `whatshap-2.3/whatshap/cpp.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from libc.stdint cimport int8_t, uint32_t, uint64_t
 from libcpp.unordered_map cimport unordered_map
 from libcpp.deque cimport deque
 
 
 cdef extern from "read.h":
     cdef cppclass Read:
-        Read(string, int, int, int, int, string) except +
+        Read(string, int, int, int, int, string, int, int) except +
         Read(Read) except +
         string toString() except +
         void addVariant(int, int, int) except +
         string getName() except +
         vector[int] getMapqs() except +
         void addMapq(int) except +
         int getPosition(int) except +
@@ -31,14 +31,18 @@
         void sortVariants() except +
         bool isSorted() except +
         int getSourceID() except +
         int getSampleID() except +
         int getReferenceStart() except +
         string getBXTag() except +
         bool hasBXTag() except +
+        int getHPTag() except +
+        bool hasHPTag() except +
+        int getPSTag() except +
+        bool hasPSTag() except +
 
 
 cdef extern from "indexset.h":
     cdef cppclass IndexSet:
         IndexSet() except +
         bool contains(int) except +
         void add(int) except +
```

### Comparing `whatshap-2.2/whatshap/graph.py` & `whatshap-2.3/whatshap/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Find connected components.
 """
+
 from abc import abstractmethod
 from collections import OrderedDict
 from typing import TypeVar, Generic, Optional, Iterable
 import typing
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Protocol
```

### Comparing `whatshap-2.2/whatshap/merge.py` & `whatshap-2.3/whatshap/merge.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/pedigree.py` & `whatshap-2.3/whatshap/pedigree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Pedigree-related functions
 """
+
 from abc import ABC, abstractmethod
 
 import math
 from pathlib import Path
 
 from typing import Optional, Union, Sequence, List, IO, Iterator, Mapping
 from collections import Counter, defaultdict
```

### Comparing `whatshap-2.2/whatshap/phred_scores.py` & `whatshap-2.3/whatshap/phred_scores.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/__init__.py` & `whatshap-2.3/whatshap/polyphase/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 @dataclass
 class PolyphaseBlockResult:
     block_id: int
     clustering: List[List[int]]
     threads: List[List[int]]
-    haplotypes: List[int]
+    haplotypes: List[List[int]]
     breakpoints: List[PhaseBreakpoint]
 
 
 @dataclass
 class PolyphaseResult:
     clustering: List[List[int]]
     threads: List[List[int]]
```

### Comparing `whatshap-2.2/whatshap/polyphase/algorithm.py` & `whatshap-2.3/whatshap/polyphase/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Algorithmic core of whatshap polyphase. Split inputs into independent blocks if possible and can be
 executed in parallel on a block level. Each block is processed in three phases: Read clustering,
 haplotype threading and reordering.
 """
+
 import logging
 
 from itertools import chain
 from multiprocessing import Pool
 from math import log
 from typing import List
 from copy import copy
```

### Comparing `whatshap-2.2/whatshap/polyphase/clusterarrangement.py` & `whatshap-2.3/whatshap/polyphase/clusterarrangement.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/offspringscoring.py` & `whatshap-2.3/whatshap/polyphase/offspringscoring.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/plots.py` & `whatshap-2.3/whatshap/polyphase/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,17 +337,19 @@
         min_pos = num_vars
         max_pos = 0
         for pos in range(num_vars):
             if c_list[c_id] in coverage[pos] and coverage[pos][c_list[c_id]] > 0:
                 min_pos = min(min_pos, pos)
                 max_pos = max(max_pos, pos)
         ys = [
-            y_offset + c_height * coverage[pos][c_list[c_id]]
-            if c_list[c_id] in coverage[pos]
-            else y_offset
+            (
+                y_offset + c_height * coverage[pos][c_list[c_id]]
+                if c_list[c_id] in coverage[pos]
+                else y_offset
+            )
             for pos in range(min_pos, max_pos + 1)
         ]
         plt.fill_between(x=xs[min_pos : max_pos + 1], y1=ys, y2=y_offset, color="gray")
         plt.hlines(
             y=y_offset + c_height + y_margin / 2,
             xmin=0,
             xmax=x_scale * num_vars - 1,
```

### Comparing `whatshap-2.2/whatshap/polyphase/reorder.py` & `whatshap-2.3/whatshap/polyphase/reorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     Does two things:
     1. Update haplotype strings inside the collapsed regions according to the solved sub-instances
     2. Collect breakpoints of global threading and integrate breakpoints of sub-instances
     """
     breakpoints = find_breakpoints(threads)
     for (cid, thread_set, subm), res in zip(sub_instances, sub_results):
         snps = [allele_matrix.globalToLocal(gpos) for gpos in subm.getPositions()]
-        assert all([0 <= pos < allele_matrix.getNumPositions() for pos in snps])
+        assert all(0 <= pos < allele_matrix.getNumPositions() for pos in snps)
 
         # reorder haplotype alleles according to subresults, but only on SNP positions
         for i, pos in enumerate(snps):
             for j, hap in enumerate(thread_set):
                 haplotypes[hap][pos] = res.haplotypes[j][i]
 
         # copy breakpoints, but map positions and haplotype ids from sub-instance to global one
```

### Comparing `whatshap-2.2/whatshap/polyphase/solver.cpp` & `whatshap-2.3/whatshap/polyphase/solver.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/solver.pxd` & `whatshap-2.3/whatshap/polyphase/solver.pxd`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/solver.pyi` & `whatshap-2.3/whatshap/polyphase/solver.pyi`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/solver.pyx` & `whatshap-2.3/whatshap/polyphase/solver.pyx`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/threading.py` & `whatshap-2.3/whatshap/polyphase/threading.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/polyphase/variantselection.py` & `whatshap-2.3/whatshap/polyphase/variantselection.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/priorityqueue.cpp` & `whatshap-2.3/whatshap/priorityqueue.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/priorityqueue.pxd` & `whatshap-2.3/whatshap/priorityqueue.pxd`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/priorityqueue.pyx` & `whatshap-2.3/whatshap/priorityqueue.pyx`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/readselect.cpp` & `whatshap-2.3/whatshap/readselect.cpp`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/readselect.pyx` & `whatshap-2.3/whatshap/readselect.pyx`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/testhelpers.py` & `whatshap-2.3/whatshap/testhelpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Utility functions only used by unit tests
 """
+
 import textwrap
 from collections import defaultdict
 from whatshap.core import Read, ReadSet, Genotype
 
 
 def string_to_readset(s, w=None, sample_ids=None, source_id=0, scale_quality=None):
     s = textwrap.dedent(s).strip()
```

### Comparing `whatshap-2.2/whatshap/timer.py` & `whatshap-2.3/whatshap/timer.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/utils.py` & `whatshap-2.3/whatshap/utils.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap/variants.py` & `whatshap-2.3/whatshap/variants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Detect variants in reads.
 """
+
 import logging
 import csv
 from collections import defaultdict, Counter
 from typing import Iterable, Iterator, List, Optional
 from dataclasses import dataclass
 
 from pysam import AlignedSegment
 
 from .vcf import VcfVariant
 from .core import Read, ReadSet, NumericSampleIds
 from .bam import SampleBamReader, MultiBamReader, BamReader
 from .align import edit_distance, edit_distance_affine_gap, kmer_align, enumerate_all_kmers
 from ._variants import _iterate_cigar, _detect_alleles
 
-
 logger = logging.getLogger(__name__)
 
 
 class ReadSetError(Exception):
     pass
 
 
@@ -62,14 +62,30 @@
     def get_resolved(self):
         return [i for i, a in enumerate(self.alleles) if a.progress == a.length]
 
     def get_pending(self):
         return [i for i, a in enumerate(self.alleles) if 0 <= a.progress < a.length]
 
 
+@dataclass
+class AlignedRead:
+    read: Read
+    is_supplementary: bool
+    is_reverse: bool
+    reference_start: int
+    reference_end: int
+
+    def distance(self, other) -> int:
+        return max(
+            other.reference_end - self.reference_start,
+            other.reference_start - self.reference_end,
+            0,
+        )
+
+
 class ReadSetReader:
     """
     Associate VCF variants with BAM reads.
 
     A VCF file contains variants, and a BAM file contain reads, but the
     information which read contains which variant is not available. This
     class re-discovers the variants in each read, using the
@@ -90,14 +106,16 @@
         default_mismatch: int = 15,
         duplicates: bool = False,
         use_kmerald: bool = False,
         kmeralign_costs_path: Optional[str] = None,
         kmer_size: int = 7,
         kmerald_gappenalty: float = 40,
         kmerald_window: int = 25,
+        use_supplementary: bool = False,
+        supplementary_distance_threshold: int = 100_000,
     ):
         """
         paths -- list of BAM paths
         reference -- path to reference FASTA (can be None)
         numeric_sample_ids -- ??
         mapq_threshold -- minimum mapping quality
         overhang -- extend alignment by this many bases to left and right
@@ -116,14 +134,16 @@
         self._use_kmerald = use_kmerald
         self._kmeralign_costs_path = kmeralign_costs_path
         self._kmer_size = kmer_size
         self._kmerald_gappenalty = kmerald_gappenalty
         self._kmerald_window = kmerald_window
         self._paths = paths
         self._reader: BamReader
+        self._use_supplementary = use_supplementary
+        self._supplementary_distance_threshold = supplementary_distance_threshold
         if len(paths) == 1:
             self._reader = SampleBamReader(paths[0], reference=reference)
         else:
             self._reader = MultiBamReader(paths, reference=reference)
 
     @property
     def n_paths(self) -> int:
@@ -152,44 +172,113 @@
         if __debug__ and variants:
             varposc = Counter(variant.position for variant in variants)
             pos, count = varposc.most_common()[0]
             assert count == 1, f"Position {pos} occurs more than once in variant list."
 
         alignments = self._usable_alignments(chromosome, sample, regions)
         reads = self._alignments_to_reads(alignments, variants, sample, reference)
-        grouped_reads = self._group_paired_reads(reads)
+        grouped_reads = self._group_reads(reads, self._supplementary_distance_threshold)
         readset = self._make_readset_from_grouped_reads(grouped_reads)
         return readset
 
     @staticmethod
     def _make_readset_from_grouped_reads(groups: Iterable[List[Read]]) -> ReadSet:
         read_set = ReadSet()
         for group in groups:
             read_set.add(merge_reads(*group))
         return read_set
 
     @staticmethod
-    def _group_paired_reads(reads: Iterable[Read]) -> Iterator[List[Read]]:
+    def create_read_from_group(group: List[AlignedRead], distance_threshold: int) -> Optional[Read]:
+        """
+        Merge multiple AlignedReads into a single Read.
+
+        Pick supplementary reads that have the same orientation as the primary and with
+        the distance at most distance_threshold from primary, find the set of variants that fully agree
+        and return these variants as a read.
+
+        If the list does not contain primary reads, then return None.
+        If the list contains more than two primary alignments, return None and report a warning.
+        """
+        logger.debug(f"Group of read {group[0].read.name!r} has {len(group)} items.")
+        primary: Optional[AlignedRead] = None
+        n_primary = 0
+        for read in group:
+            if not read.is_supplementary:
+                n_primary += 1
+                primary = read
+        if primary is None:
+            return None
+        if n_primary > 2:
+            logger.warning(
+                f"Read name {group[0].read.name!r} has more than two primary alignments."
+            )
+            return None
+        reference_start = primary.reference_start
+        variants = dict()
+        skip = set()
+        for read in group:
+            if read.is_reverse != primary.is_reverse:
+                continue
+            if primary.distance(read) > distance_threshold:
+                continue
+            reference_start = min(reference_start, read.reference_start)
+            for variant in read.read:
+                if variant.position in variants:
+                    if variants[variant.position].allele != variant.allele:
+                        skip.add(variant.position)
+                else:
+                    variants[variant.position] = variant
+        union_read = Read(
+            primary.read.name,
+            primary.read.mapqs[0],
+            primary.read.source_id,
+            primary.read.sample_id,
+            reference_start,
+            primary.read.BX_tag,
+            primary.read.HP_tag,
+            primary.read.PS_tag,
+        )
+        for position, variant in variants.items():
+            if position not in skip:
+                union_read.add_variant(variant.position, variant.allele, variant.quality)
+        union_read.sort()
+        if len(union_read) != len(primary.read):
+            logger.debug(
+                f"Converted read {primary.read.name} with {len(primary.read)} variants"
+                f" to read with {len(union_read)} variants."
+            )
+        return union_read
+
+    @staticmethod
+    def _group_reads(reads: Iterable[AlignedRead], distance_threshold: int) -> Iterator[List[Read]]:
         """
         Group reads into paired-end read pairs. Uses name, source_id and sample_id
         as grouping key.
 
         TODO
         Grouping by name should be sufficient since the SAM spec states:
         "Reads/segments having identical QNAME are regarded to come from the same template."
         """
         groups = defaultdict(list)
         for read in reads:
-            groups[(read.source_id, read.name, read.sample_id)].append(read)
+            groups[(read.read.source_id, read.read.name, read.read.sample_id)].append(read)
+        n_skipped = 0
+        n_non_singleton = 0
         for group in groups.values():
-            if len(group) > 2:
-                raise ReadSetError(
-                    f"Read name {group[0].name!r} occurs more than twice in the input file"
-                )
-            yield group
+            if len(group) > 1:
+                n_non_singleton += 1
+            read = ReadSetReader.create_read_from_group(group, distance_threshold)
+            if read is None:
+                n_skipped += 1
+            else:
+                yield [read]
+
+        logger.info(f"Number of non-singleton groups: {n_non_singleton}")
+        logger.info(f"Skipped {n_skipped} groups")
 
     def _usable_alignments(self, chromosome, sample, regions=None):
         """
         Retrieve usable (suficient mapping quality, not secondary etc.)
         alignments from the alignment file
         """
         if regions is None:
@@ -197,15 +286,15 @@
         for s, e in regions:
             for alignment in self._reader.fetch(
                 reference=chromosome, sample=sample, start=s, end=e
             ):
                 # TODO handle additional alignments correctly!
                 # find out why they are sometimes overlapping/redundant
                 if (
-                    alignment.bam_alignment.flag & 2048 != 0
+                    (not self._use_supplementary and alignment.bam_alignment.is_supplementary)
                     or alignment.bam_alignment.mapping_quality < self._mapq_threshold
                     or alignment.bam_alignment.is_secondary
                     or alignment.bam_alignment.is_unmapped
                     or (not self._duplicates and alignment.bam_alignment.is_duplicate)
                 ):
                     continue
                 yield alignment
@@ -219,14 +308,16 @@
 
         If reference is not None, alleles are detected through re-alignment.
 
         Yield Read objects.
         """
         # FIXME hard-coded zero
         numeric_sample_id = 0 if sample is None else self._numeric_sample_ids[sample]
+        number_of_alignments = 0
+        number_of_supplementary_alignments = 0
         if reference is not None:
             # Copy the pyfaidx.FastaRecord into a str for faster access
             reference = reference[:]
             normalized_variants = variants
         else:
             normalized_variants = [variant.normalized() for variant in variants]
 
@@ -251,27 +342,42 @@
                 for line in reader:
                     kmerald_costs[(int(line[0]), int(line[1]))] = line[2]
         else:
             kmerald_costs = None
             calculated_costs = None
             splitted_strings = None
 
+        def get_tag_or_default(aln, tag, default):
+            if aln.bam_alignment.has_tag(tag):
+                return aln.bam_alignment.get_tag(tag)
+            else:
+                return default
+
         for alignment in alignments:
+            barcode = get_tag_or_default(alignment, "BX", "")
+            hp = get_tag_or_default(alignment, "HP", -1)
+            ps = get_tag_or_default(alignment, "PS", -1)
+            # Some 10X bams appear to use a Z type for the PS tag even when they are integers
+            # so here we try to cast to an integer, but if that fails we raise an error
             try:
-                barcode = alignment.bam_alignment.get_tag("BX")
-            except KeyError:
-                barcode = ""
+                ps = int(ps)
+            except ValueError:
+                raise ValueError(
+                    f"Invalid PS tag value ({ps}) in read {alignment.bam_alignment.query_name}. PS must be an integer."
+                )
 
             read = Read(
-                alignment.bam_alignment.qname,
+                alignment.bam_alignment.query_name,
                 alignment.bam_alignment.mapq,
                 alignment.source_id,
                 numeric_sample_id,
                 alignment.bam_alignment.reference_start,
                 barcode,
+                hp,
+                ps,
             )
 
             if reference is None:
                 # Skip variant progress objects that are to the left of this read
                 while (
                     i < len(valid_positions)
                     and valid_positions[i] < alignment.bam_alignment.reference_start
@@ -305,15 +411,25 @@
                     calculated_costs,
                     splitted_strings,
                 )
 
             for j, allele, quality in detected:
                 read.add_variant(variants[j].position, allele, quality)
             if read:  # At least one variant covered and detected
-                yield read
+                number_of_alignments += 1
+                number_of_supplementary_alignments += alignment.bam_alignment.is_supplementary
+                yield AlignedRead(
+                    read,
+                    alignment.bam_alignment.is_supplementary,
+                    alignment.bam_alignment.is_reverse,
+                    alignment.bam_alignment.reference_start,
+                    alignment.bam_alignment.reference_end,
+                )
+
+        logger.info(f"Number of supplementary alignments: {number_of_supplementary_alignments}")
 
     def detect_non_overlapping_variants(self, variants: List[VcfVariant]):
         """
         Checks for deletion variants overlapping other variants and for variants with duplicate
         positions. Returns a set of variant indices, which are conflict with another variant and
         should not be considered for allele detection.
 
@@ -676,14 +792,16 @@
         result = Read(
             read1.name,
             read1.mapqs[0],
             read1.source_id,
             read1.sample_id,
             read1.reference_start,
             read1.BX_tag,
+            read1.HP_tag,
+            read1.PS_tag,
         )
         result.add_mapq(read2.mapqs[0])
     else:
         return read1
 
     i1 = 0
     i2 = 0
```

### Comparing `whatshap-2.2/whatshap/vcf.py` & `whatshap-2.3/whatshap/vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Functions for reading VCFs.
 """
+
 import os
 import sys
 import math
 import logging
 import itertools
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
@@ -302,24 +303,14 @@
         self.genotype_likelihoods: List[List[Optional[GenotypeLikelihoods]]] = [[] for _ in samples]
         self.variants: List[VcfVariant] = []
         self._sample_to_index = {sample: index for index, sample in enumerate(samples)}
 
     def __len__(self) -> int:
         return len(self.variants)
 
-    # fmt: off
-    # def add_sample(self, name, genotypes):
-    # "Add a column to the table"
-    # if len(genotypes) != len(self.variants):
-    # raise ValueError('Expecting as many genotypes as there are variants')
-    # self._name_to_index[name] = len(self.samples)
-    # self.samples.append(name)
-    # self.genotypes.append(genotypes)
-    # fmt: on
-
     def add_variant(
         self,
         variant: VcfVariant,
         genotypes: Sequence[Genotype],
         phases: Sequence[Optional[VariantCallPhase]],
         genotype_likelihoods: Sequence[Optional[GenotypeLikelihoods]],
         allele_depths: Sequence[Optional[int]],
@@ -475,15 +466,15 @@
             else:
                 read_map[phase.block_id] = []
                 for i, allele in enumerate(phase.phase):
                     name = f"{sample}_phase_{i}_block_{phase.block_id}"
                     r = Read(name, mapq, source_id, numeric_sample_id)
                     r.add_variant(variant.position, allele, quality)
                     read_map[phase.block_id].append(r)
-        for key, read_list in read_map.items():
+        for read_list in read_map.values():
             for read in read_list:
                 if len(read) > 1:
                     read.sort()
                     yield read
 
 
 class MixedPhasingError(Exception):
@@ -541,15 +532,17 @@
     def path(self) -> str:
         return self._vcf_reader.filename.decode()
 
     def index_exists(self) -> bool:
         """ "Check if VCF is indexed (.tbi or .csi)"""
         return self._vcf_reader.index is not None
 
-    def _fetch(self, chromosome: str, start: int = 0, end: Optional[int] = None):
+    def _fetch(
+        self, chromosome: str, start: int = 0, end: Optional[int] = None
+    ) -> Iterator[VariantRecord]:
         try:
             records = self._vcf_reader.fetch(chromosome, start=start, stop=end)
         except ValueError as e:
             if "invalid contig" in e.args[0]:
                 raise VcfInvalidChromosome(e.args[0]) from None
             elif "fetch requires an index" in e.args[0]:
                 raise VcfIndexMissing(f"{self._path} is missing an index (.tbi or .csi)") from None
@@ -585,40 +578,40 @@
 
         Multi-ALT sites are skipped.
         """
         for chromosome, records in itertools.groupby(self._vcf_reader, lambda record: record.chrom):
             yield self._process_single_chromosome(chromosome, records)
 
     @staticmethod
-    def _extract_HP_phase(call) -> Optional[VariantCallPhase]:
+    def _extract_HP_phase(call: VariantRecordSample) -> Optional[VariantCallPhase]:
         hp = call.get("HP")
         if hp is None or hp == (".",):
             return None
         fields = [[int(x) for x in s.split("-")] for s in hp]
         for i in range(len(fields)):
             assert fields[0][0] == fields[i][0]
         block_id = fields[0][0]
         order = [field[1] - 1 for field in fields]
         phase = call["GT"]
         phase = tuple(phase[order.index(i)] for i in range(len(order)))
         return VariantCallPhase(block_id=block_id, phase=phase, quality=call.get("PQ", None))
 
     @staticmethod
-    def _extract_GT_PS_phase(call) -> Optional[VariantCallPhase]:
+    def _extract_GT_PS_phase(call: VariantRecordSample) -> Optional[VariantCallPhase]:
         if not call.phased:
             return None
         is_het = not all(x == call["GT"][0] for x in call["GT"])
         if not is_het:
             return None
         block_id = call.get("PS", 0)
         phase = call["GT"]
         return VariantCallPhase(block_id=block_id, phase=phase, quality=call.get("PQ", None))
 
     @staticmethod
-    def _extract_AD_depth(call) -> int:
+    def _extract_AD_depth(call: VariantRecordSample) -> int:
         """
         Allele depth of sample are coded into a single integer to save space in memory.
         Encoding: Lowest 12 bits = depth of allele 0, next 12 bits = depth of allele 1, etc.
         Alleles with depth 0 are included. Maximum allele depths is 4095 (2^12 - 1).
         """
         depths = call["AD"]
         depth_code = 0
@@ -629,15 +622,17 @@
                         logger, "Allele depths of 4096 or higher detected. Cutting them off to 4095"
                     )
                 cnt = min(4095, depth)
                 depth_code = (depth_code << 12) + cnt
 
         return depth_code
 
-    def _process_single_chromosome(self, chromosome: str, records) -> VariantTable:
+    def _process_single_chromosome(
+        self, chromosome: str, records: Iterable[VariantRecord]
+    ) -> VariantTable:
         phase_detected = None
         n_snvs = 0
         n_other = 0
         n_multi = 0
         table = VariantTable(chromosome, self.samples)
         prev_position = None
         for record in records:
```

### Comparing `whatshap-2.2/whatshap/verification.py` & `whatshap-2.3/whatshap/verification.py`

 * *Files identical despite different names*

### Comparing `whatshap-2.2/whatshap.egg-info/PKG-INFO` & `whatshap-2.3/whatshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatshap
-Version: 2.2
+Version: 2.3
 Summary: phase genomic variants using DNA sequencing reads
 Author: WhatsHap authors
 License: MIT
 Project-URL: Homepage, https://github.com/whatshap/whatshap
 Project-URL: Changelog, https://whatshap.readthedocs.io/en/latest/changes.html
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `whatshap-2.2/whatshap.egg-info/SOURCES.txt` & `whatshap-2.3/whatshap.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .editorconfig
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 CITATION.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tox.ini
 .github/issue_template.md
 .github/workflows/ci.yml
-.github/workflows/macos.yml
 doc/Makefile
 doc/README.rst
 doc/changes.rst
 doc/conf.py
 doc/develop.rst
 doc/faq.rst
 doc/guide.rst
@@ -139,24 +139,26 @@
 tests/test_pedigree.py
 tests/test_pedigreegenotyping.py
 tests/test_pedigreephasing.py
 tests/test_pedreader.py
 tests/test_phasing.py
 tests/test_polyphasegenetic.py
 tests/test_priorityqueue.py
+tests/test_read_grouping.py
 tests/test_reads.py
 tests/test_readscoring.py
 tests/test_readselect.py
 tests/test_readsetreader.py
 tests/test_reorder.py
 tests/test_run_compare.py
 tests/test_run_find_snv_candidates.py
 tests/test_run_genotype.py
 tests/test_run_hapcut2vcf.py
 tests/test_run_haplotag.py
+tests/test_run_haplotagphase.py
 tests/test_run_learn.py
 tests/test_run_phase.py
 tests/test_run_polyphase.py
 tests/test_run_split.py
 tests/test_run_stats.py
 tests/test_run_unphase.py
 tests/test_threading.py
@@ -337,14 +339,16 @@
 tests/data/unmapped.bam
 tests/data/unmapped.bam.bai
 tests/data/unphased.vcf
 tests/data/zero-genetic-distance.map
 tests/data/pacbio/.gitignore
 tests/data/pacbio/Makefile
 tests/data/pacbio/hapcut.txt
+tests/data/pacbio/haplotagged.bam
+tests/data/pacbio/haplotagged.bam.bai
 tests/data/pacbio/haplotags.txt
 tests/data/pacbio/pacbio.bam
 tests/data/pacbio/pacbio.bam.bai
 tests/data/pacbio/pacbio.crai
 tests/data/pacbio/pacbio.cram
 tests/data/pacbio/phased.vcf
 tests/data/pacbio/phased.vcf.gz
@@ -396,14 +400,15 @@
 whatshap/priorityqueue.pyi
 whatshap/priorityqueue.pyx
 whatshap/readselect.cpp
 whatshap/readselect.pyi
 whatshap/readselect.pyx
 whatshap/testhelpers.py
 whatshap/timer.py
+whatshap/types.py
 whatshap/utils.py
 whatshap/variant.py
 whatshap/variants.py
 whatshap/vcf.py
 whatshap/verification.py
 whatshap.egg-info/PKG-INFO
 whatshap.egg-info/SOURCES.txt
@@ -413,14 +418,15 @@
 whatshap.egg-info/top_level.txt
 whatshap/cli/__init__.py
 whatshap/cli/compare.py
 whatshap/cli/find_snv_candidates.py
 whatshap/cli/genotype.py
 whatshap/cli/hapcut2vcf.py
 whatshap/cli/haplotag.py
+whatshap/cli/haplotagphase.py
 whatshap/cli/learn.py
 whatshap/cli/phase.py
 whatshap/cli/polyphase.py
 whatshap/cli/polyphasegenetic.py
 whatshap/cli/split.py
 whatshap/cli/stats.py
 whatshap/cli/unphase.py
```

