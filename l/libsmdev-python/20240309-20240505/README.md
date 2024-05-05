# Comparing `tmp/libsmdev-python-20240309.tar.gz` & `tmp/libsmdev-python-20240505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsmdev-python-20240309.tar", last modified: Sat Mar  9 06:57:49 2024, max compression
+gzip compressed data, was "libsmdev-python-20240505.tar", last modified: Sun May  5 09:14:16 2024, max compression
```

## Comparing `libsmdev-python-20240309.tar` & `libsmdev-python-20240505.tar`

### file list

```diff
@@ -1,544 +1,544 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-03-09 06:37:33.000000 libsmdev-20240309/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-03-09 06:46:05.000000 libsmdev-20240309/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:37:33.000000 libsmdev-20240309/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-03-09 06:46:06.000000 libsmdev-20240309/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11673 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31438 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8411 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17322 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11295 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-03-09 06:46:01.000000 libsmdev-20240309/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-03-09 06:46:01.000000 libsmdev-20240309/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-03-09 06:46:01.000000 libsmdev-20240309/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6438 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5819 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-03-09 06:46:01.000000 libsmdev-20240309/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-03-09 06:46:01.000000 libsmdev-20240309/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:20.000000 libsmdev-20240309/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-09 06:37:37.000000 libsmdev-20240309/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15011 2024-03-09 06:46:21.000000 libsmdev-20240309/include/libsmdev.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-03-09 06:37:33.000000 libsmdev-20240309/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15011 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/include/libsmdev/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2892 2024-03-09 06:46:21.000000 libsmdev-20240309/include/libsmdev/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-03-09 06:46:21.000000 libsmdev-20240309/include/libsmdev/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-09 06:46:21.000000 libsmdev-20240309/include/libsmdev/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-03-09 06:37:35.000000 libsmdev-20240309/include/libsmdev/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23816 2024-03-09 06:46:05.000000 libsmdev-20240309/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2348 2024-03-09 06:46:22.000000 libsmdev-20240309/libsmdev.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-03-09 06:37:35.000000 libsmdev-20240309/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-03-09 06:37:35.000000 libsmdev-20240309/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-03-09 06:37:35.000000 libsmdev-20240309/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-03-09 06:37:35.000000 libsmdev-20240309/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-03-09 06:37:35.000000 libsmdev-20240309/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-03-09 06:37:35.000000 libsmdev-20240309/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-03-09 06:37:35.000000 libsmdev-20240309/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-03-09 06:37:33.000000 libsmdev-20240309/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-03-09 06:37:35.000000 libsmdev-20240309/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-03-09 06:46:22.000000 libsmdev-20240309/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14244 2024-03-09 06:46:05.000000 libsmdev-20240309/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15088 2024-03-09 06:46:22.000000 libsmdev-20240309/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-03-09 06:37:35.000000 libsmdev-20240309/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-03-09 06:37:35.000000 libsmdev-20240309/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-03-09 06:37:35.000000 libsmdev-20240309/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20823 2024-03-09 06:46:05.000000 libsmdev-20240309/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25826 2024-03-09 06:46:06.000000 libsmdev-20240309/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-03-09 06:45:50.000000 libsmdev-20240309/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2023-12-03 09:14:09.000000 libsmdev-20240309/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:14:09.000000 libsmdev-20240309/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-03-09 06:46:05.000000 libsmdev-20240309/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-03-09 06:37:37.000000 libsmdev-20240309/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/libsmdev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/libsmdev-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/libsmdev-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-03-09 06:46:22.000000 libsmdev-20240309/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-03-09 06:37:33.000000 libsmdev-20240309/dpkg/libsmdev-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-03-09 06:46:22.000000 libsmdev-20240309/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-03-09 06:37:33.000000 libsmdev-20240309/libsmdev.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-03-09 06:37:33.000000 libsmdev-20240309/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1246584 2024-03-09 06:46:04.000000 libsmdev-20240309/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/pysmdev/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1405 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3524 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_libsmdev.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      901 2023-12-03 09:14:21.000000 libsmdev-20240309/pysmdev/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2976 2024-03-09 06:38:25.000000 libsmdev-20240309/pysmdev/pysmdev_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-09 06:38:25.000000 libsmdev-20240309/pysmdev/pysmdev.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27070 2024-03-09 06:38:25.000000 libsmdev-20240309/pysmdev/pysmdev_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9041 2024-03-09 06:38:25.000000 libsmdev-20240309/pysmdev/pysmdev.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-03-09 06:37:36.000000 libsmdev-20240309/pysmdev/pysmdev_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34566 2024-03-09 06:46:06.000000 libsmdev-20240309/pysmdev/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-03-09 06:46:05.000000 libsmdev-20240309/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-03-09 06:46:05.000000 libsmdev-20240309/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_support/smdev_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_scsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5395 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_scsi/smdev_test_scsi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdevinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6272 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdevinfo/smdevinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_track_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5333 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_track_value/smdev_test_track_value.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16841 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libsmdev.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      917 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/pysmdev/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5764 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/pysmdev/pysmdev.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libsmdev/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7679 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libsmdev/libsmdev.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5069 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_error/smdev_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5899 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_handle/smdev_test_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_optical_disc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5257 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_optical_disc/smdev_test_optical_disc.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5156 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_string/smdev_test_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_ata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5230 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_ata/smdev_test_ata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5156 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_notify/smdev_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18708 2024-03-09 06:46:06.000000 libsmdev-20240309/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/smdev_test_sector_range/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5336 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/smdev_test_sector_range/smdev_test_sector_range.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-03-09 06:39:28.000000 libsmdev-20240309/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-03-09 06:37:35.000000 libsmdev-20240309/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26590 2024-03-09 06:46:06.000000 libsmdev-20240309/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-03-09 06:45:49.000000 libsmdev-20240309/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      329 2024-03-09 06:37:33.000000 libsmdev-20240309/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-03-09 06:46:05.000000 libsmdev-20240309/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28274 2024-03-09 06:46:06.000000 libsmdev-20240309/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-09 06:45:40.000000 libsmdev-20240309/libcdata/libcdata_error.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/libsmdev/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7732 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_track_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3546 2024-03-09 06:46:22.000000 libsmdev-20240309/libsmdev/libsmdev_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25893 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_scsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3903 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_ata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33482 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_optical_disc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7015 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_sector_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-03-09 06:46:22.000000 libsmdev-20240309/libsmdev/libsmdev.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1302 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2196 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_track_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2023-12-03 09:14:20.000000 libsmdev-20240309/libsmdev/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3548 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6304 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_usb.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_optical_disc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_usb.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1941 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2245 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   121410 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9723 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_sector_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7610 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_scsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_ata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1503 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30494 2024-03-09 06:46:06.000000 libsmdev-20240309/libsmdev/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1829 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15180 2024-03-09 06:37:36.000000 libsmdev-20240309/libsmdev/libsmdev_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-03-09 06:37:33.000000 libsmdev-20240309/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-03-09 06:37:33.000000 libsmdev-20240309/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-03-09 06:46:05.000000 libsmdev-20240309/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-03-09 06:37:33.000000 libsmdev-20240309/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4682 2024-03-09 06:38:25.000000 libsmdev-20240309/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:14:09.000000 libsmdev-20240309/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28680 2024-03-09 06:46:06.000000 libsmdev-20240309/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-03-09 06:45:53.000000 libsmdev-20240309/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-03-09 06:46:06.000000 libsmdev-20240309/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      995 2023-12-03 09:14:09.000000 libsmdev-20240309/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-03-09 06:37:37.000000 libsmdev-20240309/manuals/smdevinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      158 2023-12-03 09:14:21.000000 libsmdev-20240309/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22793 2024-03-09 06:46:06.000000 libsmdev-20240309/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7354 2024-03-09 06:37:37.000000 libsmdev-20240309/manuals/libsmdev.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4984 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_ata.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/test_smdevinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libsmdev.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1957 2024-03-09 06:38:25.000000 libsmdev-20240309/tests/pysmdev_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4210 2024-03-09 06:38:04.000000 libsmdev-20240309/tests/smdev_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13563 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_track_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4367 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12776 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_optical_disc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4003 2024-03-09 06:38:04.000000 libsmdev-20240309/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-03-09 06:38:25.000000 libsmdev-20240309/tests/smdev_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25325 2024-03-09 06:38:04.000000 libsmdev-20240309/tests/smdev_test_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4078 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18686 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_scsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49135 2024-03-09 06:46:06.000000 libsmdev-20240309/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13837 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_sector_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6505 2024-03-09 06:38:25.000000 libsmdev-20240309/tests/pysmdev_test_handle.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10689 2024-03-09 06:38:04.000000 libsmdev-20240309/tests/smdev_test_functions.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4121 2024-03-09 06:38:25.000000 libsmdev-20240309/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-03-09 06:37:37.000000 libsmdev-20240309/tests/smdev_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-03-09 06:46:01.000000 libsmdev-20240309/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:20.000000 libsmdev-20240309/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:20.000000 libsmdev-20240309/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:20.000000 libsmdev-20240309/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:20.000000 libsmdev-20240309/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:20.000000 libsmdev-20240309/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:20.000000 libsmdev-20240309/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:20.000000 libsmdev-20240309/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:20.000000 libsmdev-20240309/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:20.000000 libsmdev-20240309/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-03-09 06:46:21.000000 libsmdev-20240309/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:20.000000 libsmdev-20240309/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:20.000000 libsmdev-20240309/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49392 2024-03-09 06:46:06.000000 libsmdev-20240309/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-03-09 06:45:56.000000 libsmdev-20240309/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36418 2024-03-09 06:46:05.000000 libsmdev-20240309/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:48.000000 libsmdev-20240309/smdevtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2369 2024-03-09 06:38:25.000000 libsmdev-20240309/smdevtools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libsmdev.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10555 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1085 2023-12-03 09:14:21.000000 libsmdev-20240309/smdevtools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6765 2024-03-09 06:38:25.000000 libsmdev-20240309/smdevtools/smdevinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19734 2024-03-09 06:38:25.000000 libsmdev-20240309/smdevtools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3821 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27364 2024-03-09 06:46:06.000000 libsmdev-20240309/smdevtools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-03-09 06:37:36.000000 libsmdev-20240309/smdevtools/smdevtools_getopt.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25702 2024-03-09 06:46:06.000000 libsmdev-20240309/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-03-09 06:45:52.000000 libsmdev-20240309/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 06:57:47.000000 libsmdev-20240309/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-03-09 06:45:41.000000 libsmdev-20240309/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25215 2024-03-09 06:46:06.000000 libsmdev-20240309/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56590 2024-03-09 06:46:03.000000 libsmdev-20240309/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5759 2024-03-09 06:37:33.000000 libsmdev-20240309/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2024-03-09 06:37:33.000000 libsmdev-20240309/libsmdev.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-03-09 06:57:49.477221 libsmdev-20240309/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-05 08:45:15.000000 libsmdev-20240505/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-05 09:01:46.000000 libsmdev-20240505/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:45:15.000000 libsmdev-20240505/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-05 09:01:47.000000 libsmdev-20240505/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-09 06:37:37.000000 libsmdev-20240505/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-05 09:01:42.000000 libsmdev-20240505/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-05 09:01:42.000000 libsmdev-20240505/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-05 09:01:42.000000 libsmdev-20240505/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-05 09:01:42.000000 libsmdev-20240505/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-05 09:01:42.000000 libsmdev-20240505/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-05 08:45:19.000000 libsmdev-20240505/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:20.000000 libsmdev-20240505/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-09 06:37:37.000000 libsmdev-20240505/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15011 2024-05-05 09:01:59.000000 libsmdev-20240505/include/libsmdev.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-05 08:50:46.000000 libsmdev-20240505/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15011 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/include/libsmdev/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2892 2024-05-05 09:01:59.000000 libsmdev-20240505/include/libsmdev/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4944 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4813 2024-05-05 09:01:59.000000 libsmdev-20240505/include/libsmdev/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 09:01:59.000000 libsmdev-20240505/include/libsmdev/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-05 08:45:17.000000 libsmdev-20240505/include/libsmdev/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23796 2024-05-05 09:01:46.000000 libsmdev-20240505/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2348 2024-05-05 09:01:59.000000 libsmdev-20240505/libsmdev.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-05 08:45:17.000000 libsmdev-20240505/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-05 08:45:17.000000 libsmdev-20240505/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-05 08:45:17.000000 libsmdev-20240505/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-05 08:45:17.000000 libsmdev-20240505/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-05 08:45:17.000000 libsmdev-20240505/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-05 08:45:17.000000 libsmdev-20240505/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-05 08:45:17.000000 libsmdev-20240505/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-05 08:50:46.000000 libsmdev-20240505/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-05 08:45:17.000000 libsmdev-20240505/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-05 09:01:59.000000 libsmdev-20240505/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14244 2024-05-05 09:01:46.000000 libsmdev-20240505/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15088 2024-05-05 09:01:59.000000 libsmdev-20240505/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-05 08:45:17.000000 libsmdev-20240505/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-05 08:45:17.000000 libsmdev-20240505/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-05 08:45:17.000000 libsmdev-20240505/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20830 2024-05-05 09:01:46.000000 libsmdev-20240505/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:14.000000 libsmdev-20240505/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26028 2024-05-05 09:01:47.000000 libsmdev-20240505/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-05 09:01:27.000000 libsmdev-20240505/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1631 2024-05-05 08:52:31.000000 libsmdev-20240505/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:14:09.000000 libsmdev-20240505/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-05 09:01:46.000000 libsmdev-20240505/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-05 08:45:19.000000 libsmdev-20240505/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/libsmdev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/libsmdev-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/libsmdev-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-05 09:01:59.000000 libsmdev-20240505/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-05 08:45:15.000000 libsmdev-20240505/dpkg/libsmdev-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      482 2024-05-05 09:01:59.000000 libsmdev-20240505/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-05-05 08:45:15.000000 libsmdev-20240505/libsmdev.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-05 08:45:15.000000 libsmdev-20240505/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1247176 2024-05-05 09:01:45.000000 libsmdev-20240505/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:15.000000 libsmdev-20240505/pysmdev/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1405 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3524 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_libsmdev.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      897 2024-05-05 08:52:04.000000 libsmdev-20240505/pysmdev/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2976 2024-05-05 08:46:16.000000 libsmdev-20240505/pysmdev/pysmdev_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 08:46:16.000000 libsmdev-20240505/pysmdev/pysmdev.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27070 2024-05-05 08:46:16.000000 libsmdev-20240505/pysmdev/pysmdev_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9041 2024-05-05 08:46:16.000000 libsmdev-20240505/pysmdev/pysmdev.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-05 08:45:18.000000 libsmdev-20240505/pysmdev/pysmdev_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34837 2024-05-05 09:01:47.000000 libsmdev-20240505/pysmdev/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-05 09:01:46.000000 libsmdev-20240505/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-05 09:01:46.000000 libsmdev-20240505/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5159 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdev_test_support/smdev_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_scsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5395 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/smdev_test_scsi/smdev_test_scsi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdevinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6272 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdevinfo/smdevinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_track_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5333 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdev_test_track_value/smdev_test_track_value.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16841 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/libsmdev.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      888 2024-05-05 08:51:56.000000 libsmdev-20240505/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/pysmdev/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5764 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/pysmdev/pysmdev.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libsmdev/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7679 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libsmdev/libsmdev.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5069 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdev_test_error/smdev_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5899 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/smdev_test_handle/smdev_test_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_optical_disc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5257 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/smdev_test_optical_disc/smdev_test_optical_disc.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5156 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/smdev_test_string/smdev_test_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_ata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5230 2024-05-05 08:46:04.000000 libsmdev-20240505/msvscpp/smdev_test_ata/smdev_test_ata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5156 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdev_test_notify/smdev_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18708 2024-05-05 09:01:47.000000 libsmdev-20240505/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/smdev_test_sector_range/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5336 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/smdev_test_sector_range/smdev_test_sector_range.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-05 08:45:49.000000 libsmdev-20240505/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-05-05 08:45:16.000000 libsmdev-20240505/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:15.000000 libsmdev-20240505/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26861 2024-05-05 09:01:46.000000 libsmdev-20240505/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-05 09:01:23.000000 libsmdev-20240505/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      329 2024-05-05 08:45:15.000000 libsmdev-20240505/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-05 09:01:46.000000 libsmdev-20240505/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:14.000000 libsmdev-20240505/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28774 2024-05-05 09:01:46.000000 libsmdev-20240505/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 09:01:08.000000 libsmdev-20240505/libcdata/libcdata_error.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:15.000000 libsmdev-20240505/libsmdev/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7732 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_track_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3546 2024-05-05 09:01:59.000000 libsmdev-20240505/libsmdev/libsmdev_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25893 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_scsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3903 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_ata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33482 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_optical_disc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7015 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_sector_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-05-05 09:01:59.000000 libsmdev-20240505/libsmdev/libsmdev.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1302 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2196 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_track_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1716 2024-05-05 08:51:48.000000 libsmdev-20240505/libsmdev/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3548 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6304 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_usb.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_optical_disc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_usb.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1941 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2245 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1160 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1347 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   121410 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9723 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_sector_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7610 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_scsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_ata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1503 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31031 2024-05-05 09:01:47.000000 libsmdev-20240505/libsmdev/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1829 2024-05-05 08:45:17.000000 libsmdev-20240505/libsmdev/libsmdev.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15180 2024-05-05 08:45:18.000000 libsmdev-20240505/libsmdev/libsmdev_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-05 08:45:15.000000 libsmdev-20240505/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-05-05 08:45:15.000000 libsmdev-20240505/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-05 09:01:46.000000 libsmdev-20240505/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-05 08:45:15.000000 libsmdev-20240505/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4682 2024-05-05 08:46:23.000000 libsmdev-20240505/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:14:09.000000 libsmdev-20240505/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:14.000000 libsmdev-20240505/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29213 2024-05-05 09:01:47.000000 libsmdev-20240505/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-05 09:01:32.000000 libsmdev-20240505/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-05 09:01:47.000000 libsmdev-20240505/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      995 2023-12-03 09:14:09.000000 libsmdev-20240505/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-05 08:45:19.000000 libsmdev-20240505/manuals/smdevinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      129 2024-05-05 08:51:36.000000 libsmdev-20240505/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22793 2024-05-05 09:01:47.000000 libsmdev-20240505/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7354 2024-05-05 08:45:19.000000 libsmdev-20240505/manuals/libsmdev.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4984 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_ata.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3289 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/test_smdevinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libsmdev.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1957 2024-05-05 08:46:16.000000 libsmdev-20240505/tests/pysmdev_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4210 2024-05-05 08:46:04.000000 libsmdev-20240505/tests/smdev_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13563 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_track_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4367 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12776 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_optical_disc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4020 2024-05-05 08:51:25.000000 libsmdev-20240505/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-05-05 08:46:30.000000 libsmdev-20240505/tests/smdev_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25325 2024-05-05 08:46:04.000000 libsmdev-20240505/tests/smdev_test_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4407 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18686 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_scsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49730 2024-05-05 09:01:47.000000 libsmdev-20240505/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13837 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_sector_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6505 2024-05-05 08:46:16.000000 libsmdev-20240505/tests/pysmdev_test_handle.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10689 2024-05-05 08:46:04.000000 libsmdev-20240505/tests/smdev_test_functions.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4090 2024-05-05 08:47:57.000000 libsmdev-20240505/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-05 08:45:19.000000 libsmdev-20240505/tests/smdev_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-05 09:01:41.000000 libsmdev-20240505/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:16.000000 libsmdev-20240505/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:20.000000 libsmdev-20240505/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:20.000000 libsmdev-20240505/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:20.000000 libsmdev-20240505/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:20.000000 libsmdev-20240505/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:20.000000 libsmdev-20240505/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:20.000000 libsmdev-20240505/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:20.000000 libsmdev-20240505/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:20.000000 libsmdev-20240505/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:20.000000 libsmdev-20240505/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-05 09:01:59.000000 libsmdev-20240505/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:20.000000 libsmdev-20240505/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:20.000000 libsmdev-20240505/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:14.000000 libsmdev-20240505/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52540 2024-05-05 09:01:47.000000 libsmdev-20240505/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-05 09:01:37.000000 libsmdev-20240505/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36300 2024-05-05 09:01:46.000000 libsmdev-20240505/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:15.000000 libsmdev-20240505/smdevtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2369 2024-05-05 08:46:16.000000 libsmdev-20240505/smdevtools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libsmdev.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10555 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1081 2024-05-05 08:50:56.000000 libsmdev-20240505/smdevtools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6765 2024-05-05 08:46:16.000000 libsmdev-20240505/smdevtools/smdevinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19734 2024-05-05 08:46:16.000000 libsmdev-20240505/smdevtools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3821 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27621 2024-05-05 09:01:47.000000 libsmdev-20240505/smdevtools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1552 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-05 08:45:18.000000 libsmdev-20240505/smdevtools/smdevtools_getopt.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:14.000000 libsmdev-20240505/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25897 2024-05-05 09:01:47.000000 libsmdev-20240505/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-05 09:01:29.000000 libsmdev-20240505/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 09:14:13.000000 libsmdev-20240505/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 09:01:13.000000 libsmdev-20240505/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25364 2024-05-05 09:01:46.000000 libsmdev-20240505/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56590 2024-05-05 09:01:44.000000 libsmdev-20240505/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5759 2024-05-05 08:45:15.000000 libsmdev-20240505/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2024-05-05 08:45:15.000000 libsmdev-20240505/libsmdev.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      414 2024-05-05 09:14:16.952415 libsmdev-20240505/PKG-INFO
```

### Comparing `libsmdev-20240309/COPYING` & `libsmdev-20240505/COPYING`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/install-sh` & `libsmdev-20240505/install-sh`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/depcomp` & `libsmdev-20240505/depcomp`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libcfile.m4` & `libsmdev-20240505/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
@@ -203,15 +203,15 @@
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -357,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/tests.m4` & `libsmdev-20240505/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/lib-prefix.m4` & `libsmdev-20240505/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/progtest.m4` & `libsmdev-20240505/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libuna.m4` & `libsmdev-20240505/m4/libuna.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -942,15 +942,15 @@
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -972,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/gettext.m4` & `libsmdev-20240505/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/lib-ld.m4` & `libsmdev-20240505/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libclocale.m4` & `libsmdev-20240505/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
@@ -126,15 +126,15 @@
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -219,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/libcdata.m4` & `libsmdev-20240505/m4/libcdata.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
@@ -497,15 +497,15 @@
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -527,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/common.m4` & `libsmdev-20240505/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libcthreads.m4` & `libsmdev-20240505/m4/libcthreads.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
@@ -246,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -288,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libsmdev-20240309/m4/ltversion.m4` & `libsmdev-20240505/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/ltsugar.m4` & `libsmdev-20240505/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/host-cpu-c-abi.m4` & `libsmdev-20240505/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libtool.m4` & `libsmdev-20240505/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/po.m4` & `libsmdev-20240505/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/libcerror.m4` & `libsmdev-20240505/m4/libcerror.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
@@ -99,15 +99,15 @@
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/libcnotify.m4` & `libsmdev-20240505/m4/libcnotify.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20240308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
@@ -96,15 +96,15 @@
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -137,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libsmdev-20240309/m4/intlmacosx.m4` & `libsmdev-20240505/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/lt~obsolete.m4` & `libsmdev-20240505/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/lib-link.m4` & `libsmdev-20240505/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/iconv.m4` & `libsmdev-20240505/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/ltoptions.m4` & `libsmdev-20240505/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/nls.m4` & `libsmdev-20240505/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/python.m4` & `libsmdev-20240505/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libsmdev-20240309/m4/types.m4` & `libsmdev-20240505/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/m4/pthread.m4` & `libsmdev-20240505/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev.h` & `libsmdev-20240505/include/libsmdev.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev.h.in` & `libsmdev-20240505/include/libsmdev.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/definitions.h.in` & `libsmdev-20240505/include/libsmdev/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/definitions.h` & `libsmdev-20240505/include/libsmdev/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBSMDEV_DEFINIONS_H )
 #define _LIBSMDEV_DEFINIONS_H
 
 #include <libsmdev/types.h>
 
-#define LIBSMDEV_VERSION			20240309
+#define LIBSMDEV_VERSION			20240505
 
 /* The version string
  */
-#define LIBSMDEV_VERSION_STRING			"20240309"
+#define LIBSMDEV_VERSION_STRING			"20240505"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3        set to 1 to truncate an existing file on write
  * bit 4-8      not used
  */
```

### Comparing `libsmdev-20240309/include/libsmdev/types.h.in` & `libsmdev-20240505/include/libsmdev/types.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/types.h` & `libsmdev-20240505/include/libsmdev/types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/features.h.in` & `libsmdev-20240505/include/libsmdev/features.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/error.h` & `libsmdev-20240505/include/libsmdev/error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/extern.h` & `libsmdev-20240505/include/libsmdev/extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/features.h` & `libsmdev-20240505/include/libsmdev/features.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/libsmdev/codepage.h` & `libsmdev-20240505/include/libsmdev/codepage.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/include/Makefile.in` & `libsmdev-20240505/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,20 @@
 
 EXTRA_DIST = \
 	libsmdev.h.in \
 	libsmdev/definitions.h.in \
 	libsmdev/features.h.in \
 	libsmdev/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmdev.h \
+	libsmdev/definitions.h \
+	libsmdev/features.h \
+	libsmdev/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -639,23 +644,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -737,17 +744,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsmdev.h
-	-rm -f libsmdev/definitions.h
-	-rm -f libsmdev/features.h
-	-rm -f libsmdev/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/libsmdev.spec` & `libsmdev-20240505/libsmdev.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libsmdev
-Version: 20240309
+Version: 20240505
 Release: 1
 Summary: Library to access and read storage media (SM) devices
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libsmdev
        
@@ -90,10 +90,10 @@
 %files -n libsmdev-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Mar  9 2024 Joachim Metz <joachim.metz@gmail.com> 20240309-1
+* Sun May  5 2024 Joachim Metz <joachim.metz@gmail.com> 20240505-1
 - Auto-generated
```

### Comparing `libsmdev-20240309/common/config_borlandc.h` & `libsmdev-20240505/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/file_stream.h` & `libsmdev-20240505/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/memory.h` & `libsmdev-20240505/common/memory.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/byte_stream.h` & `libsmdev-20240505/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/common.h` & `libsmdev-20240505/common/common.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/config_winapi.h` & `libsmdev-20240505/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/system_string.h` & `libsmdev-20240505/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/types.h.in` & `libsmdev-20240505/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/types.h` & `libsmdev-20240505/common/types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/config.h.in` & `libsmdev-20240505/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/config.h` & `libsmdev-20240505/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -463,24 +463,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libsmdev"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libsmdev 20240309"
+#define PACKAGE_STRING "libsmdev 20240505"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libsmdev"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240309"
+#define PACKAGE_VERSION "20240505"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -498,15 +498,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240309"
+#define VERSION "20240505"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libsmdev-20240309/common/wide_string.h` & `libsmdev-20240505/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/narrow_string.h` & `libsmdev-20240505/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/config_msc.h` & `libsmdev-20240505/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/common/Makefile.in` & `libsmdev-20240505/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -387,15 +387,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -403,15 +405,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -579,23 +584,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -675,15 +682,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/libclocale/libclocale_wide_string.c` & `libsmdev-20240505/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_support.h` & `libsmdev-20240505/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/Makefile.am` & `libsmdev-20240505/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libsmdev-20240309/libclocale/libclocale_definitions.h` & `libsmdev-20240505/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libsmdev-20240309/libclocale/libclocale_unused.h` & `libsmdev-20240505/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_libcerror.h` & `libsmdev-20240505/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_locale.h` & `libsmdev-20240505/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_support.c` & `libsmdev-20240505/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_codepage.c` & `libsmdev-20240505/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_locale.c` & `libsmdev-20240505/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/Makefile.in` & `libsmdev-20240505/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -433,30 +433,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -659,24 +660,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -763,17 +770,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libclocale/libclocale_extern.h` & `libsmdev-20240505/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_wide_string.h` & `libsmdev-20240505/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libclocale/libclocale_codepage.h` & `libsmdev-20240505/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/Makefile.am` & `libsmdev-20240505/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -51,16 +51,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libsmdev.pc \
+	libsmdev.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libsmdev.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -76,19 +83,7 @@
 	(cd $(srcdir)/libclocale && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libuna && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcfile && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libsmdev && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libsmdev.pc
-	-rm -f libsmdev.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libsmdev-20240309/config.guess` & `libsmdev-20240505/config.guess`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/dpkg/copyright` & `libsmdev-20240505/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/dpkg/control` & `libsmdev-20240505/dpkg/control`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/dpkg/rules` & `libsmdev-20240505/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev.spec.in` & `libsmdev-20240505/libsmdev.spec.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/COPYING.LESSER` & `libsmdev-20240505/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/configure` & `libsmdev-20240505/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libsmdev 20240309.
+# Generated by GNU Autoconf 2.71 for libsmdev 20240505.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libsmdev'
 PACKAGE_TARNAME='libsmdev'
-PACKAGE_VERSION='20240309'
-PACKAGE_STRING='libsmdev 20240309'
+PACKAGE_VERSION='20240505'
+PACKAGE_STRING='libsmdev 20240505'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libsmdev.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1527,15 +1527,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libsmdev 20240309 to adapt to many kinds of systems.
+\`configure' configures libsmdev 20240505 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1598,15 +1598,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libsmdev 20240309:";;
+     short | recursive ) echo "Configuration of libsmdev 20240505:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1790,15 +1790,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libsmdev configure 20240309
+libsmdev configure 20240505
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2387,15 +2387,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libsmdev $as_me 20240309, which was
+It was created by libsmdev $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -3660,15 +3660,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libsmdev'
- VERSION='20240309'
+ VERSION='20240505'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -19921,15 +19921,15 @@
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -20071,15 +20071,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -21813,15 +21813,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -22733,15 +22733,15 @@
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -26609,15 +26609,15 @@
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26642,15 +26642,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -27276,15 +27276,15 @@
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -27440,15 +27440,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -27977,15 +27977,15 @@
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -28040,15 +28040,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -35329,15 +35329,15 @@
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -35362,15 +35362,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -36630,15 +36630,15 @@
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -36952,15 +36952,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -37655,16 +37655,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -38612,15 +38616,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libsmdev $as_me 20240309, which was
+This file was extended by libsmdev $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -38680,15 +38684,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libsmdev config.status 20240309
+libsmdev config.status 20240505
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libsmdev-20240309/pysmdev/pysmdev_error.h` & `libsmdev-20240505/pysmdev/pysmdev_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_metadata.h` & `libsmdev-20240505/pysmdev/pysmdev_metadata.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_metadata.c` & `libsmdev-20240505/pysmdev/pysmdev_metadata.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_integer.h` & `libsmdev-20240505/pysmdev/pysmdev_integer.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_libsmdev.h` & `libsmdev-20240505/pysmdev/pysmdev_libsmdev.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_libclocale.h` & `libsmdev-20240505/pysmdev/pysmdev_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/Makefile.am` & `libsmdev-20240505/pysmdev/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBSMDEV_DLL_IMPORT@
 
@@ -32,13 +32,11 @@
 	@LIBCFILE_LIBADD@
 
 pysmdev_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pysmdev_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libsmdev-20240309/pysmdev/pysmdev_handle.h` & `libsmdev-20240505/pysmdev/pysmdev_handle.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev.h` & `libsmdev-20240505/pysmdev/pysmdev.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_handle.c` & `libsmdev-20240505/pysmdev/pysmdev_handle.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev.c` & `libsmdev-20240505/pysmdev/pysmdev.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_error.c` & `libsmdev-20240505/pysmdev/pysmdev_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_unused.h` & `libsmdev-20240505/pysmdev/pysmdev_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_python.h` & `libsmdev-20240505/pysmdev/pysmdev_python.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_integer.c` & `libsmdev-20240505/pysmdev/pysmdev_integer.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/pysmdev_libcerror.h` & `libsmdev-20240505/pysmdev/pysmdev_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/pysmdev/Makefile.in` & `libsmdev-20240505/pysmdev/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -463,16 +463,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBSMDEV_DLL_IMPORT@
 
@@ -495,15 +495,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@
 
 @HAVE_PYTHON_TRUE@pysmdev_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pysmdev_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -769,24 +770,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pysmdev_la-pysmdev.Plo
+	-rm -f ./$(DEPDIR)/pysmdev_la-pysmdev_error.Plo
+	-rm -f ./$(DEPDIR)/pysmdev_la-pysmdev_handle.Plo
+	-rm -f ./$(DEPDIR)/pysmdev_la-pysmdev_integer.Plo
+	-rm -f ./$(DEPDIR)/pysmdev_la-pysmdev_metadata.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -875,13 +883,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/compile` & `libsmdev-20240505/compile`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/missing` & `libsmdev-20240505/missing`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_support/smdev_test_support.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_support/smdev_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_scsi/smdev_test_scsi.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_scsi/smdev_test_scsi.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdevinfo/smdevinfo.vcproj` & `libsmdev-20240505/msvscpp/smdevinfo/smdevinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_track_value/smdev_test_track_value.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_track_value/smdev_test_track_value.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libsmdev.sln` & `libsmdev-20240505/msvscpp/libsmdev.sln`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libclocale/libclocale.vcproj` & `libsmdev-20240505/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/Makefile.am` & `libsmdev-20240505/msvscpp/Makefile.am`

 * *Files 27% similar despite different names*

```diff
@@ -20,13 +20,11 @@
 	smdev_test_track_value/smdev_test_track_value.vcproj \
 	smdevinfo/smdevinfo.vcproj \
 	libsmdev.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libsmdev-20240309/msvscpp/pysmdev/pysmdev.vcproj` & `libsmdev-20240505/msvscpp/pysmdev/pysmdev.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libcfile/libcfile.vcproj` & `libsmdev-20240505/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libcdata/libcdata.vcproj` & `libsmdev-20240505/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libsmdev/libsmdev.vcproj` & `libsmdev-20240505/msvscpp/libsmdev/libsmdev.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_error/smdev_test_error.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_error/smdev_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_handle/smdev_test_handle.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_handle/smdev_test_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_optical_disc/smdev_test_optical_disc.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_optical_disc/smdev_test_optical_disc.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libcthreads/libcthreads.vcproj` & `libsmdev-20240505/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_string/smdev_test_string.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_string/smdev_test_string.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_ata/smdev_test_ata.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_ata/smdev_test_ata.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/smdev_test_notify/smdev_test_notify.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_notify/smdev_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libuna/libuna.vcproj` & `libsmdev-20240505/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/Makefile.in` & `libsmdev-20240505/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,16 @@
 	smdev_test_track_value/smdev_test_track_value.vcproj \
 	smdevinfo/smdevinfo.vcproj \
 	libsmdev.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -507,23 +508,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -602,13 +605,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/msvscpp/smdev_test_sector_range/smdev_test_sector_range.vcproj` & `libsmdev-20240505/msvscpp/smdev_test_sector_range/smdev_test_sector_range.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libcnotify/libcnotify.vcproj` & `libsmdev-20240505/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/msvscpp/libcerror/libcerror.vcproj` & `libsmdev-20240505/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_extern.h` & `libsmdev-20240505/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_support.h` & `libsmdev-20240505/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_unused.h` & `libsmdev-20240505/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_notify.h` & `libsmdev-20240505/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_support.c` & `libsmdev-20240505/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_types.h` & `libsmdev-20240505/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/Makefile.am` & `libsmdev-20240505/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libsmdev-20240309/libcfile/libcfile_notify.c` & `libsmdev-20240505/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_system_string.h` & `libsmdev-20240505/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_file.h` & `libsmdev-20240505/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_libcnotify.h` & `libsmdev-20240505/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_system_string.c` & `libsmdev-20240505/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_error.h` & `libsmdev-20240505/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_libcerror.h` & `libsmdev-20240505/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_file.c` & `libsmdev-20240505/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_libclocale.h` & `libsmdev-20240505/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_winapi.h` & `libsmdev-20240505/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/Makefile.in` & `libsmdev-20240505/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -435,16 +435,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -459,15 +459,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -672,24 +673,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -778,17 +787,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libcfile/libcfile_error.c` & `libsmdev-20240505/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_libuna.h` & `libsmdev-20240505/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_winapi.c` & `libsmdev-20240505/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcfile/libcfile_definitions.h` & `libsmdev-20240505/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libsmdev-20240309/INSTALL` & `libsmdev-20240505/INSTALL`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_list_element.h` & `libsmdev-20240505/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_array.h` & `libsmdev-20240505/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_definitions.h` & `libsmdev-20240505/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libsmdev-20240309/libcdata/libcdata_libcerror.h` & `libsmdev-20240505/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_unused.h` & `libsmdev-20240505/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_btree.h` & `libsmdev-20240505/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_btree.c` & `libsmdev-20240505/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_support.c` & `libsmdev-20240505/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_list.c` & `libsmdev-20240505/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_extern.h` & `libsmdev-20240505/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_list.h` & `libsmdev-20240505/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_btree_values_list.h` & `libsmdev-20240505/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/Makefile.am` & `libsmdev-20240505/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libsmdev-20240309/libcdata/libcdata_btree_node.h` & `libsmdev-20240505/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_range_list_value.h` & `libsmdev-20240505/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_range_list.h` & `libsmdev-20240505/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_range_list.c` & `libsmdev-20240505/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_array.c` & `libsmdev-20240505/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_list_element.c` & `libsmdev-20240505/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_libcthreads.h` & `libsmdev-20240505/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_tree_node.h` & `libsmdev-20240505/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_error.h` & `libsmdev-20240505/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_types.h` & `libsmdev-20240505/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_btree_node.c` & `libsmdev-20240505/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_tree_node.c` & `libsmdev-20240505/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_support.h` & `libsmdev-20240505/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/Makefile.in` & `libsmdev-20240505/libcdata/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -449,16 +449,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -475,15 +475,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -693,24 +694,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -804,17 +818,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libcdata/libcdata_range_list_value.c` & `libsmdev-20240505/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_btree_values_list.c` & `libsmdev-20240505/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcdata/libcdata_error.c` & `libsmdev-20240505/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_track_value.c` & `libsmdev-20240505/libsmdev/libsmdev_track_value.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_codepage.h` & `libsmdev-20240505/libsmdev/libsmdev_codepage.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_extern.h` & `libsmdev-20240505/libsmdev/libsmdev_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_definitions.h` & `libsmdev-20240505/libsmdev/libsmdev_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 /* Define HAVE_LOCAL_LIBSMDEV for local use of libsmdev
  */
 #if !defined( HAVE_LOCAL_LIBSMDEV )
 #include <libsmdev/definitions.h>
 
 #else
 
-#define LIBSMDEV_VERSION				20240309
+#define LIBSMDEV_VERSION				20240505
 
 /* The version string
  */
-#define LIBSMDEV_VERSION_STRING				"20240309"
+#define LIBSMDEV_VERSION_STRING				"20240505"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3        set to 1 to truncate an existing file on write
  * bit 4-8      not used
  */
```

### Comparing `libsmdev-20240309/libsmdev/libsmdev_scsi.c` & `libsmdev-20240505/libsmdev/libsmdev_scsi.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_notify.h` & `libsmdev-20240505/libsmdev/libsmdev_notify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_ata.c` & `libsmdev-20240505/libsmdev/libsmdev_ata.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_optical_disc.c` & `libsmdev-20240505/libsmdev/libsmdev_optical_disc.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_sector_range.c` & `libsmdev-20240505/libsmdev/libsmdev_sector_range.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev.rc` & `libsmdev-20240505/libsmdev/libsmdev.rc`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access and read storage media (SM) devices\0"
-      VALUE "FileVersion",		"20240309" "\0"
+      VALUE "FileVersion",		"20240505" "\0"
       VALUE "InternalName",		"libsmdev.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libsmdev.dll\0"
       VALUE "ProductName",		"libsmdev\0"
-      VALUE "ProductVersion",		"20240309" "\0"
+      VALUE "ProductVersion",		"20240505" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libsmdev/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libsmdev-20240309/libsmdev/libsmdev_notify.c` & `libsmdev-20240505/libsmdev/libsmdev_notify.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_string.h` & `libsmdev-20240505/libsmdev/libsmdev_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libuna.h` & `libsmdev-20240505/libsmdev/libsmdev_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libclocale.h` & `libsmdev-20240505/libsmdev/libsmdev_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_error.h` & `libsmdev-20240505/libsmdev/libsmdev_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_track_value.h` & `libsmdev-20240505/libsmdev/libsmdev_track_value.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/Makefile.am` & `libsmdev-20240505/libsmdev/Makefile.am`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -52,21 +52,19 @@
 libsmdev_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libsmdev_definitions.h.in \
 	libsmdev.rc \
 	libsmdev.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmdev_definitions.h \
+	libsmdev.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libsmdev_definitions.h
-	-rm -f libsmdev.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsmdev ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsmdev_la_SOURCES)
```

### Comparing `libsmdev-20240309/libsmdev/libsmdev_unused.h` & `libsmdev-20240505/libsmdev/libsmdev_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_definitions.h.in` & `libsmdev-20240505/libsmdev/libsmdev_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_usb.c` & `libsmdev-20240505/libsmdev/libsmdev_usb.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_error.c` & `libsmdev-20240505/libsmdev/libsmdev_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libcdata.h` & `libsmdev-20240505/libsmdev/libsmdev_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_optical_disc.h` & `libsmdev-20240505/libsmdev/libsmdev_optical_disc.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_usb.h` & `libsmdev-20240505/libsmdev/libsmdev_usb.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_support.h` & `libsmdev-20240505/libsmdev/libsmdev_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_string.c` & `libsmdev-20240505/libsmdev/libsmdev_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libcerror.h` & `libsmdev-20240505/libsmdev/libsmdev_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_debug.c` & `libsmdev-20240505/libsmdev/libsmdev_debug.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_debug.h` & `libsmdev-20240505/libsmdev/libsmdev_debug.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libcfile.h` & `libsmdev-20240505/libsmdev/libsmdev_libcfile.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_handle.c` & `libsmdev-20240505/libsmdev/libsmdev_handle.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_handle.h` & `libsmdev-20240505/libsmdev/libsmdev_handle.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev.rc.in` & `libsmdev-20240505/libsmdev/libsmdev.rc.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_sector_range.h` & `libsmdev-20240505/libsmdev/libsmdev_sector_range.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_scsi.h` & `libsmdev-20240505/libsmdev/libsmdev_scsi.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_ata.h` & `libsmdev-20240505/libsmdev/libsmdev_ata.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_libcnotify.h` & `libsmdev-20240505/libsmdev/libsmdev_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_types.h` & `libsmdev-20240505/libsmdev/libsmdev_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/Makefile.in` & `libsmdev-20240505/libsmdev/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -464,16 +464,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -519,15 +519,18 @@
 
 libsmdev_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libsmdev_definitions.h.in \
 	libsmdev.rc \
 	libsmdev.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsmdev_definitions.h \
+	libsmdev.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -770,24 +773,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libsmdev.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_ata.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_debug.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_error.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_handle.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_notify.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_optical_disc.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_scsi.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_sector_range.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_string.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_support.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_track_value.Plo
+	-rm -f ./$(DEPDIR)/libsmdev_usb.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -883,19 +901,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsmdev_definitions.h
-	-rm -f libsmdev.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsmdev ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsmdev_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libsmdev/libsmdev.c` & `libsmdev-20240505/libsmdev/libsmdev.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libsmdev/libsmdev_support.c` & `libsmdev-20240505/libsmdev/libsmdev_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/config.sub` & `libsmdev-20240505/config.sub`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/setup.py` & `libsmdev-20240505/setup.py`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/acinclude.m4` & `libsmdev-20240505/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/config.rpath` & `libsmdev-20240505/config.rpath`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread.h` & `libsmdev-20240505/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_read_write_lock.h` & `libsmdev-20240505/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread.c` & `libsmdev-20240505/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread_pool.h` & `libsmdev-20240505/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_support.h` & `libsmdev-20240505/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_lock.h` & `libsmdev-20240505/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_unused.h` & `libsmdev-20240505/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_lock.c` & `libsmdev-20240505/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_condition.h` & `libsmdev-20240505/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_repeating_thread.h` & `libsmdev-20240505/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/Makefile.am` & `libsmdev-20240505/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libsmdev-20240309/libcthreads/libcthreads_support.c` & `libsmdev-20240505/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_mutex.c` & `libsmdev-20240505/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_queue.c` & `libsmdev-20240505/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_mutex.h` & `libsmdev-20240505/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_types.h` & `libsmdev-20240505/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread_attributes.h` & `libsmdev-20240505/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_condition.c` & `libsmdev-20240505/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_error.c` & `libsmdev-20240505/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_read_write_lock.c` & `libsmdev-20240505/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_libcerror.h` & `libsmdev-20240505/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_definitions.h` & `libsmdev-20240505/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread_pool.c` & `libsmdev-20240505/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_error.h` & `libsmdev-20240505/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_thread_attributes.c` & `libsmdev-20240505/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_extern.h` & `libsmdev-20240505/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/libcthreads_repeating_thread.c` & `libsmdev-20240505/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcthreads/Makefile.in` & `libsmdev-20240505/libcthreads/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -453,16 +453,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -477,15 +477,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -695,24 +696,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -806,17 +820,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libcthreads/libcthreads_queue.h` & `libsmdev-20240505/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/test-driver` & `libsmdev-20240505/test-driver`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/ChangeLog` & `libsmdev-20240505/ChangeLog`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/manuals/smdevinfo.1` & `libsmdev-20240505/manuals/smdevinfo.1`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/manuals/Makefile.in` & `libsmdev-20240505/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -409,15 +409,16 @@
 	libsmdev.3 \
 	smdevinfo.1
 
 EXTRA_DIST = \
 	libsmdev.3 \
 	smdevinfo.1
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -610,23 +611,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -708,13 +711,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/manuals/libsmdev.3` & `libsmdev-20240505/manuals/libsmdev.3`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_ata.c` & `libsmdev-20240505/tests/smdev_test_ata.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/test_smdevinfo.sh` & `libsmdev-20240505/tests/test_smdevinfo.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("smdevinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmdev-20240309/tests/smdev_test_error.c` & `libsmdev-20240505/tests/smdev_test_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_libcnotify.h` & `libsmdev-20240505/tests/smdev_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_getopt.h` & `libsmdev-20240505/tests/smdev_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_libsmdev.h` & `libsmdev-20240505/tests/smdev_test_libsmdev.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/pysmdev_test_support.py` & `libsmdev-20240505/tests/pysmdev_test_support.py`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_libcfile.h` & `libsmdev-20240505/tests/smdev_test_libcfile.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_support.c` & `libsmdev-20240505/tests/smdev_test_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_track_value.c` & `libsmdev-20240505/tests/smdev_test_track_value.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_string.c` & `libsmdev-20240505/tests/smdev_test_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_optical_disc.c` & `libsmdev-20240505/tests/smdev_test_optical_disc.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/Makefile.am` & `libsmdev-20240505/tests/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -180,13 +180,12 @@
 	smdev_test_track_value.c \
 	smdev_test_unused.h
 
 smdev_test_track_value_LDADD = \
 	../libsmdev/libsmdev.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libsmdev-20240309/tests/smdev_test_libclocale.h` & `libsmdev-20240505/tests/smdev_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_unused.h` & `libsmdev-20240505/tests/smdev_test_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_functions.h` & `libsmdev-20240505/tests/smdev_test_functions.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_handle.c` & `libsmdev-20240505/tests/smdev_test_handle.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/test_python_module.sh` & `libsmdev-20240505/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="handle";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libsmdev";
+PYTHON_MODULE="pysmdev";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysmdev_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysmdev_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pysmdev");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libsmdev-20240309/tests/smdev_test_memory.c` & `libsmdev-20240505/tests/smdev_test_memory.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_notify.c` & `libsmdev-20240505/tests/smdev_test_notify.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_macros.h` & `libsmdev-20240505/tests/smdev_test_macros.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/test_runner.sh` & `libsmdev-20240505/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_libuna.h` & `libsmdev-20240505/tests/smdev_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_getopt.c` & `libsmdev-20240505/tests/smdev_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_scsi.c` & `libsmdev-20240505/tests/smdev_test_scsi.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/Makefile.in` & `libsmdev-20240505/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -684,16 +684,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -855,16 +855,18 @@
 	smdev_test_track_value.c \
 	smdev_test_unused.h
 
 smdev_test_track_value_LDADD = \
 	../libsmdev/libsmdev.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1292,24 +1294,39 @@
 	-test -z "$(TEST_SUITE_LOG)" || rm -f $(TEST_SUITE_LOG)
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/smdev_test_ata.Po
+	-rm -f ./$(DEPDIR)/smdev_test_error.Po
+	-rm -f ./$(DEPDIR)/smdev_test_functions.Po
+	-rm -f ./$(DEPDIR)/smdev_test_getopt.Po
+	-rm -f ./$(DEPDIR)/smdev_test_handle.Po
+	-rm -f ./$(DEPDIR)/smdev_test_memory.Po
+	-rm -f ./$(DEPDIR)/smdev_test_notify.Po
+	-rm -f ./$(DEPDIR)/smdev_test_optical_disc.Po
+	-rm -f ./$(DEPDIR)/smdev_test_scsi.Po
+	-rm -f ./$(DEPDIR)/smdev_test_sector_range.Po
+	-rm -f ./$(DEPDIR)/smdev_test_string.Po
+	-rm -f ./$(DEPDIR)/smdev_test_support.Po
+	-rm -f ./$(DEPDIR)/smdev_test_track_value.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1405,13 +1422,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/tests/smdev_test_sector_range.c` & `libsmdev-20240505/tests/smdev_test_sector_range.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_memory.h` & `libsmdev-20240505/tests/smdev_test_memory.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/pysmdev_test_handle.py` & `libsmdev-20240505/tests/pysmdev_test_handle.py`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/smdev_test_functions.c` & `libsmdev-20240505/tests/smdev_test_functions.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/tests/test_library.sh` & `libsmdev-20240505/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="ata error notify optical_disc scsi sector_range string support track_value";
 LIBRARY_TESTS_WITH_INPUT="handle";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libsmdev-20240309/tests/smdev_test_libcerror.h` & `libsmdev-20240505/tests/smdev_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/ltmain.sh` & `libsmdev-20240505/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/remove-potcdate.sin` & `libsmdev-20240505/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/Makefile.in.in` & `libsmdev-20240505/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/en@quot.header` & `libsmdev-20240505/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/en@boldquot.header` & `libsmdev-20240505/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/insert-header.sin` & `libsmdev-20240505/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/Makevars` & `libsmdev-20240505/po/Makevars`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/Makevars.in` & `libsmdev-20240505/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/po/Rules-quot` & `libsmdev-20240505/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1251.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf16_string.c` & `libsmdev-20240505/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base16_stream.c` & `libsmdev-20240505/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf8_stream.h` & `libsmdev-20240505/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_2.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_932.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_dingbats.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf8_string.c` & `libsmdev-20240505/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base64_stream.c` & `libsmdev-20240505/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_error.h` & `libsmdev-20240505/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_turkish.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_unicode_character.c` & `libsmdev-20240505/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_gaelic.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_arabic.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_thai.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_874.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_15.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf8_string.h` & `libsmdev-20240505/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_16.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1255.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf7_stream.c` & `libsmdev-20240505/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_byte_stream.h` & `libsmdev-20240505/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_koi8_u.c` & `libsmdev-20240505/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_unused.h` & `libsmdev-20240505/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_6.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_14.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base64_stream.h` & `libsmdev-20240505/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_error.c` & `libsmdev-20240505/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_centraleurroman.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_romanian.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_6.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_9.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_russian.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_dingbats.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_15.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_936.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_croatian.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_scsu.h` & `libsmdev-20240505/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/Makefile.am` & `libsmdev-20240505/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libsmdev-20240309/libuna/libuna_utf32_stream.c` & `libsmdev-20240505/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_936.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_10.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_roman.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf7_stream.h` & `libsmdev-20240505/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_3.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_thai.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_farsi.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_ukrainian.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_inuit.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_932.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_874.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_5.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_10.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_definitions.h` & `libsmdev-20240505/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libsmdev-20240309/libuna/libuna_url_stream.h` & `libsmdev-20240505/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_icelandic.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_koi8_u.h` & `libsmdev-20240505/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf16_stream.c` & `libsmdev-20240505/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1253.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_4.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_greek.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_libcerror.h` & `libsmdev-20240505/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_centraleurroman.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1254.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_13.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_7.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1255.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_unicode_character.h` & `libsmdev-20240505/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_8.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_13.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_949.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_cyrillic.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_celtic.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_support.h` & `libsmdev-20240505/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_4.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_949.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf16_stream.h` & `libsmdev-20240505/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_symbol.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_roman.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1257.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1254.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_950.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_extern.h` & `libsmdev-20240505/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1256.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_types.h` & `libsmdev-20240505/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base32_stream.h` & `libsmdev-20240505/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1253.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_16.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf8_stream.c` & `libsmdev-20240505/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1250.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_2.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_support.c` & `libsmdev-20240505/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_koi8_r.c` & `libsmdev-20240505/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_5.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf16_string.h` & `libsmdev-20240505/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf32_string.c` & `libsmdev-20240505/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_icelandic.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1256.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf32_string.h` & `libsmdev-20240505/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_romanian.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_8.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_koi8_r.h` & `libsmdev-20240505/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_cyrillic.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_arabic.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_croatian.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_9.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_greek.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1258.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_7.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/Makefile.in` & `libsmdev-20240505/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -607,16 +607,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -682,15 +682,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -952,24 +953,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1115,17 +1181,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_3.c` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1250.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_scsu.c` & `libsmdev-20240505/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1252.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_turkish.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_ukrainian.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_russian.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1258.c` & `libsmdev-20240505/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_celtic.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_byte_stream.c` & `libsmdev-20240505/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_gaelic.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_utf32_stream.h` & `libsmdev-20240505/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_symbol.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1257.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_inuit.h` & `libsmdev-20240505/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_mac_farsi.c` & `libsmdev-20240505/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_950.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_url_stream.c` & `libsmdev-20240505/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1251.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_windows_1252.h` & `libsmdev-20240505/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_codepage_iso_8859_14.h` & `libsmdev-20240505/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base16_stream.h` & `libsmdev-20240505/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libuna/libuna_base32_stream.c` & `libsmdev-20240505/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/Makefile.in` & `libsmdev-20240505/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -544,16 +544,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libsmdev.pc \
+	libsmdev.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libsmdev.pc
 
 all: all-recursive
 
@@ -970,23 +977,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1090,22 +1100,10 @@
 	(cd $(srcdir)/libclocale && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcnotify && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libuna && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcfile && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libsmdev && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libsmdev.pc
-	-rm -f libsmdev.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/smdevtools/smdevtools_signal.h` & `libsmdev-20240505/smdevtools/smdevtools_signal.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libcerror.h` & `libsmdev-20240505/smdevtools/smdevtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/info_handle.h` & `libsmdev-20240505/smdevtools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libclocale.h` & `libsmdev-20240505/smdevtools/smdevtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libsmdev.h` & `libsmdev-20240505/smdevtools/smdevtools_libsmdev.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libbfio.h` & `libsmdev-20240505/smdevtools/smdevtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/byte_size_string.c` & `libsmdev-20240505/smdevtools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_signal.c` & `libsmdev-20240505/smdevtools/smdevtools_signal.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/Makefile.am` & `libsmdev-20240505/smdevtools/Makefile.am`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBSMDEV_DLL_IMPORT@
@@ -33,17 +33,15 @@
 smdevinfo_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsmdev/libsmdev.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on smdevinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smdevinfo_SOURCES)
```

### Comparing `libsmdev-20240309/smdevtools/smdevtools_unused.h` & `libsmdev-20240505/smdevtools/smdevtools_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevinfo.c` & `libsmdev-20240505/smdevtools/smdevinfo.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/info_handle.c` & `libsmdev-20240505/smdevtools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_getopt.h` & `libsmdev-20240505/smdevtools/smdevtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_i18n.h` & `libsmdev-20240505/smdevtools/smdevtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_output.c` & `libsmdev-20240505/smdevtools/smdevtools_output.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_output.h` & `libsmdev-20240505/smdevtools/smdevtools_output.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libcnotify.h` & `libsmdev-20240505/smdevtools/smdevtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_libuna.h` & `libsmdev-20240505/smdevtools/smdevtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/Makefile.in` & `libsmdev-20240505/smdevtools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -427,16 +427,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBSMDEV_DLL_IMPORT@
@@ -461,15 +461,16 @@
 smdevinfo_LDADD = \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsmdev/libsmdev.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -716,23 +717,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/smdevinfo.Po
+	-rm -f ./$(DEPDIR)/smdevtools_getopt.Po
+	-rm -f ./$(DEPDIR)/smdevtools_output.Po
+	-rm -f ./$(DEPDIR)/smdevtools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -821,17 +830,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on smdevinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(smdevinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsmdev-20240309/smdevtools/byte_size_string.h` & `libsmdev-20240505/smdevtools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/smdevtools/smdevtools_getopt.c` & `libsmdev-20240505/smdevtools/smdevtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_definitions.h` & `libsmdev-20240505/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libsmdev-20240309/libcnotify/libcnotify_extern.h` & `libsmdev-20240505/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_support.c` & `libsmdev-20240505/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_stream.h` & `libsmdev-20240505/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/Makefile.am` & `libsmdev-20240505/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libsmdev-20240309/libcnotify/libcnotify_unused.h` & `libsmdev-20240505/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_verbose.h` & `libsmdev-20240505/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_print.h` & `libsmdev-20240505/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_stream.c` & `libsmdev-20240505/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_support.h` & `libsmdev-20240505/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_verbose.c` & `libsmdev-20240505/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/Makefile.in` & `libsmdev-20240505/libcnotify/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -431,30 +431,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -657,24 +658,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -761,17 +768,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/libcnotify/libcnotify_libcerror.h` & `libsmdev-20240505/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcnotify/libcnotify_print.c` & `libsmdev-20240505/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_system.c` & `libsmdev-20240505/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_error.c` & `libsmdev-20240505/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_extern.h` & `libsmdev-20240505/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/Makefile.am` & `libsmdev-20240505/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libsmdev-20240309/libcerror/libcerror_types.h` & `libsmdev-20240505/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_support.h` & `libsmdev-20240505/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_error.h` & `libsmdev-20240505/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_system.h` & `libsmdev-20240505/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_definitions.h` & `libsmdev-20240505/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libsmdev-20240309/libcerror/libcerror_support.c` & `libsmdev-20240505/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/libcerror_unused.h` & `libsmdev-20240505/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/libcerror/Makefile.in` & `libsmdev-20240505/libcerror/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -428,28 +428,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -651,24 +652,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -754,17 +760,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsmdev-20240309/aclocal.m4` & `libsmdev-20240505/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libsmdev-20240309/configure.ac` & `libsmdev-20240505/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libsmdev],
- [20240309],
+ [20240505],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libsmdev.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

