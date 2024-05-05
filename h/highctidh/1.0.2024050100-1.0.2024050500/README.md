# Comparing `tmp/highctidh-1.0.2024050100.tar.gz` & `tmp/highctidh-1.0.2024050500.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highctidh-1.0.2024050100.tar", last modified: Wed May  1 14:22:24 2024, max compression
+gzip compressed data, was "highctidh-1.0.2024050500.tar", last modified: Sun May  5 15:25:47 2024, max compression
```

## Comparing `highctidh-1.0.2024050100.tar` & `highctidh-1.0.2024050500.tar`

### file list

```diff
@@ -1,373 +1,373 @@
--rw-r--r--   0        0        0       52 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/MANIFEST.in
--rw-r--r--   0        0        0    54119 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/Makefile
--rw-r--r--   0        0        0     7262 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/Makefile.packages
--rw-r--r--   0        0        0     9245 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/README.md
--rw-r--r--   0        0        0       15 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/VERSION
--rwxr-xr-x   0        0        0     1500 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/analyze-costs
--rwxr-xr-x   0        0        0     1051 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/analyze-pr
--rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/annotations.h
--rwxr-xr-x   0        0        0    55100 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/autogen
--rw-r--r--   0        0        0     3516 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/bench.c
--rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding1024.h
--rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding2048.h
--rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding511.h
--rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/binding512.h
--rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/cgo.h
--rwxr-xr-x   0        0        0     3532 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/chain.py
--rw-r--r--   0        0        0      945 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/checkct.c
--rw-r--r--   0        0        0     4341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costisog.py
--rw-r--r--   0        0        0     1564 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costpoly.c
--rw-r--r--   0        0        0     8258 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costpoly.py
--rwxr-xr-x   0        0        0     4505 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/costs.py
--rw-r--r--   0        0        0      239 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/cpucycles.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh.c
--rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh.h
--rw-r--r--   0        0        0     1352 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh_all_clearnamespaces.h
--rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/csidh_namespace.h
--rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/annotations.h
--rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/binding1024.h
--rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/cgo.h
--rw-r--r--   0        0        0     5446 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/common.go
--rw-r--r--   0        0        0      874 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/common_test.go
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh.c
--rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh.h
--rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/csidh_namespace.h
--rw-r--r--   0        0        0     8023 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024.go
--rw-r--r--   0        0        0     1773 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024_bench_test.go
--rw-r--r--   0        0        0     2389 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/ctidh1024_test.go
--rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator.c
--rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator.h
--rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/elligator_namespace.h
--rw-r--r--   0        0        0      833 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/error.go
--rw-r--r--   0        0        0   701424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fiat_p1024.c
--rw-r--r--   0        0        0     4970 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fiat_p1024.h
--rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp.h
--rw-r--r--   0        0        0    14162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp1024.S
--rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp2fiat.c
--rw-r--r--   0        0        0    30384 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_inv1024.c
--rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_namespace.h
--rw-r--r--   0        0        0    30472 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/fp_sqrt1024.c
--rw-r--r--   0        0        0      274 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/golang-misc.c
--rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_minmax.h
--rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort.c
--rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort.h
--rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int32mask.h
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/int64mask.h
--rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont.c
--rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont.h
--rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/mont_namespace.h
--rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/naidne.h
--rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly.c
--rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly.h
--rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes.h
--rw-r--r--   0        0        0     2820 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes1024.c
--rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/proj.h
--rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random.c
--rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random.h
--rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/random_namespace.h
--rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/randombytes.c
--rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/randombytes.h
--rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/skgen.c
--rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps.c
--rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps.h
--rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig.h
--rw-r--r--   0        0        0     3514 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig1024.S
--rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/validate.c
--rw-r--r--   0        0        0     6948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh1024/vectors1024_test.go
--rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/annotations.h
--rw-r--r--   0        0        0      378 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/binding2048.h
--rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/cgo.h
--rw-r--r--   0        0        0     5447 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/common.go
--rw-r--r--   0        0        0      874 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/common_test.go
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh.c
--rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh.h
--rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/csidh_namespace.h
--rw-r--r--   0        0        0     8023 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048.go
--rw-r--r--   0        0        0     1773 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048_bench_test.go
--rw-r--r--   0        0        0     2389 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/ctidh2048_test.go
--rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator.c
--rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator.h
--rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/elligator_namespace.h
--rw-r--r--   0        0        0      833 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/error.go
--rw-r--r--   0        0        0  2648362 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fiat_p2048.c
--rw-r--r--   0        0        0     3115 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fiat_p2048.h
--rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp.h
--rw-r--r--   0        0        0    27054 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp2048.S
--rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp2fiat.c
--rw-r--r--   0        0        0    93576 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_inv2048.c
--rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_namespace.h
--rw-r--r--   0        0        0    93008 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/fp_sqrt2048.c
--rw-r--r--   0        0        0      311 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/golang-misc.c
--rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_minmax.h
--rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort.c
--rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort.h
--rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int32mask.h
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/int64mask.h
--rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont.c
--rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont.h
--rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/mont_namespace.h
--rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/naidne.h
--rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly.c
--rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly.h
--rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes.h
--rw-r--r--   0        0        0     4460 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes2048.c
--rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/proj.h
--rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random.c
--rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random.h
--rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/random_namespace.h
--rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/randombytes.c
--rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/randombytes.h
--rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/skgen.c
--rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps.c
--rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps.h
--rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig.h
--rw-r--r--   0        0        0     5374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig2048.S
--rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/validate.c
--rw-r--r--   0        0        0    10005 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh2048/vectors2048_test.go
--rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/annotations.h
--rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/binding511.h
--rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/cgo.h
--rw-r--r--   0        0        0     5433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/common.go
--rw-r--r--   0        0        0      873 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/common_test.go
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh.c
--rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh.h
--rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/csidh_namespace.h
--rw-r--r--   0        0        0     8016 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511.go
--rw-r--r--   0        0        0     1772 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511_bench_test.go
--rw-r--r--   0        0        0     2388 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/ctidh511_test.go
--rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator.c
--rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator.h
--rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/elligator_namespace.h
--rw-r--r--   0        0        0      832 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/error.go
--rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fiat_p511.c
--rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fiat_p511.h
--rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp.h
--rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp2fiat.c
--rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp511.S
--rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_inv511.c
--rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_namespace.h
--rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/fp_sqrt511.c
--rw-r--r--   0        0        0      272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/golang-misc.c
--rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_minmax.h
--rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort.c
--rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort.h
--rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int32mask.h
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/int64mask.h
--rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont.c
--rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont.h
--rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/mont_namespace.h
--rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/naidne.h
--rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly.c
--rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly.h
--rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes.h
--rw-r--r--   0        0        0     1826 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes511.c
--rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/proj.h
--rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random.c
--rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random.h
--rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/random_namespace.h
--rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/randombytes.c
--rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/randombytes.h
--rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/skgen.c
--rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps.c
--rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps.h
--rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig.h
--rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig511.S
--rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/validate.c
--rw-r--r--   0        0        0     5360 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh511/vectors511_test.go
--rw-r--r--   0        0        0      424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/annotations.h
--rw-r--r--   0        0        0      374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/binding512.h
--rw-r--r--   0        0        0      341 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/cgo.h
--rw-r--r--   0        0        0     5433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/common.go
--rw-r--r--   0        0        0      873 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/common_test.go
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify.c
--rw-r--r--   0        0        0      195 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify.h
--rw-r--r--   0        0        0       55 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_classify_namespace.h
--rw-r--r--   0        0        0      236 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify.c
--rw-r--r--   0        0        0      203 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify.h
--rw-r--r--   0        0        0       59 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/crypto_declassify_namespace.h
--rw-r--r--   0        0        0    11320 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh.c
--rw-r--r--   0        0        0     3301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh.h
--rw-r--r--   0        0        0      583 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/csidh_namespace.h
--rw-r--r--   0        0        0     8016 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512.go
--rw-r--r--   0        0        0     1772 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512_bench_test.go
--rw-r--r--   0        0        0     2388 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/ctidh512_test.go
--rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator.c
--rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator.h
--rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/elligator_namespace.h
--rw-r--r--   0        0        0      832 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/error.go
--rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fiat_p512.c
--rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fiat_p512.h
--rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp.h
--rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp2fiat.c
--rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp512.S
--rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_inv512.c
--rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_namespace.h
--rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/fp_sqrt512.c
--rw-r--r--   0        0        0      271 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/golang-misc.c
--rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_minmax.h
--rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort.c
--rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort.h
--rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int32mask.h
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/int64mask.h
--rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont.c
--rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont.h
--rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/mont_namespace.h
--rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/naidne.h
--rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly.c
--rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly.h
--rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes.h
--rw-r--r--   0        0        0     1822 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes512.c
--rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/proj.h
--rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random.c
--rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random.h
--rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/random_namespace.h
--rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/randombytes.c
--rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/randombytes.h
--rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/skgen.c
--rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps.c
--rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps.h
--rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/steps_untuned.c
--rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig.h
--rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig512.S
--rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/uintbig_namespace.h
--rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/validate.c
--rw-r--r--   0        0        0     5361 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ctidh512/vectors512_test.go
--rwxr-xr-x   0        0        0      433 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/debian-rules
--rwxr-xr-x   0        0        0     5471 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/distmults.py
--rw-r--r--   0        0        0     1978 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator.c
--rw-r--r--   0        0        0      162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator.h
--rw-r--r--   0        0        0       43 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/elligator_namespace.h
--rw-r--r--   0        0        0     2928 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/example-ctidh.c
--rw-r--r--   0        0        0     2943 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/examples_static.c
--rw-r--r--   0        0        0   701424 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p1024.c
--rw-r--r--   0        0        0     4970 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p1024.h
--rw-r--r--   0        0        0  2648362 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p2048.c
--rw-r--r--   0        0        0     3115 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p2048.h
--rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p511.c
--rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p511.h
--rw-r--r--   0        0        0   199383 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p512.c
--rw-r--r--   0        0        0     3734 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fiat_p512.h
--rw-r--r--   0        0        0     4261 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp.h
--rw-r--r--   0        0        0    14162 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp1024.S
--rw-r--r--   0        0        0    27054 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp2048.S
--rw-r--r--   0        0        0    15552 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp2fiat.c
--rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp511.S
--rw-r--r--   0        0        0     7860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp512.S
--rw-r--r--   0        0        0    30384 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv1024.c
--rw-r--r--   0        0        0    93576 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv2048.c
--rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv511.c
--rw-r--r--   0        0        0    11084 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_inv512.c
--rw-r--r--   0        0        0     1272 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_namespace.h
--rw-r--r--   0        0        0    30472 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt1024.c
--rw-r--r--   0        0        0    93008 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt2048.c
--rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt511.c
--rw-r--r--   0        0        0    10975 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/fp_sqrt512.c
--rw-r--r--   0        0        0     1923 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/go-tests/ctidh_test.go
--rwxr-xr-x   0        0        0     5846 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/greedy
--rw-r--r--   0        0        0     5286 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh.h
--rwxr-xr-x   0        0        0    19804 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/__init__.py
--rw-r--r--   0        0        0       27 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/__version__.py
--rwxr-xr-x   0        0        0     5176 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh/bench.py
--rw-r--r--   0        0        0      977 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/highctidh_macros.h
--rw-r--r--   0        0        0      872 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_minmax.h
--rw-r--r--   0        0        0      980 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort.c
--rw-r--r--   0        0        0      794 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort.h
--rw-r--r--   0        0        0    36687 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32_sort_x86.c
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int32mask.h
--rw-r--r--   0        0        0      506 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/int64mask.h
--rwxr-xr-x   0        0        0      452 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/memoized.py
--rw-r--r--   0        0        0    17478 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont.c
--rw-r--r--   0        0        0      950 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont.h
--rw-r--r--   0        0        0      850 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/mont_namespace.h
--rw-r--r--   0        0        0     1127 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/naidne.h
--rw-r--r--   0        0        0    37107 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly.c
--rw-r--r--   0        0        0     2173 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly.h
--rw-r--r--   0        0        0     1948 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/poly_namespace.h
--rw-r--r--   0        0        0     1033 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes.h
--rw-r--r--   0        0        0     2820 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes1024.c
--rw-r--r--   0        0        0     4460 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes2048.c
--rw-r--r--   0        0        0     1826 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes511.c
--rw-r--r--   0        0        0     1822 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes512.c
--rw-r--r--   0        0        0      483 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/primes_namespace.h
--rw-r--r--   0        0        0      731 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/proj.h
--rw-r--r--   0        0        0      733 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/pyproject.toml
--rw-r--r--   0        0        0     3860 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random.c
--rw-r--r--   0        0        0      809 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random.h
--rw-r--r--   0        0        0      301 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/random_namespace.h
--rw-r--r--   0        0        0     1771 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/randombytes.c
--rw-r--r--   0        0        0      224 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/randombytes.h
--rw-r--r--   0        0        0      531 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/setup.cfg
--rw-r--r--   0        0        0    14530 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/setup.py
--rwxr-xr-x   0        0        0     3134 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/sim.py
--rw-r--r--   0        0        0      630 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/skgen.c
--rw-r--r--   0        0        0      319 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/stdeb.cfg
--rw-r--r--   0        0        0      730 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps.c
--rw-r--r--   0        0        0      541 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps.h
--rw-r--r--   0        0        0      163 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps_namespace.h
--rw-r--r--   0        0        0      156 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/steps_untuned.c
--rwxr-xr-x   0        0        0      487 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test-python.sh
--rwxr-xr-x   0        0        0       69 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test-quick.sh
--rw-r--r--   0        0        0    63364 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test.c
--rwxr-xr-x   0        0        0      543 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/test.sh
--rw-r--r--   0        0        0     7175 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/testrandom.c
--rw-r--r--   0        0        0        0 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tests/__init__.py
--rwxr-xr-x   0        0        0    87795 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tests/test_highctidh.py
--rwxr-xr-x   0        0        0      749 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tune2c
--rw-r--r--   0        0        0     2793 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tunecycles.c
--rw-r--r--   0        0        0     1747 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/tunemults.c
--rw-r--r--   0        0        0     7007 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/ubench.c
--rw-r--r--   0        0        0     1688 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig.h
--rw-r--r--   0        0        0     3514 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig1024.S
--rw-r--r--   0        0        0     5374 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig2048.S
--rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig511.S
--rw-r--r--   0        0        0     2566 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig512.S
--rw-r--r--   0        0        0      844 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/uintbig_namespace.h
--rw-r--r--   0        0        0     3099 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/umults.c
--rw-r--r--   0        0        0     2481 2024-05-01 14:22:24.000000 highctidh-1.0.2024050100/validate.c
--rw-r--r--   0        0        0     9805 1970-01-01 00:00:00.000000 highctidh-1.0.2024050100/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/MANIFEST.in
+-rw-r--r--   0        0        0    54119 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/Makefile
+-rw-r--r--   0        0        0     7696 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/Makefile.packages
+-rw-r--r--   0        0        0     9879 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/README.md
+-rw-r--r--   0        0        0       15 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/VERSION
+-rwxr-xr-x   0        0        0     1500 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/analyze-costs
+-rwxr-xr-x   0        0        0     1051 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/analyze-pr
+-rw-r--r--   0        0        0      424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/annotations.h
+-rwxr-xr-x   0        0        0    55100 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/autogen
+-rw-r--r--   0        0        0     3516 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/bench.c
+-rw-r--r--   0        0        0      569 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/binding1024.h
+-rw-r--r--   0        0        0      569 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/binding2048.h
+-rw-r--r--   0        0        0      562 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/binding511.h
+-rw-r--r--   0        0        0      562 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/binding512.h
+-rw-r--r--   0        0        0      341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/cgo.h
+-rwxr-xr-x   0        0        0     3532 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/chain.py
+-rw-r--r--   0        0        0      945 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/checkct.c
+-rw-r--r--   0        0        0     4341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/costisog.py
+-rw-r--r--   0        0        0     1564 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/costpoly.c
+-rw-r--r--   0        0        0     8258 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/costpoly.py
+-rwxr-xr-x   0        0        0     4505 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/costs.py
+-rw-r--r--   0        0        0      239 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/cpucycles.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/csidh.h
+-rw-r--r--   0        0        0     1352 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/csidh_all_clearnamespaces.h
+-rw-r--r--   0        0        0      583 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/csidh_namespace.h
+-rw-r--r--   0        0        0      424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/annotations.h
+-rw-r--r--   0        0        0      569 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/binding1024.h
+-rw-r--r--   0        0        0      341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/cgo.h
+-rw-r--r--   0        0        0     5609 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/common.go
+-rw-r--r--   0        0        0      874 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/csidh_namespace.h
+-rw-r--r--   0        0        0     8033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/ctidh1024.go
+-rw-r--r--   0        0        0     1773 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/ctidh1024_bench_test.go
+-rw-r--r--   0        0        0     2389 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/ctidh1024_test.go
+-rw-r--r--   0        0        0     1978 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/elligator_namespace.h
+-rw-r--r--   0        0        0      833 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/error.go
+-rw-r--r--   0        0        0   701424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fiat_p1024.c
+-rw-r--r--   0        0        0     4970 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fiat_p1024.h
+-rw-r--r--   0        0        0     4261 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp.h
+-rw-r--r--   0        0        0    14162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp1024.S
+-rw-r--r--   0        0        0    15535 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp2fiat.c
+-rw-r--r--   0        0        0    30384 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp_inv1024.c
+-rw-r--r--   0        0        0     1272 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp_namespace.h
+-rw-r--r--   0        0        0    30472 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/fp_sqrt1024.c
+-rw-r--r--   0        0        0       87 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/mont.c
+-rw-r--r--   0        0        0      950 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/mont.h
+-rw-r--r--   0        0        0      850 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/primes.h
+-rw-r--r--   0        0        0     2820 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/primes1024.c
+-rw-r--r--   0        0        0      483 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/random.c
+-rw-r--r--   0        0        0      809 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/random.h
+-rw-r--r--   0        0        0      301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/random_namespace.h
+-rw-r--r--   0        0        0     1835 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/randombytes.c
+-rw-r--r--   0        0        0      546 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/steps.c
+-rw-r--r--   0        0        0      541 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/steps.h
+-rw-r--r--   0        0        0      163 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/uintbig.h
+-rw-r--r--   0        0        0     3514 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/uintbig1024.S
+-rw-r--r--   0        0        0      844 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/validate.c
+-rw-r--r--   0        0        0     6948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh1024/vectors1024_test.go
+-rw-r--r--   0        0        0      424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/annotations.h
+-rw-r--r--   0        0        0      569 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/binding2048.h
+-rw-r--r--   0        0        0      341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/cgo.h
+-rw-r--r--   0        0        0     5610 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/common.go
+-rw-r--r--   0        0        0      874 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/csidh_namespace.h
+-rw-r--r--   0        0        0     8033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/ctidh2048.go
+-rw-r--r--   0        0        0     1773 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/ctidh2048_bench_test.go
+-rw-r--r--   0        0        0     2389 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/ctidh2048_test.go
+-rw-r--r--   0        0        0     1978 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/elligator_namespace.h
+-rw-r--r--   0        0        0      833 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/error.go
+-rw-r--r--   0        0        0  2648362 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fiat_p2048.c
+-rw-r--r--   0        0        0     3115 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fiat_p2048.h
+-rw-r--r--   0        0        0     4261 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp.h
+-rw-r--r--   0        0        0    27054 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp2048.S
+-rw-r--r--   0        0        0    15535 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp2fiat.c
+-rw-r--r--   0        0        0    93576 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp_inv2048.c
+-rw-r--r--   0        0        0     1272 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp_namespace.h
+-rw-r--r--   0        0        0    93008 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/fp_sqrt2048.c
+-rw-r--r--   0        0        0       87 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/mont.c
+-rw-r--r--   0        0        0      950 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/mont.h
+-rw-r--r--   0        0        0      850 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/primes.h
+-rw-r--r--   0        0        0     4460 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/primes2048.c
+-rw-r--r--   0        0        0      483 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/random.c
+-rw-r--r--   0        0        0      809 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/random.h
+-rw-r--r--   0        0        0      301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/random_namespace.h
+-rw-r--r--   0        0        0     1835 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/randombytes.c
+-rw-r--r--   0        0        0      546 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/steps.c
+-rw-r--r--   0        0        0      541 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/steps.h
+-rw-r--r--   0        0        0      163 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/uintbig.h
+-rw-r--r--   0        0        0     5374 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/uintbig2048.S
+-rw-r--r--   0        0        0      844 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/validate.c
+-rw-r--r--   0        0        0    10005 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh2048/vectors2048_test.go
+-rw-r--r--   0        0        0      424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/annotations.h
+-rw-r--r--   0        0        0      562 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/binding511.h
+-rw-r--r--   0        0        0      341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/cgo.h
+-rw-r--r--   0        0        0     5595 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/common.go
+-rw-r--r--   0        0        0      873 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/csidh_namespace.h
+-rw-r--r--   0        0        0     8024 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/ctidh511.go
+-rw-r--r--   0        0        0     1772 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/ctidh511_bench_test.go
+-rw-r--r--   0        0        0     2388 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/ctidh511_test.go
+-rw-r--r--   0        0        0     1978 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/elligator_namespace.h
+-rw-r--r--   0        0        0      832 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/error.go
+-rw-r--r--   0        0        0   199383 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fiat_p511.c
+-rw-r--r--   0        0        0     3734 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fiat_p511.h
+-rw-r--r--   0        0        0     4261 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp.h
+-rw-r--r--   0        0        0    15535 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp511.S
+-rw-r--r--   0        0        0    11084 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp_inv511.c
+-rw-r--r--   0        0        0     1272 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp_namespace.h
+-rw-r--r--   0        0        0    10975 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/fp_sqrt511.c
+-rw-r--r--   0        0        0       86 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/mont.c
+-rw-r--r--   0        0        0      950 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/mont.h
+-rw-r--r--   0        0        0      850 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/primes.h
+-rw-r--r--   0        0        0     1826 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/primes511.c
+-rw-r--r--   0        0        0      483 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/random.c
+-rw-r--r--   0        0        0      809 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/random.h
+-rw-r--r--   0        0        0      301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/random_namespace.h
+-rw-r--r--   0        0        0     1835 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/randombytes.c
+-rw-r--r--   0        0        0      546 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/steps.c
+-rw-r--r--   0        0        0      541 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/steps.h
+-rw-r--r--   0        0        0      163 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/uintbig.h
+-rw-r--r--   0        0        0     2566 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/uintbig511.S
+-rw-r--r--   0        0        0      844 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/validate.c
+-rw-r--r--   0        0        0     5360 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh511/vectors511_test.go
+-rw-r--r--   0        0        0      424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/annotations.h
+-rw-r--r--   0        0        0      562 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/binding512.h
+-rw-r--r--   0        0        0      341 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/cgo.h
+-rw-r--r--   0        0        0     5602 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/common.go
+-rw-r--r--   0        0        0      873 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/common_test.go
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_classify.c
+-rw-r--r--   0        0        0      195 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_classify.h
+-rw-r--r--   0        0        0       55 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_classify_namespace.h
+-rw-r--r--   0        0        0      236 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_declassify.c
+-rw-r--r--   0        0        0      203 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_declassify.h
+-rw-r--r--   0        0        0       59 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/crypto_declassify_namespace.h
+-rw-r--r--   0        0        0    11320 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/csidh.c
+-rw-r--r--   0        0        0     3301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/csidh.h
+-rw-r--r--   0        0        0      583 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/csidh_namespace.h
+-rw-r--r--   0        0        0     8024 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/ctidh512.go
+-rw-r--r--   0        0        0     1772 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/ctidh512_bench_test.go
+-rw-r--r--   0        0        0     2388 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/ctidh512_test.go
+-rw-r--r--   0        0        0     1978 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/elligator_namespace.h
+-rw-r--r--   0        0        0      832 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/error.go
+-rw-r--r--   0        0        0   199383 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fiat_p512.c
+-rw-r--r--   0        0        0     3734 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fiat_p512.h
+-rw-r--r--   0        0        0     4261 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp.h
+-rw-r--r--   0        0        0    15535 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp512.S
+-rw-r--r--   0        0        0    11084 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp_inv512.c
+-rw-r--r--   0        0        0     1272 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp_namespace.h
+-rw-r--r--   0        0        0    10975 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/fp_sqrt512.c
+-rw-r--r--   0        0        0       86 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/golang-misc.c
+-rw-r--r--   0        0        0      872 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/int64mask.h
+-rw-r--r--   0        0        0    17478 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/mont.c
+-rw-r--r--   0        0        0      950 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/mont.h
+-rw-r--r--   0        0        0      850 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/primes.h
+-rw-r--r--   0        0        0     1822 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/primes512.c
+-rw-r--r--   0        0        0      483 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/proj.h
+-rw-r--r--   0        0        0     3860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/random.c
+-rw-r--r--   0        0        0      809 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/random.h
+-rw-r--r--   0        0        0      301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/random_namespace.h
+-rw-r--r--   0        0        0     1835 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/randombytes.c
+-rw-r--r--   0        0        0      546 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/randombytes.h
+-rw-r--r--   0        0        0      630 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/skgen.c
+-rw-r--r--   0        0        0      730 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/steps.c
+-rw-r--r--   0        0        0      541 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/steps.h
+-rw-r--r--   0        0        0      163 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/steps_untuned.c
+-rw-r--r--   0        0        0     1688 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/uintbig.h
+-rw-r--r--   0        0        0     2566 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/uintbig512.S
+-rw-r--r--   0        0        0      844 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/uintbig_namespace.h
+-rw-r--r--   0        0        0     2481 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/validate.c
+-rw-r--r--   0        0        0     5361 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ctidh512/vectors512_test.go
+-rwxr-xr-x   0        0        0      433 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/debian-rules
+-rwxr-xr-x   0        0        0     5471 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/distmults.py
+-rw-r--r--   0        0        0     1978 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/elligator.c
+-rw-r--r--   0        0        0      162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/elligator.h
+-rw-r--r--   0        0        0       43 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/elligator_namespace.h
+-rw-r--r--   0        0        0     3079 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/example-ctidh.c
+-rw-r--r--   0        0        0     2943 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/examples_static.c
+-rw-r--r--   0        0        0   701424 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p1024.c
+-rw-r--r--   0        0        0     4970 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p1024.h
+-rw-r--r--   0        0        0  2648362 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p2048.c
+-rw-r--r--   0        0        0     3115 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p2048.h
+-rw-r--r--   0        0        0   199383 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p511.c
+-rw-r--r--   0        0        0     3734 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p511.h
+-rw-r--r--   0        0        0   199383 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p512.c
+-rw-r--r--   0        0        0     3734 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fiat_p512.h
+-rw-r--r--   0        0        0     4261 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp.h
+-rw-r--r--   0        0        0    14162 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp1024.S
+-rw-r--r--   0        0        0    27054 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp2048.S
+-rw-r--r--   0        0        0    15535 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp2fiat.c
+-rw-r--r--   0        0        0     7860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp511.S
+-rw-r--r--   0        0        0     7860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp512.S
+-rw-r--r--   0        0        0    30384 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_inv1024.c
+-rw-r--r--   0        0        0    93576 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_inv2048.c
+-rw-r--r--   0        0        0    11084 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_inv511.c
+-rw-r--r--   0        0        0    11084 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_inv512.c
+-rw-r--r--   0        0        0     1272 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_namespace.h
+-rw-r--r--   0        0        0    30472 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_sqrt1024.c
+-rw-r--r--   0        0        0    93008 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_sqrt2048.c
+-rw-r--r--   0        0        0    10975 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_sqrt511.c
+-rw-r--r--   0        0        0    10975 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/fp_sqrt512.c
+-rw-r--r--   0        0        0     1923 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/go-tests/ctidh_test.go
+-rwxr-xr-x   0        0        0     5846 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/greedy
+-rw-r--r--   0        0        0     5286 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/highctidh.h
+-rwxr-xr-x   0        0        0    19804 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/highctidh/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/highctidh/__version__.py
+-rwxr-xr-x   0        0        0     5176 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/highctidh/bench.py
+-rw-r--r--   0        0        0      977 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/highctidh_macros.h
+-rw-r--r--   0        0        0      872 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int32_minmax.h
+-rw-r--r--   0        0        0      980 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int32_sort.c
+-rw-r--r--   0        0        0      794 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int32_sort.h
+-rw-r--r--   0        0        0    36687 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int32_sort_x86.c
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int32mask.h
+-rw-r--r--   0        0        0      506 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/int64mask.h
+-rwxr-xr-x   0        0        0      452 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/memoized.py
+-rw-r--r--   0        0        0    17478 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/mont.c
+-rw-r--r--   0        0        0      950 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/mont.h
+-rw-r--r--   0        0        0      850 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/mont_namespace.h
+-rw-r--r--   0        0        0     1127 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/naidne.h
+-rw-r--r--   0        0        0    37107 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/poly.c
+-rw-r--r--   0        0        0     2173 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/poly.h
+-rw-r--r--   0        0        0     1948 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/poly_namespace.h
+-rw-r--r--   0        0        0     1033 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes.h
+-rw-r--r--   0        0        0     2820 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes1024.c
+-rw-r--r--   0        0        0     4460 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes2048.c
+-rw-r--r--   0        0        0     1826 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes511.c
+-rw-r--r--   0        0        0     1822 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes512.c
+-rw-r--r--   0        0        0      483 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/primes_namespace.h
+-rw-r--r--   0        0        0      731 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/proj.h
+-rw-r--r--   0        0        0      733 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/pyproject.toml
+-rw-r--r--   0        0        0     3860 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/random.c
+-rw-r--r--   0        0        0      809 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/random.h
+-rw-r--r--   0        0        0      301 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/random_namespace.h
+-rw-r--r--   0        0        0     1792 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/randombytes.c
+-rw-r--r--   0        0        0      546 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/randombytes.h
+-rw-r--r--   0        0        0      531 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/setup.cfg
+-rw-r--r--   0        0        0    15066 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/setup.py
+-rwxr-xr-x   0        0        0     3134 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/sim.py
+-rw-r--r--   0        0        0      630 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/skgen.c
+-rw-r--r--   0        0        0      319 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/stdeb.cfg
+-rw-r--r--   0        0        0      730 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/steps.c
+-rw-r--r--   0        0        0      541 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/steps.h
+-rw-r--r--   0        0        0      163 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/steps_namespace.h
+-rw-r--r--   0        0        0      156 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/steps_untuned.c
+-rwxr-xr-x   0        0        0      487 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/test-python.sh
+-rwxr-xr-x   0        0        0       69 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/test-quick.sh
+-rw-r--r--   0        0        0    63364 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/test.c
+-rwxr-xr-x   0        0        0      543 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/test.sh
+-rw-r--r--   0        0        0     7175 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/testrandom.c
+-rw-r--r--   0        0        0        0 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/tests/__init__.py
+-rwxr-xr-x   0        0        0    87795 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/tests/test_highctidh.py
+-rwxr-xr-x   0        0        0      749 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/tune2c
+-rw-r--r--   0        0        0     2793 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/tunecycles.c
+-rw-r--r--   0        0        0     1747 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/tunemults.c
+-rw-r--r--   0        0        0     7007 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/ubench.c
+-rw-r--r--   0        0        0     1688 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig.h
+-rw-r--r--   0        0        0     3514 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig1024.S
+-rw-r--r--   0        0        0     5374 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig2048.S
+-rw-r--r--   0        0        0     2566 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig511.S
+-rw-r--r--   0        0        0     2566 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig512.S
+-rw-r--r--   0        0        0      844 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/uintbig_namespace.h
+-rw-r--r--   0        0        0     3099 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/umults.c
+-rw-r--r--   0        0        0     2481 2024-05-05 15:25:47.000000 highctidh-1.0.2024050500/validate.c
+-rw-r--r--   0        0        0    10439 1970-01-01 00:00:00.000000 highctidh-1.0.2024050500/PKG-INFO
```

### Comparing `highctidh-1.0.2024050100/Makefile` & `highctidh-1.0.2024050500/Makefile`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/Makefile.packages` & `highctidh-1.0.2024050500/Makefile.packages`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,26 @@
 	SOURCE_DATE_EPOCH=${SOURCE_DATE_EPOCH} python3 -m build --wheel
 	-ls -alh ${WORKDIR}/dist/*.whl
 	-sha256sum ${WORKDIR}/dist/*.whl
 
 test:
 	python3 setup.py test
 
+test-python:
+	mkdir -p build/src
+	mkdir -p dist/tmp
+	python3 -m build
+	pip install --break-system-packages --force-reinstall dist/highctidh-*.whl
+	python3 -c 'from highctidh import bench; bench.simple_bench()'
+	python3 -m pytest -v -n auto --doctest-modules -k 511
+	python3 -m pytest -v -n auto --doctest-modules -k 512
+	python3 -m pytest -v -n auto --doctest-modules -k 1024
+	python3 -m pytest -v -n auto --doctest-modules -k 2048
+
+
 sdist: ${SDIST_GZ}
 ${SDIST_GZ}:
 	-mkdir -p dist/source
 	-mkdir -p build/tmp
 	SOURCE_DATE_EPOCH=${SOURCE_DATE_EPOCH} flit build \
 			  --format sdist
 	-ls -alh ${SDIST_GZ}
```

### Comparing `highctidh-1.0.2024050100/README.md` & `highctidh-1.0.2024050500/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -155,26 +155,45 @@
 - Rockylinux 9, 9.3 (GNU libc)
 - Solaris 11.4 (Solaris libc)
 - Ubuntu 22.03, 23.10, 24.04 (GNU libc)
 - Windows Server 2019, 2022 (MSVCRT)
 
 ## Notes on building
 
-Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is supported using the
-`gmake` command. GNU/Linux and MacOS are supported with the `make` command.
+Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is
+supported using the `gmake` command. GNU/Linux and MacOS are supported with the
+`make` command.
 
-Windows support is extremely experimental. The Python and Golang modules may
-not be functional on Windows. Building the main C library on Windows Server
-2019 and Windows Server 2022 should be possible with `clang` as is demonstrated
-in the continuous integration configuration `windows-fiat-c-library-test.yml`.
-It has only been tested with the Windows Server 2022 image preloaded with
-`clang`, `bash`, `make`, and other related tools
+MacOS 11, 12, 13, and 14 support is functional for building the C library.
+MacOS 14 support is functional for the Golang bindings with Golang 1.19, 1.20,
+1.21.x, and 1.22.0.
+MacOS 14 supports the Python module with Python 3.9, 3.10, 3.11, and 3.12.
+
+Windows support is extremely experimental. The Python and Golang modules are
+almost certianly not be functional on Windows. Building the main C library on
+Windows Server 2019 and Windows Server 2022 should be possible with `clang` as
+is demonstrated in the continuous integration configuration
+`windows-fiat-c-library-test.yml`.  It has only been tested with the Windows
+Server 2022 image preloaded with `clang`, `bash`, `make`, and other related
+tools
 [https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md](available
 as a part of the CI configuration).
 
+Building and performing minimal testing manually requires using `bash` as
+provided by `git` on Windows, GNU `make`, and `clang` using the following
+commands:
+```
+export HIGHCTIDH_PORTABLE=1
+export WINDOWS=1
+export CC=${{ matrix.CC }} MAKE=make
+mkdir -p src/build/src
+mkdir -p src/dist/tmp
+cd src/ && make && make testrandom test512 && ./testrandom && ./test512
+```
+
 ### Additional notes on building the C library
  
 To build and install we recommend:
 ```
    sudo apt install gcc clang make
    make
    sudo make install
```

### Comparing `highctidh-1.0.2024050100/analyze-costs` & `highctidh-1.0.2024050500/analyze-costs`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/analyze-pr` & `highctidh-1.0.2024050500/analyze-pr`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/autogen` & `highctidh-1.0.2024050500/autogen`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/bench.c` & `highctidh-1.0.2024050500/bench.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/chain.py` & `highctidh-1.0.2024050500/chain.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/checkct.c` & `highctidh-1.0.2024050500/checkct.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/costisog.py` & `highctidh-1.0.2024050500/costisog.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/costpoly.c` & `highctidh-1.0.2024050500/costpoly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/costpoly.py` & `highctidh-1.0.2024050500/costpoly.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/costs.py` & `highctidh-1.0.2024050500/costs.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/csidh.c` & `highctidh-1.0.2024050500/csidh.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/csidh.h` & `highctidh-1.0.2024050500/csidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/csidh_all_clearnamespaces.h` & `highctidh-1.0.2024050500/csidh_all_clearnamespaces.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/csidh_namespace.h` & `highctidh-1.0.2024050500/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/common.go` & `highctidh-1.0.2024050500/ctidh511/common.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-package ctidh1024
+package ctidh511
 
 /*
- #cgo CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -O2
+ #cgo CFLAGS: -DBITS=511 -DCGONUTS -O2
  #cgo LDFLAGS:
- #cgo linux CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
  #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
  #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
  #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
- #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -D__ARM64__ -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
  #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
- #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -march=native -mtune=native -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // Generic flags for amd64
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
  #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
- #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -DCGONUTS -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
  #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
  #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
@@ -65,23 +65,23 @@
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
  #cgo mipsle CFLAGS: -DPLATFORM=mipsle -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
  // CC=mips-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=mips  go build
  // With clang, -fforce-enable-int128 must be added to the CFLAGS
  #cgo mips CFLAGS: -DPLATFORM=mips -DPLATFORM_SIZE=32 -DHIGHCTIDH_PORTABLE=1
 
- // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
+ // CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
  #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
  #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
- #include "binding1024.h"
+ #include "binding511.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
 	"unsafe"
 
@@ -89,20 +89,20 @@
 )
 
 //
 // This function wraps go_fillrandom, so we can emulate the calls from the
 // C library and test the results
 //
 func test_go_fillrandom(context unsafe.Pointer, outptr []byte) {
-	highctidh_1024_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
+	highctidh_511_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
 }
 
 // This is called from the C library, DO NOT CHANGE THE FUNCTION INTERFACE
-//export highctidh_1024_go_fillrandom
-func highctidh_1024_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
+//export highctidh_511_go_fillrandom
+func highctidh_511_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
 	rng := gopointer.Restore(context).(io.Reader)
 	buf := make([]byte, outsz)
 	count, err := rng.Read(buf)
 	if err != nil {
 		panic(err)
 	}
 	if count != int(outsz) {
```

### Comparing `highctidh-1.0.2024050100/ctidh1024/common_test.go` & `highctidh-1.0.2024050500/ctidh1024/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/csidh.c` & `highctidh-1.0.2024050500/ctidh1024/csidh.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/csidh.h` & `highctidh-1.0.2024050500/ctidh1024/csidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/csidh_namespace.h` & `highctidh-1.0.2024050500/ctidh1024/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/ctidh1024.go` & `highctidh-1.0.2024050500/ctidh1024/ctidh1024.go`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 package ctidh1024
 
 /*
 #include "binding1024.h"
 #include <csidh.h>
 
-extern ctidh_fillrandom fillrandom_custom;
+extern ctidh_fillrandom fillrandom_1024_custom;
 
 __attribute__((weak))
 void custom_gen_private(void *const context, private_key *priv) {
-  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_custom);
+  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_1024_custom);
 }
 */
 import "C"
 import (
 	"crypto/hmac"
 	"encoding/base64"
 	"io"
```

### Comparing `highctidh-1.0.2024050100/ctidh1024/ctidh1024_bench_test.go` & `highctidh-1.0.2024050500/ctidh1024/ctidh1024_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/ctidh1024_test.go` & `highctidh-1.0.2024050500/ctidh1024/ctidh1024_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/elligator.c` & `highctidh-1.0.2024050500/ctidh1024/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/error.go` & `highctidh-1.0.2024050500/ctidh1024/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fiat_p1024.c` & `highctidh-1.0.2024050500/ctidh1024/fiat_p1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fiat_p1024.h` & `highctidh-1.0.2024050500/ctidh1024/fiat_p1024.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp.h` & `highctidh-1.0.2024050500/ctidh1024/fp.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp1024.S` & `highctidh-1.0.2024050500/ctidh1024/fp1024.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp2fiat.c` & `highctidh-1.0.2024050500/ctidh1024/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
+#if HIGHCTIDH_PORTABLE == 0 && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
-#elif defined(CGONUTS)
-#define DONTMINDIFIDO
-
 #else
+#if defined(CGONUTS)
+#define DONTMINDIFIDO
+#endif
 /*
  * The definitions in this unit are only needed when they are not provided
  * by the optimizied assembly units.
  */
 
 /*
  * These are replacements for uintbig512.S:
```

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp_inv1024.c` & `highctidh-1.0.2024050500/ctidh1024/fp_inv1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp_namespace.h` & `highctidh-1.0.2024050500/ctidh1024/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/fp_sqrt1024.c` & `highctidh-1.0.2024050500/ctidh1024/fp_sqrt1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/int32_minmax.h` & `highctidh-1.0.2024050500/ctidh1024/int32_minmax.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/int32_sort.c` & `highctidh-1.0.2024050500/ctidh1024/int32_sort.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/int32_sort.h` & `highctidh-1.0.2024050500/ctidh1024/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/int32_sort_x86.c` & `highctidh-1.0.2024050500/ctidh1024/int32_sort_x86.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/mont.c` & `highctidh-1.0.2024050500/ctidh1024/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/mont.h` & `highctidh-1.0.2024050500/ctidh1024/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/mont_namespace.h` & `highctidh-1.0.2024050500/ctidh1024/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/naidne.h` & `highctidh-1.0.2024050500/ctidh1024/naidne.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/poly.c` & `highctidh-1.0.2024050500/ctidh1024/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/poly.h` & `highctidh-1.0.2024050500/ctidh1024/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/poly_namespace.h` & `highctidh-1.0.2024050500/ctidh1024/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/primes.h` & `highctidh-1.0.2024050500/ctidh1024/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/primes1024.c` & `highctidh-1.0.2024050500/ctidh1024/primes1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/proj.h` & `highctidh-1.0.2024050500/ctidh1024/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/random.c` & `highctidh-1.0.2024050500/ctidh1024/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/random.h` & `highctidh-1.0.2024050500/ctidh1024/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/randombytes.c` & `highctidh-1.0.2024050500/ctidh1024/randombytes.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 #include "randombytes.h"
 
 #include <stdlib.h>
-#ifndef _MSC_VER
-#include <unistd.h>
-#include <fcntl.h>
-#else // e.g. (defined(__Windows__) || defined (__WIN64))
-#include <basetsd.h>
-#define ssize_t SSIZE_T
-#include <windows.h>
-#define SystemFunction036 NTAPI SystemFunction036
-#include <ntsecapi.h>
-#undef SystemFunction036
-#pragma comment(lib, "advapi32.lib")
-#define getrandom(x, y) RtlGenRandom(x, y)
-#endif
 
 #include "crypto_classify.h"
 #include "random_namespace.h"
 
 #if defined(GETRANDOM) && (defined(__linux__) || defined(__sun))
 #include <sys/random.h>
 
@@ -26,28 +13,45 @@
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i, 0)))
       exit(2);
   crypto_classify(x,l);
 }
 
+#elif (defined(GETRANDOM) && defined(__Darwin__))
+#include <sys/random.h>
+// This could be CCRandomGenerateBytes
+void randombytes(void *x, size_t l)
+{
+  ssize_t n;
+  for (size_t i = 0; i < l; i += n)
+    if (0 >= (n = getentropy((char *) x + i, l - i)))
+      exit(2);
+  crypto_classify(x,l);
+}
+
 #elif (defined(__Windows__) || defined(__WIN64) || defined(__WIN32))
 /*
  *
  * XXX This is not secure or audited or even worth considering for anything
  * beyond proof of concept that the software can be built on Windows.
  *
  * DO NOT USE THIS FOR ANYTHING SERIOUS AT ALL - THIS IS NOT REASONABLE OR SAFE
  * AND HAS NOT BEEN AUDITED BY ANYONE. THIS IS A "IT COMPILES" LEVEL OF
  * COMPLETENESS.
  *
  * YOU HAVE BEEN WARNED. THIS, LIKE THE REST OF THE LIBRARY, IS NOT ELIGIBLE
  * FOR A CVE!
  */
 
+ssize_t getrandom(char *buf, size_t buflen);
+#include <windows.h>
+#include <ntsecapi.h>
+#define getrandom(x, y) RtlGenRandom(x, y)
+
 void randombytes(void *x, size_t l)
 {
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i)))
       exit(2);
   crypto_classify(x,l);
```

### Comparing `highctidh-1.0.2024050100/ctidh1024/skgen.c` & `highctidh-1.0.2024050500/ctidh1024/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/steps.c` & `highctidh-1.0.2024050500/ctidh1024/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/steps.h` & `highctidh-1.0.2024050500/ctidh1024/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/uintbig.h` & `highctidh-1.0.2024050500/ctidh1024/uintbig.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/uintbig1024.S` & `highctidh-1.0.2024050500/ctidh1024/uintbig1024.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/uintbig_namespace.h` & `highctidh-1.0.2024050500/ctidh1024/uintbig_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/validate.c` & `highctidh-1.0.2024050500/ctidh1024/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh1024/vectors1024_test.go` & `highctidh-1.0.2024050500/ctidh1024/vectors1024_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/common.go` & `highctidh-1.0.2024050500/ctidh2048/common.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 package ctidh2048
 
 /*
- #cgo CFLAGS: -DBITS=2048 -DGETRANDOM -DCGONUTS -O2
+ #cgo CFLAGS: -DBITS=2048 -DCGONUTS -O2
  #cgo LDFLAGS:
  #cgo linux CFLAGS: -DBITS=2048 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
  #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
  #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
  #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
- #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -D__ARM64__ -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
  #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
- #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -march=native -mtune=native -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // Generic flags for amd64 
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
  #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
- #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -DCGONUTS -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
  #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
  #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
```

### Comparing `highctidh-1.0.2024050100/ctidh2048/common_test.go` & `highctidh-1.0.2024050500/ctidh2048/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/csidh.c` & `highctidh-1.0.2024050500/ctidh2048/csidh.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/csidh.h` & `highctidh-1.0.2024050500/ctidh2048/csidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/csidh_namespace.h` & `highctidh-1.0.2024050500/ctidh2048/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/ctidh2048.go` & `highctidh-1.0.2024050500/ctidh2048/ctidh2048.go`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 package ctidh2048
 
 /*
 #include "binding2048.h"
 #include <csidh.h>
 
-extern ctidh_fillrandom fillrandom_custom;
+extern ctidh_fillrandom fillrandom_2048_custom;
 
 __attribute__((weak))
 void custom_gen_private(void *const context, private_key *priv) {
-  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_custom);
+  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_2048_custom);
 }
 */
 import "C"
 import (
 	"crypto/hmac"
 	"encoding/base64"
 	"io"
```

### Comparing `highctidh-1.0.2024050100/ctidh2048/ctidh2048_bench_test.go` & `highctidh-1.0.2024050500/ctidh2048/ctidh2048_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/ctidh2048_test.go` & `highctidh-1.0.2024050500/ctidh2048/ctidh2048_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/elligator.c` & `highctidh-1.0.2024050500/ctidh2048/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/error.go` & `highctidh-1.0.2024050500/ctidh2048/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fiat_p2048.c` & `highctidh-1.0.2024050500/ctidh2048/fiat_p2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fiat_p2048.h` & `highctidh-1.0.2024050500/ctidh2048/fiat_p2048.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp.h` & `highctidh-1.0.2024050500/ctidh2048/fp.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp2048.S` & `highctidh-1.0.2024050500/ctidh2048/fp2048.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp2fiat.c` & `highctidh-1.0.2024050500/ctidh2048/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
+#if HIGHCTIDH_PORTABLE == 0 && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
-#elif defined(CGONUTS)
-#define DONTMINDIFIDO
-
 #else
+#if defined(CGONUTS)
+#define DONTMINDIFIDO
+#endif
 /*
  * The definitions in this unit are only needed when they are not provided
  * by the optimizied assembly units.
  */
 
 /*
  * These are replacements for uintbig512.S:
```

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp_inv2048.c` & `highctidh-1.0.2024050500/ctidh2048/fp_inv2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp_namespace.h` & `highctidh-1.0.2024050500/ctidh2048/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/fp_sqrt2048.c` & `highctidh-1.0.2024050500/ctidh2048/fp_sqrt2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/int32_minmax.h` & `highctidh-1.0.2024050500/ctidh2048/int32_minmax.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/int32_sort.c` & `highctidh-1.0.2024050500/ctidh2048/int32_sort.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/int32_sort.h` & `highctidh-1.0.2024050500/ctidh2048/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/int32_sort_x86.c` & `highctidh-1.0.2024050500/ctidh2048/int32_sort_x86.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/mont.c` & `highctidh-1.0.2024050500/ctidh2048/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/mont.h` & `highctidh-1.0.2024050500/ctidh2048/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/mont_namespace.h` & `highctidh-1.0.2024050500/ctidh2048/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/naidne.h` & `highctidh-1.0.2024050500/ctidh2048/naidne.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/poly.c` & `highctidh-1.0.2024050500/ctidh2048/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/poly.h` & `highctidh-1.0.2024050500/ctidh2048/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/poly_namespace.h` & `highctidh-1.0.2024050500/ctidh2048/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/primes.h` & `highctidh-1.0.2024050500/ctidh2048/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/primes2048.c` & `highctidh-1.0.2024050500/ctidh2048/primes2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/proj.h` & `highctidh-1.0.2024050500/ctidh2048/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/random.c` & `highctidh-1.0.2024050500/ctidh2048/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/random.h` & `highctidh-1.0.2024050500/ctidh2048/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/randombytes.c` & `highctidh-1.0.2024050500/ctidh2048/randombytes.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 #include "randombytes.h"
 
 #include <stdlib.h>
-#ifndef _MSC_VER
-#include <unistd.h>
-#include <fcntl.h>
-#else // e.g. (defined(__Windows__) || defined (__WIN64))
-#include <basetsd.h>
-#define ssize_t SSIZE_T
-#include <windows.h>
-#define SystemFunction036 NTAPI SystemFunction036
-#include <ntsecapi.h>
-#undef SystemFunction036
-#pragma comment(lib, "advapi32.lib")
-#define getrandom(x, y) RtlGenRandom(x, y)
-#endif
 
 #include "crypto_classify.h"
 #include "random_namespace.h"
 
 #if defined(GETRANDOM) && (defined(__linux__) || defined(__sun))
 #include <sys/random.h>
 
@@ -26,28 +13,45 @@
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i, 0)))
       exit(2);
   crypto_classify(x,l);
 }
 
+#elif (defined(GETRANDOM) && defined(__Darwin__))
+#include <sys/random.h>
+// This could be CCRandomGenerateBytes
+void randombytes(void *x, size_t l)
+{
+  ssize_t n;
+  for (size_t i = 0; i < l; i += n)
+    if (0 >= (n = getentropy((char *) x + i, l - i)))
+      exit(2);
+  crypto_classify(x,l);
+}
+
 #elif (defined(__Windows__) || defined(__WIN64) || defined(__WIN32))
 /*
  *
  * XXX This is not secure or audited or even worth considering for anything
  * beyond proof of concept that the software can be built on Windows.
  *
  * DO NOT USE THIS FOR ANYTHING SERIOUS AT ALL - THIS IS NOT REASONABLE OR SAFE
  * AND HAS NOT BEEN AUDITED BY ANYONE. THIS IS A "IT COMPILES" LEVEL OF
  * COMPLETENESS.
  *
  * YOU HAVE BEEN WARNED. THIS, LIKE THE REST OF THE LIBRARY, IS NOT ELIGIBLE
  * FOR A CVE!
  */
 
+ssize_t getrandom(char *buf, size_t buflen);
+#include <windows.h>
+#include <ntsecapi.h>
+#define getrandom(x, y) RtlGenRandom(x, y)
+
 void randombytes(void *x, size_t l)
 {
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i)))
       exit(2);
   crypto_classify(x,l);
```

### Comparing `highctidh-1.0.2024050100/ctidh2048/skgen.c` & `highctidh-1.0.2024050500/ctidh2048/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/steps.c` & `highctidh-1.0.2024050500/ctidh2048/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/steps.h` & `highctidh-1.0.2024050500/ctidh2048/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/uintbig.h` & `highctidh-1.0.2024050500/ctidh2048/uintbig.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/uintbig2048.S` & `highctidh-1.0.2024050500/ctidh2048/uintbig2048.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/uintbig_namespace.h` & `highctidh-1.0.2024050500/ctidh2048/uintbig_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/validate.c` & `highctidh-1.0.2024050500/ctidh2048/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh2048/vectors2048_test.go` & `highctidh-1.0.2024050500/ctidh2048/vectors2048_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/common.go` & `highctidh-1.0.2024050500/ctidh512/common.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-package ctidh511
+package ctidh512
 
 /*
- #cgo CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -O2
+ #cgo CFLAGS: -DBITS=512 -DCGONUTS -O2
  #cgo LDFLAGS:
- #cgo linux CFLAGS: -DBITS=511 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
  #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
  #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
  #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
- #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -D__ARM64__ -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
  #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
- #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -march=native -mtune=native -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // Generic flags for amd64
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
  #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
- #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -DCGONUTS -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
  #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
  #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
@@ -73,15 +73,15 @@
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
  #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
  #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
- #include "binding511.h"
+ #include "binding512.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
 	"unsafe"
 
@@ -89,20 +89,20 @@
 )
 
 //
 // This function wraps go_fillrandom, so we can emulate the calls from the
 // C library and test the results
 //
 func test_go_fillrandom(context unsafe.Pointer, outptr []byte) {
-	highctidh_511_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
+	highctidh_512_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
 }
 
 // This is called from the C library, DO NOT CHANGE THE FUNCTION INTERFACE
-//export highctidh_511_go_fillrandom
-func highctidh_511_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
+//export highctidh_512_go_fillrandom
+func highctidh_512_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
 	rng := gopointer.Restore(context).(io.Reader)
 	buf := make([]byte, outsz)
 	count, err := rng.Read(buf)
 	if err != nil {
 		panic(err)
 	}
 	if count != int(outsz) {
```

### Comparing `highctidh-1.0.2024050100/ctidh511/common_test.go` & `highctidh-1.0.2024050500/ctidh511/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/csidh.c` & `highctidh-1.0.2024050500/ctidh511/csidh.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/csidh.h` & `highctidh-1.0.2024050500/ctidh511/csidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/csidh_namespace.h` & `highctidh-1.0.2024050500/ctidh511/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/ctidh511.go` & `highctidh-1.0.2024050500/ctidh511/ctidh511.go`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 package ctidh511
 
 /*
 #include "binding511.h"
 #include <csidh.h>
 
-extern ctidh_fillrandom fillrandom_custom;
+extern ctidh_fillrandom fillrandom_511_custom;
 
 __attribute__((weak))
 void custom_gen_private(void *const context, private_key *priv) {
-  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_custom);
+  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_511_custom);
 }
 */
 import "C"
 import (
 	"crypto/hmac"
 	"encoding/base64"
 	"io"
```

### Comparing `highctidh-1.0.2024050100/ctidh511/ctidh511_bench_test.go` & `highctidh-1.0.2024050500/ctidh511/ctidh511_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/ctidh511_test.go` & `highctidh-1.0.2024050500/ctidh511/ctidh511_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/elligator.c` & `highctidh-1.0.2024050500/ctidh511/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/error.go` & `highctidh-1.0.2024050500/ctidh511/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fiat_p511.c` & `highctidh-1.0.2024050500/ctidh511/fiat_p511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fiat_p511.h` & `highctidh-1.0.2024050500/ctidh511/fiat_p511.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fp.h` & `highctidh-1.0.2024050500/ctidh511/fp.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fp2fiat.c` & `highctidh-1.0.2024050500/ctidh511/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
+#if HIGHCTIDH_PORTABLE == 0 && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
-#elif defined(CGONUTS)
-#define DONTMINDIFIDO
-
 #else
+#if defined(CGONUTS)
+#define DONTMINDIFIDO
+#endif
 /*
  * The definitions in this unit are only needed when they are not provided
  * by the optimizied assembly units.
  */
 
 /*
  * These are replacements for uintbig512.S:
```

### Comparing `highctidh-1.0.2024050100/ctidh511/fp511.S` & `highctidh-1.0.2024050500/ctidh511/fp511.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fp_inv511.c` & `highctidh-1.0.2024050500/ctidh511/fp_inv511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fp_namespace.h` & `highctidh-1.0.2024050500/ctidh511/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/fp_sqrt511.c` & `highctidh-1.0.2024050500/ctidh511/fp_sqrt511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/int32_minmax.h` & `highctidh-1.0.2024050500/ctidh511/int32_minmax.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/int32_sort.c` & `highctidh-1.0.2024050500/ctidh511/int32_sort.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/int32_sort.h` & `highctidh-1.0.2024050500/ctidh511/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/int32_sort_x86.c` & `highctidh-1.0.2024050500/ctidh511/int32_sort_x86.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/mont.c` & `highctidh-1.0.2024050500/ctidh511/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/mont.h` & `highctidh-1.0.2024050500/ctidh511/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/mont_namespace.h` & `highctidh-1.0.2024050500/ctidh511/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/naidne.h` & `highctidh-1.0.2024050500/ctidh511/naidne.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/poly.c` & `highctidh-1.0.2024050500/ctidh511/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/poly.h` & `highctidh-1.0.2024050500/ctidh511/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/poly_namespace.h` & `highctidh-1.0.2024050500/ctidh511/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/primes.h` & `highctidh-1.0.2024050500/ctidh511/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/primes511.c` & `highctidh-1.0.2024050500/ctidh511/primes511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/proj.h` & `highctidh-1.0.2024050500/ctidh511/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/random.c` & `highctidh-1.0.2024050500/ctidh511/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/random.h` & `highctidh-1.0.2024050500/ctidh511/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/randombytes.c` & `highctidh-1.0.2024050500/ctidh511/randombytes.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 #include "randombytes.h"
 
 #include <stdlib.h>
-#ifndef _MSC_VER
-#include <unistd.h>
-#include <fcntl.h>
-#else // e.g. (defined(__Windows__) || defined (__WIN64))
-#include <basetsd.h>
-#define ssize_t SSIZE_T
-#include <windows.h>
-#define SystemFunction036 NTAPI SystemFunction036
-#include <ntsecapi.h>
-#undef SystemFunction036
-#pragma comment(lib, "advapi32.lib")
-#define getrandom(x, y) RtlGenRandom(x, y)
-#endif
 
 #include "crypto_classify.h"
 #include "random_namespace.h"
 
 #if defined(GETRANDOM) && (defined(__linux__) || defined(__sun))
 #include <sys/random.h>
 
@@ -26,28 +13,45 @@
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i, 0)))
       exit(2);
   crypto_classify(x,l);
 }
 
+#elif (defined(GETRANDOM) && defined(__Darwin__))
+#include <sys/random.h>
+// This could be CCRandomGenerateBytes
+void randombytes(void *x, size_t l)
+{
+  ssize_t n;
+  for (size_t i = 0; i < l; i += n)
+    if (0 >= (n = getentropy((char *) x + i, l - i)))
+      exit(2);
+  crypto_classify(x,l);
+}
+
 #elif (defined(__Windows__) || defined(__WIN64) || defined(__WIN32))
 /*
  *
  * XXX This is not secure or audited or even worth considering for anything
  * beyond proof of concept that the software can be built on Windows.
  *
  * DO NOT USE THIS FOR ANYTHING SERIOUS AT ALL - THIS IS NOT REASONABLE OR SAFE
  * AND HAS NOT BEEN AUDITED BY ANYONE. THIS IS A "IT COMPILES" LEVEL OF
  * COMPLETENESS.
  *
  * YOU HAVE BEEN WARNED. THIS, LIKE THE REST OF THE LIBRARY, IS NOT ELIGIBLE
  * FOR A CVE!
  */
 
+ssize_t getrandom(char *buf, size_t buflen);
+#include <windows.h>
+#include <ntsecapi.h>
+#define getrandom(x, y) RtlGenRandom(x, y)
+
 void randombytes(void *x, size_t l)
 {
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i)))
       exit(2);
   crypto_classify(x,l);
```

### Comparing `highctidh-1.0.2024050100/ctidh511/skgen.c` & `highctidh-1.0.2024050500/ctidh511/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/steps.c` & `highctidh-1.0.2024050500/ctidh511/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/steps.h` & `highctidh-1.0.2024050500/ctidh511/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/uintbig.h` & `highctidh-1.0.2024050500/ctidh511/uintbig.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/uintbig511.S` & `highctidh-1.0.2024050500/ctidh511/uintbig511.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/uintbig_namespace.h` & `highctidh-1.0.2024050500/ctidh511/uintbig_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/validate.c` & `highctidh-1.0.2024050500/ctidh511/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh511/vectors511_test.go` & `highctidh-1.0.2024050500/ctidh511/vectors511_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/common.go` & `highctidh-1.0.2024050500/ctidh1024/common.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-package ctidh512
+package ctidh1024
 
 /*
- #cgo CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -O2
+ #cgo CFLAGS: -DBITS=1024 -DCGONUTS -O2
  #cgo LDFLAGS:
- #cgo linux CFLAGS: -DBITS=512 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
+ #cgo linux CFLAGS: -DBITS=1024 -DGETRANDOM -DCGONUTS -Wformat -Werror=format-security -D_FORTIFY_SOURCE=2 -fstack-protector-all -fpie -fPIC -O2
  #cgo linux LDFLAGS: -Wl,-z,noexecstack -Wl,-z,relro
  #cgo windows CFLAGS: -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds and as cross compiled builds.
  // Example cross compile build lines are provided as examples.
 
  // CC=aarch64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=arm64 go build -v
  #cgo arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=arm64 go build -v
- #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/arm64 CFLAGS: -DPLATFORM=aarch64 -DPLATFORM_SIZE=64 -D__ARM64__ -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // export CGO_CFLAGS_ALLOW="-fforce-enable-int128";
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=arm ARMVER=7  go build
  #cgo arm CFLAGS: -DPLATFORM=arm -DPLATFORM_SIZE=32 -D__ARM32__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=clang CGO_ENABLED=1 GOOS=darwin GOARCH=amd64 go build -v
- #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
+ #cgo darwin/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -march=native -mtune=native -D__Darwin__ -DGETRANDOM -DHIGHCTIDH_PORTABLE=1
 
  // Generic flags for amd64
- #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64
+ #cgo amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=gcc CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -v
- #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native
+ #cgo linux/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -march=native -mtune=native -D__x86_64__ -fpie -fPIC -DHIGHCTIDH_PORTABLE=1
 
  // CC=??? CGO_ENABLED=1 GOOS=windows GOARCH=arm64 go build
  #cgo windows/arm64 CFLAGS: -DPLATFORM=arm64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=/usr/bin/x86_64-w64-mingw32-gcc CGO_ENABLED=1 GOOS=windows GOARCH=amd64 go build
- #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -D__Windows__ -DHIGHCTIDH_PORTABLE=1
+ #cgo windows/amd64 CFLAGS: -DPLATFORM=x86_64 -DPLATFORM_SIZE=64 -DCGONUTS -D__Windows__ -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64le-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64le go build -v
  #cgo ppc64le CFLAGS: -DPLATFORM=ppc64le -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
  // CC=powerpc64-linux-gnu-gcc CGO_ENABLED=1 GOOS=linux GOARCH=ppc64 go build -v
  #cgo ppc64 CFLAGS: -DPLATFORM=ppc64 -DPLATFORM_SIZE=64 -DHIGHCTIDH_PORTABLE=1
 
@@ -73,15 +73,15 @@
  // CC=clang CGO_ENABLED=1 GOOS=linux GOARCH=386  go build
  #cgo 386 CFLAGS: -DPLATFORM=i386 -DPLATFORM_SIZE=32 -fforce-enable-int128 -D__i386__ -DHIGHCTIDH_PORTABLE=1
 
  // The following should work as native builds with clang:
 
  #cgo loong64 CFLAGS: -DPLATFORM=loongarch64 -DPLATFORM_SIZE=64 -march=native -mtune=native -DHIGHCTIDH_PORTABLE=1
 
- #include "binding512.h"
+ #include "binding1024.h"
 */
 import "C"
 import (
 	"fmt"
 	"io"
 	"unsafe"
 
@@ -89,20 +89,20 @@
 )
 
 //
 // This function wraps go_fillrandom, so we can emulate the calls from the
 // C library and test the results
 //
 func test_go_fillrandom(context unsafe.Pointer, outptr []byte) {
-	highctidh_512_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
+	highctidh_1024_go_fillrandom(context, unsafe.Pointer(&outptr[0]), C.size_t(len(outptr)))
 }
 
 // This is called from the C library, DO NOT CHANGE THE FUNCTION INTERFACE
-//export highctidh_512_go_fillrandom
-func highctidh_512_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
+//export highctidh_1024_go_fillrandom
+func highctidh_1024_go_fillrandom(context unsafe.Pointer, outptr unsafe.Pointer, outsz C.size_t) {
 	rng := gopointer.Restore(context).(io.Reader)
 	buf := make([]byte, outsz)
 	count, err := rng.Read(buf)
 	if err != nil {
 		panic(err)
 	}
 	if count != int(outsz) {
```

### Comparing `highctidh-1.0.2024050100/ctidh512/common_test.go` & `highctidh-1.0.2024050500/ctidh512/common_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/csidh.c` & `highctidh-1.0.2024050500/ctidh512/csidh.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/csidh.h` & `highctidh-1.0.2024050500/ctidh512/csidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/csidh_namespace.h` & `highctidh-1.0.2024050500/ctidh512/csidh_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/ctidh512.go` & `highctidh-1.0.2024050500/ctidh512/ctidh512.go`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 package ctidh512
 
 /*
 #include "binding512.h"
 #include <csidh.h>
 
-extern ctidh_fillrandom fillrandom_custom;
+extern ctidh_fillrandom fillrandom_512_custom;
 
 __attribute__((weak))
 void custom_gen_private(void *const context, private_key *priv) {
-  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_custom);
+  csidh_private_withrng(priv, (uintptr_t)context, fillrandom_512_custom);
 }
 */
 import "C"
 import (
 	"crypto/hmac"
 	"encoding/base64"
 	"io"
```

### Comparing `highctidh-1.0.2024050100/ctidh512/ctidh512_bench_test.go` & `highctidh-1.0.2024050500/ctidh512/ctidh512_bench_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/ctidh512_test.go` & `highctidh-1.0.2024050500/ctidh512/ctidh512_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/elligator.c` & `highctidh-1.0.2024050500/ctidh512/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/error.go` & `highctidh-1.0.2024050500/ctidh512/error.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fiat_p512.c` & `highctidh-1.0.2024050500/ctidh512/fiat_p512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fiat_p512.h` & `highctidh-1.0.2024050500/ctidh512/fiat_p512.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fp.h` & `highctidh-1.0.2024050500/ctidh512/fp.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fp2fiat.c` & `highctidh-1.0.2024050500/ctidh512/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
+#if HIGHCTIDH_PORTABLE == 0 && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
-#elif defined(CGONUTS)
-#define DONTMINDIFIDO
-
 #else
+#if defined(CGONUTS)
+#define DONTMINDIFIDO
+#endif
 /*
  * The definitions in this unit are only needed when they are not provided
  * by the optimizied assembly units.
  */
 
 /*
  * These are replacements for uintbig512.S:
```

### Comparing `highctidh-1.0.2024050100/ctidh512/fp512.S` & `highctidh-1.0.2024050500/ctidh512/fp512.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fp_inv512.c` & `highctidh-1.0.2024050500/ctidh512/fp_inv512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fp_namespace.h` & `highctidh-1.0.2024050500/ctidh512/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/fp_sqrt512.c` & `highctidh-1.0.2024050500/ctidh512/fp_sqrt512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/int32_minmax.h` & `highctidh-1.0.2024050500/ctidh512/int32_minmax.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/int32_sort.c` & `highctidh-1.0.2024050500/ctidh512/int32_sort.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/int32_sort.h` & `highctidh-1.0.2024050500/ctidh512/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/int32_sort_x86.c` & `highctidh-1.0.2024050500/ctidh512/int32_sort_x86.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/mont.c` & `highctidh-1.0.2024050500/ctidh512/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/mont.h` & `highctidh-1.0.2024050500/ctidh512/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/mont_namespace.h` & `highctidh-1.0.2024050500/ctidh512/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/naidne.h` & `highctidh-1.0.2024050500/ctidh512/naidne.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/poly.c` & `highctidh-1.0.2024050500/ctidh512/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/poly.h` & `highctidh-1.0.2024050500/ctidh512/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/poly_namespace.h` & `highctidh-1.0.2024050500/ctidh512/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/primes.h` & `highctidh-1.0.2024050500/ctidh512/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/primes512.c` & `highctidh-1.0.2024050500/ctidh512/primes512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/proj.h` & `highctidh-1.0.2024050500/ctidh512/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/random.c` & `highctidh-1.0.2024050500/ctidh512/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/random.h` & `highctidh-1.0.2024050500/ctidh512/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/randombytes.c` & `highctidh-1.0.2024050500/ctidh512/randombytes.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 #include "randombytes.h"
 
 #include <stdlib.h>
-#ifndef _MSC_VER
-#include <unistd.h>
-#include <fcntl.h>
-#else // e.g. (defined(__Windows__) || defined (__WIN64))
-#include <basetsd.h>
-#define ssize_t SSIZE_T
-#include <windows.h>
-#define SystemFunction036 NTAPI SystemFunction036
-#include <ntsecapi.h>
-#undef SystemFunction036
-#pragma comment(lib, "advapi32.lib")
-#define getrandom(x, y) RtlGenRandom(x, y)
-#endif
 
 #include "crypto_classify.h"
 #include "random_namespace.h"
 
 #if defined(GETRANDOM) && (defined(__linux__) || defined(__sun))
 #include <sys/random.h>
 
@@ -26,28 +13,45 @@
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i, 0)))
       exit(2);
   crypto_classify(x,l);
 }
 
+#elif (defined(GETRANDOM) && defined(__Darwin__))
+#include <sys/random.h>
+// This could be CCRandomGenerateBytes
+void randombytes(void *x, size_t l)
+{
+  ssize_t n;
+  for (size_t i = 0; i < l; i += n)
+    if (0 >= (n = getentropy((char *) x + i, l - i)))
+      exit(2);
+  crypto_classify(x,l);
+}
+
 #elif (defined(__Windows__) || defined(__WIN64) || defined(__WIN32))
 /*
  *
  * XXX This is not secure or audited or even worth considering for anything
  * beyond proof of concept that the software can be built on Windows.
  *
  * DO NOT USE THIS FOR ANYTHING SERIOUS AT ALL - THIS IS NOT REASONABLE OR SAFE
  * AND HAS NOT BEEN AUDITED BY ANYONE. THIS IS A "IT COMPILES" LEVEL OF
  * COMPLETENESS.
  *
  * YOU HAVE BEEN WARNED. THIS, LIKE THE REST OF THE LIBRARY, IS NOT ELIGIBLE
  * FOR A CVE!
  */
 
+ssize_t getrandom(char *buf, size_t buflen);
+#include <windows.h>
+#include <ntsecapi.h>
+#define getrandom(x, y) RtlGenRandom(x, y)
+
 void randombytes(void *x, size_t l)
 {
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i)))
       exit(2);
   crypto_classify(x,l);
```

### Comparing `highctidh-1.0.2024050100/ctidh512/skgen.c` & `highctidh-1.0.2024050500/ctidh512/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/steps.c` & `highctidh-1.0.2024050500/ctidh512/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/steps.h` & `highctidh-1.0.2024050500/ctidh512/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/uintbig.h` & `highctidh-1.0.2024050500/ctidh512/uintbig.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/uintbig512.S` & `highctidh-1.0.2024050500/ctidh512/uintbig512.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/uintbig_namespace.h` & `highctidh-1.0.2024050500/ctidh512/uintbig_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/validate.c` & `highctidh-1.0.2024050500/ctidh512/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ctidh512/vectors512_test.go` & `highctidh-1.0.2024050500/ctidh512/vectors512_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/distmults.py` & `highctidh-1.0.2024050500/distmults.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/elligator.c` & `highctidh-1.0.2024050500/elligator.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/example-ctidh.c` & `highctidh-1.0.2024050500/example-ctidh.c`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,20 @@
  *  -l highctidh_2048
  *
  * */
 
 #include <stdio.h>
 #include <libhighctidh/csidh.h>
 
+#if (defined(__ARM32__) || defined(__i386__))
+#define STR_FMT "%u"
+#else
+#define STR_FMT "%lu"
+#endif
+
 void print_hex_key(void *k, unsigned int l)
 { 
   printf("0x");
   for (unsigned int i = 0; i < l; i++)
   {
     printf("%02x", i[(unsigned char *) k]);
   }
@@ -43,55 +49,55 @@
   public_key pk_a, pk_b;
   public_key s_a, s_b;
   bool ok = 0;
 
   printf("CTIDH %i vector example\n\n", BITS);
   fflush(stdout);
 
-  printf("Generating Alice's private_key (%li bytes):\n", sizeof(private_key));
+  printf("Generating Alice's private_key (" STR_FMT " bytes):\n", sizeof(private_key));
   fflush(stdout);
   csidh_private(&sk_a);
   print_hex_key(&sk_a, sizeof(private_key));
-  printf("Generating Alice's public_key (%li bytes):\n", sizeof(public_key));
+  printf("Generating Alice's public_key (" STR_FMT " bytes):\n", sizeof(public_key));
   fflush(stdout);
   ok = csidh(&pk_a, &base, &sk_a);
   if (!validate(&pk_a))
   {
     printf("Invalid public key:\n");
   }
   print_hex_key(&pk_a, sizeof(public_key));
   printf("Result: %i\n", ok);
   printf("\n");
   fflush(stdout);
 
-  printf("Generating Bob's private_key (%li bytes):\n", sizeof(private_key));
+  printf("Generating Bob's private_key (" STR_FMT " bytes):\n", sizeof(private_key));
   fflush(stdout);
   csidh_private(&sk_b);
   print_hex_key(&sk_b, sizeof(private_key));
-  printf("Generating Bob's public_key (%li bytes):\n", sizeof(public_key));
+  printf("Generating Bob's public_key (" STR_FMT " bytes):\n", sizeof(public_key));
   fflush(stdout);
   ok = csidh(&pk_b, &base, &sk_b);
   if (!validate(&pk_a))
   {
     printf("Invalid public key:\n");
   }
   print_hex_key(&pk_b, sizeof(public_key));
   printf("Result: %i\n", ok);
   printf("\n");
   fflush(stdout);
 
-  printf("Computing DH for Alice (%li bytes):\n", sizeof(public_key));
+  printf("Computing DH for Alice (" STR_FMT " bytes):\n", sizeof(public_key));
   fflush(stdout);
   ok = csidh(&s_a, &pk_b, &sk_a);
   print_hex_key(&s_a, sizeof(public_key));
   printf("Result: %i\n", ok);
   printf("\n");
   fflush(stdout);
 
-  printf("Computing DH for Bob (%li bytes):\n", sizeof(public_key));
+  printf("Computing DH for Bob (" STR_FMT " bytes):\n", sizeof(public_key));
   fflush(stdout);
   ok = csidh(&s_b, &pk_a, &sk_b);
   print_hex_key(&s_b, sizeof(public_key));
   printf("Result: %i\n", ok);
   printf("\n");
   fflush(stdout);
```

### Comparing `highctidh-1.0.2024050100/examples_static.c` & `highctidh-1.0.2024050500/examples_static.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p1024.c` & `highctidh-1.0.2024050500/fiat_p1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p1024.h` & `highctidh-1.0.2024050500/fiat_p1024.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p2048.c` & `highctidh-1.0.2024050500/fiat_p2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p2048.h` & `highctidh-1.0.2024050500/fiat_p2048.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p511.c` & `highctidh-1.0.2024050500/fiat_p511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p511.h` & `highctidh-1.0.2024050500/fiat_p511.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p512.c` & `highctidh-1.0.2024050500/fiat_p512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fiat_p512.h` & `highctidh-1.0.2024050500/fiat_p512.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp.h` & `highctidh-1.0.2024050500/fp.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp1024.S` & `highctidh-1.0.2024050500/fp1024.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp2048.S` & `highctidh-1.0.2024050500/fp2048.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp2fiat.c` & `highctidh-1.0.2024050500/fp2fiat.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #include <string.h>
 
 
 #include "uintbig_namespace.h"
 #include "fp.h"
 #include "annotations.h"
 
-#if HIGHCTIDH_PORTABLE == 0 && !defined(CGONUTS) && (defined(__x86_64__) || defined(__i86pc__))
+#if HIGHCTIDH_PORTABLE == 0 && (defined(__x86_64__) || defined(__i86pc__))
 #define highctidh_macro_stringize(x) #x
 #define highctidh_macro_str(y) highctidh_macro_stringize(y)
 __asm__ (".include \"uintbig" highctidh_macro_str(BITS)  ".S\"");
 __asm__ (".include \"fp" highctidh_macro_str(BITS) ".S\"");
 
-#elif defined(CGONUTS)
-#define DONTMINDIFIDO
-
 #else
+#if defined(CGONUTS)
+#define DONTMINDIFIDO
+#endif
 /*
  * The definitions in this unit are only needed when they are not provided
  * by the optimizied assembly units.
  */
 
 /*
  * These are replacements for uintbig512.S:
```

### Comparing `highctidh-1.0.2024050100/fp511.S` & `highctidh-1.0.2024050500/fp511.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp512.S` & `highctidh-1.0.2024050500/fp512.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_inv1024.c` & `highctidh-1.0.2024050500/fp_inv1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_inv2048.c` & `highctidh-1.0.2024050500/fp_inv2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_inv511.c` & `highctidh-1.0.2024050500/fp_inv511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_inv512.c` & `highctidh-1.0.2024050500/fp_inv512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_namespace.h` & `highctidh-1.0.2024050500/fp_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_sqrt1024.c` & `highctidh-1.0.2024050500/fp_sqrt1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_sqrt2048.c` & `highctidh-1.0.2024050500/fp_sqrt2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_sqrt511.c` & `highctidh-1.0.2024050500/fp_sqrt511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/fp_sqrt512.c` & `highctidh-1.0.2024050500/fp_sqrt512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/go-tests/ctidh_test.go` & `highctidh-1.0.2024050500/go-tests/ctidh_test.go`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/greedy` & `highctidh-1.0.2024050500/greedy`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/highctidh.h` & `highctidh-1.0.2024050500/highctidh.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/highctidh/__init__.py` & `highctidh-1.0.2024050500/highctidh/__init__.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/highctidh/bench.py` & `highctidh-1.0.2024050500/highctidh/bench.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/highctidh_macros.h` & `highctidh-1.0.2024050500/highctidh_macros.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/int32_minmax.h` & `highctidh-1.0.2024050500/int32_minmax.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/int32_sort.c` & `highctidh-1.0.2024050500/int32_sort.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/int32_sort.h` & `highctidh-1.0.2024050500/int32_sort.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/int32_sort_x86.c` & `highctidh-1.0.2024050500/int32_sort_x86.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/mont.c` & `highctidh-1.0.2024050500/mont.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/mont.h` & `highctidh-1.0.2024050500/mont.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/mont_namespace.h` & `highctidh-1.0.2024050500/mont_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/naidne.h` & `highctidh-1.0.2024050500/naidne.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/poly.c` & `highctidh-1.0.2024050500/poly.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/poly.h` & `highctidh-1.0.2024050500/poly.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/poly_namespace.h` & `highctidh-1.0.2024050500/poly_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/primes.h` & `highctidh-1.0.2024050500/primes.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/primes1024.c` & `highctidh-1.0.2024050500/primes1024.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/primes2048.c` & `highctidh-1.0.2024050500/primes2048.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/primes511.c` & `highctidh-1.0.2024050500/primes511.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/primes512.c` & `highctidh-1.0.2024050500/primes512.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/proj.h` & `highctidh-1.0.2024050500/proj.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/pyproject.toml` & `highctidh-1.0.2024050500/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "highctidh"
-version = "1.0.2024050100"
+version = "1.0.2024050500"
 description = "highctidh bindings with included C library"
 readme = "README.md"
 requires-python = ">=3.9.6"
 keywords = ["post-quantum cryptography", "cryptography", "csidh", "ctidh", "C", "highctidh"]
 authors = [ {email = "jacob@appelbaum.net"}, {name = "Jacob Appelbaum"} ]
 maintainers = [ {email = "jacob@appelbaum.net"}, {name = "Jacob Appelbaum"} ]
 dependencies = [ ]
```

### Comparing `highctidh-1.0.2024050100/random.c` & `highctidh-1.0.2024050500/random.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/random.h` & `highctidh-1.0.2024050500/random.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/randombytes.c` & `highctidh-1.0.2024050500/randombytes.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 #include "randombytes.h"
 
 #include <stdlib.h>
-#ifndef _MSC_VER
-#include <unistd.h>
-#include <fcntl.h>
-#else // e.g. (defined(__Windows__) || defined (__WIN64))
-#include <basetsd.h>
-#define ssize_t SSIZE_T
-#include <windows.h>
-#define SystemFunction036 NTAPI SystemFunction036
-#include <ntsecapi.h>
-#undef SystemFunction036
-#pragma comment(lib, "advapi32.lib")
-#define getrandom(x, y) RtlGenRandom(x, y)
-#endif
 
 #include "crypto_classify.h"
 #include "random_namespace.h"
 
 #if defined(GETRANDOM) && (defined(__linux__) || defined(__sun))
 #include <sys/random.h>
 
@@ -26,28 +13,45 @@
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i, 0)))
       exit(2);
   crypto_classify(x,l);
 }
 
+#elif (defined(GETRANDOM) && defined(__Darwin__))
+#include <CommonCrypto/CommonRandom.h>
+void randombytes(void *x, size_t l)
+{
+  ssize_t n;
+  n = CCRandomGenerateBytes((char *) x, l);
+  if (n != kCCSuccess) {
+    exit(2);
+  }
+  crypto_classify(x,l);
+}
+
 #elif (defined(__Windows__) || defined(__WIN64) || defined(__WIN32))
 /*
  *
  * XXX This is not secure or audited or even worth considering for anything
  * beyond proof of concept that the software can be built on Windows.
  *
  * DO NOT USE THIS FOR ANYTHING SERIOUS AT ALL - THIS IS NOT REASONABLE OR SAFE
  * AND HAS NOT BEEN AUDITED BY ANYONE. THIS IS A "IT COMPILES" LEVEL OF
  * COMPLETENESS.
  *
  * YOU HAVE BEEN WARNED. THIS, LIKE THE REST OF THE LIBRARY, IS NOT ELIGIBLE
  * FOR A CVE!
  */
 
+ssize_t getrandom(char *buf, size_t buflen);
+#include <windows.h>
+#include <ntsecapi.h>
+#define getrandom(x, y) RtlGenRandom(x, y)
+
 void randombytes(void *x, size_t l)
 {
   ssize_t n;
   for (size_t i = 0; i < l; i += n)
     if (0 >= (n = getrandom((char *) x + i, l - i)))
       exit(2);
   crypto_classify(x,l);
```

### Comparing `highctidh-1.0.2024050100/setup.cfg` & `highctidh-1.0.2024050500/setup.cfg`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/setup.py` & `highctidh-1.0.2024050500/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,28 +54,30 @@
     # files for the extensions but then it fails to link as it attempts to use
     # gcc for that task. See pypi/setuptools #1442 for more information.  When
     # used with debian/rules for building, corresponding PYBUILD_* options must
     # be set to ensure everything works as intended.  Please consult
     # misc/debian-rules for an example.
     #
     def build_extensions(self):
-        print(f"Compiler was: {self.compiler.linker_exe}")
-        print(f"Linker was: {self.compiler.linker_so}")
-        # NOTE:
-        # This entire class is to work around a pernicous and annoying bug that
-        # previously prevented using any compiler other than gcc on GNU/Linux
-        # platforms for certain kinds of builds.  By setting CC=clang or
-        # CC=gcc, builds will be compiled by the selected compiler as expected.
-        # However, self.compiler.linker_exe is mistakenly not updated by
-        # setting the CC environment variable.  To work around this bug which
-        # only impacts users of an alternative compiler, we hot patch only the
-        # linker executable name:
-        self.compiler.linker_so[0] = self.compiler.linker_exe[0]
-        print(f"Compiler is now: {self.compiler.linker_exe}")
-        print(f"Linker is now: {self.compiler.linker_so}")
+        print(self.compiler)
+        if OS != 'Windows':
+            print(f"Compiler was: {self.compiler.linker_exe}")
+            print(f"Linker was: {self.compiler.linker_so}")
+            # NOTE:
+            # This entire class is to work around a pernicous and annoying bug that
+            # previously prevented using any compiler other than gcc on GNU/Linux
+            # platforms for certain kinds of builds.  By setting CC=clang or
+            # CC=gcc, builds will be compiled by the selected compiler as expected.
+            # However, self.compiler.linker_exe is mistakenly not updated by
+            # setting the CC environment variable.  To work around this bug which
+            # only impacts users of an alternative compiler, we hot patch only the
+            # linker executable name:
+            self.compiler.linker_so[0] = self.compiler.linker_exe[0]
+            print(f"Compiler is now: {self.compiler.linker_exe}")
+            print(f"Linker is now: {self.compiler.linker_so}")
         build_ext.build_extensions(self)
 
     def run(self):
         build_ext.run(self)
 
 
 requirements = []
@@ -125,15 +127,20 @@
         pass
 
 CC = None
 if "CC" in environ:
     CC = str(environ["CC"])
     print(f"CC={CC}")
 
-VERSION = open("VERSION", "r").read().strip()
+try:
+    VERSION = open("src/VERSION", "r").read().strip()
+except FileNotFoundError:
+    VERSION = open("VERSION", "r").read().strip()
+except AttributeError:
+    VERSION = "3.141592653"
 
 base_src = [
     "crypto_classify.c",
     "crypto_declassify.c",
     "csidh.c",
     "elligator.c",
     "fp2fiat.c",
@@ -145,16 +152,19 @@
     "steps.c",
     "steps_untuned.c",
     "umults.c",
     "validate.c",
     "int32_sort.c",
 ]
 
-cflags = get_config_var("CFLAGS").split()
-cflags = ["-Wextra"]
+cflags = get_config_var("CFLAGS")
+if cflags is not None and cflags is str:
+  cflags = cflags.split()
+else:
+  cflags = ["-Wextra"]
 cflags += ["-Wall", "-fpie", "-fPIC", "-fwrapv", "-pedantic", "-O2", "-g0", "-fno-lto"]
 cflags += ["-DGETRANDOM", f"-DPLATFORM={PLATFORM}", f"-DPLATFORM_SIZE={PLATFORM_SIZE}"]
 cflags += [
     "-Wformat",
     "-Werror=format-security",
     "-D_FORTIFY_SOURCE=2",
     "-fstack-protector-strong",
@@ -172,21 +182,19 @@
             "-Wl,-z,relro",
             "-Wl,-z,now",
             "-Wl,--reduce-memory-overheads",
             "-Wl,--no-keep-memory",
         ]
 
 print(f"Building for platform: {PLATFORM} on {OS}")
-if PLATFORM == "aarch64":
+if PLATFORM == "aarch64" or PLATFORM == "arm64":
+    cflags += ["-D__ARM64__"]
     if OS == "Darwin":
       cflags += ["-D__Darwin__"]
-      if CC == "clang":
-          cflags += ["-DHIGHCTIDH_PORTABLE=1"]
-      if CC == "gcc":
-          cflags += ["-DHIGHCTIDH_PORTABLE=1"]
+      cflags += ["-DHIGHCTIDH_PORTABLE=1"]
     else:
       if CC == "clang":
           cflags += ["-DHIGHCTIDH_PORTABLE=1"]
       if CC == "gcc":
           cflags += ["-march=native", "-mtune=native", "-DHIGHCTIDH_PORTABLE=1"]
 elif PLATFORM == "armv7l":
     # clang required
@@ -225,15 +233,15 @@
     # Solaris 11, SunOS has default flags that do not work for both gcc and clang
     # compilers. We wrap the function that returns these flags internally during
     # the build process to override them for a value that works for both.
     import distutils.sysconfig as _wrapped_distutils
     from distutils.sysconfig import get_config_vars as _get_config_vars
 
     _config_vars = _get_config_vars().copy()
-    default_cflags += [
+    default_cflags = [
         " -O2 -DNDEBUG -Wall -m64 -fPIC -fpie -DPIC -ffile-prefix-map=..=. "
     ]
     _config_vars["CFLAGS"] = default_cflags
 
     def get_config_vars_wrapper(*a):
         return [_config_vars.get(n) for n in a] if a else _config_vars
 
@@ -250,50 +258,50 @@
     if PLATFORM == "sun4v":
         cflags += ["-D__sun4v__"]
         cflags += ["-DHIGHCTIDH_PORTABLE=1"]
         if CC == "clang":
             cflags += ["-fforce-enable-int128"]
     cflags += ["-Wextra", "-fwrapv", "-pedantic", "-Werror", "-DGETRANDOM"]
     cflags += [f"-DPLATFORM={PLATFORM}", f"-DPLATFORM_SIZE={PLATFORM_SIZE}"]
-elif PLATFORM == "x86_64" and OS == 'Windows':
+elif PLATFORM == "x86_64" and OS == 'Windows' or PLATFORM == "AMD64" and OS == 'Windows':
     # Windows only builds with clang on Windows under the CI
     # It should also build with other compilers.
     # As with Solaris we wrap the function that returns these flags internally
     # during the build process to override them for a value that works for
     # both.
     import distutils.sysconfig as _wrapped_distutils
     from distutils.sysconfig import get_config_vars as _get_config_vars
 
     _config_vars = _get_config_vars().copy()
-    default_cflags += [
-        " -Wall -Wextra -pedantic -O2 -fwrapv -ffile-prefix-map=..=."
+    default_cflags = [
+        " -Wall -pedantic -O2 -fwrapv -ffile-prefix-map=..=."
     ]
     _config_vars["CFLAGS"] = default_cflags
 
     def get_config_vars_wrapper(*a):
         return [_config_vars.get(n) for n in a] if a else _config_vars
 
     _wrapped_distutils.get_config_vars = get_config_vars_wrapper
     # Set Windows specific build options
     cflags = ["-D__Windows__"]
-    ldflags = ["-LAdvapi32.dll"]
+    ldflags = ["-LAdvapi32.lib"]
+    if PLATFORM == "AMD64":
+        cflags += ["-D__x86_64__"]
+        cflags += ["-D__AMD64__"]
+        cflags += ["-DHIGHCTIDH_PORTABLE=" + HIGHCTIDH_PORTABLE]
     if PLATFORM == "x86_64":
         cflags += ["-D__x86_64__"]
         cflags += ["-DHIGHCTIDH_PORTABLE=" + HIGHCTIDH_PORTABLE]
     cflags += [f"-DPLATFORM={PLATFORM}", f"-DPLATFORM_SIZE={PLATFORM_SIZE}"]
-    if CC == "clang":
-        cflangs += "-Wno-unused-command-line-argument"
 elif PLATFORM == "x86_64":
     if PLATFORM_SIZE == 64:
+        cflags += ["-D__x86_64__"]
         if OS == "Darwin":
           cflags += ["-D__Darwin__"]
-          if CC == "clang":
-              cflags += ["-D__x86_64__"]
-          if CC == "gcc":
-              cflags += ["-D__x86_64__"]
+          cflags += ["-DHIGHCTIDH_PORTABLE=1"]
         else:
           if CC == "clang":
               cflags += ["-DHIGHCTIDH_PORTABLE=1"]
           if CC == "gcc":
               cflags += ["-march=native", "-mtune=native"]
         if HIGHCTIDH_PORTABLE == "1":
             if CC == "clang":
@@ -382,14 +390,18 @@
     "-DNAMESPACEBITS(x)=highctidh_2048_##x",
     "-DNAMESPACEGENERIC(x)=highctidh_##x",
 ]
 print(f"511 files: {src_511=}")
 print(f"512 files: {src_512=}")
 print(f"1024 files: {src_1024=}")
 print(f"2048 files: {src_2048=}")
+print(f"511 cflags: {extra_compile_args_511=}")
+print(f"512 cflags: {extra_compile_args_512=}")
+print(f"1024 cflags: {extra_compile_args_1024=}")
+print(f"2048 cflags: {extra_compile_args_2048=}")
 if __name__ == "__main__":
     setup(
         name="highctidh",
         version=VERSION,
         author="Jacob Appelbaum",
         zip_safe=False,
         author_email="jacob@appelbaum.net",
```

### Comparing `highctidh-1.0.2024050100/sim.py` & `highctidh-1.0.2024050500/sim.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/skgen.c` & `highctidh-1.0.2024050500/skgen.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/steps.c` & `highctidh-1.0.2024050500/steps.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/steps.h` & `highctidh-1.0.2024050500/steps.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/test.c` & `highctidh-1.0.2024050500/test.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/test.sh` & `highctidh-1.0.2024050500/test.sh`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/testrandom.c` & `highctidh-1.0.2024050500/testrandom.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/tests/test_highctidh.py` & `highctidh-1.0.2024050500/tests/test_highctidh.py`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/tune2c` & `highctidh-1.0.2024050500/tune2c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/tunecycles.c` & `highctidh-1.0.2024050500/tunecycles.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/tunemults.c` & `highctidh-1.0.2024050500/tunemults.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/ubench.c` & `highctidh-1.0.2024050500/ubench.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig.h` & `highctidh-1.0.2024050500/uintbig.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig1024.S` & `highctidh-1.0.2024050500/uintbig1024.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig2048.S` & `highctidh-1.0.2024050500/uintbig2048.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig511.S` & `highctidh-1.0.2024050500/uintbig511.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig512.S` & `highctidh-1.0.2024050500/uintbig512.S`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/uintbig_namespace.h` & `highctidh-1.0.2024050500/uintbig_namespace.h`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/umults.c` & `highctidh-1.0.2024050500/umults.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/validate.c` & `highctidh-1.0.2024050500/validate.c`

 * *Files identical despite different names*

### Comparing `highctidh-1.0.2024050100/PKG-INFO` & `highctidh-1.0.2024050500/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highctidh
-Version: 1.0.2024050100
+Version: 1.0.2024050500
 Summary: highctidh bindings with included C library
 Keywords: post-quantum cryptography,cryptography,csidh,ctidh,C,highctidh
 Author: Jacob Appelbaum
 Author-email: jacob@appelbaum.net
 Maintainer: Jacob Appelbaum
 Maintainer-email: jacob@appelbaum.net
 Requires-Python: >=3.9.6
@@ -171,26 +171,45 @@
 - Rockylinux 9, 9.3 (GNU libc)
 - Solaris 11.4 (Solaris libc)
 - Ubuntu 22.03, 23.10, 24.04 (GNU libc)
 - Windows Server 2019, 2022 (MSVCRT)
 
 ## Notes on building
 
-Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is supported using the
-`gmake` command. GNU/Linux and MacOS are supported with the `make` command.
-
-Windows support is extremely experimental. The Python and Golang modules may
-not be functional on Windows. Building the main C library on Windows Server
-2019 and Windows Server 2022 should be possible with `clang` as is demonstrated
-in the continuous integration configuration `windows-fiat-c-library-test.yml`.
-It has only been tested with the Windows Server 2022 image preloaded with
-`clang`, `bash`, `make`, and other related tools
+Building on Solaris, CheriBSD, FreeBSD, NetBSD, and OpenBSD building is
+supported using the `gmake` command. GNU/Linux and MacOS are supported with the
+`make` command.
+
+MacOS 11, 12, 13, and 14 support is functional for building the C library.
+MacOS 14 support is functional for the Golang bindings with Golang 1.19, 1.20,
+1.21.x, and 1.22.0.
+MacOS 14 supports the Python module with Python 3.9, 3.10, 3.11, and 3.12.
+
+Windows support is extremely experimental. The Python and Golang modules are
+almost certianly not be functional on Windows. Building the main C library on
+Windows Server 2019 and Windows Server 2022 should be possible with `clang` as
+is demonstrated in the continuous integration configuration
+`windows-fiat-c-library-test.yml`.  It has only been tested with the Windows
+Server 2022 image preloaded with `clang`, `bash`, `make`, and other related
+tools
 [https://github.com/actions/runner-images/blob/main/images/windows/Windows2022-Readme.md](available
 as a part of the CI configuration).
 
+Building and performing minimal testing manually requires using `bash` as
+provided by `git` on Windows, GNU `make`, and `clang` using the following
+commands:
+```
+export HIGHCTIDH_PORTABLE=1
+export WINDOWS=1
+export CC=${{ matrix.CC }} MAKE=make
+mkdir -p src/build/src
+mkdir -p src/dist/tmp
+cd src/ && make && make testrandom test512 && ./testrandom && ./test512
+```
+
 ### Additional notes on building the C library
  
 To build and install we recommend:
 ```
    sudo apt install gcc clang make
    make
    sudo make install
```

