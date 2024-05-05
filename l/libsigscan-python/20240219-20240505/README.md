# Comparing `tmp/libsigscan-python-20240219.tar.gz` & `tmp/libsigscan-python-20240505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsigscan-python-20240219.tar", last modified: Mon Feb 19 19:13:52 2024, max compression
+gzip compressed data, was "libsigscan-python-20240505.tar", last modified: Sun May  5 08:27:57 2024, max compression
```

## Comparing `libsigscan-python-20240219.tar` & `libsigscan-python-20240505.tar`

### file list

```diff
@@ -1,694 +1,694 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2384 2024-02-19 19:03:51.000000 libsigscan-20240219/libsigscan.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-19 16:18:53.000000 libsigscan-20240219/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-19 19:03:42.000000 libsigscan-20240219/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 16:18:53.000000 libsigscan-20240219/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-19 19:03:43.000000 libsigscan-20240219/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-19 19:03:39.000000 libsigscan-20240219/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-19 19:03:39.000000 libsigscan-20240219/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-19 19:03:39.000000 libsigscan-20240219/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-19 19:03:39.000000 libsigscan-20240219/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-19 19:03:39.000000 libsigscan-20240219/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:05.000000 libsigscan-20240219/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:14:04.000000 libsigscan-20240219/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      504 2024-02-19 16:18:53.000000 libsigscan-20240219/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10431 2024-02-19 19:03:51.000000 libsigscan-20240219/include/libsigscan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25315 2024-02-19 19:03:42.000000 libsigscan-20240219/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/include/libsigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1970 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1968 2024-02-19 19:03:51.000000 libsigscan-20240219/include/libsigscan/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5048 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4917 2024-02-19 19:03:51.000000 libsigscan-20240219/include/libsigscan/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-02-19 16:20:08.000000 libsigscan-20240219/include/libsigscan/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-19 19:03:51.000000 libsigscan-20240219/include/libsigscan/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10431 2024-02-19 16:18:53.000000 libsigscan-20240219/include/libsigscan.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-19 16:18:53.000000 libsigscan-20240219/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-19 16:18:53.000000 libsigscan-20240219/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-19 16:18:53.000000 libsigscan-20240219/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-19 16:18:53.000000 libsigscan-20240219/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-19 16:18:53.000000 libsigscan-20240219/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-19 16:18:53.000000 libsigscan-20240219/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-19 16:18:53.000000 libsigscan-20240219/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-19 16:18:53.000000 libsigscan-20240219/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-19 16:18:53.000000 libsigscan-20240219/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-02-19 19:03:51.000000 libsigscan-20240219/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14666 2024-02-19 19:03:42.000000 libsigscan-20240219/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15551 2024-02-19 19:03:51.000000 libsigscan-20240219/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-19 16:18:53.000000 libsigscan-20240219/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-19 16:18:53.000000 libsigscan-20240219/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-19 16:18:53.000000 libsigscan-20240219/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22284 2024-02-19 19:03:42.000000 libsigscan-20240219/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27287 2024-02-19 19:03:42.000000 libsigscan-20240219/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-19 19:03:28.000000 libsigscan-20240219/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2097 2023-12-03 09:13:56.000000 libsigscan-20240219/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30746 2024-02-19 19:03:42.000000 libsigscan-20240219/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-19 19:03:22.000000 libsigscan-20240219/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:13:56.000000 libsigscan-20240219/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-19 19:03:42.000000 libsigscan-20240219/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-02-19 16:18:54.000000 libsigscan-20240219/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/libsigscan-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2132 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       55 2024-02-19 16:20:08.000000 libsigscan-20240219/dpkg/libsigscan-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      785 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-02-19 19:03:51.000000 libsigscan-20240219/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/libsigscan-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-19 16:18:53.000000 libsigscan-20240219/dpkg/libsigscan.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      492 2024-02-19 19:03:51.000000 libsigscan-20240219/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-19 16:18:53.000000 libsigscan-20240219/COPYING.LESSER
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3020 2024-02-19 16:20:13.000000 libsigscan-20240219/libsigscan.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1521655 2024-02-19 19:03:41.000000 libsigscan-20240219/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-19 19:03:42.000000 libsigscan-20240219/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-19 19:03:42.000000 libsigscan-20240219/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_signatures_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5579 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_signatures_list/sigscan_test_signatures_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_identifier/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5649 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_identifier/sigscan_test_identifier.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_signature_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5664 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_signature_table/sigscan_test_signature_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_offsets_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_offsets_list/sigscan_test_offsets_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_pattern_weights/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5664 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_pattern_weights/sigscan_test_pattern_weights.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_result/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5567 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_result/sigscan_test_scan_result.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27621 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/libsigscan.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_tree_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5576 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_tree_node/sigscan_test_scan_tree_node.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1725 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_object/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5567 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_object/sigscan_test_scan_object.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_signature_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5579 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_signature_group/sigscan_test_signature_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scanner/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_scanner/sigscan_test_scanner.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_byte_value_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5667 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_byte_value_group/sigscan_test_byte_value_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5386 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_notify/sigscan_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5297 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_error/sigscan_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_skip_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5564 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_skip_table/sigscan_test_skip_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6558 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan/sigscan.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/pysigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6845 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/pysigscan/pysigscan.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_state/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5649 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_state/sigscan_test_scan_state.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5646 2024-02-19 16:19:49.000000 libsigscan-20240219/msvscpp/sigscan_test_scan_tree/sigscan_test_scan_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_weight_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_weight_group/sigscan_test_weight_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20977 2024-02-19 19:03:43.000000 libsigscan-20240219/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_offset_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_offset_group/sigscan_test_offset_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/libsigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/libsigscan/libsigscan.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_signature/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_signature/sigscan_test_signature.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/msvscpp/sigscan_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5389 2024-02-19 16:19:09.000000 libsigscan-20240219/msvscpp/sigscan_test_support/sigscan_test_support.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      572 2024-02-19 16:18:53.000000 libsigscan-20240219/libsigscan.pc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-02-19 16:18:53.000000 libsigscan-20240219/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28051 2024-02-19 19:03:42.000000 libsigscan-20240219/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-19 19:03:27.000000 libsigscan-20240219/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      385 2024-02-19 16:18:53.000000 libsigscan-20240219/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-19 19:03:42.000000 libsigscan-20240219/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29735 2024-02-19 19:03:42.000000 libsigscan-20240219/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-19 19:03:24.000000 libsigscan-20240219/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-19 16:18:53.000000 libsigscan-20240219/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      493 2024-02-19 16:18:53.000000 libsigscan-20240219/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-19 19:03:42.000000 libsigscan-20240219/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:14:07.000000 libsigscan-20240219/etc/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      966 2023-12-03 09:14:07.000000 libsigscan-20240219/etc/sigscan.conf
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-19 16:18:53.000000 libsigscan-20240219/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-02-19 16:20:08.000000 libsigscan-20240219/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:13:56.000000 libsigscan-20240219/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2024-02-19 19:03:43.000000 libsigscan-20240219/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-19 19:03:33.000000 libsigscan-20240219/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-19 19:03:43.000000 libsigscan-20240219/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27329 2024-02-19 19:03:43.000000 libsigscan-20240219/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-19 19:03:30.000000 libsigscan-20240219/libcpath/libcpath_path.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/pysigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8912 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34058 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4194 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28617 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scanner.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2509 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scan_state.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9537 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_scan_results.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2533 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_scan_results.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13031 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scan_state.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2023-12-03 09:14:05.000000 libsigscan-20240219/pysigscan/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8634 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scan_result.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6925 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_signature_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6037 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scan_result.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_libsigscan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2902 2024-02-19 16:20:08.000000 libsigscan-20240219/pysigscan/pysigscan_scanner.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43837 2024-02-19 19:03:43.000000 libsigscan-20240219/pysigscan/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_signature_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-02-19 16:18:54.000000 libsigscan-20240219/pysigscan/pysigscan_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 09:13:56.000000 libsigscan-20240219/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-02-19 16:18:54.000000 libsigscan-20240219/manuals/sigscan.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      158 2023-12-03 09:14:05.000000 libsigscan-20240219/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5301 2024-02-19 16:20:08.000000 libsigscan-20240219/manuals/libsigscan.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24254 2024-02-19 19:03:43.000000 libsigscan-20240219/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21185 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_signature_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4664 2024-02-19 16:20:08.000000 libsigscan-20240219/tests/pysigscan_test_scanner.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23984 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_signature.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4308 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19045 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_skip_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15169 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_scan_result.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      715 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/test_pysigscan_scanner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14926 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_weight_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_offsets_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7986 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5462 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_signatures_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17982 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_offset_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17096 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37686 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_scan_state.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29802 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_scan_tree.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libsigscan.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4078 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_scan_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58738 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_scanner.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4417 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27625 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_pattern_weights.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24526 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_byte_value_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14593 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_scan_object.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/pysigscan_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_error.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3428 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/test_sigscan.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25190 2024-02-19 16:19:49.000000 libsigscan-20240219/tests/sigscan_test_signature_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64606 2024-02-19 19:03:43.000000 libsigscan-20240219/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15754 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_functions.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4286 2024-02-19 16:20:08.000000 libsigscan-20240219/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-02-19 16:18:54.000000 libsigscan-20240219/tests/sigscan_test_memory.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-02-19 16:18:54.000000 libsigscan-20240219/ossfuzz/scanner_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      526 2023-12-03 09:14:06.000000 libsigscan-20240219/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-02-19 16:18:54.000000 libsigscan-20240219/ossfuzz/ossfuzz_libsigscan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28628 2024-02-19 19:03:43.000000 libsigscan-20240219/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-19 19:03:39.000000 libsigscan-20240219/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28109 2024-02-19 19:03:43.000000 libsigscan-20240219/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-19 19:03:31.000000 libsigscan-20240219/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:05.000000 libsigscan-20240219/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:05.000000 libsigscan-20240219/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:05.000000 libsigscan-20240219/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:05.000000 libsigscan-20240219/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:05.000000 libsigscan-20240219/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:05.000000 libsigscan-20240219/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:05.000000 libsigscan-20240219/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:05.000000 libsigscan-20240219/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:05.000000 libsigscan-20240219/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-02-19 19:03:51.000000 libsigscan-20240219/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:05.000000 libsigscan-20240219/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:05.000000 libsigscan-20240219/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50853 2024-02-19 19:03:43.000000 libsigscan-20240219/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-19 19:03:35.000000 libsigscan-20240219/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39140 2024-02-19 19:03:42.000000 libsigscan-20240219/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27163 2024-02-19 19:03:42.000000 libsigscan-20240219/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-19 19:03:29.000000 libsigscan-20240219/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:50.000000 libsigscan-20240219/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-19 19:03:25.000000 libsigscan-20240219/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26676 2024-02-19 19:03:42.000000 libsigscan-20240219/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/libsigscan/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_state.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10945 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_skip_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33614 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scanner.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12964 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_byte_value_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41178 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_state.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65475 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4337 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2355 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_result.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21332 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signature_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17552 2024-02-19 18:57:45.000000 libsigscan-20240219/libsigscan/libsigscan_scan_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3008 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_byte_value_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3233 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_pattern_weights.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2057 2024-02-19 18:33:36.000000 libsigscan-20240219/libsigscan/libsigscan_scan_object.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2604 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signature_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1591 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3952 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scanner.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3156 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2023-12-03 09:14:03.000000 libsigscan-20240219/libsigscan/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3489 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signature_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6902 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_result.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2778 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7557 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8941 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signature_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6616 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_weight_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2892 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_scan_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3590 2024-02-19 18:06:42.000000 libsigscan-20240219/libsigscan/libsigscan_signature.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1350 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signatures_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9360 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_offset_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3384 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_signatures_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_weight_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3154 2024-02-19 19:03:51.000000 libsigscan-20240219/libsigscan/libsigscan_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21454 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_pattern_weights.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20161 2024-02-19 18:11:26.000000 libsigscan-20240219/libsigscan/libsigscan_signature.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-02-19 18:34:28.000000 libsigscan-20240219/libsigscan/libsigscan_scan_object.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-02-19 19:03:51.000000 libsigscan-20240219/libsigscan/libsigscan.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2763 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1767 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_offsets_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2409 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_offset_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6786 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_offsets_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34888 2024-02-19 19:03:43.000000 libsigscan-20240219/libsigscan/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_skip_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2493 2024-02-19 16:18:54.000000 libsigscan-20240219/libsigscan/libsigscan_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56677 2024-02-19 19:03:40.000000 libsigscan-20240219/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-19 19:13:51.000000 libsigscan-20240219/sigscantools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3431 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26536 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/scan_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-12-03 09:14:05.000000 libsigscan-20240219/sigscantools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1754 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2473 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/scan_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6619 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libsigscan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28764 2024-02-19 19:03:43.000000 libsigscan-20240219/sigscantools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-02-19 16:18:54.000000 libsigscan-20240219/sigscantools/sigscantools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6602 2024-02-19 16:18:53.000000 libsigscan-20240219/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      424 2024-02-19 19:13:52.357641 libsigscan-20240219/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2384 2024-05-05 08:13:23.000000 libsigscan-20240505/libsigscan.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-05 07:10:04.000000 libsigscan-20240505/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-05 08:13:07.000000 libsigscan-20240505/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 07:10:04.000000 libsigscan-20240505/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-05 08:13:08.000000 libsigscan-20240505/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:53.000000 libsigscan-20240505/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:14:04.000000 libsigscan-20240505/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-03-15 03:17:09.000000 libsigscan-20240505/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-05 08:13:02.000000 libsigscan-20240505/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-05 08:13:02.000000 libsigscan-20240505/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-05 08:13:02.000000 libsigscan-20240505/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-05 08:13:02.000000 libsigscan-20240505/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-05 08:13:02.000000 libsigscan-20240505/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:14:05.000000 libsigscan-20240505/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-05 07:10:09.000000 libsigscan-20240505/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:14:04.000000 libsigscan-20240505/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-03-15 03:17:09.000000 libsigscan-20240505/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:53.000000 libsigscan-20240505/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      455 2024-05-05 07:30:01.000000 libsigscan-20240505/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10431 2024-05-05 08:13:23.000000 libsigscan-20240505/include/libsigscan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25295 2024-05-05 08:13:07.000000 libsigscan-20240505/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:53.000000 libsigscan-20240505/include/libsigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1970 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1968 2024-05-05 08:13:23.000000 libsigscan-20240505/include/libsigscan/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5048 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4917 2024-05-05 08:13:23.000000 libsigscan-20240505/include/libsigscan/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1467 2024-05-05 07:29:11.000000 libsigscan-20240505/include/libsigscan/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6894 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-05-05 08:13:23.000000 libsigscan-20240505/include/libsigscan/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10431 2024-05-05 07:10:06.000000 libsigscan-20240505/include/libsigscan.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-05 07:10:06.000000 libsigscan-20240505/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-05 07:10:06.000000 libsigscan-20240505/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-05 07:10:06.000000 libsigscan-20240505/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-05 07:10:06.000000 libsigscan-20240505/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-05 07:10:06.000000 libsigscan-20240505/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-05 07:10:06.000000 libsigscan-20240505/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-05 07:10:06.000000 libsigscan-20240505/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-05 07:30:01.000000 libsigscan-20240505/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-05 07:10:06.000000 libsigscan-20240505/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7376 2024-05-05 08:13:23.000000 libsigscan-20240505/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14666 2024-05-05 08:13:07.000000 libsigscan-20240505/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15551 2024-05-05 08:13:23.000000 libsigscan-20240505/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-05 07:10:06.000000 libsigscan-20240505/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-05 07:10:06.000000 libsigscan-20240505/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-05 07:10:06.000000 libsigscan-20240505/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22291 2024-05-05 08:13:07.000000 libsigscan-20240505/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27489 2024-05-05 08:13:08.000000 libsigscan-20240505/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-05 08:12:41.000000 libsigscan-20240505/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2024-05-05 07:32:15.000000 libsigscan-20240505/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:55.000000 libsigscan-20240505/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31341 2024-05-05 08:13:07.000000 libsigscan-20240505/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-05 08:12:33.000000 libsigscan-20240505/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:13:56.000000 libsigscan-20240505/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-05 08:13:07.000000 libsigscan-20240505/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:53.000000 libsigscan-20240505/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1030 2024-05-05 07:10:09.000000 libsigscan-20240505/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/libsigscan-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:53.000000 libsigscan-20240505/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2132 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       55 2024-05-05 07:28:45.000000 libsigscan-20240505/dpkg/libsigscan-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      785 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      123 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      142 2024-05-05 08:13:23.000000 libsigscan-20240505/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/libsigscan-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-05 07:10:04.000000 libsigscan-20240505/dpkg/libsigscan.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      492 2024-05-05 08:13:23.000000 libsigscan-20240505/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-05 07:10:04.000000 libsigscan-20240505/COPYING.LESSER
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3020 2024-05-05 07:28:45.000000 libsigscan-20240505/libsigscan.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1523645 2024-05-05 08:13:06.000000 libsigscan-20240505/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-05 08:13:07.000000 libsigscan-20240505/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-05 08:13:07.000000 libsigscan-20240505/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_signatures_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5579 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_signatures_list/sigscan_test_signatures_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_identifier/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5649 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_identifier/sigscan_test_identifier.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_signature_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5664 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_signature_table/sigscan_test_signature_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_offsets_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_offsets_list/sigscan_test_offsets_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_pattern_weights/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5664 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_pattern_weights/sigscan_test_pattern_weights.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_result/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5567 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_result/sigscan_test_scan_result.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27621 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/libsigscan.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_tree_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5576 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_tree_node/sigscan_test_scan_tree_node.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-05 07:31:42.000000 libsigscan-20240505/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_object/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5567 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_object/sigscan_test_scan_object.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_signature_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5579 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_signature_group/sigscan_test_signature_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scanner/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_scanner/sigscan_test_scanner.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_byte_value_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5667 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_byte_value_group/sigscan_test_byte_value_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5386 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_notify/sigscan_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5297 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_error/sigscan_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_skip_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5564 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_skip_table/sigscan_test_skip_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6558 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan/sigscan.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/pysigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6845 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/pysigscan/pysigscan.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_state/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5649 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_state/sigscan_test_scan_state.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5646 2024-05-05 07:27:55.000000 libsigscan-20240505/msvscpp/sigscan_test_scan_tree/sigscan_test_scan_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_weight_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_weight_group/sigscan_test_weight_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20977 2024-05-05 08:13:08.000000 libsigscan-20240505/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_offset_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5570 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_offset_group/sigscan_test_offset_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/libsigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/libsigscan/libsigscan.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_signature/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5561 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_signature/sigscan_test_signature.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/msvscpp/sigscan_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5389 2024-05-05 07:10:42.000000 libsigscan-20240505/msvscpp/sigscan_test_support/sigscan_test_support.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      572 2024-05-05 07:10:04.000000 libsigscan-20240505/libsigscan.pc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       94 2024-05-05 07:10:06.000000 libsigscan-20240505/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:55.000000 libsigscan-20240505/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28322 2024-05-05 08:13:08.000000 libsigscan-20240505/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-05 08:12:40.000000 libsigscan-20240505/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      385 2024-05-05 07:10:04.000000 libsigscan-20240505/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-05 08:13:07.000000 libsigscan-20240505/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30235 2024-05-05 08:13:07.000000 libsigscan-20240505/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 08:12:34.000000 libsigscan-20240505/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-05 07:10:04.000000 libsigscan-20240505/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      493 2024-05-05 07:10:04.000000 libsigscan-20240505/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-05 08:13:07.000000 libsigscan-20240505/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-03-09 08:08:14.000000 libsigscan-20240505/etc/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      966 2023-12-03 09:14:07.000000 libsigscan-20240505/etc/sigscan.conf
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-05 07:10:04.000000 libsigscan-20240505/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-05-05 07:28:25.000000 libsigscan-20240505/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:13:56.000000 libsigscan-20240505/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30674 2024-05-05 08:13:08.000000 libsigscan-20240505/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-05 08:12:52.000000 libsigscan-20240505/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-05 08:13:08.000000 libsigscan-20240505/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:55.000000 libsigscan-20240505/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27520 2024-05-05 08:13:08.000000 libsigscan-20240505/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-05 08:12:45.000000 libsigscan-20240505/libcpath/libcpath_path.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:56.000000 libsigscan-20240505/pysigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8912 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9586 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34058 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4194 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28617 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scanner.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2509 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scan_state.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9537 2024-05-05 07:10:08.000000 libsigscan-20240505/pysigscan/pysigscan_scan_results.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2533 2024-05-05 07:10:08.000000 libsigscan-20240505/pysigscan/pysigscan_scan_results.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13031 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scan_state.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-05 07:30:58.000000 libsigscan-20240505/pysigscan/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8634 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scan_result.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1331 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6925 2024-05-05 07:10:08.000000 libsigscan-20240505/pysigscan/pysigscan_signature_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 07:10:08.000000 libsigscan-20240505/pysigscan/pysigscan_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6037 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2103 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scan_result.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_libsigscan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2902 2024-05-05 07:28:11.000000 libsigscan-20240505/pysigscan/pysigscan_scanner.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44382 2024-05-05 08:13:08.000000 libsigscan-20240505/pysigscan/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-05-05 07:10:08.000000 libsigscan-20240505/pysigscan/pysigscan_signature_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-05-05 07:10:07.000000 libsigscan-20240505/pysigscan/pysigscan_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1320 2023-12-03 09:13:56.000000 libsigscan-20240505/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:56.000000 libsigscan-20240505/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2024-05-05 07:10:09.000000 libsigscan-20240505/manuals/sigscan.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      129 2024-05-05 07:30:49.000000 libsigscan-20240505/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5301 2024-05-05 07:29:22.000000 libsigscan-20240505/manuals/libsigscan.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24254 2024-05-05 08:13:08.000000 libsigscan-20240505/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21185 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_signature_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4664 2024-05-05 07:28:11.000000 libsigscan-20240505/tests/pysigscan_test_scanner.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23984 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_signature.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4308 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19045 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_skip_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15169 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_scan_result.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      715 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/test_pysigscan_scanner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1715 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14926 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_weight_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5968 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_offsets_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8003 2024-05-05 07:31:29.000000 libsigscan-20240505/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8644 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5462 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_signatures_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17982 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_offset_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17096 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37686 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_scan_state.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29802 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_scan_tree.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libsigscan.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4405 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3010 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_scan_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1724 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58738 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_scanner.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4417 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27625 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_pattern_weights.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24526 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_byte_value_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14593 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_scan_object.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/pysigscan_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3219 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_error.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3397 2024-05-05 08:03:00.000000 libsigscan-20240505/tests/test_sigscan.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25190 2024-05-05 07:27:56.000000 libsigscan-20240505/tests/sigscan_test_signature_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65746 2024-05-05 08:13:08.000000 libsigscan-20240505/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15754 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_functions.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4255 2024-05-05 07:29:50.000000 libsigscan-20240505/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4794 2024-05-05 07:10:08.000000 libsigscan-20240505/tests/sigscan_test_memory.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:57.000000 libsigscan-20240505/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-05-05 07:10:07.000000 libsigscan-20240505/ossfuzz/scanner_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      522 2024-05-05 07:30:41.000000 libsigscan-20240505/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      982 2024-05-05 07:10:07.000000 libsigscan-20240505/ossfuzz/ossfuzz_libsigscan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28692 2024-05-05 08:13:08.000000 libsigscan-20240505/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-05 08:13:02.000000 libsigscan-20240505/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28417 2024-05-05 08:13:08.000000 libsigscan-20240505/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-05 08:12:48.000000 libsigscan-20240505/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:56.000000 libsigscan-20240505/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:14:05.000000 libsigscan-20240505/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:14:05.000000 libsigscan-20240505/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:14:05.000000 libsigscan-20240505/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:14:05.000000 libsigscan-20240505/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:14:05.000000 libsigscan-20240505/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:14:05.000000 libsigscan-20240505/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:14:05.000000 libsigscan-20240505/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:14:05.000000 libsigscan-20240505/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:14:05.000000 libsigscan-20240505/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1856 2024-05-05 08:13:23.000000 libsigscan-20240505/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:14:05.000000 libsigscan-20240505/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:14:05.000000 libsigscan-20240505/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:55.000000 libsigscan-20240505/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54001 2024-05-05 08:13:08.000000 libsigscan-20240505/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-05 08:12:58.000000 libsigscan-20240505/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39022 2024-05-05 08:13:07.000000 libsigscan-20240505/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27358 2024-05-05 08:13:08.000000 libsigscan-20240505/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-05 08:12:43.000000 libsigscan-20240505/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:54.000000 libsigscan-20240505/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-05 08:12:36.000000 libsigscan-20240505/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26825 2024-05-05 08:13:08.000000 libsigscan-20240505/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:55.000000 libsigscan-20240505/libsigscan/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5503 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_state.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10945 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_skip_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33614 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scanner.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12964 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_byte_value_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41178 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_state.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65475 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4337 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2355 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_result.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21332 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17552 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1827 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3008 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_byte_value_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3233 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_pattern_weights.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2057 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_object.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2604 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1591 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1078 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3952 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scanner.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3156 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2473 2024-05-05 07:30:32.000000 libsigscan-20240505/libsigscan/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3489 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6902 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_result.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2778 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7557 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8941 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6616 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_weight_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2892 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3590 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1350 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signatures_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9360 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_offset_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3384 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signatures_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2273 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_weight_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3154 2024-05-05 08:13:23.000000 libsigscan-20240505/libsigscan/libsigscan_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21454 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_pattern_weights.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20161 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_signature.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_scan_object.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2938 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-05-05 08:13:23.000000 libsigscan-20240505/libsigscan/libsigscan.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2763 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1767 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_offsets_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2409 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_offset_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6786 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_offsets_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35880 2024-05-05 08:13:08.000000 libsigscan-20240505/libsigscan/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_skip_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2493 2024-05-05 07:10:07.000000 libsigscan-20240505/libsigscan/libsigscan_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56677 2024-05-05 08:13:04.000000 libsigscan-20240505/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-05 08:27:56.000000 libsigscan-20240505/sigscantools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5801 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1510 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3431 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26536 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/scan_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1226 2024-05-05 07:30:15.000000 libsigscan-20240505/sigscantools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4543 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1754 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1473 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2473 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/scan_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6619 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      997 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libsigscan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28985 2024-05-05 08:13:08.000000 libsigscan-20240505/sigscantools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-05-05 07:10:08.000000 libsigscan-20240505/sigscantools/sigscantools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6602 2024-05-05 07:10:04.000000 libsigscan-20240505/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      424 2024-05-05 08:27:57.947288 libsigscan-20240505/PKG-INFO
```

### Comparing `libsigscan-20240219/libsigscan.spec` & `libsigscan-20240505/libsigscan.spec`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libsigscan
-Version: 20240219
+Version: 20240505
 Release: 1
 Summary: Library for binary signature scanning
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libsigscan
           
@@ -91,10 +91,10 @@
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 %config %{_sysconfdir}/sigscan.conf
 
 %changelog
-* Mon Feb 19 2024 Joachim Metz <joachim.metz@gmail.com> 20240219-1
+* Sun May  5 2024 Joachim Metz <joachim.metz@gmail.com> 20240505-1
 - Auto-generated
```

### Comparing `libsigscan-20240219/COPYING` & `libsigscan-20240505/COPYING`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/install-sh` & `libsigscan-20240505/install-sh`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/depcomp` & `libsigscan-20240505/depcomp`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libcfile.m4` & `libsigscan-20240505/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
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

### Comparing `libsigscan-20240219/m4/tests.m4` & `libsigscan-20240505/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libcpath.m4` & `libsigscan-20240505/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libsigscan-20240219/m4/lib-prefix.m4` & `libsigscan-20240505/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/progtest.m4` & `libsigscan-20240505/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libuna.m4` & `libsigscan-20240505/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
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

### Comparing `libsigscan-20240219/m4/gettext.m4` & `libsigscan-20240505/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/lib-ld.m4` & `libsigscan-20240505/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libclocale.m4` & `libsigscan-20240505/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
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

### Comparing `libsigscan-20240219/m4/libcdata.m4` & `libsigscan-20240505/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
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

### Comparing `libsigscan-20240219/m4/libcsplit.m4` & `libsigscan-20240505/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libsigscan-20240219/m4/common.m4` & `libsigscan-20240505/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libsigscan-20240219/m4/libcthreads.m4` & `libsigscan-20240505/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
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

### Comparing `libsigscan-20240219/m4/ltversion.m4` & `libsigscan-20240505/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/ltsugar.m4` & `libsigscan-20240505/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/host-cpu-c-abi.m4` & `libsigscan-20240505/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libtool.m4` & `libsigscan-20240505/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/po.m4` & `libsigscan-20240505/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/libcerror.m4` & `libsigscan-20240505/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
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

### Comparing `libsigscan-20240219/m4/libcnotify.m4` & `libsigscan-20240505/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
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

### Comparing `libsigscan-20240219/m4/libbfio.m4` & `libsigscan-20240505/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libsigscan-20240219/m4/intlmacosx.m4` & `libsigscan-20240505/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/lt~obsolete.m4` & `libsigscan-20240505/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/lib-link.m4` & `libsigscan-20240505/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/iconv.m4` & `libsigscan-20240505/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/ltoptions.m4` & `libsigscan-20240505/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/nls.m4` & `libsigscan-20240505/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/python.m4` & `libsigscan-20240505/m4/python.m4`

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

### Comparing `libsigscan-20240219/m4/types.m4` & `libsigscan-20240505/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/m4/pthread.m4` & `libsigscan-20240505/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libsigscan-20240219/include/libsigscan.h` & `libsigscan-20240505/include/libsigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/Makefile.in` & `libsigscan-20240505/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,20 @@
 
 EXTRA_DIST = \
 	libsigscan.h.in \
 	libsigscan/definitions.h.in \
 	libsigscan/features.h.in \
 	libsigscan/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsigscan.h \
+	libsigscan/definitions.h \
+	libsigscan/features.h \
+	libsigscan/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -674,23 +679,25 @@
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
@@ -772,17 +779,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsigscan.h
-	-rm -f libsigscan/definitions.h
-	-rm -f libsigscan/features.h
-	-rm -f libsigscan/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsigscan-20240219/include/libsigscan/definitions.h.in` & `libsigscan-20240505/include/libsigscan/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/definitions.h` & `libsigscan-20240505/include/libsigscan/definitions.h`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBSIGSCAN_DEFINITIONS_H )
 #define _LIBSIGSCAN_DEFINITIONS_H
 
 #include <libsigscan/types.h>
 
-#define LIBSIGSCAN_VERSION					20240219
+#define LIBSIGSCAN_VERSION					20240505
 
 /* The version string
  */
-#define LIBSIGSCAN_VERSION_STRING				"20240219"
+#define LIBSIGSCAN_VERSION_STRING				"20240505"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBSIGSCAN_ACCESS_FLAGS
```

### Comparing `libsigscan-20240219/include/libsigscan/types.h.in` & `libsigscan-20240505/include/libsigscan/types.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/types.h` & `libsigscan-20240505/include/libsigscan/types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/features.h.in` & `libsigscan-20240505/include/libsigscan/features.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/error.h` & `libsigscan-20240505/include/libsigscan/error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/extern.h` & `libsigscan-20240505/include/libsigscan/extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/features.h` & `libsigscan-20240505/include/libsigscan/features.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan/codepage.h` & `libsigscan-20240505/include/libsigscan/codepage.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/include/libsigscan.h.in` & `libsigscan-20240505/include/libsigscan.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/config_borlandc.h` & `libsigscan-20240505/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/file_stream.h` & `libsigscan-20240505/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/memory.h` & `libsigscan-20240505/common/memory.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/byte_stream.h` & `libsigscan-20240505/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/common.h` & `libsigscan-20240505/common/common.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/config_winapi.h` & `libsigscan-20240505/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/system_string.h` & `libsigscan-20240505/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/types.h.in` & `libsigscan-20240505/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/types.h` & `libsigscan-20240505/common/types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/config.h.in` & `libsigscan-20240505/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/config.h` & `libsigscan-20240505/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -481,24 +481,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libsigscan"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libsigscan 20240219"
+#define PACKAGE_STRING "libsigscan 20240505"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libsigscan"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240219"
+#define PACKAGE_VERSION "20240505"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -516,15 +516,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240219"
+#define VERSION "20240505"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libsigscan-20240219/common/wide_string.h` & `libsigscan-20240505/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/narrow_string.h` & `libsigscan-20240505/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/config_msc.h` & `libsigscan-20240505/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/common/Makefile.in` & `libsigscan-20240505/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -422,15 +422,17 @@
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
@@ -438,15 +440,18 @@
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
@@ -614,23 +619,25 @@
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
@@ -710,15 +717,10 @@
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

### Comparing `libsigscan-20240219/libclocale/libclocale_wide_string.c` & `libsigscan-20240505/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_support.h` & `libsigscan-20240505/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/Makefile.am` & `libsigscan-20240505/libclocale/Makefile.am`

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

### Comparing `libsigscan-20240219/libclocale/libclocale_definitions.h` & `libsigscan-20240505/libclocale/libclocale_definitions.h`

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

### Comparing `libsigscan-20240219/libclocale/libclocale_unused.h` & `libsigscan-20240505/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_libcerror.h` & `libsigscan-20240505/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_locale.h` & `libsigscan-20240505/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_support.c` & `libsigscan-20240505/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_codepage.c` & `libsigscan-20240505/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_locale.c` & `libsigscan-20240505/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/Makefile.in` & `libsigscan-20240505/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,30 +468,31 @@
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
@@ -694,24 +695,30 @@
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
 
@@ -798,17 +805,14 @@
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

### Comparing `libsigscan-20240219/libclocale/libclocale_extern.h` & `libsigscan-20240505/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_wide_string.h` & `libsigscan-20240505/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libclocale/libclocale_codepage.h` & `libsigscan-20240505/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libbfio/libbfio_file_range.h` & `libsigscan-20240505/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_range_io_handle.c` & `libsigscan-20240505/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_support.c` & `libsigscan-20240505/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libcpath.h` & `libsigscan-20240505/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_error.h` & `libsigscan-20240505/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libclocale.h` & `libsigscan-20240505/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_error.c` & `libsigscan-20240505/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libuna.h` & `libsigscan-20240505/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_io_handle.h` & `libsigscan-20240505/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_pool.h` & `libsigscan-20240505/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_range.c` & `libsigscan-20240505/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_types.h` & `libsigscan-20240505/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_unused.h` & `libsigscan-20240505/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libcdata.h` & `libsigscan-20240505/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file.h` & `libsigscan-20240505/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/Makefile.am` & `libsigscan-20240505/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libcfile.h` & `libsigscan-20240505/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_definitions.h` & `libsigscan-20240505/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libsigscan-20240219/libbfio/libbfio_codepage.h` & `libsigscan-20240505/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_io_handle.c` & `libsigscan-20240505/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_support.h` & `libsigscan-20240505/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_memory_range.h` & `libsigscan-20240505/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_pool.c` & `libsigscan-20240505/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file_range_io_handle.h` & `libsigscan-20240505/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libcthreads.h` & `libsigscan-20240505/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_system_string.h` & `libsigscan-20240505/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_memory_range_io_handle.c` & `libsigscan-20240505/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_handle.c` & `libsigscan-20240505/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_file.c` & `libsigscan-20240505/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_handle.h` & `libsigscan-20240505/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_memory_range.c` & `libsigscan-20240505/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_pool.c` & `libsigscan-20240505/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_libcerror.h` & `libsigscan-20240505/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/Makefile.in` & `libsigscan-20240505/libbfio/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -488,16 +488,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -528,15 +528,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -747,24 +748,38 @@
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
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -833,14 +848,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -851,23 +868,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsigscan-20240219/libbfio/libbfio_system_string.c` & `libsigscan-20240505/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_memory_range_io_handle.h` & `libsigscan-20240505/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_extern.h` & `libsigscan-20240505/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/libbfio/libbfio_pool.h` & `libsigscan-20240505/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libsigscan-20240219/config.guess` & `libsigscan-20240505/config.guess`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/dpkg/copyright` & `libsigscan-20240505/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/dpkg/control` & `libsigscan-20240505/dpkg/control`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/dpkg/rules` & `libsigscan-20240505/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/COPYING.LESSER` & `libsigscan-20240505/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan.spec.in` & `libsigscan-20240505/libsigscan.spec.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/configure` & `libsigscan-20240505/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libsigscan 20240219.
+# Generated by GNU Autoconf 2.71 for libsigscan 20240505.
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
 PACKAGE_NAME='libsigscan'
 PACKAGE_TARNAME='libsigscan'
-PACKAGE_VERSION='20240219'
-PACKAGE_STRING='libsigscan 20240219'
+PACKAGE_VERSION='20240505'
+PACKAGE_STRING='libsigscan 20240505'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libsigscan.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1583,15 +1583,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libsigscan 20240219 to adapt to many kinds of systems.
+\`configure' configures libsigscan 20240505 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1654,15 +1654,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libsigscan 20240219:";;
+     short | recursive ) echo "Configuration of libsigscan 20240505:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1870,15 +1870,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libsigscan configure 20240219
+libsigscan configure 20240505
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2591,15 +2591,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libsigscan $as_me 20240219, which was
+It was created by libsigscan $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4080,15 +4080,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libsigscan'
- VERSION='20240219'
+ VERSION='20240505'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23675,15 +23675,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24174,15 +24174,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24324,15 +24325,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24426,15 +24427,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26066,15 +26067,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26128,47 +26129,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26202,15 +26208,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26244,15 +26250,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26287,15 +26293,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26329,15 +26335,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26371,15 +26377,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26413,15 +26419,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26455,15 +26461,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26498,15 +26504,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26540,15 +26546,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26582,15 +26588,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26624,15 +26630,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26666,15 +26672,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26709,15 +26715,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26751,15 +26757,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26793,15 +26799,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26835,15 +26841,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26877,15 +26883,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26920,67 +26926,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
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
 
@@ -27068,15 +27083,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30847,15 +30862,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30880,15 +30896,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -30958,15 +30974,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31513,15 +31529,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31677,15 +31694,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31755,15 +31772,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32213,15 +32230,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32276,15 +32294,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32354,15 +32372,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33077,15 +33095,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33110,15 +33129,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33188,15 +33207,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40398,15 +40417,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40431,15 +40451,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40509,15 +40529,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41698,15 +41718,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42020,15 +42041,15 @@
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
@@ -42098,15 +42119,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -42903,15 +42924,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43101,15 +43123,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43179,15 +43201,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45297,15 +45319,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45330,15 +45353,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45649,16 +45672,20 @@
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
 
@@ -46660,15 +46687,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libsigscan $as_me 20240219, which was
+This file was extended by libsigscan $as_me 20240505, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -46728,15 +46755,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libsigscan config.status 20240219
+libsigscan config.status 20240505
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libsigscan-20240219/compile` & `libsigscan-20240505/compile`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/missing` & `libsigscan-20240505/missing`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_signatures_list/sigscan_test_signatures_list.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_signatures_list/sigscan_test_signatures_list.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_identifier/sigscan_test_identifier.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_identifier/sigscan_test_identifier.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_signature_table/sigscan_test_signature_table.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_signature_table/sigscan_test_signature_table.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_offsets_list/sigscan_test_offsets_list.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_offsets_list/sigscan_test_offsets_list.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_pattern_weights/sigscan_test_pattern_weights.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_pattern_weights/sigscan_test_pattern_weights.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scan_result/sigscan_test_scan_result.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scan_result/sigscan_test_scan_result.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libclocale/libclocale.vcproj` & `libsigscan-20240505/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libsigscan.sln` & `libsigscan-20240505/msvscpp/libsigscan.sln`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scan_tree_node/sigscan_test_scan_tree_node.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scan_tree_node/sigscan_test_scan_tree_node.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/Makefile.am` & `libsigscan-20240505/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -33,13 +33,11 @@
 	sigscan_test_support/sigscan_test_support.vcproj \
 	sigscan_test_weight_group/sigscan_test_weight_group.vcproj \
 	libsigscan.sln
 
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

### Comparing `libsigscan-20240219/msvscpp/libbfio/libbfio.vcproj` & `libsigscan-20240505/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scan_object/sigscan_test_scan_object.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scan_object/sigscan_test_scan_object.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_signature_group/sigscan_test_signature_group.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_signature_group/sigscan_test_signature_group.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scanner/sigscan_test_scanner.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scanner/sigscan_test_scanner.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcfile/libcfile.vcproj` & `libsigscan-20240505/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_byte_value_group/sigscan_test_byte_value_group.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_byte_value_group/sigscan_test_byte_value_group.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcdata/libcdata.vcproj` & `libsigscan-20240505/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_notify/sigscan_test_notify.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_notify/sigscan_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_error/sigscan_test_error.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_error/sigscan_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcthreads/libcthreads.vcproj` & `libsigscan-20240505/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_skip_table/sigscan_test_skip_table.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_skip_table/sigscan_test_skip_table.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan/sigscan.vcproj` & `libsigscan-20240505/msvscpp/sigscan/sigscan.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcpath/libcpath.vcproj` & `libsigscan-20240505/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/pysigscan/pysigscan.vcproj` & `libsigscan-20240505/msvscpp/pysigscan/pysigscan.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scan_state/sigscan_test_scan_state.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scan_state/sigscan_test_scan_state.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_scan_tree/sigscan_test_scan_tree.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_scan_tree/sigscan_test_scan_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_weight_group/sigscan_test_weight_group.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_weight_group/sigscan_test_weight_group.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcsplit/libcsplit.vcproj` & `libsigscan-20240505/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libuna/libuna.vcproj` & `libsigscan-20240505/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/Makefile.in` & `libsigscan-20240505/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -443,15 +443,16 @@
 	sigscan_test_support/sigscan_test_support.vcproj \
 	sigscan_test_weight_group/sigscan_test_weight_group.vcproj \
 	libsigscan.sln
 
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
@@ -555,23 +556,25 @@
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
@@ -650,13 +653,10 @@
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

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_offset_group/sigscan_test_offset_group.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_offset_group/sigscan_test_offset_group.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcnotify/libcnotify.vcproj` & `libsigscan-20240505/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libcerror/libcerror.vcproj` & `libsigscan-20240505/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/libsigscan/libsigscan.vcproj` & `libsigscan-20240505/msvscpp/libsigscan/libsigscan.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_signature/sigscan_test_signature.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_signature/sigscan_test_signature.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/msvscpp/sigscan_test_support/sigscan_test_support.vcproj` & `libsigscan-20240505/msvscpp/sigscan_test_support/sigscan_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan.pc.in` & `libsigscan-20240505/libsigscan.pc.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_extern.h` & `libsigscan-20240505/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_support.h` & `libsigscan-20240505/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_unused.h` & `libsigscan-20240505/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_notify.h` & `libsigscan-20240505/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_support.c` & `libsigscan-20240505/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_types.h` & `libsigscan-20240505/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/Makefile.am` & `libsigscan-20240505/libcfile/Makefile.am`

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

### Comparing `libsigscan-20240219/libcfile/libcfile_notify.c` & `libsigscan-20240505/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_system_string.h` & `libsigscan-20240505/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_file.h` & `libsigscan-20240505/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_libcnotify.h` & `libsigscan-20240505/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_system_string.c` & `libsigscan-20240505/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_error.h` & `libsigscan-20240505/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_libcerror.h` & `libsigscan-20240505/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_file.c` & `libsigscan-20240505/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_libclocale.h` & `libsigscan-20240505/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_winapi.h` & `libsigscan-20240505/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/Makefile.in` & `libsigscan-20240505/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -470,16 +470,16 @@
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
@@ -494,15 +494,16 @@
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
@@ -707,24 +708,32 @@
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
 
@@ -813,17 +822,14 @@
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

### Comparing `libsigscan-20240219/libcfile/libcfile_error.c` & `libsigscan-20240505/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_libuna.h` & `libsigscan-20240505/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_winapi.c` & `libsigscan-20240505/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcfile/libcfile_definitions.h` & `libsigscan-20240505/libcfile/libcfile_definitions.h`

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

### Comparing `libsigscan-20240219/INSTALL` & `libsigscan-20240505/INSTALL`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_list_element.h` & `libsigscan-20240505/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_array.h` & `libsigscan-20240505/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_definitions.h` & `libsigscan-20240505/libcdata/libcdata_definitions.h`

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

### Comparing `libsigscan-20240219/libcdata/libcdata_libcerror.h` & `libsigscan-20240505/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_unused.h` & `libsigscan-20240505/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_btree.h` & `libsigscan-20240505/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_btree.c` & `libsigscan-20240505/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_support.c` & `libsigscan-20240505/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_list.c` & `libsigscan-20240505/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_extern.h` & `libsigscan-20240505/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_list.h` & `libsigscan-20240505/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_btree_values_list.h` & `libsigscan-20240505/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/Makefile.am` & `libsigscan-20240505/libcdata/Makefile.am`

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

### Comparing `libsigscan-20240219/libcdata/libcdata_btree_node.h` & `libsigscan-20240505/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_range_list_value.h` & `libsigscan-20240505/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_range_list.h` & `libsigscan-20240505/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_range_list.c` & `libsigscan-20240505/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_array.c` & `libsigscan-20240505/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_list_element.c` & `libsigscan-20240505/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_libcthreads.h` & `libsigscan-20240505/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_tree_node.h` & `libsigscan-20240505/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_error.h` & `libsigscan-20240505/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_types.h` & `libsigscan-20240505/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_btree_node.c` & `libsigscan-20240505/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_tree_node.c` & `libsigscan-20240505/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_support.h` & `libsigscan-20240505/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/Makefile.in` & `libsigscan-20240505/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -484,16 +484,16 @@
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
@@ -510,15 +510,16 @@
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
@@ -728,24 +729,37 @@
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
 
@@ -839,17 +853,14 @@
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

### Comparing `libsigscan-20240219/libcdata/libcdata_range_list_value.c` & `libsigscan-20240505/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_btree_values_list.c` & `libsigscan-20240505/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcdata/libcdata_error.c` & `libsigscan-20240505/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/config.sub` & `libsigscan-20240505/config.sub`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/etc/sigscan.conf` & `libsigscan-20240505/etc/sigscan.conf`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/setup.py` & `libsigscan-20240505/setup.py`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/acinclude.m4` & `libsigscan-20240505/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/config.rpath` & `libsigscan-20240505/config.rpath`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread.h` & `libsigscan-20240505/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_read_write_lock.h` & `libsigscan-20240505/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread.c` & `libsigscan-20240505/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread_pool.h` & `libsigscan-20240505/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_support.h` & `libsigscan-20240505/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_lock.h` & `libsigscan-20240505/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_unused.h` & `libsigscan-20240505/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_lock.c` & `libsigscan-20240505/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_condition.h` & `libsigscan-20240505/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_repeating_thread.h` & `libsigscan-20240505/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/Makefile.am` & `libsigscan-20240505/libcthreads/Makefile.am`

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

### Comparing `libsigscan-20240219/libcthreads/libcthreads_support.c` & `libsigscan-20240505/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_mutex.c` & `libsigscan-20240505/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_queue.c` & `libsigscan-20240505/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_mutex.h` & `libsigscan-20240505/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_types.h` & `libsigscan-20240505/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread_attributes.h` & `libsigscan-20240505/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_condition.c` & `libsigscan-20240505/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_error.c` & `libsigscan-20240505/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_read_write_lock.c` & `libsigscan-20240505/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_libcerror.h` & `libsigscan-20240505/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_definitions.h` & `libsigscan-20240505/libcthreads/libcthreads_definitions.h`

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

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread_pool.c` & `libsigscan-20240505/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_error.h` & `libsigscan-20240505/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_thread_attributes.c` & `libsigscan-20240505/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_extern.h` & `libsigscan-20240505/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/libcthreads_repeating_thread.c` & `libsigscan-20240505/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcthreads/Makefile.in` & `libsigscan-20240505/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -488,16 +488,16 @@
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
@@ -512,15 +512,16 @@
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
@@ -730,24 +731,37 @@
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
 
@@ -841,17 +855,14 @@
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

### Comparing `libsigscan-20240219/libcthreads/libcthreads_queue.h` & `libsigscan-20240505/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/test-driver` & `libsigscan-20240505/test-driver`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_support.c` & `libsigscan-20240505/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_libcerror.h` & `libsigscan-20240505/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_definitions.h` & `libsigscan-20240505/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libsigscan-20240219/libcpath/Makefile.am` & `libsigscan-20240505/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
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
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libsigscan-20240219/libcpath/libcpath_error.c` & `libsigscan-20240505/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_extern.h` & `libsigscan-20240505/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_system_string.h` & `libsigscan-20240505/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_support.h` & `libsigscan-20240505/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_libcsplit.h` & `libsigscan-20240505/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_system_string.c` & `libsigscan-20240505/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_libclocale.h` & `libsigscan-20240505/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_error.h` & `libsigscan-20240505/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/Makefile.in` & `libsigscan-20240505/libcpath/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -464,16 +464,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -485,15 +485,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -696,24 +697,30 @@
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
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -800,17 +807,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsigscan-20240219/libcpath/libcpath_libuna.h` & `libsigscan-20240505/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_unused.h` & `libsigscan-20240505/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_path.c` & `libsigscan-20240505/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcpath/libcpath_path.h` & `libsigscan-20240505/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_integer.c` & `libsigscan-20240505/pysigscan/pysigscan_integer.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_error.c` & `libsigscan-20240505/pysigscan/pysigscan_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_file_object_io_handle.c` & `libsigscan-20240505/pysigscan/pysigscan_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_libbfio.h` & `libsigscan-20240505/pysigscan/pysigscan_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_file_object_io_handle.h` & `libsigscan-20240505/pysigscan/pysigscan_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scanner.c` & `libsigscan-20240505/pysigscan/pysigscan_scanner.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_state.h` & `libsigscan-20240505/pysigscan/pysigscan_scan_state.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_results.c` & `libsigscan-20240505/pysigscan/pysigscan_scan_results.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_error.h` & `libsigscan-20240505/pysigscan/pysigscan_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_results.h` & `libsigscan-20240505/pysigscan/pysigscan_scan_results.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_libclocale.h` & `libsigscan-20240505/pysigscan/pysigscan_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_state.c` & `libsigscan-20240505/pysigscan/pysigscan_scan_state.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/Makefile.am` & `libsigscan-20240505/pysigscan/Makefile.am`

 * *Files 9% similar despite different names*

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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -43,13 +43,11 @@
 	@LIBBFIO_LIBADD@
 
 pysigscan_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pysigscan_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_result.c` & `libsigscan-20240505/pysigscan/pysigscan_scan_result.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan.h` & `libsigscan-20240505/pysigscan/pysigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_signature_flags.c` & `libsigscan-20240505/pysigscan/pysigscan_signature_flags.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_python.h` & `libsigscan-20240505/pysigscan/pysigscan_python.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_unused.h` & `libsigscan-20240505/pysigscan/pysigscan_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_libcerror.h` & `libsigscan-20240505/pysigscan/pysigscan_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan.c` & `libsigscan-20240505/pysigscan/pysigscan.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scan_result.h` & `libsigscan-20240505/pysigscan/pysigscan_scan_result.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_libsigscan.h` & `libsigscan-20240505/pysigscan/pysigscan_libsigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_scanner.h` & `libsigscan-20240505/pysigscan/pysigscan_scanner.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/Makefile.in` & `libsigscan-20240505/pysigscan/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -514,16 +514,16 @@
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
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -557,15 +557,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pysigscan_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pysigscan_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -863,24 +864,35 @@
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
+		-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_error.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_integer.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_scan_result.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_scan_results.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_scan_state.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_scanner.Plo
+	-rm -f ./$(DEPDIR)/pysigscan_la-pysigscan_signature_flags.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -973,13 +985,10 @@
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

### Comparing `libsigscan-20240219/pysigscan/pysigscan_signature_flags.h` & `libsigscan-20240505/pysigscan/pysigscan_signature_flags.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/pysigscan/pysigscan_integer.h` & `libsigscan-20240505/pysigscan/pysigscan_integer.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/ChangeLog` & `libsigscan-20240505/ChangeLog`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/manuals/sigscan.1` & `libsigscan-20240505/manuals/sigscan.1`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/manuals/libsigscan.3` & `libsigscan-20240505/manuals/libsigscan.3`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/manuals/Makefile.in` & `libsigscan-20240505/manuals/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -444,15 +444,16 @@
 	sigscan.1 \
 	libsigscan.3
 
 EXTRA_DIST = \
 	sigscan.1 \
 	libsigscan.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -645,23 +646,25 @@
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
@@ -743,13 +746,10 @@
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

### Comparing `libsigscan-20240219/tests/sigscan_test_signature_group.c` & `libsigscan-20240505/tests/sigscan_test_signature_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_functions.h` & `libsigscan-20240505/tests/sigscan_test_functions.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/pysigscan_test_scanner.py` & `libsigscan-20240505/tests/pysigscan_test_scanner.py`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_signature.c` & `libsigscan-20240505/tests/sigscan_test_signature.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_support.c` & `libsigscan-20240505/tests/sigscan_test_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_skip_table.c` & `libsigscan-20240505/tests/sigscan_test_skip_table.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_getopt.h` & `libsigscan-20240505/tests/sigscan_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scan_result.c` & `libsigscan-20240505/tests/sigscan_test_scan_result.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/test_pysigscan_scanner.sh` & `libsigscan-20240505/tests/test_pysigscan_scanner.sh`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libbfio.h` & `libsigscan-20240505/tests/sigscan_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_weight_group.c` & `libsigscan-20240505/tests/sigscan_test_weight_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libcerror.h` & `libsigscan-20240505/tests/sigscan_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_offsets_list.c` & `libsigscan-20240505/tests/sigscan_test_offsets_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_getopt.c` & `libsigscan-20240505/tests/sigscan_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libuna.h` & `libsigscan-20240505/tests/sigscan_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/Makefile.am` & `libsigscan-20240505/tests/Makefile.am`

 * *Files 1% similar despite different names*

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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -315,13 +315,12 @@
 	sigscan_test_unused.h \
 	sigscan_test_weight_group.c
 
 sigscan_test_weight_group_LDADD = \
 	../libsigscan/libsigscan.la \
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

### Comparing `libsigscan-20240219/tests/sigscan_test_macros.h` & `libsigscan-20240505/tests/sigscan_test_macros.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libcnotify.h` & `libsigscan-20240505/tests/sigscan_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_signatures_list.c` & `libsigscan-20240505/tests/sigscan_test_signatures_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_offset_group.c` & `libsigscan-20240505/tests/sigscan_test_offset_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_identifier.c` & `libsigscan-20240505/tests/sigscan_test_identifier.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scan_state.c` & `libsigscan-20240505/tests/sigscan_test_scan_state.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scan_tree.c` & `libsigscan-20240505/tests/sigscan_test_scan_tree.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libsigscan.h` & `libsigscan-20240505/tests/sigscan_test_libsigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/test_python_module.sh` & `libsigscan-20240505/tests/test_library.sh`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 #!/usr/bin/env bash
-# Tests Python module functions and types.
+# Tests library functions and types.
 #
-# Version: 20240120
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
-EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
-TEST_FUNCTIONS="support";
-TEST_FUNCTIONS_WITH_INPUT="";
+LIBRARY_TESTS="byte_value_group error identifier notify offset_group offsets_list pattern_weights scan_object scan_result scan_state scan_tree scan_tree_node signature signature_group signature_table signatures_list skip_table support weight_group";
+LIBRARY_TESTS_WITH_INPUT="scanner";
 OPTION_SETS=();
 
-TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
-test_python_function()
+run_test()
 {
-	local TEST_FUNCTION=$1;
+	local TEST_NAME=$1;
 
-	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysigscan_test_${TEST_FUNCTION}.py";
+	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
+	local TEST_EXECUTABLE="./sigscan_test_${TEST_NAME}";
 
-	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
+	if ! test -x "${TEST_EXECUTABLE}";
+	then
+		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
+	fi
+
+	# TODO: add support for TEST_PROFILE and OPTION_SETS?
+	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_EXECUTABLE}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
-test_python_function_with_input()
+run_test_with_input()
 {
-	local TEST_FUNCTION=$1;
+	local TEST_NAME=$1;
 
-	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pysigscan_test_${TEST_FUNCTION}.py";
+	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
+	local TEST_EXECUTABLE="./sigscan_test_${TEST_NAME}";
+
+	if ! test -x "${TEST_EXECUTABLE}";
+	then
+		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
+	fi
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pysigscan");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libsigscan");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -73,39 +82,46 @@
 		then
 			IFS="" read -a INPUT_FILES <<< $(cat ${TEST_SET_DIRECTORY}/files | sed "s?^?${TEST_SET_INPUT_DIRECTORY}/?");
 		else
 			IFS="" read -a INPUT_FILES <<< $(ls -1d ${TEST_SET_INPUT_DIRECTORY}/${INPUT_GLOB});
 		fi
 		for INPUT_FILE in "${INPUT_FILES[@]}";
 		do
+			OPTION_INPUT_FILE="${INPUT_FILE}";
+
+			if test "${OSTYPE}" = "msys";
+			then
+				# A test executable built with MinGW expects a Windows path.
+				INPUT_FILE=`echo ${INPUT_FILE} | sed 's?/?\\\\?g'`;
+			fi
 			local TESTED_WITH_OPTIONS=0;
 
 			for OPTION_SET in ${OPTION_SETS[@]};
 			do
-				local TEST_DATA_OPTION_FILE=$(get_test_data_option_file "${TEST_SET_DIRECTORY}" "${INPUT_FILE}" "${OPTION_SET}");
+				local TEST_DATA_OPTION_FILE=$(get_test_data_option_file "${TEST_SET_DIRECTORY}" "${OPTION_INPUT_FILE}" "${OPTION_SET}");
 
 				if test -f ${TEST_DATA_OPTION_FILE};
 				then
 					TESTED_WITH_OPTIONS=1;
 
 					IFS=" " read -a OPTIONS <<< $(read_test_data_option_file "${TEST_SET_DIRECTORY}" "${INPUT_FILE}" "${OPTION_SET}");
 
-					run_test_on_input_file "${TEST_SET_DIRECTORY}" "${TEST_DESCRIPTION}" "default" "${OPTION_SET}" "${TEST_SCRIPT}" "${INPUT_FILE}" "${OPTIONS[@]}";
+					run_test_on_input_file "${TEST_SET_DIRECTORY}" "${TEST_DESCRIPTION}" "default" "${OPTION_SET}" "${TEST_EXECUTABLE}" "${INPUT_FILE}" "${OPTIONS[@]}";
 					RESULT=$?;
 
 					if test ${RESULT} -ne ${EXIT_SUCCESS};
 					then
 						break;
 					fi
 				fi
 			done
 
 			if test ${TESTED_WITH_OPTIONS} -eq 0;
 			then
-				run_test_on_input_file "${TEST_SET_DIRECTORY}" "${TEST_DESCRIPTION}" "default" "" "${TEST_SCRIPT}" "${INPUT_FILE}";
+				run_test_on_input_file "${TEST_SET_DIRECTORY}" "${TEST_DESCRIPTION}" "default" "" "${TEST_EXECUTABLE}" "${INPUT_FILE}";
 				RESULT=$?;
 			fi
 
 			if test ${RESULT} -ne ${EXIT_SUCCESS};
 			then
 				break;
 			fi
@@ -116,72 +132,62 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_PYTHON_TESTS}";
+if test -n "${SKIP_LIBRARY_TESTS}";
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
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_FUNCTION in ${TEST_FUNCTIONS};
+for TEST_NAME in ${LIBRARY_TESTS};
 do
-	test_python_function "${TEST_FUNCTION}";
+	run_test "${TEST_NAME}";
 	RESULT=$?;
 
-	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
-	then
-		RESULT=${EXIT_IGNORE};
-	fi
-	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
+	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_FUNCTION in ${TEST_FUNCTIONS_WITH_INPUT};
+for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
-		test_python_function_with_input "${TEST_FUNCTION}";
+		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
-		test_python_function "${TEST_FUNCTION}";
+		run_test "${TEST_NAME}";
 		RESULT=$?;
 	fi
-	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
-	then
-		RESULT=${EXIT_IGNORE};
-	fi
-	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
+
+	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libsigscan-20240219/tests/sigscan_test_libcdata.h` & `libsigscan-20240505/tests/sigscan_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_unused.h` & `libsigscan-20240505/tests/sigscan_test_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/test_runner.sh` & `libsigscan-20240505/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scan_tree_node.c` & `libsigscan-20240505/tests/sigscan_test_scan_tree_node.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_memory.h` & `libsigscan-20240505/tests/sigscan_test_memory.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_libclocale.h` & `libsigscan-20240505/tests/sigscan_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scanner.c` & `libsigscan-20240505/tests/sigscan_test_scanner.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_notify.c` & `libsigscan-20240505/tests/sigscan_test_notify.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_pattern_weights.c` & `libsigscan-20240505/tests/sigscan_test_pattern_weights.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_byte_value_group.c` & `libsigscan-20240505/tests/sigscan_test_byte_value_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_scan_object.c` & `libsigscan-20240505/tests/sigscan_test_scan_object.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/pysigscan_test_support.py` & `libsigscan-20240505/tests/pysigscan_test_support.py`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_error.c` & `libsigscan-20240505/tests/sigscan_test_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/test_sigscan.sh` & `libsigscan-20240505/tests/test_sigscan.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Scan tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("sigscan");
 OPTIONS_PER_PROFILE=("-c../../etc/sigscan.conf");
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

### Comparing `libsigscan-20240219/tests/sigscan_test_signature_table.c` & `libsigscan-20240505/tests/sigscan_test_signature_table.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/Makefile.in` & `libsigscan-20240505/tests/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -836,16 +836,16 @@
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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1132,16 +1132,18 @@
 	sigscan_test_unused.h \
 	sigscan_test_weight_group.c
 
 sigscan_test_weight_group_LDADD = \
 	../libsigscan/libsigscan.la \
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
@@ -1626,24 +1628,49 @@
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
+		-rm -f ./$(DEPDIR)/sigscan_test_byte_value_group.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_error.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_functions.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_getopt.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_identifier.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_memory.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_notify.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_offset_group.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_offsets_list.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_pattern_weights.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scan_object.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scan_result.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scan_state.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scan_tree.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scan_tree_node.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_scanner.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_signature.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_signature_group.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_signature_table.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_signatures_list.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_skip_table.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_support.Po
+	-rm -f ./$(DEPDIR)/sigscan_test_weight_group.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1749,13 +1776,10 @@
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

### Comparing `libsigscan-20240219/tests/sigscan_test_functions.c` & `libsigscan-20240505/tests/sigscan_test_functions.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/tests/sigscan_test_memory.c` & `libsigscan-20240505/tests/sigscan_test_memory.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/ossfuzz/scanner_fuzzer.cc` & `libsigscan-20240505/ossfuzz/scanner_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/ossfuzz/Makefile.am` & `libsigscan-20240505/ossfuzz/Makefile.am`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common
 
 bin_PROGRAMS = \
 	scanner_fuzzer
 
 scanner_fuzzer_SOURCES = \
 	ossfuzz_libsigscan.h \
 	scanner_fuzzer.cc
 
 scanner_fuzzer_LDADD = \
 	@LIB_FUZZING_ENGINE@ \
 	../libsigscan/libsigscan.la
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on scanner_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(scanner_fuzzer_SOURCES)
```

### Comparing `libsigscan-20240219/ossfuzz/ossfuzz_libsigscan.h` & `libsigscan-20240505/ossfuzz/ossfuzz_libsigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/ossfuzz/Makefile.in` & `libsigscan-20240505/ossfuzz/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -477,26 +477,27 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@scanner_fuzzer_SOURCES = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	ossfuzz_libsigscan.h \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	scanner_fuzzer.cc
 
 @HAVE_LIB_FUZZING_ENGINE_TRUE@scanner_fuzzer_LDADD = \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIB_FUZZING_ENGINE@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libsigscan/libsigscan.la
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -738,23 +739,26 @@
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
+		-rm -f ./$(DEPDIR)/scanner_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -838,17 +842,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on scanner_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(scanner_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsigscan-20240219/ltmain.sh` & `libsigscan-20240505/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_narrow_string.c` & `libsigscan-20240505/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_definitions.h` & `libsigscan-20240505/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libsigscan-20240219/libcsplit/libcsplit_types.h` & `libsigscan-20240505/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_wide_split_string.c` & `libsigscan-20240505/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_support.h` & `libsigscan-20240505/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/Makefile.am` & `libsigscan-20240505/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
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
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libsigscan-20240219/libcsplit/libcsplit_libcerror.h` & `libsigscan-20240505/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_wide_string.c` & `libsigscan-20240505/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_unused.h` & `libsigscan-20240505/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_wide_split_string.h` & `libsigscan-20240505/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_error.c` & `libsigscan-20240505/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_narrow_split_string.c` & `libsigscan-20240505/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_extern.h` & `libsigscan-20240505/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_error.h` & `libsigscan-20240505/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_support.c` & `libsigscan-20240505/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_wide_string.h` & `libsigscan-20240505/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/Makefile.in` & `libsigscan-20240505/libcsplit/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -474,16 +474,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -492,15 +492,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -705,24 +706,32 @@
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
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -811,17 +820,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsigscan-20240219/libcsplit/libcsplit_narrow_split_string.h` & `libsigscan-20240505/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcsplit/libcsplit_narrow_string.h` & `libsigscan-20240505/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/remove-potcdate.sin` & `libsigscan-20240505/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/Makefile.in.in` & `libsigscan-20240505/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/en@quot.header` & `libsigscan-20240505/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/en@boldquot.header` & `libsigscan-20240505/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/insert-header.sin` & `libsigscan-20240505/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/Makevars` & `libsigscan-20240505/po/Makevars`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/Makevars.in` & `libsigscan-20240505/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/po/Rules-quot` & `libsigscan-20240505/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1251.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf16_string.c` & `libsigscan-20240505/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base16_stream.c` & `libsigscan-20240505/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf8_stream.h` & `libsigscan-20240505/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_2.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_932.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_dingbats.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf8_string.c` & `libsigscan-20240505/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base64_stream.c` & `libsigscan-20240505/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_error.h` & `libsigscan-20240505/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_turkish.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_unicode_character.c` & `libsigscan-20240505/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_gaelic.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_arabic.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_thai.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_874.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_15.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf8_string.h` & `libsigscan-20240505/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_16.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1255.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf7_stream.c` & `libsigscan-20240505/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_byte_stream.h` & `libsigscan-20240505/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_koi8_u.c` & `libsigscan-20240505/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_unused.h` & `libsigscan-20240505/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_6.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_14.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base64_stream.h` & `libsigscan-20240505/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_error.c` & `libsigscan-20240505/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_centraleurroman.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_romanian.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_6.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_9.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_russian.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_dingbats.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_15.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_936.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_croatian.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_scsu.h` & `libsigscan-20240505/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/Makefile.am` & `libsigscan-20240505/libuna/Makefile.am`

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

### Comparing `libsigscan-20240219/libuna/libuna_utf32_stream.c` & `libsigscan-20240505/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_936.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_10.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_roman.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf7_stream.h` & `libsigscan-20240505/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_3.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_thai.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_farsi.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_ukrainian.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_inuit.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_932.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_874.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_5.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_10.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_definitions.h` & `libsigscan-20240505/libuna/libuna_definitions.h`

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

### Comparing `libsigscan-20240219/libuna/libuna_url_stream.h` & `libsigscan-20240505/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_icelandic.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_koi8_u.h` & `libsigscan-20240505/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf16_stream.c` & `libsigscan-20240505/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1253.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_4.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_greek.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_libcerror.h` & `libsigscan-20240505/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_centraleurroman.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1254.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_13.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_7.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1255.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_unicode_character.h` & `libsigscan-20240505/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_8.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_13.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_949.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_cyrillic.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_celtic.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_support.h` & `libsigscan-20240505/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_4.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_949.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf16_stream.h` & `libsigscan-20240505/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_symbol.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_roman.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1257.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1254.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_950.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_extern.h` & `libsigscan-20240505/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1256.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_types.h` & `libsigscan-20240505/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base32_stream.h` & `libsigscan-20240505/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1253.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_16.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf8_stream.c` & `libsigscan-20240505/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1250.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_2.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_support.c` & `libsigscan-20240505/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_koi8_r.c` & `libsigscan-20240505/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_5.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf16_string.h` & `libsigscan-20240505/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf32_string.c` & `libsigscan-20240505/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_icelandic.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1256.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf32_string.h` & `libsigscan-20240505/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_romanian.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_8.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_koi8_r.h` & `libsigscan-20240505/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_cyrillic.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_arabic.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_croatian.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_9.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_greek.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1258.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_7.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/Makefile.in` & `libsigscan-20240505/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -642,16 +642,16 @@
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
@@ -717,15 +717,16 @@
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
@@ -987,24 +988,89 @@
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
 
@@ -1150,17 +1216,14 @@
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

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_3.c` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1250.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_scsu.c` & `libsigscan-20240505/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1252.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_turkish.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_ukrainian.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_russian.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1258.c` & `libsigscan-20240505/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_celtic.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_byte_stream.c` & `libsigscan-20240505/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_gaelic.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_utf32_stream.h` & `libsigscan-20240505/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_symbol.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1257.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_inuit.h` & `libsigscan-20240505/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_mac_farsi.c` & `libsigscan-20240505/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_950.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_url_stream.c` & `libsigscan-20240505/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1251.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_windows_1252.h` & `libsigscan-20240505/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_codepage_iso_8859_14.h` & `libsigscan-20240505/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base16_stream.h` & `libsigscan-20240505/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libuna/libuna_base32_stream.c` & `libsigscan-20240505/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/Makefile.in` & `libsigscan-20240505/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -588,16 +588,23 @@
 	etc \
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
+	libsigscan.pc \
+	libsigscan.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libsigscan.pc
 
 all: all-recursive
 
@@ -1035,23 +1042,26 @@
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
 
@@ -1159,22 +1169,10 @@
 	(cd $(srcdir)/libuna && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcfile && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcpath && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libsigscan && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libsigscan.pc
-	-rm -f libsigscan.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsigscan-20240219/libcnotify/libcnotify_definitions.h` & `libsigscan-20240505/libcnotify/libcnotify_definitions.h`

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

### Comparing `libsigscan-20240219/libcnotify/libcnotify_extern.h` & `libsigscan-20240505/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_support.c` & `libsigscan-20240505/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_stream.h` & `libsigscan-20240505/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/Makefile.am` & `libsigscan-20240505/libcnotify/Makefile.am`

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

### Comparing `libsigscan-20240219/libcnotify/libcnotify_unused.h` & `libsigscan-20240505/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_verbose.h` & `libsigscan-20240505/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_print.h` & `libsigscan-20240505/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_stream.c` & `libsigscan-20240505/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_support.h` & `libsigscan-20240505/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_verbose.c` & `libsigscan-20240505/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/Makefile.in` & `libsigscan-20240505/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -466,30 +466,31 @@
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
@@ -692,24 +693,30 @@
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
 
@@ -796,17 +803,14 @@
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

### Comparing `libsigscan-20240219/libcnotify/libcnotify_libcerror.h` & `libsigscan-20240505/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcnotify/libcnotify_print.c` & `libsigscan-20240505/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_system.c` & `libsigscan-20240505/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_error.c` & `libsigscan-20240505/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_extern.h` & `libsigscan-20240505/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/Makefile.am` & `libsigscan-20240505/libcerror/Makefile.am`

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

### Comparing `libsigscan-20240219/libcerror/libcerror_types.h` & `libsigscan-20240505/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_support.h` & `libsigscan-20240505/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_error.h` & `libsigscan-20240505/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_system.h` & `libsigscan-20240505/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_definitions.h` & `libsigscan-20240505/libcerror/libcerror_definitions.h`

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

### Comparing `libsigscan-20240219/libcerror/libcerror_support.c` & `libsigscan-20240505/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/libcerror_unused.h` & `libsigscan-20240505/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libcerror/Makefile.in` & `libsigscan-20240505/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -463,28 +463,29 @@
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
@@ -686,24 +687,29 @@
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
 
@@ -789,17 +795,14 @@
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

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_state.h` & `libsigscan-20240505/libsigscan/libsigscan_scan_state.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_skip_table.c` & `libsigscan-20240505/libsigscan/libsigscan_skip_table.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scanner.c` & `libsigscan-20240505/libsigscan/libsigscan_scanner.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_byte_value_group.c` & `libsigscan-20240505/libsigscan/libsigscan_byte_value_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_state.c` & `libsigscan-20240505/libsigscan/libsigscan_scan_state.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_identifier.h` & `libsigscan-20240505/libsigscan/libsigscan_identifier.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_tree.c` & `libsigscan-20240505/libsigscan/libsigscan_scan_tree.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_tree.h` & `libsigscan-20240505/libsigscan/libsigscan_scan_tree.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_result.h` & `libsigscan-20240505/libsigscan/libsigscan_scan_result.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature_table.c` & `libsigscan-20240505/libsigscan/libsigscan_signature_table.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_tree_node.c` & `libsigscan-20240505/libsigscan/libsigscan_scan_tree_node.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan.c` & `libsigscan-20240505/libsigscan/libsigscan.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_byte_value_group.h` & `libsigscan-20240505/libsigscan/libsigscan_byte_value_group.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_pattern_weights.h` & `libsigscan-20240505/libsigscan/libsigscan_pattern_weights.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_object.h` & `libsigscan-20240505/libsigscan/libsigscan_scan_object.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_types.h` & `libsigscan-20240505/libsigscan/libsigscan_types.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature_group.h` & `libsigscan-20240505/libsigscan/libsigscan_signature_group.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_extern.h` & `libsigscan-20240505/libsigscan/libsigscan_extern.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_support.h` & `libsigscan-20240505/libsigscan/libsigscan_support.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan.rc.in` & `libsigscan-20240505/libsigscan/libsigscan.rc.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scanner.h` & `libsigscan-20240505/libsigscan/libsigscan_scanner.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_unused.h` & `libsigscan-20240505/libsigscan/libsigscan_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_definitions.h.in` & `libsigscan-20240505/libsigscan/libsigscan_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/Makefile.am` & `libsigscan-20240505/libsigscan/Makefile.am`

 * *Files 5% similar despite different names*

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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -66,21 +66,19 @@
 libsigscan_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libsigscan_definitions.h.in \
 	libsigscan.rc \
 	libsigscan.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsigscan_definitions.h \
+	libsigscan.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libsigscan_definitions.h
-	-rm -f libsigscan.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsigscan ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsigscan_la_SOURCES)
```

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature_table.h` & `libsigscan-20240505/libsigscan/libsigscan_signature_table.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_notify.h` & `libsigscan-20240505/libsigscan/libsigscan_notify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_result.c` & `libsigscan-20240505/libsigscan/libsigscan_scan_result.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_notify.c` & `libsigscan-20240505/libsigscan/libsigscan_notify.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_identifier.c` & `libsigscan-20240505/libsigscan/libsigscan_identifier.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature_group.c` & `libsigscan-20240505/libsigscan/libsigscan_signature_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_weight_group.c` & `libsigscan-20240505/libsigscan/libsigscan_weight_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_tree_node.h` & `libsigscan-20240505/libsigscan/libsigscan_scan_tree_node.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature.h` & `libsigscan-20240505/libsigscan/libsigscan_signature.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signatures_list.h` & `libsigscan-20240505/libsigscan/libsigscan_signatures_list.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_offset_group.c` & `libsigscan-20240505/libsigscan/libsigscan_offset_group.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signatures_list.c` & `libsigscan-20240505/libsigscan/libsigscan_signatures_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_weight_group.h` & `libsigscan-20240505/libsigscan/libsigscan_weight_group.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_definitions.h` & `libsigscan-20240505/libsigscan/libsigscan_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBSIGSCAN )
 #include <libsigscan/definitions.h>
 
 /* The definitions in <libsigscan/definitions.h> are copied here
  * for local use of libsigscan
  */
 #else
-#define LIBSIGSCAN_VERSION					20240219
+#define LIBSIGSCAN_VERSION					20240505
 
 /* The version string
  */
-#define LIBSIGSCAN_VERSION_STRING				"20240219"
+#define LIBSIGSCAN_VERSION_STRING				"20240505"
 
 /* The access flags definitions
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBSIGSCAN_ACCESS_FLAGS
```

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libbfio.h` & `libsigscan-20240505/libsigscan/libsigscan_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libcnotify.h` & `libsigscan-20240505/libsigscan/libsigscan_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_pattern_weights.c` & `libsigscan-20240505/libsigscan/libsigscan_pattern_weights.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_signature.c` & `libsigscan-20240505/libsigscan/libsigscan_signature.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_scan_object.c` & `libsigscan-20240505/libsigscan/libsigscan_scan_object.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libuna.h` & `libsigscan-20240505/libsigscan/libsigscan_libuna.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_error.c` & `libsigscan-20240505/libsigscan/libsigscan_error.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_error.h` & `libsigscan-20240505/libsigscan/libsigscan_error.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan.rc` & `libsigscan-20240505/libsigscan/libsigscan.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library for binary signature scanning\0"
-      VALUE "FileVersion",		"20240219" "\0"
+      VALUE "FileVersion",		"20240505" "\0"
       VALUE "InternalName",		"libsigscan.dll\0"
       VALUE "LegalCopyright",		"(C) 2014-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libsigscan.dll\0"
       VALUE "ProductName",		"libsigscan\0"
-      VALUE "ProductVersion",		"20240219" "\0"
+      VALUE "ProductVersion",		"20240505" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libsigscan/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libsigscan-20240219/libsigscan/libsigscan_codepage.h` & `libsigscan-20240505/libsigscan/libsigscan_codepage.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_offsets_list.h` & `libsigscan-20240505/libsigscan/libsigscan_offsets_list.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_offset_group.h` & `libsigscan-20240505/libsigscan/libsigscan_offset_group.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libclocale.h` & `libsigscan-20240505/libsigscan/libsigscan_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libcdata.h` & `libsigscan-20240505/libsigscan/libsigscan_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_offsets_list.c` & `libsigscan-20240505/libsigscan/libsigscan_offsets_list.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/Makefile.in` & `libsigscan-20240505/libsigscan/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -515,16 +515,16 @@
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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -584,15 +584,18 @@
 
 libsigscan_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libsigscan_definitions.h.in \
 	libsigscan.rc \
 	libsigscan.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libsigscan_definitions.h \
+	libsigscan.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -843,24 +846,47 @@
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
+		-rm -f ./$(DEPDIR)/libsigscan.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_byte_value_group.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_error.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_identifier.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_notify.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_offset_group.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_offsets_list.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_pattern_weights.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scan_object.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scan_result.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scan_state.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scan_tree.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scan_tree_node.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_scanner.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_signature.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_signature_group.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_signature_table.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_signatures_list.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_skip_table.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_support.Plo
+	-rm -f ./$(DEPDIR)/libsigscan_weight_group.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -964,19 +990,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libsigscan_definitions.h
-	-rm -f libsigscan.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libsigscan ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libsigscan_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libsigscan-20240219/libsigscan/libsigscan_skip_table.h` & `libsigscan-20240505/libsigscan/libsigscan_skip_table.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_libcerror.h` & `libsigscan-20240505/libsigscan/libsigscan_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/libsigscan/libsigscan_support.c` & `libsigscan-20240505/libsigscan/libsigscan_support.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/aclocal.m4` & `libsigscan-20240505/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_signal.c` & `libsigscan-20240505/sigscantools/sigscantools_signal.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libcdata.h` & `libsigscan-20240505/sigscantools/sigscantools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libclocale.h` & `libsigscan-20240505/sigscantools/sigscantools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_output.c` & `libsigscan-20240505/sigscantools/sigscantools_output.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/scan_handle.c` & `libsigscan-20240505/sigscantools/scan_handle.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/Makefile.am` & `libsigscan-20240505/sigscantools/Makefile.am`

 * *Files 17% similar despite different names*

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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -39,17 +39,15 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsigscan/libsigscan.la \
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
 	@echo "Running splint on sigscan..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sigscan_SOURCES)
```

### Comparing `libsigscan-20240219/sigscantools/sigscantools_unused.h` & `libsigscan-20240505/sigscantools/sigscantools_unused.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_i18n.h` & `libsigscan-20240505/sigscantools/sigscantools_i18n.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libcnotify.h` & `libsigscan-20240505/sigscantools/sigscantools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_getopt.c` & `libsigscan-20240505/sigscantools/sigscantools_getopt.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libbfio.h` & `libsigscan-20240505/sigscantools/sigscantools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libcfile.h` & `libsigscan-20240505/sigscantools/sigscantools_libcfile.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_getopt.h` & `libsigscan-20240505/sigscantools/sigscantools_getopt.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_output.h` & `libsigscan-20240505/sigscantools/sigscantools_output.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/scan_handle.h` & `libsigscan-20240505/sigscantools/scan_handle.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_signal.h` & `libsigscan-20240505/sigscantools/sigscantools_signal.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscan.c` & `libsigscan-20240505/sigscantools/sigscan.c`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libsigscan.h` & `libsigscan-20240505/sigscantools/sigscantools_libsigscan.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libuna.h` & `libsigscan-20240505/sigscantools/sigscantools_libuna.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/sigscantools/Makefile.in` & `libsigscan-20240505/sigscantools/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -460,16 +460,16 @@
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
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -500,15 +500,16 @@
 	@LIBUNA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libsigscan/libsigscan.la \
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
@@ -754,23 +755,30 @@
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
+		-rm -f ./$(DEPDIR)/scan_handle.Po
+	-rm -f ./$(DEPDIR)/sigscan.Po
+	-rm -f ./$(DEPDIR)/sigscantools_getopt.Po
+	-rm -f ./$(DEPDIR)/sigscantools_output.Po
+	-rm -f ./$(DEPDIR)/sigscantools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -858,17 +866,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on sigscan..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(sigscan_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libsigscan-20240219/sigscantools/sigscantools_libcerror.h` & `libsigscan-20240505/sigscantools/sigscantools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libsigscan-20240219/configure.ac` & `libsigscan-20240505/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libsigscan],
- [20240219],
+ [20240505],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libsigscan.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

